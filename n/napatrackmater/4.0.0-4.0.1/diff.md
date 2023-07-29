# Comparing `tmp/napatrackmater-4.0.0.tar.gz` & `tmp/napatrackmater-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-4.0.0.tar", last modified: Sat Jul 29 17:21:37 2023, max compression
+gzip compressed data, was "napatrackmater-4.0.1.tar", last modified: Sat Jul 29 17:36:39 2023, max compression
```

## Comparing `napatrackmater-4.0.0.tar` & `napatrackmater-4.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.747521 napatrackmater-4.0.0/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:21:37.747392 napatrackmater-4.0.0/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.746320 napatrackmater-4.0.0/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   116626 2023-07-29 17:20:59.000000 napatrackmater-4.0.0/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 17:21:03.000000 napatrackmater-4.0.0/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.747142 napatrackmater-4.0.0/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 17:21:37.747562 napatrackmater-4.0.0/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:36:39.123500 napatrackmater-4.0.1/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:36:39.123399 napatrackmater-4.0.1/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:36:39.122481 napatrackmater-4.0.1/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   120529 2023-07-29 17:36:06.000000 napatrackmater-4.0.1/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 17:36:10.000000 napatrackmater-4.0.1/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:36:39.123247 napatrackmater-4.0.1/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 17:36:39.000000 napatrackmater-4.0.1/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 17:36:39.123532 napatrackmater-4.0.1/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-4.0.1/setup.py
```

### Comparing `napatrackmater-4.0.0/LICENSE` & `napatrackmater-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/PKG-INFO` & `napatrackmater-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 4.0.0
+Version: 4.0.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-4.0.0/README.md` & `napatrackmater-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-4.0.1/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-4.0.1/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/Trackmate.py` & `napatrackmater-4.0.1/napatrackmater/Trackmate.py`

 * *Files 2% similar despite different names*

```diff
@@ -987,6304 +987,6548 @@
 00003da0: 6361 6c69 6272 6174 696f 6e2c 2073 656c  calibration, sel
 00003db0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
 00003dc0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
 00003dd0: 6e29 0d0a 0d0a 2020 2020 2020 2020 2020  n)....          
 00003de0: 0d0a 2020 2020 6465 6620 5f67 6574 5f74  ..    def _get_t
 00003df0: 7261 636b 5f66 6561 7475 7265 7328 7365  rack_features(se
 00003e00: 6c66 2c20 7472 6163 6b29 3a0d 0a20 2020  lf, track):..   
-00003e10: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00003e20: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00003e30: 2020 2074 7261 636b 5f64 6973 706c 6163     track_displac
-00003e40: 656d 656e 7420 3d20 666c 6f61 7428 7472  ement = float(tr
-00003e50: 6163 6b2e 6765 7428 7365 6c66 2e64 6973  ack.get(self.dis
-00003e60: 706c 6163 656d 656e 745f 6b65 7929 290d  placement_key)).
-00003e70: 0a20 2020 2020 2020 2074 6f74 616c 5f74  .        total_t
-00003e80: 7261 636b 5f64 6973 7461 6e63 6520 3d20  rack_distance = 
-00003e90: 666c 6f61 7428 7472 6163 6b2e 6765 7428  float(track.get(
-00003ea0: 7365 6c66 2e74 6f74 616c 5f74 7261 636b  self.total_track
-00003eb0: 5f64 6973 7461 6e63 655f 6b65 7929 290d  _distance_key)).
-00003ec0: 0a20 2020 2020 2020 206d 6178 5f74 7261  .        max_tra
-00003ed0: 636b 5f64 6973 7461 6e63 6520 3d20 666c  ck_distance = fl
-00003ee0: 6f61 7428 7472 6163 6b2e 6765 7428 7365  oat(track.get(se
-00003ef0: 6c66 2e6d 6178 5f64 6973 7461 6e63 655f  lf.max_distance_
-00003f00: 7472 6176 656c 6564 5f6b 6579 2929 0d0a  traveled_key))..
-00003f10: 2020 2020 2020 2020 7472 6163 6b5f 6475          track_du
-00003f20: 7261 7469 6f6e 203d 2066 6c6f 6174 2874  ration = float(t
-00003f30: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
-00003f40: 6163 6b5f 6475 7261 7469 6f6e 5f6b 6579  ack_duration_key
-00003f50: 2929 0d0a 2020 2020 2020 2020 0d0a 2020  ))..        ..  
-00003f60: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
-00003f70: 636b 5f64 6973 706c 6163 656d 656e 742c  ck_displacement,
-00003f80: 2074 6f74 616c 5f74 7261 636b 5f64 6973   total_track_dis
-00003f90: 7461 6e63 652c 206d 6178 5f74 7261 636b  tance, max_track
-00003fa0: 5f64 6973 7461 6e63 652c 2074 7261 636b  _distance, track
-00003fb0: 5f64 7572 6174 696f 6e0d 0a20 2020 2020  _duration..     
-00003fc0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
-00003fd0: 6765 6e65 7261 7465 5f67 656e 6572 6174  generate_generat
-00003fe0: 696f 6e73 2873 656c 662c 2074 7261 636b  ions(self, track
-00003ff0: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00004000: 2020 2020 2020 2061 6c6c 5f73 6f75 7263         all_sourc
-00004010: 655f 6964 7320 3d20 5b5d 0d0a 2020 2020  e_ids = []..    
-00004020: 2020 2020 616c 6c5f 7461 7267 6574 5f69      all_target_i
-00004030: 6473 203d 205b 5d20 0d0a 0d0a 0d0a 2020  ds = [] ......  
-00004040: 2020 2020 2020 666f 7220 6564 6765 2069        for edge i
-00004050: 6e20 7472 6163 6b2e 6669 6e64 616c 6c28  n track.findall(
-00004060: 2745 6467 6527 293a 0d0a 0d0a 2020 2020  'Edge'):....    
-00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004080: 2020 2020 2020 2020 736f 7572 6365 5f69          source_i
-00004090: 6420 3d20 696e 7428 6564 6765 2e67 6574  d = int(edge.get
-000040a0: 2873 656c 662e 7370 6f74 5f73 6f75 7263  (self.spot_sourc
-000040b0: 655f 6964 5f6b 6579 2929 0d0a 2020 2020  e_id_key))..    
-000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040d0: 2020 2020 2020 2020 7461 7267 6574 5f69          target_i
-000040e0: 6420 3d20 696e 7428 6564 6765 2e67 6574  d = int(edge.get
-000040f0: 2873 656c 662e 7370 6f74 5f74 6172 6765  (self.spot_targe
-00004100: 745f 6964 5f6b 6579 2929 0d0a 2020 2020  t_id_key))..    
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2020 2020 2020 616c 6c5f 736f 7572          all_sour
-00004130: 6365 5f69 6473 2e61 7070 656e 6428 736f  ce_ids.append(so
-00004140: 7572 6365 5f69 6429 0d0a 2020 2020 2020  urce_id)..      
-00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 2020 2020 616c 6c5f 7461 7267 6574        all_target
-00004170: 5f69 6473 2e61 7070 656e 6428 7461 7267  _ids.append(targ
-00004180: 6574 5f69 6429 0d0a 2020 2020 2020 2020  et_id)..        
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
-000041b0: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-000041c0: 7267 6574 5f6c 6f6f 6b75 702e 6b65 7973  rget_lookup.keys
-000041d0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041f0: 2020 2020 7365 6c66 2e65 6467 655f 7461      self.edge_ta
-00004200: 7267 6574 5f6c 6f6f 6b75 705b 736f 7572  rget_lookup[sour
-00004210: 6365 5f69 645d 2e61 7070 656e 6428 7461  ce_id].append(ta
-00004220: 7267 6574 5f69 6429 0d0a 2020 2020 2020  rget_id)..      
-00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2020 2020 2020 656c 7365 3a20 2020 2020        else:     
-00004250: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004270: 2020 7365 6c66 2e65 6467 655f 7461 7267    self.edge_targ
-00004280: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00004290: 5f69 645d 203d 205b 7461 7267 6574 5f69  _id] = [target_i
-000042a0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-000042d0: 5f6c 6f6f 6b75 705b 7461 7267 6574 5f69  _lookup[target_i
-000042e0: 645d 203d 2073 6f75 7263 655f 6964 200d  d] = source_id .
-000042f0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00004300: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
-00004310: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
-00004320: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
-00004330: 6372 6561 7465 5f67 656e 6572 6174 696f  create_generatio
-00004340: 6e73 2873 656c 662c 2061 6c6c 5f73 6f75  ns(self, all_sou
-00004350: 7263 655f 6964 733a 206c 6973 7429 3a0d  rce_ids: list):.
-00004360: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-00004370: 2020 2020 726f 6f74 5f6c 6561 6620 3d20      root_leaf = 
-00004380: 5b5d 0d0a 2020 2020 2020 2020 726f 6f74  []..        root
-00004390: 5f72 6f6f 7420 3d20 5b5d 0d0a 2020 2020  _root = []..    
-000043a0: 2020 2020 726f 6f74 5f73 706c 6974 7320      root_splits 
-000043b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2347  = []..        #G
-000043c0: 6574 2074 6865 2072 6f6f 7420 6964 0d0a  et the root id..
-000043d0: 2020 2020 2020 2020 666f 7220 736f 7572          for sour
-000043e0: 6365 5f69 6420 696e 2061 6c6c 5f73 6f75  ce_id in all_sou
-000043f0: 7263 655f 6964 733a 0d0a 2020 2020 2020  rce_ids:..      
-00004400: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
-00004410: 655f 6964 2069 6e20 7365 6c66 2e65 6467  e_id in self.edg
-00004420: 655f 736f 7572 6365 5f6c 6f6f 6b75 703a  e_source_lookup:
-00004430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004440: 2020 736f 7572 6365 5f74 6172 6765 745f    source_target_
-00004450: 6964 203d 2073 656c 662e 6564 6765 5f73  id = self.edge_s
-00004460: 6f75 7263 655f 6c6f 6f6b 7570 5b73 6f75  ource_lookup[sou
-00004470: 7263 655f 6964 5d0d 0a20 2020 2020 2020  rce_id]..       
-00004480: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00004490: 2020 2020 2020 2020 2020 2020 2020 736f                so
-000044a0: 7572 6365 5f74 6172 6765 745f 6964 203d  urce_target_id =
-000044b0: 204e 6f6e 6520 2020 2020 2020 2020 200d   None          .
-000044c0: 0a20 2020 2020 2020 2020 2020 2020 2074  .              t
-000044d0: 6172 6765 745f 7461 7267 6574 5f69 6420  arget_target_id 
-000044e0: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
-000044f0: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00004500: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00004510: 2020 2020 6966 2073 6f75 7263 655f 7461      if source_ta
-00004520: 7267 6574 5f69 6420 6973 204e 6f6e 653a  rget_id is None:
-00004530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004540: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00004550: 6420 6e6f 7420 696e 2072 6f6f 745f 726f  d not in root_ro
-00004560: 6f74 3a0d 0a20 2020 2020 2020 2020 2020  ot:..           
-00004570: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00004580: 726f 6f74 2e61 7070 656e 6428 736f 7572  root.append(sour
-00004590: 6365 5f69 6429 200d 0a20 2020 2020 2020  ce_id) ..       
-000045a0: 2020 2020 2020 2069 6620 6c65 6e28 7461         if len(ta
-000045b0: 7267 6574 5f74 6172 6765 745f 6964 2920  rget_target_id) 
-000045c0: 3e20 313a 0d0a 2020 2020 2020 2020 2020  > 1:..          
-000045d0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
-000045e0: 6365 5f69 6420 6e6f 7420 696e 2072 6f6f  ce_id not in roo
-000045f0: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2072 6f6f 745f 7370 6c69 7473 2e61 7070   root_splits.app
-00004620: 656e 6428 736f 7572 6365 5f69 6429 0d0a  end(source_id)..
-00004630: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004640: 2074 6172 6765 745f 7461 7267 6574 5f69   target_target_i
-00004650: 645b 305d 206e 6f74 2069 6e20 7365 6c66  d[0] not in self
-00004660: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00004670: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00004680: 2020 2020 2020 2020 2072 6f6f 745f 6c65           root_le
-00004690: 6166 2e61 7070 656e 6428 7461 7267 6574  af.append(target
-000046a0: 5f74 6172 6765 745f 6964 5b30 5d29 2020  _target_id[0])  
-000046b0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000046c0: 2020 2020 7265 7475 726e 2072 6f6f 745f      return root_
-000046d0: 726f 6f74 2c20 726f 6f74 5f73 706c 6974  root, root_split
-000046e0: 732c 2072 6f6f 745f 6c65 6166 0d0a 0d0a  s, root_leaf....
-000046f0: 2020 2020 6465 6620 5f73 6f72 745f 6469      def _sort_di
-00004700: 7669 6469 6e67 5f63 656c 6c73 2873 656c  viding_cells(sel
-00004710: 662c 2072 6f6f 745f 7370 6c69 7473 293a  f, root_splits):
-00004720: 0d0a 2020 2020 2020 2020 2020 2063 656c  ..           cel
-00004730: 6c5f 6964 5f74 696d 6573 203d 205b 5d0d  l_id_times = [].
-00004740: 0a20 2020 2020 2020 2020 2020 6365 6c6c  .           cell
-00004750: 5f69 6473 203d 205b 5d0d 0a20 2020 2020  _ids = []..     
-00004760: 2020 2020 2020 666f 7220 726f 6f74 5f73        for root_s
-00004770: 706c 6974 2069 6e20 726f 6f74 5f73 706c  plit in root_spl
-00004780: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-00004790: 2020 2020 2020 2020 7370 6c69 745f 6365          split_ce
-000047a0: 6c6c 5f69 645f 7469 6d65 203d 2073 656c  ll_id_time = sel
-000047b0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000047c0: 6f70 6572 7469 6573 5b72 6f6f 745f 7370  operties[root_sp
-000047d0: 6c69 745d 5b73 656c 662e 6672 616d 6569  lit][self.framei
-000047e0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-000047f0: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-00004800: 645f 7469 6d65 732e 6170 7065 6e64 2873  d_times.append(s
-00004810: 706c 6974 5f63 656c 6c5f 6964 5f74 696d  plit_cell_id_tim
-00004820: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00004830: 2020 2020 2020 6365 6c6c 5f69 6473 2e61        cell_ids.a
-00004840: 7070 656e 6428 726f 6f74 5f73 706c 6974  ppend(root_split
-00004850: 290d 0a20 2020 2020 2020 2020 2020 736f  )..           so
-00004860: 7274 6564 5f69 6e64 6963 6573 203d 2073  rted_indices = s
-00004870: 6f72 7465 6428 7261 6e67 6528 6c65 6e28  orted(range(len(
-00004880: 6365 6c6c 5f69 645f 7469 6d65 7329 292c  cell_id_times)),
-00004890: 206b 6579 3d6c 616d 6264 6120 6b3a 2063   key=lambda k: c
-000048a0: 656c 6c5f 6964 5f74 696d 6573 5b6b 5d29  ell_id_times[k])
-000048b0: 0d0a 2020 2020 2020 2020 2020 2073 6f72  ..           sor
-000048c0: 7465 645f 6365 6c6c 5f69 6473 203d 205b  ted_cell_ids = [
-000048d0: 6365 6c6c 5f69 6473 5b69 5d20 666f 7220  cell_ids[i] for 
-000048e0: 6920 696e 2073 6f72 7465 645f 696e 6469  i in sorted_indi
-000048f0: 6365 735d 0d0a 0d0a 2020 2020 2020 2020  ces]....        
-00004900: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00004910: 5f63 656c 6c5f 6964 7320 2020 2020 2020  _cell_ids       
-00004920: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004930: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00004940: 2020 6465 6620 5f69 7465 7261 7465 5f64    def _iterate_d
-00004950: 6976 6964 696e 675f 7265 6375 7273 6976  ividing_recursiv
-00004960: 6528 7365 6c66 2c20 726f 6f74 5f6c 6561  e(self, root_lea
-00004970: 662c 2074 6172 6765 745f 6365 6c6c 2c20  f, target_cell, 
-00004980: 736f 7274 6564 5f72 6f6f 745f 7370 6c69  sorted_root_spli
-00004990: 7473 2c20 6765 6e5f 636f 756e 742c 2074  ts, gen_count, t
-000049a0: 7261 636b 6c65 745f 636f 756e 742c 2074  racklet_count, t
-000049b0: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-000049c0: 6b65 6e29 3a0d 0a20 2020 2020 2020 2020  ken):..         
-000049d0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-000049e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000049f0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00004a00: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
-00004a10: 7267 6574 5f63 656c 6c5d 203d 2067 656e  rget_cell] = gen
-00004a20: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-00004a30: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00004a40: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
-00004a50: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
-00004a60: 6574 5f63 6f75 6e74 0d0a 0d0a 2020 2020  et_count....    
-00004a70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00004a80: 6172 6765 745f 6365 6c6c 203d 3d20 726f  arget_cell == ro
-00004a90: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004ab0: 7475 726e 0d0a 2020 2020 2020 2020 2020  turn..          
-00004ac0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00004ad0: 2020 2020 2020 2020 6e65 7874 5f74 6172          next_tar
-00004ae0: 6765 745f 6365 6c6c 203d 204e 6f6e 650d  get_cell = None.
-00004af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004b10: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-00004b20: 6c20 696e 2073 6f72 7465 645f 726f 6f74  l in sorted_root
-00004b30: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b50: 2020 2020 206e 6578 745f 6765 6e5f 636f       next_gen_co
-00004b60: 756e 7420 3d20 6765 6e5f 636f 756e 7420  unt = gen_count 
-00004b70: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
-00004ba0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-00004bb0: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bd0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00004be0: 6574 5f63 656c 6c73 203d 2073 656c 662e  et_cells = self.
-00004bf0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00004c00: 7570 5b74 6172 6765 745f 6365 6c6c 5d0d  up[target_cell].
-00004c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
-00004c40: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
-00004c50: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2020 2020 2020 2020 2064 6175 6768 7465           daughte
-00004c80: 725f 7461 7267 6574 5f63 656c 6c20 3d20  r_target_cell = 
-00004c90: 7461 7267 6574 5f63 656c 6c73 5b6b 5d0d  target_cells[k].
-00004ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
-00004cd0: 756e 7420 3d20 7472 6163 6b6c 6574 5f63  unt = tracklet_c
-00004ce0: 6f75 6e74 202b 2031 202b 206b 0d0a 2020  ount + 1 + k..  
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2020 7472 6163 6b6c 6574 5f63 6f75 6e74    tracklet_count
-00004d20: 203d 2073 656c 662e 5f75 6e69 7175 655f   = self._unique_
-00004d30: 7472 6163 6b6c 6574 5f63 6f75 6e74 2874  tracklet_count(t
-00004d40: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-00004d50: 6b65 6e2c 2074 7261 636b 6c65 745f 636f  ken, tracklet_co
-00004d60: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d80: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
-00004d90: 6574 5f63 6f75 6e74 5f74 616b 656e 2e61  et_count_taken.a
-00004da0: 7070 656e 6428 7472 6163 6b6c 6574 5f63  ppend(tracklet_c
-00004db0: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
-00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004de0: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
-00004df0: 675f 7265 6375 7273 6976 6528 726f 6f74  g_recursive(root
-00004e00: 5f6c 6561 662c 2064 6175 6768 7465 725f  _leaf, daughter_
-00004e10: 7461 7267 6574 5f63 656c 6c2c 2073 6f72  target_cell, sor
-00004e20: 7465 645f 726f 6f74 5f73 706c 6974 732c  ted_root_splits,
-00004e30: 206e 6578 745f 6765 6e5f 636f 756e 742c   next_gen_count,
-00004e40: 2074 7261 636b 6c65 745f 636f 756e 742c   tracklet_count,
-00004e50: 2074 7261 636b 6c65 745f 636f 756e 745f   tracklet_count_
-00004e60: 7461 6b65 6e29 2020 2020 2020 0d0a 0d0a  taken)      ....
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00004e90: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
-00004ea0: 6365 6c6c 2069 6e20 7365 6c66 2e65 6467  cell in self.edg
-00004eb0: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004ed0: 2020 2020 2020 6e65 7874 5f74 6172 6765        next_targe
-00004ee0: 745f 6365 6c6c 7320 3d20 7365 6c66 2e65  t_cells = self.e
-00004ef0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004f00: 705b 7461 7267 6574 5f63 656c 6c5d 0d0a  p[target_cell]..
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 6e65 7874 5f74 6172 6765 745f      next_target_
-00004f30: 6365 6c6c 203d 206e 6578 745f 7461 7267  cell = next_targ
-00004f40: 6574 5f63 656c 6c73 5b30 5d0d 0a20 2020  et_cells[0]..   
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00003e10: 2020 2020 200d 0a20 2020 2020 2020 2074       ..        t
+00003e20: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+00003e30: 7420 3d20 666c 6f61 7428 7472 6163 6b2e  t = float(track.
+00003e40: 6765 7428 7365 6c66 2e64 6973 706c 6163  get(self.displac
+00003e50: 656d 656e 745f 6b65 7929 290d 0a20 2020  ement_key))..   
+00003e60: 2020 2020 2074 6f74 616c 5f74 7261 636b       total_track
+00003e70: 5f64 6973 7461 6e63 6520 3d20 666c 6f61  _distance = floa
+00003e80: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+00003e90: 2e74 6f74 616c 5f74 7261 636b 5f64 6973  .total_track_dis
+00003ea0: 7461 6e63 655f 6b65 7929 290d 0a20 2020  tance_key))..   
+00003eb0: 2020 2020 206d 6178 5f74 7261 636b 5f64       max_track_d
+00003ec0: 6973 7461 6e63 6520 3d20 666c 6f61 7428  istance = float(
+00003ed0: 7472 6163 6b2e 6765 7428 7365 6c66 2e6d  track.get(self.m
+00003ee0: 6178 5f64 6973 7461 6e63 655f 7472 6176  ax_distance_trav
+00003ef0: 656c 6564 5f6b 6579 2929 0d0a 2020 2020  eled_key))..    
+00003f00: 2020 2020 7472 6163 6b5f 6475 7261 7469      track_durati
+00003f10: 6f6e 203d 2066 6c6f 6174 2874 7261 636b  on = float(track
+00003f20: 2e67 6574 2873 656c 662e 7472 6163 6b5f  .get(self.track_
+00003f30: 6475 7261 7469 6f6e 5f6b 6579 2929 0d0a  duration_key))..
+00003f40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003f50: 2020 7265 7475 726e 2074 7261 636b 5f64    return track_d
+00003f60: 6973 706c 6163 656d 656e 742c 2074 6f74  isplacement, tot
+00003f70: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+00003f80: 652c 206d 6178 5f74 7261 636b 5f64 6973  e, max_track_dis
+00003f90: 7461 6e63 652c 2074 7261 636b 5f64 7572  tance, track_dur
+00003fa0: 6174 696f 6e0d 0a20 2020 2020 2020 200d  ation..        .
+00003fb0: 0a0d 0a20 2020 2064 6566 205f 6765 6e65  ...    def _gene
+00003fc0: 7261 7465 5f67 656e 6572 6174 696f 6e73  rate_generations
+00003fd0: 2873 656c 662c 2074 7261 636b 293a 0d0a  (self, track):..
+00003fe0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003ff0: 2020 2061 6c6c 5f73 6f75 7263 655f 6964     all_source_id
+00004000: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00004010: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
+00004020: 205b 5d20 0d0a 0d0a 0d0a 2020 2020 2020   [] ......      
+00004030: 2020 666f 7220 6564 6765 2069 6e20 7472    for edge in tr
+00004040: 6163 6b2e 6669 6e64 616c 6c28 2745 6467  ack.findall('Edg
+00004050: 6527 293a 0d0a 0d0a 2020 2020 2020 2020  e'):....        
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 2020 736f 7572 6365 5f69 6420 3d20      source_id = 
+00004080: 696e 7428 6564 6765 2e67 6574 2873 656c  int(edge.get(sel
+00004090: 662e 7370 6f74 5f73 6f75 7263 655f 6964  f.spot_source_id
+000040a0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 7461 7267 6574 5f69 6420 3d20      target_id = 
+000040d0: 696e 7428 6564 6765 2e67 6574 2873 656c  int(edge.get(sel
+000040e0: 662e 7370 6f74 5f74 6172 6765 745f 6964  f.spot_target_id
+000040f0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 616c 6c5f 736f 7572 6365 5f69      all_source_i
+00004120: 6473 2e61 7070 656e 6428 736f 7572 6365  ds.append(source
+00004130: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004150: 2020 616c 6c5f 7461 7267 6574 5f69 6473    all_target_ids
+00004160: 2e61 7070 656e 6428 7461 7267 6574 5f69  .append(target_i
+00004170: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 6966 2073 6f75 7263 655f 6964 2069 6e20  if source_id in 
+000041a0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000041b0: 5f6c 6f6f 6b75 702e 6b65 7973 2829 3a0d  _lookup.keys():.
+000041c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041e0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000041f0: 5f6c 6f6f 6b75 705b 736f 7572 6365 5f69  _lookup[source_i
+00004200: 645d 2e61 7070 656e 6428 7461 7267 6574  d].append(target
+00004210: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004230: 2020 656c 7365 3a20 2020 2020 200d 0a20    else:      .. 
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004260: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00004270: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
+00004280: 203d 205b 7461 7267 6574 5f69 645d 0d0a   = [target_id]..
+00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000042b0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+000042c0: 6b75 705b 7461 7267 6574 5f69 645d 203d  kup[target_id] =
+000042d0: 2073 6f75 7263 655f 6964 200d 0a0d 0a20   source_id .... 
+000042e0: 2020 2020 2020 2072 6574 7572 6e20 616c         return al
+000042f0: 6c5f 736f 7572 6365 5f69 6473 2c20 616c  l_source_ids, al
+00004300: 6c5f 7461 7267 6574 5f69 6473 200d 0a0d  l_target_ids ...
+00004310: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
+00004320: 7465 5f67 656e 6572 6174 696f 6e73 2873  te_generations(s
+00004330: 656c 662c 2061 6c6c 5f73 6f75 7263 655f  elf, all_source_
+00004340: 6964 733a 206c 6973 7429 3a0d 0a20 2020  ids: list):..   
+00004350: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004360: 726f 6f74 5f6c 6561 6620 3d20 5b5d 0d0a  root_leaf = []..
+00004370: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
+00004380: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
+00004390: 726f 6f74 5f73 706c 6974 7320 3d20 5b5d  root_splits = []
+000043a0: 0d0a 2020 2020 2020 2020 2347 6574 2074  ..        #Get t
+000043b0: 6865 2072 6f6f 7420 6964 0d0a 2020 2020  he root id..    
+000043c0: 2020 2020 666f 7220 736f 7572 6365 5f69      for source_i
+000043d0: 6420 696e 2061 6c6c 5f73 6f75 7263 655f  d in all_source_
+000043e0: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+000043f0: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
+00004400: 2069 6e20 7365 6c66 2e65 6467 655f 736f   in self.edge_so
+00004410: 7572 6365 5f6c 6f6f 6b75 703a 0d0a 2020  urce_lookup:..  
+00004420: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00004430: 7572 6365 5f74 6172 6765 745f 6964 203d  urce_target_id =
+00004440: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
+00004450: 655f 6c6f 6f6b 7570 5b73 6f75 7263 655f  e_lookup[source_
+00004460: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
+00004470: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00004480: 2020 2020 2020 2020 2020 736f 7572 6365            source
+00004490: 5f74 6172 6765 745f 6964 203d 204e 6f6e  _target_id = Non
+000044a0: 6520 2020 2020 2020 2020 200d 0a20 2020  e          ..   
+000044b0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000044c0: 745f 7461 7267 6574 5f69 6420 3d20 7365  t_target_id = se
+000044d0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+000044e0: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
+000044f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004500: 6966 2073 6f75 7263 655f 7461 7267 6574  if source_target
+00004510: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
+00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004530: 2069 6620 736f 7572 6365 5f69 6420 6e6f   if source_id no
+00004540: 7420 696e 2072 6f6f 745f 726f 6f74 3a0d  t in root_root:.
+00004550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004560: 2020 2020 2020 2072 6f6f 745f 726f 6f74         root_root
+00004570: 2e61 7070 656e 6428 736f 7572 6365 5f69  .append(source_i
+00004580: 6429 200d 0a20 2020 2020 2020 2020 2020  d) ..           
+00004590: 2020 2069 6620 6c65 6e28 7461 7267 6574     if len(target
+000045a0: 5f74 6172 6765 745f 6964 2920 3e20 313a  _target_id) > 1:
+000045b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000045c0: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
+000045d0: 6420 6e6f 7420 696e 2072 6f6f 745f 7370  d not in root_sp
+000045e0: 6c69 7473 3a0d 0a20 2020 2020 2020 2020  lits:..         
+000045f0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00004600: 745f 7370 6c69 7473 2e61 7070 656e 6428  t_splits.append(
+00004610: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
+00004620: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+00004630: 6765 745f 7461 7267 6574 5f69 645b 305d  get_target_id[0]
+00004640: 206e 6f74 2069 6e20 7365 6c66 2e65 6467   not in self.edg
+00004650: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
+00004660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004670: 2020 2020 2072 6f6f 745f 6c65 6166 2e61       root_leaf.a
+00004680: 7070 656e 6428 7461 7267 6574 5f74 6172  ppend(target_tar
+00004690: 6765 745f 6964 5b30 5d29 2020 2020 2020  get_id[0])      
+000046a0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+000046b0: 7265 7475 726e 2072 6f6f 745f 726f 6f74  return root_root
+000046c0: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+000046d0: 6f6f 745f 6c65 6166 0d0a 0d0a 2020 2020  oot_leaf....    
+000046e0: 6465 6620 5f73 6f72 745f 6469 7669 6469  def _sort_dividi
+000046f0: 6e67 5f63 656c 6c73 2873 656c 662c 2072  ng_cells(self, r
+00004700: 6f6f 745f 7370 6c69 7473 293a 0d0a 2020  oot_splits):..  
+00004710: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+00004720: 5f74 696d 6573 203d 205b 5d0d 0a20 2020  _times = []..   
+00004730: 2020 2020 2020 2020 6365 6c6c 5f69 6473          cell_ids
+00004740: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00004750: 2020 666f 7220 726f 6f74 5f73 706c 6974    for root_split
+00004760: 2069 6e20 726f 6f74 5f73 706c 6974 733a   in root_splits:
+00004770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004780: 2020 2020 7370 6c69 745f 6365 6c6c 5f69      split_cell_i
+00004790: 645f 7469 6d65 203d 2073 656c 662e 756e  d_time = self.un
+000047a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000047b0: 7469 6573 5b72 6f6f 745f 7370 6c69 745d  ties[root_split]
+000047c0: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
+000047d0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+000047e0: 2020 2020 2020 6365 6c6c 5f69 645f 7469        cell_id_ti
+000047f0: 6d65 732e 6170 7065 6e64 2873 706c 6974  mes.append(split
+00004800: 5f63 656c 6c5f 6964 5f74 696d 6529 0d0a  _cell_id_time)..
+00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004820: 2020 6365 6c6c 5f69 6473 2e61 7070 656e    cell_ids.appen
+00004830: 6428 726f 6f74 5f73 706c 6974 290d 0a20  d(root_split).. 
+00004840: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+00004850: 5f69 6e64 6963 6573 203d 2073 6f72 7465  _indices = sorte
+00004860: 6428 7261 6e67 6528 6c65 6e28 6365 6c6c  d(range(len(cell
+00004870: 5f69 645f 7469 6d65 7329 292c 206b 6579  _id_times)), key
+00004880: 3d6c 616d 6264 6120 6b3a 2063 656c 6c5f  =lambda k: cell_
+00004890: 6964 5f74 696d 6573 5b6b 5d29 0d0a 2020  id_times[k])..  
+000048a0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
+000048b0: 6365 6c6c 5f69 6473 203d 205b 6365 6c6c  cell_ids = [cell
+000048c0: 5f69 6473 5b69 5d20 666f 7220 6920 696e  _ids[i] for i in
+000048d0: 2073 6f72 7465 645f 696e 6469 6365 735d   sorted_indices]
+000048e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2072  ....           r
+000048f0: 6574 7572 6e20 736f 7274 6564 5f63 656c  eturn sorted_cel
+00004900: 6c5f 6964 7320 2020 2020 2020 0d0a 0d0a  l_ids       ....
+00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
+00004930: 6620 5f69 7465 7261 7465 5f64 6976 6964  f _iterate_divid
+00004940: 696e 675f 7265 6375 7273 6976 6528 7365  ing_recursive(se
+00004950: 6c66 2c20 726f 6f74 5f6c 6561 662c 2074  lf, root_leaf, t
+00004960: 6172 6765 745f 6365 6c6c 2c20 736f 7274  arget_cell, sort
+00004970: 6564 5f72 6f6f 745f 7370 6c69 7473 2c20  ed_root_splits, 
+00004980: 6765 6e5f 636f 756e 742c 2074 7261 636b  gen_count, track
+00004990: 6c65 745f 636f 756e 742c 2074 7261 636b  let_count, track
+000049a0: 6c65 745f 636f 756e 745f 7461 6b65 6e29  let_count_taken)
+000049b0: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+000049c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000049d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000049e0: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+000049f0: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
+00004a00: 5f63 656c 6c5d 203d 2067 656e 5f63 6f75  _cell] = gen_cou
+00004a10: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00004a20: 2020 2020 7365 6c66 2e74 7261 636b 6c65      self.trackle
+00004a30: 745f 6469 6374 5b74 6172 6765 745f 6365  t_dict[target_ce
+00004a40: 6c6c 5d20 3d20 7472 6163 6b6c 6574 5f63  ll] = tracklet_c
+00004a50: 6f75 6e74 0d0a 0d0a 2020 2020 2020 2020  ount....        
+00004a60: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004a70: 745f 6365 6c6c 203d 3d20 726f 6f74 5f6c  t_cell == root_l
+00004a80: 6561 663a 0d0a 2020 2020 2020 2020 2020  eaf:..          
+00004a90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00004aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ab0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00004ac0: 2020 2020 6e65 7874 5f74 6172 6765 745f      next_target_
+00004ad0: 6365 6c6c 203d 204e 6f6e 650d 0a20 2020  cell = None..   
+00004ae0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00004af0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004b00: 6620 7461 7267 6574 5f63 656c 6c20 696e  f target_cell in
+00004b10: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
+00004b20: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 206e 6578 745f 6765 6e5f 636f 756e 7420   next_gen_count 
+00004b50: 3d20 6765 6e5f 636f 756e 7420 2b20 310d  = gen_count + 1.
+00004b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b70: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+00004b80: 6172 6765 745f 6365 6c6c 2069 6e20 7365  arget_cell in se
+00004b90: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00004ba0: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+00004bd0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+00004be0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
+00004bf0: 6172 6765 745f 6365 6c6c 5d0d 0a20 2020  arget_cell]..   
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00004c20: 206b 2069 6e20 7261 6e67 6528 6c65 6e28   k in range(len(
+00004c30: 7461 7267 6574 5f63 656c 6c73 2929 3a0d  target_cells)):.
+00004c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2064 6175 6768 7465 725f 7461       daughter_ta
+00004c70: 7267 6574 5f63 656c 6c20 3d20 7461 7267  rget_cell = targ
+00004c80: 6574 5f63 656c 6c73 5b6b 5d0d 0a20 2020  et_cells[k]..   
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
+00004cc0: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
+00004cd0: 202b 2031 202b 206b 0d0a 2020 2020 2020   + 1 + k..      
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00004d00: 6163 6b6c 6574 5f63 6f75 6e74 203d 2073  acklet_count = s
+00004d10: 656c 662e 5f75 6e69 7175 655f 7472 6163  elf._unique_trac
+00004d20: 6b6c 6574 5f63 6f75 6e74 2874 7261 636b  klet_count(track
+00004d30: 6c65 745f 636f 756e 745f 7461 6b65 6e2c  let_count_taken,
+00004d40: 2074 7261 636b 6c65 745f 636f 756e 7429   tracklet_count)
+00004d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 7472 6163 6b6c 6574 5f63        tracklet_c
+00004d80: 6f75 6e74 5f74 616b 656e 2e61 7070 656e  ount_taken.appen
+00004d90: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
+00004da0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2020 2020 2020 2073 656c 662e 5f69 7465         self._ite
+00004dd0: 7261 7465 5f64 6976 6964 696e 675f 7265  rate_dividing_re
+00004de0: 6375 7273 6976 6528 726f 6f74 5f6c 6561  cursive(root_lea
+00004df0: 662c 2064 6175 6768 7465 725f 7461 7267  f, daughter_targ
+00004e00: 6574 5f63 656c 6c2c 2073 6f72 7465 645f  et_cell, sorted_
+00004e10: 726f 6f74 5f73 706c 6974 732c 206e 6578  root_splits, nex
+00004e20: 745f 6765 6e5f 636f 756e 742c 2074 7261  t_gen_count, tra
+00004e30: 636b 6c65 745f 636f 756e 742c 2074 7261  cklet_count, tra
+00004e40: 636b 6c65 745f 636f 756e 745f 7461 6b65  cklet_count_take
+00004e50: 6e29 2020 2020 2020 0d0a 0d0a 2020 2020  n)      ....    
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e80: 2020 6966 2074 6172 6765 745f 6365 6c6c    if target_cell
+00004e90: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
+00004ea0: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ec0: 2020 6e65 7874 5f74 6172 6765 745f 6365    next_target_ce
+00004ed0: 6c6c 7320 3d20 7365 6c66 2e65 6467 655f  lls = self.edge_
+00004ee0: 7461 7267 6574 5f6c 6f6f 6b75 705b 7461  target_lookup[ta
+00004ef0: 7267 6574 5f63 656c 6c5d 0d0a 2020 2020  rget_cell]..    
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f10: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+00004f20: 203d 206e 6578 745f 7461 7267 6574 5f63   = next_target_c
+00004f30: 656c 6c73 5b30 5d0d 0a20 2020 2020 2020  ells[0]..       
+00004f40: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00004f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004f90: 2020 2020 2020 7768 696c 6520 6e65 7874        while next
-00004fa0: 5f74 6172 6765 745f 6365 6c6c 206e 6f74  _target_cell not
-00004fb0: 2069 6e20 736f 7274 6564 5f72 6f6f 745f   in sorted_root_
-00004fc0: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00004ff0: 5f64 6963 745b 6e65 7874 5f74 6172 6765  _dict[next_targe
-00005000: 745f 6365 6c6c 5d20 3d20 6765 6e5f 636f  t_cell] = gen_co
-00005010: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00005020: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005030: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-00005040: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
-00005050: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
-00005060: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00005070: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005080: 6578 745f 7461 7267 6574 5f63 656c 6c20  ext_target_cell 
-00005090: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000050c0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-000050d0: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-000050e0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005110: 2e74 7261 636b 6c65 745f 6469 6374 5b74  .tracklet_dict[t
-00005120: 6172 6765 745f 6365 6c6c 5d20 3d20 7472  arget_cell] = tr
-00005130: 6163 6b6c 6574 5f63 6f75 6e74 0d0a 2020  acklet_count..  
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00005160: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
-00005170: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005180: 6578 745f 7461 7267 6574 5f63 656c 6c20  ext_target_cell 
-00005190: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
-000051a0: 6765 745f 6c6f 6f6b 7570 3a0d 0a20 2020  get_lookup:..   
-000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-000051d0: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
-000051e0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-000051f0: 6f6b 7570 5b6e 6578 745f 7461 7267 6574  okup[next_target
-00005200: 5f63 656c 6c5d 0d0a 2020 2020 2020 2020  _cell]..        
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2020 2020 6e65 7874 5f74 6172 6765 745f      next_target_
-00005230: 6365 6c6c 203d 206e 6578 745f 7461 7267  cell = next_targ
-00005240: 6574 5f63 656c 6c73 5b30 5d0d 0a20 2020  et_cells[0]..   
-00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005260: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
-00005270: 5f74 6172 6765 745f 6365 6c6c 2069 6e20  _target_cell in 
-00005280: 726f 6f74 5f6c 6561 663a 0d0a 2020 2020  root_leaf:..    
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000052b0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-000052c0: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
-000052d0: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00005300: 6163 6b6c 6574 5f64 6963 745b 7461 7267  acklet_dict[targ
-00005310: 6574 5f63 656c 6c5d 203d 2074 7261 636b  et_cell] = track
-00005320: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-00005350: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00005360: 2020 2069 6620 6e65 7874 5f74 6172 6765     if next_targe
-00005370: 745f 6365 6c6c 2069 7320 6e6f 7420 4e6f  t_cell is not No
-00005380: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00005390: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-000053a0: 6e65 7261 7469 6f6e 5f64 6963 745b 6e65  neration_dict[ne
-000053b0: 7874 5f74 6172 6765 745f 6365 6c6c 5d20  xt_target_cell] 
-000053c0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053e0: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-000053f0: 6963 745b 6e65 7874 5f74 6172 6765 745f  ict[next_target_
-00005400: 6365 6c6c 5d20 3d20 7472 6163 6b6c 6574  cell] = tracklet
-00005410: 5f63 6f75 6e74 2020 0d0a 2020 2020 2020  _count  ..      
-00005420: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00005430: 7874 5f67 656e 5f63 6f75 6e74 203d 2067  xt_gen_count = g
-00005440: 656e 5f63 6f75 6e74 202b 2031 0d0a 2020  en_count + 1..  
+00004f80: 2020 7768 696c 6520 6e65 7874 5f74 6172    while next_tar
+00004f90: 6765 745f 6365 6c6c 206e 6f74 2069 6e20  get_cell not in 
+00004fa0: 736f 7274 6564 5f72 6f6f 745f 7370 6c69  sorted_root_spli
+00004fb0: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00004fc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004fd0: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
+00004fe0: 745b 6e65 7874 5f74 6172 6765 745f 6365  t[next_target_ce
+00004ff0: 6c6c 5d20 3d20 6765 6e5f 636f 756e 740d  ll] = gen_count.
+00005000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005010: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+00005020: 6163 6b6c 6574 5f64 6963 745b 6e65 7874  acklet_dict[next
+00005030: 5f74 6172 6765 745f 6365 6c6c 5d20 3d20  _target_cell] = 
+00005040: 7472 6163 6b6c 6574 5f63 6f75 6e74 0d0a  tracklet_count..
+00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005060: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+00005070: 7461 7267 6574 5f63 656c 6c20 696e 2072  target_cell in r
+00005080: 6f6f 745f 6c65 6166 3a0d 0a20 2020 2020  oot_leaf:..     
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+000050b0: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
+000050c0: 6172 6765 745f 6365 6c6c 5d20 3d20 6765  arget_cell] = ge
+000050d0: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00005100: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
+00005110: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
+00005120: 6574 5f63 6f75 6e74 0d0a 2020 2020 2020  et_count..      
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+00005170: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
+00005180: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+00005190: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 206e 6578 745f 7461 7267 6574       next_target
+000051c0: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+000051d0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+000051e0: 5b6e 6578 745f 7461 7267 6574 5f63 656c  [next_target_cel
+000051f0: 6c5d 0d0a 2020 2020 2020 2020 2020 2020  l]..            
+00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005210: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+00005220: 203d 206e 6578 745f 7461 7267 6574 5f63   = next_target_c
+00005230: 656c 6c73 5b30 5d0d 0a20 2020 2020 2020  ells[0]..       
+00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005250: 2020 2020 2069 6620 6e65 7874 5f74 6172       if next_tar
+00005260: 6765 745f 6365 6c6c 2069 6e20 726f 6f74  get_cell in root
+00005270: 5f6c 6561 663a 0d0a 2020 2020 2020 2020  _leaf:..        
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
+000052a0: 7261 7469 6f6e 5f64 6963 745b 7461 7267  ration_dict[targ
+000052b0: 6574 5f63 656c 6c5d 203d 2067 656e 5f63  et_cell] = gen_c
+000052c0: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
+000052f0: 6574 5f64 6963 745b 7461 7267 6574 5f63  et_dict[target_c
+00005300: 656c 6c5d 203d 2074 7261 636b 6c65 745f  ell] = tracklet_
+00005310: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 2020 6272 6561 6b0d 0a0d 0a20        break.... 
+00005340: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005350: 6620 6e65 7874 5f74 6172 6765 745f 6365  f next_target_ce
+00005360: 6c6c 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ll is not None:.
+00005370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005380: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+00005390: 7469 6f6e 5f64 6963 745b 6e65 7874 5f74  tion_dict[next_t
+000053a0: 6172 6765 745f 6365 6c6c 5d20 3d20 6765  arget_cell] = ge
+000053b0: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
+000053c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000053d0: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+000053e0: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+000053f0: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
+00005400: 6e74 2020 0d0a 2020 2020 2020 2020 2020  nt  ..          
+00005410: 2020 2020 2020 2020 2020 6e65 7874 5f67            next_g
+00005420: 656e 5f63 6f75 6e74 203d 2067 656e 5f63  en_count = gen_c
+00005430: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+00005440: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00005470: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
-00005480: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
-00005490: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-000054a0: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
-000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-000054d0: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
-000054e0: 7267 6574 5f6c 6f6f 6b75 705b 6e65 7874  rget_lookup[next
-000054f0: 5f74 6172 6765 745f 6365 6c6c 5d0d 0a20  _target_cell].. 
-00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005510: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00005520: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
-00005530: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005560: 6172 6765 745f 6365 6c6c 203d 2074 6172  arget_cell = tar
-00005570: 6765 745f 6365 6c6c 735b 6b5d 0d0a 2020  get_cells[k]..  
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000055a0: 6163 6b6c 6574 5f63 6f75 6e74 203d 2074  acklet_count = t
-000055b0: 7261 636b 6c65 745f 636f 756e 7420 2b20  racklet_count + 
-000055c0: 3120 2b20 6b0d 0a20 2020 2020 2020 2020  1 + k..         
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
-000055f0: 636f 756e 7420 3d20 7365 6c66 2e5f 756e  count = self._un
-00005600: 6971 7565 5f74 7261 636b 6c65 745f 636f  ique_tracklet_co
-00005610: 756e 7428 7472 6163 6b6c 6574 5f63 6f75  unt(tracklet_cou
-00005620: 6e74 5f74 616b 656e 2c20 7472 6163 6b6c  nt_taken, trackl
-00005630: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00005660: 6c65 745f 636f 756e 745f 7461 6b65 6e2e  let_count_taken.
-00005670: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-00005680: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056a0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-000056b0: 6572 6174 655f 6469 7669 6469 6e67 5f72  erate_dividing_r
-000056c0: 6563 7572 7369 7665 2872 6f6f 745f 6c65  ecursive(root_le
-000056d0: 6166 2c20 7461 7267 6574 5f63 656c 6c2c  af, target_cell,
-000056e0: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
-000056f0: 6974 732c 206e 6578 745f 6765 6e5f 636f  its, next_gen_co
-00005700: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
-00005710: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
-00005720: 756e 745f 7461 6b65 6e29 2020 2020 2020  unt_taken)      
-00005730: 0d0a 0d0a 0d0a 0d0a 2020 2020 6465 6620  ........    def 
-00005740: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
-00005750: 6728 7365 6c66 2c20 726f 6f74 5f72 6f6f  g(self, root_roo
-00005760: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
-00005770: 6f74 5f73 706c 6974 7329 3a0d 0a20 2020  ot_splits):..   
-00005780: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005790: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000057a0: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
-000057b0: 300d 0a20 2020 2020 2020 2020 2020 2074  0..            t
-000057c0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-000057d0: 300d 0a20 2020 2020 2020 2020 2020 2074  0..            t
-000057e0: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-000057f0: 6b65 6e20 3d20 5b5d 0d0a 2020 2020 2020  ken = []..      
-00005800: 2020 2020 2020 666f 7220 726f 6f74 5f61        for root_a
-00005810: 6c6c 2069 6e20 726f 6f74 5f72 6f6f 743a  ll in root_root:
-00005820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005830: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-00005840: 6174 696f 6e5f 6469 6374 5b72 6f6f 745f  ation_dict[root_
-00005850: 616c 6c5d 203d 2067 656e 5f63 6f75 6e74  all] = gen_count
-00005860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005870: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00005880: 6c65 745f 6469 6374 5b72 6f6f 745f 616c  let_dict[root_al
-00005890: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-000058a0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000058b0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-000058c0: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
-000058d0: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-000058e0: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-000058f0: 2020 2020 2020 2020 2020 6966 2072 6f6f            if roo
-00005900: 745f 616c 6c20 696e 2073 656c 662e 6564  t_all in self.ed
-00005910: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00005920: 2061 6e64 2072 6f6f 745f 616c 6c20 6e6f   and root_all no
-00005930: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
-00005940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005950: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00005960: 6574 5f63 656c 6c20 3d20 7365 6c66 2e65  et_cell = self.e
-00005970: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00005980: 705b 726f 6f74 5f61 6c6c 5d5b 305d 0d0a  p[root_all][0]..
-00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059a0: 2020 2020 2020 2020 2077 6869 6c65 2074           while t
-000059b0: 6172 6765 745f 6365 6c6c 206e 6f74 2069  arget_cell not i
-000059c0: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
-00005a00: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-00005a10: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a40: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
-00005a50: 6469 6374 5b74 6172 6765 745f 6365 6c6c  dict[target_cell
-00005a60: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-00005aa0: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
-00005ab0: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-00005ac0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-00005af0: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
-00005b00: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00005b10: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005b40: 5f63 656c 6c20 3d20 7365 6c66 2e65 6467  _cell = self.edg
-00005b50: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
-00005b60: 7461 7267 6574 5f63 656c 6c5d 5b30 5d0d  target_cell][0].
-00005b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005bc0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-00005bd0: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-00005be0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c10: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-00005c20: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
-00005c30: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-00005c40: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00005c70: 6c65 745f 636f 756e 745f 7461 6b65 6e2e  let_count_taken.
-00005c80: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-00005c90: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00005cc0: 6561 6b20 0d0a 2020 2020 2020 2020 2020  eak ..          
-00005cd0: 2020 2020 2020 2020 2020 2353 7461 7274            #Start
-00005ce0: 206f 6620 7472 6163 6b20 6973 2061 2064   of track is a d
-00005cf0: 6976 6964 696e 6720 6365 6c6c 2020 2020  ividing cell    
-00005d00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005d20: 6620 726f 6f74 5f61 6c6c 2069 6e20 7365  f root_all in se
-00005d30: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00005d40: 6f6f 6b75 7020 616e 6420 726f 6f74 5f61  ookup and root_a
-00005d50: 6c6c 2069 6e20 726f 6f74 5f73 706c 6974  ll in root_split
-00005d60: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005d70: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00005d80: 6765 745f 6365 6c6c 7320 3d20 7365 6c66  get_cells = self
-00005d90: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00005da0: 6b75 705b 726f 6f74 5f61 6c6c 5d0d 0a20  kup[root_all].. 
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2020 2020 6765 6e5f 636f 756e          gen_coun
-00005dd0: 7420 3d20 6765 6e5f 636f 756e 7420 2b20  t = gen_count + 
-00005de0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-00005df0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005e00: 6a20 696e 2072 616e 6765 286c 656e 2874  j in range(len(t
-00005e10: 6172 6765 745f 6365 6c6c 7329 293a 0d0a  arget_cells)):..
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 7461 7267 6574 5f63 656c 6c20 3d20 7461  target_cell = ta
-00005e50: 7267 6574 5f63 656c 6c73 5b6a 5d0d 0a20  rget_cells[j].. 
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005e80: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-00005e90: 7472 6163 6b6c 6574 5f63 6f75 6e74 202b  tracklet_count +
-00005ea0: 2031 202b 206a 0d0a 2020 2020 2020 2020   1 + j..        
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ec0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00005ed0: 5f63 6f75 6e74 203d 2073 656c 662e 5f75  _count = self._u
-00005ee0: 6e69 7175 655f 7472 6163 6b6c 6574 5f63  nique_tracklet_c
-00005ef0: 6f75 6e74 2874 7261 636b 6c65 745f 636f  ount(tracklet_co
-00005f00: 756e 745f 7461 6b65 6e2c 2074 7261 636b  unt_taken, track
-00005f10: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00005f40: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
-00005f50: 2e61 7070 656e 6428 7472 6163 6b6c 6574  .append(tracklet
-00005f60: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
-00005f90: 7465 7261 7465 5f64 6976 6964 696e 675f  terate_dividing_
-00005fa0: 7265 6375 7273 6976 6528 726f 6f74 5f6c  recursive(root_l
-00005fb0: 6561 662c 2074 6172 6765 745f 6365 6c6c  eaf, target_cell
-00005fc0: 2c20 726f 6f74 5f73 706c 6974 732c 2067  , root_splits, g
-00005fd0: 656e 5f63 6f75 6e74 2c20 7472 6163 6b6c  en_count, trackl
-00005fe0: 6574 5f63 6f75 6e74 2c20 7472 6163 6b6c  et_count, trackl
-00005ff0: 6574 5f63 6f75 6e74 5f74 616b 656e 290d  et_count_taken).
-00006000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006020: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00006050: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00006060: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
-00006070: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00006080: 2020 2020 2020 2020 736f 7274 6564 5f72          sorted_r
-00006090: 6f6f 745f 7370 6c69 7473 203d 2073 656c  oot_splits = sel
-000060a0: 662e 5f73 6f72 745f 6469 7669 6469 6e67  f._sort_dividing
-000060b0: 5f63 656c 6c73 2872 6f6f 745f 7370 6c69  _cells(root_spli
-000060c0: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-000060d0: 2020 2020 2020 2020 2066 6972 7374 5f73           first_s
-000060e0: 706c 6974 203d 2073 6f72 7465 645f 726f  plit = sorted_ro
-000060f0: 6f74 5f73 706c 6974 735b 305d 0d0a 2020  ot_splits[0]..  
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
-00006120: 6e5f 6469 6374 5b66 6972 7374 5f73 706c  n_dict[first_spl
-00006130: 6974 5d20 3d20 6765 6e5f 636f 756e 740d  it] = gen_count.
-00006140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006150: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-00006160: 6574 5f64 6963 745b 6669 7273 745f 7370  et_dict[first_sp
-00006170: 6c69 745d 203d 2074 7261 636b 6c65 745f  lit] = tracklet_
-00006180: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00006190: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-000061a0: 7273 745f 7370 6c69 7420 696e 2073 656c  rst_split in sel
-000061b0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-000061c0: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000061e0: 6172 6765 745f 6365 6c6c 7320 3d20 7365  arget_cells = se
-000061f0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00006200: 6f6f 6b75 705b 6669 7273 745f 7370 6c69  ookup[first_spli
-00006210: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
-00006220: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
-00006230: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
-00006240: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-00006250: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00006260: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00006270: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
-00006280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006290: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000062a0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-000062b0: 7472 6163 6b6c 6574 5f63 6f75 6e74 202b  tracklet_count +
-000062c0: 2031 202b 2069 0d0a 2020 2020 2020 2020   1 + i..        
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
-000062f0: 6e74 203d 2073 656c 662e 5f75 6e69 7175  nt = self._uniqu
-00006300: 655f 7472 6163 6b6c 6574 5f63 6f75 6e74  e_tracklet_count
-00006310: 2874 7261 636b 6c65 745f 636f 756e 745f  (tracklet_count_
-00006320: 7461 6b65 6e2c 2074 7261 636b 6c65 745f  taken, tracklet_
-00006330: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
-00006360: 6e74 5f74 616b 656e 2e61 7070 656e 6428  nt_taken.append(
-00006370: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
-00006380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006390: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-000063a0: 6765 745f 6365 6c6c 203d 2074 6172 6765  get_cell = targe
-000063b0: 745f 6365 6c6c 735b 695d 0d0a 2020 2020  t_cells[i]..    
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063d0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-000063e0: 6572 6174 655f 6469 7669 6469 6e67 5f72  erate_dividing_r
-000063f0: 6563 7572 7369 7665 2872 6f6f 745f 6c65  ecursive(root_le
-00006400: 6166 2c20 7461 7267 6574 5f63 656c 6c2c  af, target_cell,
-00006410: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
-00006420: 6974 732c 2067 656e 5f63 6f75 6e74 2c20  its, gen_count, 
-00006430: 7472 6163 6b6c 6574 5f63 6f75 6e74 2c20  tracklet_count, 
-00006440: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
-00006450: 616b 656e 290d 0a20 2020 2020 2020 2020  aken)..         
-00006460: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006470: 2064 6566 205f 756e 6971 7565 5f74 7261   def _unique_tra
-00006480: 636b 6c65 745f 636f 756e 7428 7365 6c66  cklet_count(self
-00006490: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-000064a0: 5f74 616b 656e 2c20 7472 6163 6b6c 6574  _taken, tracklet
-000064b0: 5f63 6f75 6e74 293a 0d0a 2020 2020 2020  _count):..      
-000064c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000064d0: 2020 7768 696c 6520 7472 6163 6b6c 6574    while tracklet
-000064e0: 5f63 6f75 6e74 2069 6e20 7472 6163 6b6c  _count in trackl
-000064f0: 6574 5f63 6f75 6e74 5f74 616b 656e 3a0d  et_count_taken:.
-00006500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006510: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
-00006520: 7420 203d 2074 7261 636b 6c65 745f 636f  t  = tracklet_co
-00006530: 756e 7420 2b20 3120 0d0a 2020 2020 2020  unt + 1 ..      
-00006540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006550: 2e5f 756e 6971 7565 5f74 7261 636b 6c65  ._unique_trackle
-00006560: 745f 636f 756e 7428 7472 6163 6b6c 6574  t_count(tracklet
-00006570: 5f63 6f75 6e74 5f74 616b 656e 2c20 7472  _count_taken, tr
-00006580: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
-00006590: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000065a0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-000065b0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
-000065c0: 6465 6620 5f69 7465 7261 7465 5f73 706c  def _iterate_spl
-000065d0: 6974 5f64 6f77 6e28 7365 6c66 2c20 726f  it_down(self, ro
-000065e0: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-000065f0: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-00006600: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
-00006610: 2020 2020 2020 7365 6c66 2e5f 6974 6572        self._iter
-00006620: 6174 655f 6469 7669 6469 6e67 2872 6f6f  ate_dividing(roo
-00006630: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
-00006640: 662c 2072 6f6f 745f 7370 6c69 7473 290d  f, root_splits).
-00006650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006660: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006680: 2020 0d0a 2020 2020 6465 6620 5f67 6574    ..    def _get
-00006690: 5f62 6f75 6e64 6172 795f 6469 7374 2873  _boundary_dist(s
-000066a0: 656c 662c 2066 7261 6d65 2c20 7465 7374  elf, frame, test
-000066b0: 6c6f 6361 7469 6f6e 293a 0d0a 2020 2020  location):..    
-000066c0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000066d0: 6620 7365 6c66 2e6d 6173 6b20 6973 206e  f self.mask is n
-000066e0: 6f74 204e 6f6e 653a 0d0a 0d0a 2020 2020  ot None:....    
-000066f0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00006700: 2c20 696e 6469 6365 732c 206d 6173 6b63  , indices, maskc
-00006710: 656e 7472 6f69 6420 3d20 7365 6c66 2e74  entroid = self.t
-00006720: 696d 6564 5f6d 6173 6b5b 7374 7228 696e  imed_mask[str(in
-00006730: 7428 666c 6f61 7428 6672 616d 6529 2929  t(float(frame)))
-00006740: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00006750: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006760: 2020 2020 2020 2020 2020 2020 2023 2047               # G
-00006770: 6574 2074 6865 206c 6f63 6174 696f 6e20  et the location 
-00006780: 616e 6420 6469 7374 616e 6365 2074 6f20  and distance to 
-00006790: 7468 6520 6e65 6172 6573 7420 626f 756e  the nearest boun
-000067a0: 6461 7279 2070 6f69 6e74 0d0a 2020 2020  dary point..    
-000067b0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-000067c0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
-000067d0: 6c6f 6361 7469 6f6e 696e 6465 7820 3d20  locationindex = 
-000067e0: 7472 6565 2e71 7565 7279 2874 6573 746c  tree.query(testl
-000067f0: 6f63 6174 696f 6e29 0d0a 2020 2020 2020  ocation)..      
-00006800: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-00006810: 6365 5f63 656c 6c5f 6d61 736b 203d 206d  ce_cell_mask = m
-00006820: 6178 2830 2c20 6469 7374 616e 6365 5f63  ax(0, distance_c
-00006830: 656c 6c5f 6d61 736b 290d 0a20 2020 2020  ell_mask)..     
-00006840: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006850: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00006860: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006870: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00006880: 6b20 3d20 300d 0a20 2020 2020 2020 2020  k = 0..         
-00006890: 2020 2020 2020 206d 6173 6b63 656e 7472         maskcentr
-000068a0: 6f69 6420 3d20 2831 2c31 2c31 290d 0a0d  oid = (1,1,1)...
-000068b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000068c0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000068d0: 736b 2c20 6d61 736b 6365 6e74 726f 6964  sk, maskcentroid
-000068e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000068f0: 2020 200d 0a20 2020 2064 6566 205f 676c     ..    def _gl
-00006900: 6f62 616c 5f74 7261 636b 5f69 6428 7365  obal_track_id(se
-00006910: 6c66 2c20 7472 6163 6b5f 6964 293a 0d0a  lf, track_id):..
-00006920: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006930: 2020 2020 206e 756d 5f64 6967 6974 7320       num_digits 
-00006940: 3d20 6c65 6e28 7374 7228 7365 6c66 2e6d  = len(str(self.m
-00006950: 6178 5f74 7261 636b 5f64 6967 6974 2929  ax_track_digit))
-00006960: 0d0a 0d0a 2020 2020 2020 2020 7472 6163  ....        trac
-00006970: 6b5f 6964 5f73 7472 203d 2073 7472 2874  k_id_str = str(t
-00006980: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-00006990: 2020 6966 206c 656e 2874 7261 636b 5f69    if len(track_i
-000069a0: 645f 7374 7229 203c 206e 756d 5f64 6967  d_str) < num_dig
-000069b0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-000069c0: 2020 2074 7261 636b 5f69 645f 7374 7220     track_id_str 
-000069d0: 3d20 7472 6163 6b5f 6964 5f73 7472 2e7a  = track_id_str.z
-000069e0: 6669 6c6c 286e 756d 5f64 6967 6974 7329  fill(num_digits)
-000069f0: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-00006a00: 6964 203d 2069 6e74 2874 7261 636b 5f69  id = int(track_i
-00006a10: 645f 7374 7229 0d0a 2020 2020 2020 2020  d_str)..        
-00006a20: 7265 7475 726e 2074 7261 636b 5f69 640d  return track_id.
-00006a30: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
-00006a40: 676c 6f62 616c 5f67 656e 6572 6174 696f  global_generatio
-00006a50: 6e5f 6964 2873 656c 662c 2067 656e 6572  n_id(self, gener
-00006a60: 6174 696f 6e5f 6964 293a 0d0a 2020 2020  ation_id):..    
-00006a70: 2020 2020 0d0a 2020 2020 2020 2020 6e75      ..        nu
-00006a80: 6d5f 6469 6769 7473 203d 206c 656e 2873  m_digits = len(s
-00006a90: 7472 2873 656c 662e 6d61 785f 7472 6163  tr(self.max_trac
-00006aa0: 6b5f 6469 6769 7429 290d 0a20 2020 2020  k_digit))..     
-00006ab0: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
-00006ac0: 5f73 7472 203d 2073 7472 2867 656e 6572  _str = str(gener
-00006ad0: 6174 696f 6e5f 6964 290d 0a20 2020 2020  ation_id)..     
-00006ae0: 2020 2069 6620 6c65 6e28 6765 6e65 7261     if len(genera
-00006af0: 7469 6f6e 5f69 645f 7374 7229 203c 206e  tion_id_str) < n
-00006b00: 756d 5f64 6967 6974 733a 0d0a 2020 2020  um_digits:..    
-00006b10: 2020 2020 2020 2020 2020 2020 6765 6e65              gene
-00006b20: 7261 7469 6f6e 5f69 645f 7374 7220 3d20  ration_id_str = 
-00006b30: 6765 6e65 7261 7469 6f6e 5f69 645f 7374  generation_id_st
-00006b40: 722e 7a66 696c 6c28 6e75 6d5f 6469 6769  r.zfill(num_digi
-00006b50: 7473 290d 0a20 2020 2020 2020 2067 656e  ts)..        gen
-00006b60: 6572 6174 696f 6e5f 6964 203d 2069 6e74  eration_id = int
-00006b70: 2867 656e 6572 6174 696f 6e5f 6964 5f73  (generation_id_s
-00006b80: 7472 290d 0a0d 0a20 2020 2020 2020 2072  tr)....        r
-00006b90: 6574 7572 6e20 6765 6e65 7261 7469 6f6e  eturn generation
-00006ba0: 5f69 640d 0a0d 0a0d 0a20 2020 2064 6566  _id......    def
-00006bb0: 205f 7472 6163 6b5f 636f 6d70 7574 6572   _track_computer
-00006bc0: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
-00006bd0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00006c40: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 2020 756e 6971 7565 5f74 7261        unique_tra
-00006c70: 636b 6c65 745f 6964 7320 3d20 5b5d 0d0a  cklet_ids = []..
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00006ca0: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-00006cb0: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-00006cc0: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-00006cd0: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-00006ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006cf0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00006d00: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-00006d10: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-00006d20: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-00006d30: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-00006d40: 7572 6365 5f69 6473 2920 0d0a 2020 2020  urce_ids) ..    
-00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d60: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00006d70: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
-00006d80: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
-00006d90: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-00006da0: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00006de0: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
-00006df0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00006e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006e20: 4465 7465 726d 696e 6520 6966 2061 2074  Determine if a t
-00006e30: 7261 636b 2068 6173 2064 6976 6973 696f  rack has divisio
-00006e40: 6e73 206f 7220 6e6f 6e65 0d0a 2020 2020  ns or none..    
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00006e70: 6f6f 745f 7370 6c69 7473 2920 3e20 303a  oot_splits) > 0:
-00006e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ea0: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
-00006eb0: 6163 6b5f 6d69 746f 7369 735f 6c61 6265  ack_mitosis_labe
-00006ec0: 6c5b 7472 6163 6b5f 6964 5d20 3d20 5b31  l[track_id] = [1
-00006ed0: 2c20 6e75 6d62 6572 5f64 6976 6964 696e  , number_dividin
-00006ee0: 675d 0d0a 2020 2020 2020 2020 2020 2020  g]..            
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
-00006f10: 6a65 6374 6f72 7920 3d20 5472 7565 0d0a  jectory = True..
-00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-00006f50: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
-00006f60: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
-00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006f90: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-00006fa0: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
-00006fb0: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
-00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fd0: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-00006fe0: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
-00006ff0: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-00007000: 6b49 6473 3a20 2020 2020 0d0a 2020 2020  kIds:     ..    
-00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-00007040: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
-00007050: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 2020 2020 6966 206e 6578 745f 7461 7267      if next_targ
+00005470: 6574 5f63 656c 6c20 696e 2073 656c 662e  et_cell in self.
+00005480: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
+00005490: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054b0: 2074 6172 6765 745f 6365 6c6c 7320 3d20   target_cells = 
+000054c0: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+000054d0: 5f6c 6f6f 6b75 705b 6e65 7874 5f74 6172  _lookup[next_tar
+000054e0: 6765 745f 6365 6c6c 5d0d 0a20 2020 2020  get_cell]..     
+000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005500: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00005510: 7261 6e67 6528 6c65 6e28 7461 7267 6574  range(len(target
+00005520: 5f63 656c 6c73 2929 3a0d 0a20 2020 2020  _cells)):..     
+00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005540: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+00005550: 745f 6365 6c6c 203d 2074 6172 6765 745f  t_cell = target_
+00005560: 6365 6c6c 735b 6b5d 0d0a 2020 2020 2020  cells[k]..      
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
+00005590: 6574 5f63 6f75 6e74 203d 2074 7261 636b  et_count = track
+000055a0: 6c65 745f 636f 756e 7420 2b20 3120 2b20  let_count + 1 + 
+000055b0: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055d0: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
+000055e0: 7420 3d20 7365 6c66 2e5f 756e 6971 7565  t = self._unique
+000055f0: 5f74 7261 636b 6c65 745f 636f 756e 7428  _tracklet_count(
+00005600: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
+00005610: 616b 656e 2c20 7472 6163 6b6c 6574 5f63  aken, tracklet_c
+00005620: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+00005650: 636f 756e 745f 7461 6b65 6e2e 6170 7065  count_taken.appe
+00005660: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
+00005670: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 2020 2020 7365 6c66 2e5f 6974 6572 6174      self._iterat
+000056a0: 655f 6469 7669 6469 6e67 5f72 6563 7572  e_dividing_recur
+000056b0: 7369 7665 2872 6f6f 745f 6c65 6166 2c20  sive(root_leaf, 
+000056c0: 7461 7267 6574 5f63 656c 6c2c 2073 6f72  target_cell, sor
+000056d0: 7465 645f 726f 6f74 5f73 706c 6974 732c  ted_root_splits,
+000056e0: 206e 6578 745f 6765 6e5f 636f 756e 742c   next_gen_count,
+000056f0: 2074 7261 636b 6c65 745f 636f 756e 742c   tracklet_count,
+00005700: 2074 7261 636b 6c65 745f 636f 756e 745f   tracklet_count_
+00005710: 7461 6b65 6e29 2020 2020 2020 0d0a 0d0a  taken)      ....
+00005720: 0d0a 0d0a 2020 2020 6465 6620 5f69 7465  ....    def _ite
+00005730: 7261 7465 5f64 6976 6964 696e 6728 7365  rate_dividing(se
+00005740: 6c66 2c20 726f 6f74 5f72 6f6f 742c 2072  lf, root_root, r
+00005750: 6f6f 745f 6c65 6166 2c20 726f 6f74 5f73  oot_leaf, root_s
+00005760: 706c 6974 7329 3a0d 0a20 2020 2020 2020  plits):..       
+00005770: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005780: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005790: 6765 6e5f 636f 756e 7420 3d20 300d 0a20  gen_count = 0.. 
+000057a0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+000057b0: 6c65 745f 636f 756e 7420 3d20 300d 0a20  let_count = 0.. 
+000057c0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+000057d0: 6c65 745f 636f 756e 745f 7461 6b65 6e20  let_count_taken 
+000057e0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000057f0: 2020 666f 7220 726f 6f74 5f61 6c6c 2069    for root_all i
+00005800: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
+00005830: 6e5f 6469 6374 5b72 6f6f 745f 616c 6c5d  n_dict[root_all]
+00005840: 203d 2067 656e 5f63 6f75 6e74 0d0a 2020   = gen_count..  
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
+00005870: 6469 6374 5b72 6f6f 745f 616c 6c5d 203d  dict[root_all] =
+00005880: 2074 7261 636b 6c65 745f 636f 756e 740d   tracklet_count.
+00005890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058a0: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+000058b0: 756e 745f 7461 6b65 6e2e 6170 7065 6e64  unt_taken.append
+000058c0: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+000058d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000058e0: 2020 2020 2020 6966 2072 6f6f 745f 616c        if root_al
+000058f0: 6c20 696e 2073 656c 662e 6564 6765 5f74  l in self.edge_t
+00005900: 6172 6765 745f 6c6f 6f6b 7570 2061 6e64  arget_lookup and
+00005910: 2072 6f6f 745f 616c 6c20 6e6f 7420 696e   root_all not in
+00005920: 2072 6f6f 745f 7370 6c69 7473 3a0d 0a20   root_splits:.. 
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 2020 2020 7461 7267 6574 5f63          target_c
+00005950: 656c 6c20 3d20 7365 6c66 2e65 6467 655f  ell = self.edge_
+00005960: 7461 7267 6574 5f6c 6f6f 6b75 705b 726f  target_lookup[ro
+00005970: 6f74 5f61 6c6c 5d5b 305d 0d0a 2020 2020  ot_all][0]..    
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 2020 2077 6869 6c65 2074 6172 6765       while targe
+000059a0: 745f 6365 6c6c 206e 6f74 2069 6e20 726f  t_cell not in ro
+000059b0: 6f74 5f73 706c 6974 733a 0d0a 2020 2020  ot_splits:..    
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+000059e0: 6172 6765 745f 6365 6c6c 2069 6e20 7365  arget_cell in se
+000059f0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00005a00: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005a30: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
+00005a40: 5b74 6172 6765 745f 6365 6c6c 5d20 3d20  [target_cell] = 
+00005a50: 6765 6e5f 636f 756e 740d 0a20 2020 2020  gen_count..     
+00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005a80: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+00005a90: 745b 7461 7267 6574 5f63 656c 6c5d 203d  t[target_cell] =
+00005aa0: 2074 7261 636b 6c65 745f 636f 756e 740d   tracklet_count.
+00005ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+00005ae0: 756e 745f 7461 6b65 6e2e 6170 7065 6e64  unt_taken.append
+00005af0: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+00005b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00005b30: 6c20 3d20 7365 6c66 2e65 6467 655f 7461  l = self.edge_ta
+00005b40: 7267 6574 5f6c 6f6f 6b75 705b 7461 7267  rget_lookup[targ
+00005b50: 6574 5f63 656c 6c5d 5b30 5d0d 0a20 2020  et_cell][0]..   
+00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b70: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00005b80: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00005bb0: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
+00005bc0: 6172 6765 745f 6365 6c6c 5d20 3d20 6765  arget_cell] = ge
+00005bd0: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
+00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005c00: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+00005c10: 745b 7461 7267 6574 5f63 656c 6c5d 203d  t[target_cell] =
+00005c20: 2074 7261 636b 6c65 745f 636f 756e 740d   tracklet_count.
+00005c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+00005c60: 636f 756e 745f 7461 6b65 6e2e 6170 7065  count_taken.appe
+00005c70: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
+00005c80: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 2020 2020 2020 2020 6272 6561 6b20            break 
+00005cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005cc0: 2020 2020 2020 2353 7461 7274 206f 6620        #Start of 
+00005cd0: 7472 6163 6b20 6973 2061 2064 6976 6964  track is a divid
+00005ce0: 696e 6720 6365 6c6c 2020 2020 2020 2020  ing cell        
+00005cf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00005d00: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+00005d10: 6f74 5f61 6c6c 2069 6e20 7365 6c66 2e65  ot_all in self.e
+00005d20: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+00005d30: 7020 616e 6420 726f 6f74 5f61 6c6c 2069  p and root_all i
+00005d40: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00005d70: 6365 6c6c 7320 3d20 7365 6c66 2e65 6467  cells = self.edg
+00005d80: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
+00005d90: 726f 6f74 5f61 6c6c 5d0d 0a20 2020 2020  root_all]..     
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
+00005dc0: 6765 6e5f 636f 756e 7420 2b20 310d 0a20  gen_count + 1.. 
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00005df0: 2072 616e 6765 286c 656e 2874 6172 6765   range(len(targe
+00005e00: 745f 6365 6c6c 7329 293a 0d0a 2020 2020  t_cells)):..    
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00005e30: 6574 5f63 656c 6c20 3d20 7461 7267 6574  et_cell = target
+00005e40: 5f63 656c 6c73 5b6a 5d0d 0a20 2020 2020  _cells[j]..     
+00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e60: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00005e70: 6c65 745f 636f 756e 7420 3d20 7472 6163  let_count = trac
+00005e80: 6b6c 6574 5f63 6f75 6e74 202b 2031 202b  klet_count + 1 +
+00005e90: 206a 0d0a 2020 2020 2020 2020 2020 2020   j..            
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00005ec0: 6e74 203d 2073 656c 662e 5f75 6e69 7175  nt = self._uniqu
+00005ed0: 655f 7472 6163 6b6c 6574 5f63 6f75 6e74  e_tracklet_count
+00005ee0: 2874 7261 636b 6c65 745f 636f 756e 745f  (tracklet_count_
+00005ef0: 7461 6b65 6e2c 2074 7261 636b 6c65 745f  taken, tracklet_
+00005f00: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
+00005f30: 5f63 6f75 6e74 5f74 616b 656e 2e61 7070  _count_taken.app
+00005f40: 656e 6428 7472 6163 6b6c 6574 5f63 6f75  end(tracklet_cou
+00005f50: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
+00005f80: 7465 5f64 6976 6964 696e 675f 7265 6375  te_dividing_recu
+00005f90: 7273 6976 6528 726f 6f74 5f6c 6561 662c  rsive(root_leaf,
+00005fa0: 2074 6172 6765 745f 6365 6c6c 2c20 726f   target_cell, ro
+00005fb0: 6f74 5f73 706c 6974 732c 2067 656e 5f63  ot_splits, gen_c
+00005fc0: 6f75 6e74 2c20 7472 6163 6b6c 6574 5f63  ount, tracklet_c
+00005fd0: 6f75 6e74 2c20 7472 6163 6b6c 6574 5f63  ount, tracklet_c
+00005fe0: 6f75 6e74 5f74 616b 656e 290d 0a20 2020  ount_taken)..   
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006030: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006040: 2020 2020 2020 6966 206c 656e 2872 6f6f        if len(roo
+00006050: 745f 7370 6c69 7473 2920 3e20 303a 0d0a  t_splits) > 0:..
+00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006070: 2020 2020 736f 7274 6564 5f72 6f6f 745f      sorted_root_
+00006080: 7370 6c69 7473 203d 2073 656c 662e 5f73  splits = self._s
+00006090: 6f72 745f 6469 7669 6469 6e67 5f63 656c  ort_dividing_cel
+000060a0: 6c73 2872 6f6f 745f 7370 6c69 7473 290d  ls(root_splits).
+000060b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000060c0: 2020 2020 2066 6972 7374 5f73 706c 6974       first_split
+000060d0: 203d 2073 6f72 7465 645f 726f 6f74 5f73   = sorted_root_s
+000060e0: 706c 6974 735b 305d 0d0a 2020 2020 2020  plits[0]..      
+000060f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006100: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00006110: 6374 5b66 6972 7374 5f73 706c 6974 5d20  ct[first_split] 
+00006120: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
+00006150: 6963 745b 6669 7273 745f 7370 6c69 745d  ict[first_split]
+00006160: 203d 2074 7261 636b 6c65 745f 636f 756e   = tracklet_coun
+00006170: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00006180: 2020 2020 2020 2069 6620 6669 7273 745f         if first_
+00006190: 7370 6c69 7420 696e 2073 656c 662e 6564  split in self.ed
+000061a0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+000061b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000061c0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+000061d0: 745f 6365 6c6c 7320 3d20 7365 6c66 2e65  t_cells = self.e
+000061e0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+000061f0: 705b 6669 7273 745f 7370 6c69 745d 0d0a  p[first_split]..
+00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006210: 2020 2020 2020 2020 6765 6e5f 636f 756e          gen_coun
+00006220: 7420 3d20 6765 6e5f 636f 756e 7420 2b20  t = gen_count + 
+00006230: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+00006240: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00006250: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+00006260: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00006290: 6c65 745f 636f 756e 7420 3d20 7472 6163  let_count = trac
+000062a0: 6b6c 6574 5f63 6f75 6e74 202b 2031 202b  klet_count + 1 +
+000062b0: 2069 0d0a 2020 2020 2020 2020 2020 2020   i..            
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062d0: 7472 6163 6b6c 6574 5f63 6f75 6e74 203d  tracklet_count =
+000062e0: 2073 656c 662e 5f75 6e69 7175 655f 7472   self._unique_tr
+000062f0: 6163 6b6c 6574 5f63 6f75 6e74 2874 7261  acklet_count(tra
+00006300: 636b 6c65 745f 636f 756e 745f 7461 6b65  cklet_count_take
+00006310: 6e2c 2074 7261 636b 6c65 745f 636f 756e  n, tracklet_coun
+00006320: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006340: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
+00006350: 616b 656e 2e61 7070 656e 6428 7472 6163  aken.append(trac
+00006360: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006380: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00006390: 6365 6c6c 203d 2074 6172 6765 745f 6365  cell = target_ce
+000063a0: 6c6c 735b 695d 0d0a 2020 2020 2020 2020  lls[i]..        
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 7365 6c66 2e5f 6974 6572 6174      self._iterat
+000063d0: 655f 6469 7669 6469 6e67 5f72 6563 7572  e_dividing_recur
+000063e0: 7369 7665 2872 6f6f 745f 6c65 6166 2c20  sive(root_leaf, 
+000063f0: 7461 7267 6574 5f63 656c 6c2c 2073 6f72  target_cell, sor
+00006400: 7465 645f 726f 6f74 5f73 706c 6974 732c  ted_root_splits,
+00006410: 2067 656e 5f63 6f75 6e74 2c20 7472 6163   gen_count, trac
+00006420: 6b6c 6574 5f63 6f75 6e74 2c20 7472 6163  klet_count, trac
+00006430: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
+00006440: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006450: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00006460: 205f 756e 6971 7565 5f74 7261 636b 6c65   _unique_trackle
+00006470: 745f 636f 756e 7428 7365 6c66 2c20 7472  t_count(self, tr
+00006480: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
+00006490: 656e 2c20 7472 6163 6b6c 6574 5f63 6f75  en, tracklet_cou
+000064a0: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
+000064b0: 200d 0a20 2020 2020 2020 2020 2020 7768   ..           wh
+000064c0: 696c 6520 7472 6163 6b6c 6574 5f63 6f75  ile tracklet_cou
+000064d0: 6e74 2069 6e20 7472 6163 6b6c 6574 5f63  nt in tracklet_c
+000064e0: 6f75 6e74 5f74 616b 656e 3a0d 0a20 2020  ount_taken:..   
+000064f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00006500: 7261 636b 6c65 745f 636f 756e 7420 203d  racklet_count  =
+00006510: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
+00006520: 2b20 3120 0d0a 2020 2020 2020 2020 2020  + 1 ..          
+00006530: 2020 2020 2020 2020 7365 6c66 2e5f 756e          self._un
+00006540: 6971 7565 5f74 7261 636b 6c65 745f 636f  ique_tracklet_co
+00006550: 756e 7428 7472 6163 6b6c 6574 5f63 6f75  unt(tracklet_cou
+00006560: 6e74 5f74 616b 656e 2c20 7472 6163 6b6c  nt_taken, trackl
+00006570: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00006580: 2020 2020 2020 7265 7475 726e 2074 7261        return tra
+00006590: 636b 6c65 745f 636f 756e 7420 2020 2020  cklet_count     
+000065a0: 2020 0d0a 0d0a 0d0a 2020 2020 6465 6620    ......    def 
+000065b0: 5f69 7465 7261 7465 5f73 706c 6974 5f64  _iterate_split_d
+000065c0: 6f77 6e28 7365 6c66 2c20 726f 6f74 5f72  own(self, root_r
+000065d0: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
+000065e0: 726f 6f74 5f73 706c 6974 7329 3a0d 0a20  root_splits):.. 
+000065f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006600: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+00006610: 6469 7669 6469 6e67 2872 6f6f 745f 726f  dividing(root_ro
+00006620: 6f74 2c20 726f 6f74 5f6c 6561 662c 2072  ot, root_leaf, r
+00006630: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
+00006640: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006660: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00006670: 2020 2020 6465 6620 5f67 6574 5f62 6f75      def _get_bou
+00006680: 6e64 6172 795f 6469 7374 2873 656c 662c  ndary_dist(self,
+00006690: 2066 7261 6d65 2c20 7465 7374 6c6f 6361   frame, testloca
+000066a0: 7469 6f6e 293a 0d0a 2020 2020 2020 2020  tion):..        
+000066b0: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
+000066c0: 6c66 2e6d 6173 6b20 6973 206e 6f74 204e  lf.mask is not N
+000066d0: 6f6e 653a 0d0a 0d0a 2020 2020 2020 2020  one:....        
+000066e0: 2020 2020 2020 2020 7472 6565 2c20 696e          tree, in
+000066f0: 6469 6365 732c 206d 6173 6b63 656e 7472  dices, maskcentr
+00006700: 6f69 6420 3d20 7365 6c66 2e74 696d 6564  oid = self.timed
+00006710: 5f6d 6173 6b5b 7374 7228 696e 7428 666c  _mask[str(int(fl
+00006720: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
+00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006740: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006750: 2020 2020 2020 2020 2023 2047 6574 2074           # Get t
+00006760: 6865 206c 6f63 6174 696f 6e20 616e 6420  he location and 
+00006770: 6469 7374 616e 6365 2074 6f20 7468 6520  distance to the 
+00006780: 6e65 6172 6573 7420 626f 756e 6461 7279  nearest boundary
+00006790: 2070 6f69 6e74 0d0a 2020 2020 2020 2020   point..        
+000067a0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+000067b0: 5f63 656c 6c5f 6d61 736b 2c20 6c6f 6361  _cell_mask, loca
+000067c0: 7469 6f6e 696e 6465 7820 3d20 7472 6565  tionindex = tree
+000067d0: 2e71 7565 7279 2874 6573 746c 6f63 6174  .query(testlocat
+000067e0: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+000067f0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+00006800: 656c 6c5f 6d61 736b 203d 206d 6178 2830  ell_mask = max(0
+00006810: 2c20 6469 7374 616e 6365 5f63 656c 6c5f  , distance_cell_
+00006820: 6d61 736b 290d 0a20 2020 2020 2020 2020  mask)..         
+00006830: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006840: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00006850: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+00006860: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00006870: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00006880: 2020 206d 6173 6b63 656e 7472 6f69 6420     maskcentroid 
+00006890: 3d20 2831 2c31 2c31 290d 0a0d 0a20 2020  = (1,1,1)....   
+000068a0: 2020 2020 2072 6574 7572 6e20 6469 7374       return dist
+000068b0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+000068c0: 6d61 736b 6365 6e74 726f 6964 2020 2020  maskcentroid    
+000068d0: 2020 2020 0d0a 2020 2020 2020 2020 200d      ..         .
+000068e0: 0a20 2020 2064 6566 205f 676c 6f62 616c  .    def _global
+000068f0: 5f74 7261 636b 5f69 6428 7365 6c66 2c20  _track_id(self, 
+00006900: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
+00006910: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00006920: 206e 756d 5f64 6967 6974 7320 3d20 6c65   num_digits = le
+00006930: 6e28 7374 7228 7365 6c66 2e6d 6178 5f74  n(str(self.max_t
+00006940: 7261 636b 5f64 6967 6974 2929 0d0a 0d0a  rack_digit))....
+00006950: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+00006960: 5f73 7472 203d 2073 7472 2874 7261 636b  _str = str(track
+00006970: 5f69 6429 0d0a 2020 2020 2020 2020 6966  _id)..        if
+00006980: 206c 656e 2874 7261 636b 5f69 645f 7374   len(track_id_st
+00006990: 7229 203c 206e 756d 5f64 6967 6974 733a  r) < num_digits:
+000069a0: 0d0a 2020 2020 2020 2020 2020 2020 2074  ..             t
+000069b0: 7261 636b 5f69 645f 7374 7220 3d20 7472  rack_id_str = tr
+000069c0: 6163 6b5f 6964 5f73 7472 2e7a 6669 6c6c  ack_id_str.zfill
+000069d0: 286e 756d 5f64 6967 6974 7329 0d0a 2020  (num_digits)..  
+000069e0: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+000069f0: 2069 6e74 2874 7261 636b 5f69 645f 7374   int(track_id_st
+00006a00: 7229 0d0a 2020 2020 2020 2020 7265 7475  r)..        retu
+00006a10: 726e 2074 7261 636b 5f69 640d 0a20 2020  rn track_id..   
+00006a20: 200d 0a20 2020 2064 6566 205f 676c 6f62   ..    def _glob
+00006a30: 616c 5f67 656e 6572 6174 696f 6e5f 6964  al_generation_id
+00006a40: 2873 656c 662c 2067 656e 6572 6174 696f  (self, generatio
+00006a50: 6e5f 6964 293a 0d0a 2020 2020 2020 2020  n_id):..        
+00006a60: 0d0a 2020 2020 2020 2020 6e75 6d5f 6469  ..        num_di
+00006a70: 6769 7473 203d 206c 656e 2873 7472 2873  gits = len(str(s
+00006a80: 656c 662e 6d61 785f 7472 6163 6b5f 6469  elf.max_track_di
+00006a90: 6769 7429 290d 0a20 2020 2020 2020 2067  git))..        g
+00006aa0: 656e 6572 6174 696f 6e5f 6964 5f73 7472  eneration_id_str
+00006ab0: 203d 2073 7472 2867 656e 6572 6174 696f   = str(generatio
+00006ac0: 6e5f 6964 290d 0a20 2020 2020 2020 2069  n_id)..        i
+00006ad0: 6620 6c65 6e28 6765 6e65 7261 7469 6f6e  f len(generation
+00006ae0: 5f69 645f 7374 7229 203c 206e 756d 5f64  _id_str) < num_d
+00006af0: 6967 6974 733a 0d0a 2020 2020 2020 2020  igits:..        
+00006b00: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+00006b10: 6f6e 5f69 645f 7374 7220 3d20 6765 6e65  on_id_str = gene
+00006b20: 7261 7469 6f6e 5f69 645f 7374 722e 7a66  ration_id_str.zf
+00006b30: 696c 6c28 6e75 6d5f 6469 6769 7473 290d  ill(num_digits).
+00006b40: 0a20 2020 2020 2020 2067 656e 6572 6174  .        generat
+00006b50: 696f 6e5f 6964 203d 2069 6e74 2867 656e  ion_id = int(gen
+00006b60: 6572 6174 696f 6e5f 6964 5f73 7472 290d  eration_id_str).
+00006b70: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00006b80: 6e20 6765 6e65 7261 7469 6f6e 5f69 640d  n generation_id.
+00006b90: 0a0d 0a0d 0a20 2020 2064 6566 205f 7472  .....    def _tr
+00006ba0: 6163 6b5f 636f 6d70 7574 6572 2873 656c  ack_computer(sel
+00006bb0: 662c 2074 7261 636b 2c20 7472 6163 6b5f  f, track, track_
+00006bc0: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006c10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00006c20: 7572 7265 6e74 5f63 656c 6c5f 6964 7320  urrent_cell_ids 
+00006c30: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c50: 2020 756e 6971 7565 5f74 7261 636b 6c65    unique_trackle
+00006c60: 745f 6964 7320 3d20 5b5d 0d0a 2020 2020  t_ids = []..    
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c80: 2020 2020 2020 2020 7472 6163 6b5f 6469          track_di
+00006c90: 7370 6c61 6365 6d65 6e74 2c74 6f74 616c  splacement,total
+00006ca0: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
+00006cb0: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
+00006cc0: 6e63 652c 2074 7261 636b 5f64 7572 6174  nce, track_durat
+00006cd0: 696f 6e20 203d 2020 7365 6c66 2e5f 6765  ion  =  self._ge
+00006ce0: 745f 7472 6163 6b5f 6665 6174 7572 6573  t_track_features
+00006cf0: 2874 7261 636b 290d 0a0d 0a20 2020 2020  (track)....     
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 2020 2020 2020 2061 6c6c 5f73 6f75 7263         all_sourc
+00006d20: 655f 6964 732c 2061 6c6c 5f74 6172 6765  e_ids, all_targe
+00006d30: 745f 6964 7320 3d20 2073 656c 662e 5f67  t_ids =  self._g
+00006d40: 656e 6572 6174 655f 6765 6e65 7261 7469  enerate_generati
+00006d50: 6f6e 7328 7472 6163 6b29 0d0a 2020 2020  ons(track)..    
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
+00006d80: 742c 2072 6f6f 745f 7370 6c69 7473 2c20  t, root_splits, 
+00006d90: 726f 6f74 5f6c 6561 6620 3d20 7365 6c66  root_leaf = self
+00006da0: 2e5f 6372 6561 7465 5f67 656e 6572 6174  ._create_generat
+00006db0: 696f 6e73 2861 6c6c 5f73 6f75 7263 655f  ions(all_source_
+00006dc0: 6964 7329 200d 0a20 2020 2020 2020 2020  ids) ..         
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
+00006df0: 5f73 706c 6974 5f64 6f77 6e28 726f 6f74  _split_down(root
+00006e00: 5f72 6f6f 742c 2072 6f6f 745f 6c65 6166  _root, root_leaf
+00006e10: 2c20 726f 6f74 5f73 706c 6974 7329 0d0a  , root_splits)..
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e50: 2020 2020 2020 2020 206e 756d 6265 725f           number_
+00006e60: 6469 7669 6469 6e67 203d 206c 656e 2872  dividing = len(r
+00006e70: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e90: 2020 2020 2020 2020 2023 2044 6574 6572           # Deter
+00006ea0: 6d69 6e65 2069 6620 6120 7472 6163 6b20  mine if a track 
+00006eb0: 6861 7320 6469 7669 7369 6f6e 7320 6f72  has divisions or
+00006ec0: 206e 6f6e 650d 0a20 2020 2020 2020 2020   none..         
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ee0: 2020 2069 6620 6c65 6e28 726f 6f74 5f73     if len(root_s
+00006ef0: 706c 6974 7329 203e 2030 3a0d 0a20 2020  plits) > 0:..   
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006f20: 662e 756e 6971 7565 5f74 7261 636b 5f6d  f.unique_track_m
+00006f30: 6974 6f73 6973 5f6c 6162 656c 5b74 7261  itosis_label[tra
+00006f40: 636b 5f69 645d 203d 205b 312c 206e 756d  ck_id] = [1, num
+00006f50: 6265 725f 6469 7669 6469 6e67 5d0d 0a20  ber_dividing].. 
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006f80: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00006f90: 7279 203d 2054 7275 650d 0a20 2020 2020  ry = True..     
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00006fc0: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
+00006fd0: 696e 2073 656c 662e 416c 6c54 7261 636b  in self.AllTrack
+00006fe0: 4964 733a 0d0a 2020 2020 2020 2020 2020  Ids:..          
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00007010: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+00007020: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+00007030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
+00007060: 6429 206e 6f74 2069 6e20 7365 6c66 2e44  d) not in self.D
+00007070: 6976 6964 696e 6754 7261 636b 4964 733a  ividingTrackIds:
 00007080: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000070d0: 6e69 7175 655f 7472 6163 6b5f 6d69 746f  nique_track_mito
-000070e0: 7369 735f 6c61 6265 6c5b 7472 6163 6b5f  sis_label[track_
-000070f0: 6964 5d20 3d20 5b30 2c20 305d 0d0a 2020  id] = [0, 0]..  
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00007120: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00007130: 7920 3d20 4661 6c73 650d 0a20 2020 2020  y = False..     
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00007160: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
-00007170: 696e 2073 656c 662e 416c 6c54 7261 636b  in self.AllTrack
-00007180: 4964 733a 0d0a 2020 2020 2020 2020 2020  Ids:..          
-00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071a0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-000071b0: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-000071c0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
-000071d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
-00007200: 6429 206e 6f74 2069 6e20 7365 6c66 2e4e  d) not in self.N
-00007210: 6f72 6d61 6c54 7261 636b 4964 733a 2020  ormalTrackIds:  
-00007220: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007240: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-00007250: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-00007260: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00007270: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007290: 2066 6f72 206c 6561 6620 696e 2072 6f6f   for leaf in roo
-000072a0: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
+000070a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000070b0: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+000070c0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+000070d0: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007110: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00007120: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007150: 5f74 7261 636b 5f6d 6974 6f73 6973 5f6c  _track_mitosis_l
+00007160: 6162 656c 5b74 7261 636b 5f69 645d 203d  abel[track_id] =
+00007170: 205b 302c 2030 5d0d 0a20 2020 2020 2020   [0, 0]..       
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+000071a0: 675f 7472 616a 6563 746f 7279 203d 2046  g_trajectory = F
+000071b0: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071d0: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
+000071e0: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
+000071f0: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
+00007200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007220: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+00007230: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+00007240: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007270: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
+00007280: 7420 696e 2073 656c 662e 4e6f 726d 616c  t in self.Normal
+00007290: 5472 6163 6b49 6473 3a20 2020 200d 0a20  TrackIds:    .. 
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-000072d0: 6365 5f6c 6561 6620 3d20 7365 6c66 2e65  ce_leaf = self.e
-000072e0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-000072f0: 705b 6c65 6166 5d0d 0a20 2020 2020 2020  p[leaf]..       
-00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00007320: 656e 745f 6365 6c6c 5f69 6473 2e61 7070  ent_cell_ids.app
-00007330: 656e 6428 6c65 6166 2920 0d0a 2020 2020  end(leaf) ..    
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007360: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
-00007370: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
-00007380: 5f69 6473 2c20 6c65 6166 2c20 7472 6163  _ids, leaf, trac
-00007390: 6b5f 6964 2c20 736f 7572 6365 5f6c 6561  k_id, source_lea
-000073a0: 662c 204e 6f6e 6529 0d0a 2020 2020 2020  f, None)..      
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000073d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000073e0: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
-000073f0: 7064 6174 6528 7b73 656c 662e 6469 7669  pdate({self.divi
-00007400: 6469 6e67 5f6b 6579 203a 2064 6976 6964  ding_key : divid
-00007410: 696e 675f 7472 616a 6563 746f 7279 7d29  ing_trajectory})
-00007420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000072c0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+000072d0: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
+000072e0: 7428 7472 6163 6b5f 6964 2929 0d0a 0d0a  t(track_id))....
+000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007300: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007310: 6c65 6166 2069 6e20 726f 6f74 5f6c 6561  leaf in root_lea
+00007320: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 2020 2073 6f75 7263 655f 6c65         source_le
+00007350: 6166 203d 2073 656c 662e 6564 6765 5f73  af = self.edge_s
+00007360: 6f75 7263 655f 6c6f 6f6b 7570 5b6c 6561  ource_lookup[lea
+00007370: 665d 0d0a 2020 2020 2020 2020 2020 2020  f]..            
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000073a0: 656c 6c5f 6964 732e 6170 7065 6e64 286c  ell_ids.append(l
+000073b0: 6561 6629 200d 0a20 2020 2020 2020 2020  eaf) ..         
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000073e0: 6469 6374 5f75 7064 6174 6528 756e 6971  dict_update(uniq
+000073f0: 7565 5f74 7261 636b 6c65 745f 6964 732c  ue_tracklet_ids,
+00007400: 206c 6561 662c 2074 7261 636b 5f69 642c   leaf, track_id,
+00007410: 2073 6f75 7263 655f 6c65 6166 2c20 4e6f   source_leaf, No
+00007420: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
 00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00007450: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007460: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
-00007470: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-00007480: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-00007490: 5f64 6976 6964 696e 677d 290d 0a0d 0a20  _dividing}).... 
+00007440: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007450: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00007460: 6965 735b 6c65 6166 5d2e 7570 6461 7465  ies[leaf].update
+00007470: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
+00007480: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
+00007490: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
 000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-000074c0: 6f75 7263 655f 6964 2069 6e20 616c 6c5f  ource_id in all_
-000074d0: 736f 7572 6365 5f69 6473 3a0d 0a20 2020  source_ids:..   
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007500: 2020 2020 2074 6172 6765 745f 6964 7320       target_ids 
-00007510: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
-00007520: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00007530: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00007560: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
-00007570: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
-00007580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 2020 2020 2020 2352 6f6f 740d            #Root.
-000075b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-000075e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000075f0: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
-00007600: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-00007610: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-00007620: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-00007630: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007660: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00007670: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-00007680: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
-00007690: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-000076a0: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
-000076b0: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 6966 2073 6f75 7263 655f 6964 206e 6f74  if source_id not
-000076f0: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
-00007700: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000074d0: 5f70 726f 7065 7274 6965 735b 6c65 6166  _properties[leaf
+000074e0: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+000074f0: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00007500: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+00007510: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+00007520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007540: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00007550: 6572 7469 6573 5b6c 6561 665d 2e75 7064  erties[leaf].upd
+00007560: 6174 6528 7b73 656c 662e 6469 7370 6c61  ate({self.displa
+00007570: 6365 6d65 6e74 5f6b 6579 203a 2074 7261  cement_key : tra
+00007580: 636b 5f64 6973 706c 6163 656d 656e 747d  ck_displacement}
+00007590: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000075c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000075d0: 735b 6c65 6166 5d2e 7570 6461 7465 287b  s[leaf].update({
+000075e0: 7365 6c66 2e74 6f74 616c 5f74 7261 636b  self.total_track
+000075f0: 5f64 6973 7461 6e63 655f 6b65 7920 3a20  _distance_key : 
+00007600: 746f 7461 6c5f 7472 6163 6b5f 6469 7374  total_track_dist
+00007610: 616e 6365 7d29 0d0a 2020 2020 2020 2020  ance})..        
+00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007640: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00007650: 6572 7469 6573 5b6c 6561 665d 2e75 7064  erties[leaf].upd
+00007660: 6174 6528 7b73 656c 662e 6d61 785f 6469  ate({self.max_di
+00007670: 7374 616e 6365 5f74 7261 7665 6c65 645f  stance_traveled_
+00007680: 6b65 7920 3a20 6d61 785f 7472 6163 6b5f  key : max_track_
+00007690: 6469 7374 616e 6365 7d29 0d0a 2020 2020  distance})..    
+000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000076c0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000076d0: 7072 6f70 6572 7469 6573 5b6c 6561 665d  properties[leaf]
+000076e0: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+000076f0: 6163 6b5f 6475 7261 7469 6f6e 5f6b 6579  ack_duration_key
+00007700: 203a 2074 7261 636b 5f64 7572 6174 696f   : track_duratio
+00007710: 6e7d 290d 0a0d 0a20 2020 2020 2020 2020  n})....         
 00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007760: 2020 2020 2020 2066 6f72 2074 6172 6765         for targe
-00007770: 745f 6964 2069 6e20 7461 7267 6574 5f69  t_id in target_i
-00007780: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
-000077c0: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
-000077d0: 5f74 7261 636b 6c65 745f 6964 732c 2073  _tracklet_ids, s
-000077e0: 6f75 7263 655f 6964 2c20 7472 6163 6b5f  ource_id, track_
-000077f0: 6964 2c20 4e6f 6e65 2c20 7461 7267 6574  id, None, target
-00007800: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00007730: 2020 2066 6f72 2073 6f75 7263 655f 6964     for source_id
+00007740: 2069 6e20 616c 6c5f 736f 7572 6365 5f69   in all_source_i
+00007750: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
+00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007770: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00007780: 6765 745f 6964 7320 3d20 7365 6c66 2e65  get_ids = self.e
+00007790: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
+000077a0: 705b 736f 7572 6365 5f69 645d 0d0a 2020  p[source_id]..  
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
+000077e0: 6c6c 5f69 6473 2e61 7070 656e 6428 736f  ll_ids.append(so
+000077f0: 7572 6365 5f69 6429 0d0a 2020 2020 2020  urce_id)..      
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007840: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007850: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
-00007860: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-00007870: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-00007880: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-00007890: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2352 6f6f 740d 0a20 2020 2020 2020    #Root..       
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007850: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00007860: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
+00007870: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
+00007880: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+00007890: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
+000078a0: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
 000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078c0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000078d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000078e0: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
-000078f0: 6174 6528 7b73 656c 662e 6e75 6d62 6572  ate({self.number
-00007900: 5f64 6976 6964 696e 675f 6b65 7920 3a20  _dividing_key : 
-00007910: 6e75 6d62 6572 5f64 6976 6964 696e 677d  number_dividing}
-00007920: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000078e0: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+000078f0: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00007900: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
+00007910: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
+00007920: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
 00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007940: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 234e 6f72 6d61 6c20 2020 2020 2020 200d  #Normal        .
-00007990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000079c0: 6f75 7263 655f 736f 7572 6365 5f69 6420  ource_source_id 
-000079d0: 3d20 7365 6c66 2e65 6467 655f 736f 7572  = self.edge_sour
-000079e0: 6365 5f6c 6f6f 6b75 705b 736f 7572 6365  ce_lookup[source
-000079f0: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
-00007a30: 6420 696e 2074 6172 6765 745f 6964 733a  d in target_ids:
-00007a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007960: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00007970: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
+00007980: 7064 6174 6528 7b73 656c 662e 6469 7370  pdate({self.disp
+00007990: 6c61 6365 6d65 6e74 5f6b 6579 203a 2074  lacement_key : t
+000079a0: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+000079b0: 747d 290d 0a20 2020 2020 2020 2020 2020  t})..           
+000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000079e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000079f0: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00007a00: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00007a10: 2e74 6f74 616c 5f74 7261 636b 5f64 6973  .total_track_dis
+00007a20: 7461 6e63 655f 6b65 7920 3a20 746f 7461  tance_key : tota
+00007a30: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+00007a40: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
 00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 7365 6c66 2e5f 6469 6374        self._dict
-00007a80: 5f75 7064 6174 6528 756e 6971 7565 5f74  _update(unique_t
-00007a90: 7261 636b 6c65 745f 6964 732c 2073 6f75  racklet_ids, sou
-00007aa0: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
-00007ab0: 2c20 736f 7572 6365 5f73 6f75 7263 655f  , source_source_
-00007ac0: 6964 2c20 7461 7267 6574 5f69 6429 200d  id, target_id) .
-00007ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007a70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00007a80: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00007a90: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00007aa0: 6d61 785f 6469 7374 616e 6365 5f74 7261  max_distance_tra
+00007ab0: 7665 6c65 645f 6b65 7920 3a20 6d61 785f  veled_key : max_
+00007ac0: 7472 6163 6b5f 6469 7374 616e 6365 7d29  track_distance})
+00007ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00007b10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007b20: 5b74 6172 6765 745f 6964 5d2e 7570 6461  [target_id].upda
-00007b30: 7465 287b 7365 6c66 2e64 6976 6964 696e  te({self.dividin
-00007b40: 675f 6b65 7920 3a20 6469 7669 6469 6e67  g_key : dividing
-00007b50: 5f74 7261 6a65 6374 6f72 797d 2920 0d0a  _trajectory}) ..
+00007af0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007b00: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00007b10: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
+00007b20: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+00007b30: 6163 6b5f 6475 7261 7469 6f6e 5f6b 6579  ack_duration_key
+00007b40: 203a 2074 7261 636b 5f64 7572 6174 696f   : track_duratio
+00007b50: 6e7d 290d 0a20 2020 2020 2020 2020 2020  n})..           
 00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00007ba0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00007bb0: 7461 7267 6574 5f69 645d 2e75 7064 6174  target_id].updat
-00007bc0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00007bd0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007be0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00007b80: 736f 7572 6365 5f69 6420 6e6f 7420 696e  source_id not in
+00007b90: 2061 6c6c 5f74 6172 6765 745f 6964 733a   all_target_ids:
+00007ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c00: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
+00007c10: 6420 696e 2074 6172 6765 745f 6964 733a  d in target_ids:
+00007c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
-00007c90: 726f 6f74 2069 6e20 726f 6f74 5f72 6f6f  root in root_roo
-00007ca0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2020 2073 656c 662e 5f64 6963 745f       self._dict_
+00007c60: 7570 6461 7465 2875 6e69 7175 655f 7472  update(unique_tr
+00007c70: 6163 6b6c 6574 5f69 6473 2c20 736f 7572  acklet_ids, sour
+00007c80: 6365 5f69 642c 2074 7261 636b 5f69 642c  ce_id, track_id,
+00007c90: 204e 6f6e 652c 2074 6172 6765 745f 6964   None, target_id
+00007ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00007cd0: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
-00007ce0: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
-00007cf0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007d00: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
-00007d10: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cd0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00007ce0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00007cf0: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
+00007d00: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
+00007d10: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
+00007d20: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d50: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
-00007d60: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
-00007d70: 696e 7428 7472 6163 6b5f 6964 295d 203d  int(track_id)] =
-00007d80: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
-00007d90: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00007da0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00007db0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00007dc0: 6e28 6375 7272 656e 745f 6365 6c6c 5f69  n(current_cell_i
-00007dd0: 6473 2929 3a0d 0a20 2020 2020 2020 2020  ds)):..         
+00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d60: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007d70: 706f 745f 7072 6f70 6572 7469 6573 5b74  pot_properties[t
+00007d80: 6172 6765 745f 6964 5d2e 7570 6461 7465  arget_id].update
+00007d90: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
+00007da0: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
+00007db0: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 206b 203d 2069 6e74 2863 7572       k = int(cur
-00007e30: 7265 6e74 5f63 656c 6c5f 6964 735b 695d  rent_cell_ids[i]
-00007e40: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
+00007df0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007e00: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00007e10: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00007e20: 287b 7365 6c66 2e64 6973 706c 6163 656d  ({self.displacem
+00007e30: 656e 745f 6b65 7920 3a20 7472 6163 6b5f  ent_key : track_
+00007e40: 6469 7370 6c61 6365 6d65 6e74 7d29 0d0a  displacement})..
 00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00007e70: 6963 745f 7661 6c75 6573 203d 2073 656c  ict_values = sel
-00007e80: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007e90: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00007ef0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00007f00: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00007f10: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00007f40: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00007f50: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-00007f60: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-00007f90: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00007fa0: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-00007fb0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00007fe0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00007ff0: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00008000: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e80: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007e90: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00007ea0: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00007eb0: 287b 7365 6c66 2e74 6f74 616c 5f74 7261  ({self.total_tra
+00007ec0: 636b 5f64 6973 7461 6e63 655f 6b65 7920  ck_distance_key 
+00007ed0: 3a20 746f 7461 6c5f 7472 6163 6b5f 6469  : total_track_di
+00007ee0: 7374 616e 6365 7d29 0d0a 2020 2020 2020  stance})..      
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007f20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00007f30: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00007f40: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00007f50: 2e6d 6178 5f64 6973 7461 6e63 655f 7472  .max_distance_tr
+00007f60: 6176 656c 6564 5f6b 6579 203a 206d 6178  aveled_key : max
+00007f70: 5f74 7261 636b 5f64 6973 7461 6e63 657d  _track_distance}
+00007f80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fb0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00007fc0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00007fd0: 735b 736f 7572 6365 5f69 645d 2e75 7064  s[source_id].upd
+00007fe0: 6174 6528 7b73 656c 662e 7472 6163 6b5f  ate({self.track_
+00007ff0: 6475 7261 7469 6f6e 5f6b 6579 203a 2074  duration_key : t
+00008000: 7261 636b 5f64 7572 6174 696f 6e7d 290d  rack_duration}).
+00008010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00008030: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008050: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-00008060: 745f 6365 6e74 726f 6964 203d 2028 726f  t_centroid = (ro
-00008070: 756e 6428 7a29 2f73 656c 662e 7a63 616c  und(z)/self.zcal
-00008080: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
-00008090: 7929 2f73 656c 662e 7963 616c 6962 7261  y)/self.ycalibra
-000080a0: 7469 6f6e 2c20 726f 756e 6428 7829 2f73  tion, round(x)/s
-000080b0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-000080c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
-000080f0: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
-00008100: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
-00008110: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
-00008120: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
-00008130: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
-00008140: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
-00008150: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008180: 756e 6971 7565 5f73 706f 745f 6365 6e74  unique_spot_cent
-00008190: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
-000081a0: 6365 6e74 726f 6964 5d20 3d20 6b0d 0a20  centroid] = k.. 
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2020 2020 2020 234e                #N
+00008070: 6f72 6d61 6c20 2020 2020 2020 200d 0a20  ormal        .. 
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080a0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+000080b0: 7263 655f 736f 7572 6365 5f69 6420 3d20  rce_source_id = 
+000080c0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
+000080d0: 5f6c 6f6f 6b75 705b 736f 7572 6365 5f69  _lookup[source_i
+000080e0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2020 666f 7220 7461 7267 6574 5f69 6420    for target_id 
+00008120: 696e 2074 6172 6765 745f 6964 733a 0d0a  in target_ids:..
+00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 2020 2020 7365 6c66 2e5f 6469 6374 5f75      self._dict_u
+00008170: 7064 6174 6528 756e 6971 7565 5f74 7261  pdate(unique_tra
+00008180: 636b 6c65 745f 6964 732c 2073 6f75 7263  cklet_ids, sourc
+00008190: 655f 6964 2c20 7472 6163 6b5f 6964 2c20  e_id, track_id, 
+000081a0: 736f 7572 6365 5f73 6f75 7263 655f 6964  source_source_id
+000081b0: 2c20 7461 7267 6574 5f69 6429 200d 0a20  , target_id) .. 
 000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081d0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-000081e0: 7261 636b 5f63 656e 7472 6f69 645b 6672  rack_centroid[fr
-000081f0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00008200: 645d 203d 2074 7261 636b 5f69 640d 0a0d  d] = track_id...
-00008210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 2020 2069 6620 7374 7228 7429 2069       if str(t) i
-00008240: 6e20 7365 6c66 2e5f 7469 6d65 645f 6365  n self._timed_ce
-00008250: 6e74 726f 6964 3a0d 0a20 2020 2020 2020  ntroid:..       
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00008200: 706f 745f 7072 6f70 6572 7469 6573 5b74  pot_properties[t
+00008210: 6172 6765 745f 6964 5d2e 7570 6461 7465  arget_id].update
+00008220: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
+00008230: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
+00008240: 7261 6a65 6374 6f72 797d 2920 0d0a 2020  rajectory}) ..  
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008280: 2020 2020 7472 6565 2c20 7370 6f74 5f63      tree, spot_c
-00008290: 656e 7472 6f69 6473 203d 2073 656c 662e  entroids = self.
-000082a0: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
-000082b0: 7374 7228 7429 5d0d 0a20 2020 2020 2020  str(t)]..       
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082e0: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-000082f0: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
-00008300: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
-00008310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
-00008340: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
-00008350: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008280: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00008290: 6f74 5f70 726f 7065 7274 6965 735b 7461  ot_properties[ta
+000082a0: 7267 6574 5f69 645d 2e75 7064 6174 6528  rget_id].update(
+000082b0: 7b73 656c 662e 6e75 6d62 6572 5f64 6976  {self.number_div
+000082c0: 6964 696e 675f 6b65 7920 3a20 6e75 6d62  iding_key : numb
+000082d0: 6572 5f64 6976 6964 696e 677d 290d 0a20  er_dividing}).. 
+000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00008320: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00008330: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00008340: 287b 7365 6c66 2e64 6973 706c 6163 656d  ({self.displacem
+00008350: 656e 745f 6b65 7920 3a20 7472 6163 6b5f  ent_key : track_
+00008360: 6469 7370 6c61 6365 6d65 6e74 7d29 0d0a  displacement})..
 00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
-00008390: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
-000083a0: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
-000083b0: 745f 6365 6e74 726f 6964 7320 0d0a 2020  t_centroids ..  
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00008420: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-00008430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00008460: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
-00008470: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084a0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
-000084b0: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
-000084c0: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
-00008500: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
-00008510: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
-00008520: 745f 6365 6e74 726f 6964 730d 0a20 2020  t_centroids..   
-00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00008550: 2064 6566 205f 6d61 7374 6572 5f74 7261   def _master_tra
-00008560: 636b 5f63 6f6d 7075 7465 7228 7365 6c66  ck_computer(self
-00008570: 2c20 7472 6163 6b2c 2074 7261 636b 5f69  , track, track_i
-00008580: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
+00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000083b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000083c0: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
+000083d0: 6528 7b73 656c 662e 746f 7461 6c5f 7472  e({self.total_tr
+000083e0: 6163 6b5f 6469 7374 616e 6365 5f6b 6579  ack_distance_key
+000083f0: 203a 2074 6f74 616c 5f74 7261 636b 5f64   : total_track_d
+00008400: 6973 7461 6e63 657d 290d 0a20 2020 2020  istance})..     
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008440: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00008450: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
+00008460: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
+00008470: 6c66 2e6d 6178 5f64 6973 7461 6e63 655f  lf.max_distance_
+00008480: 7472 6176 656c 6564 5f6b 6579 203a 206d  traveled_key : m
+00008490: 6178 5f74 7261 636b 5f64 6973 7461 6e63  ax_track_distanc
+000084a0: 657d 290d 0a20 2020 2020 2020 2020 2020  e})..           
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000084e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000084f0: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+00008500: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
+00008510: 636b 5f64 7572 6174 696f 6e5f 6b65 7920  ck_duration_key 
+00008520: 3a20 7472 6163 6b5f 6475 7261 7469 6f6e  : track_duration
+00008530: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008550: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000085a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000085d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000085e0: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
-000085f0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008620: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008640: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00008650: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-00008660: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-00008670: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-00008680: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-00008690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000086a0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-000086b0: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-000086c0: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-000086d0: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-000086e0: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-000086f0: 7572 6365 5f69 6473 2920 0d0a 2020 2020  urce_ids) ..    
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00008720: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
-00008730: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
-00008740: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-00008750: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00008780: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008790: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
-000087a0: 7472 6163 6b20 6861 7320 6469 7669 7369  track has divisi
-000087b0: 6f6e 7320 6f72 206e 6f6e 650d 0a20 2020  ons or none..   
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 2020 2020 2020 2020 206e 756d 6265 725f           number_
-000087e0: 6469 7669 6469 6e67 203d 206c 656e 2872  dividing = len(r
-000087f0: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00008820: 726f 6f74 5f73 706c 6974 7329 203e 2030  root_splits) > 0
-00008830: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008850: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00008860: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00008870: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
-00008880: 312c 206e 756d 6265 725f 6469 7669 6469  1, number_dividi
-00008890: 6e67 5d0d 0a20 2020 2020 2020 2020 2020  ng]..           
-000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088b0: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
-000088c0: 616a 6563 746f 7279 203d 2054 7275 650d  ajectory = True.
-000088d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088f0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-00008900: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-00008910: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00008950: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00008960: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
-00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008980: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00008990: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-000089a0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-000089b0: 636b 4964 733a 2020 2020 200d 0a20 2020  ckIds:     ..   
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-000089f0: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
-00008a00: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
+000085c0: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
+000085d0: 6e74 5f72 6f6f 7420 696e 2072 6f6f 745f  nt_root in root_
+000085e0: 726f 6f74 3a0d 0a20 2020 2020 2020 2020  root:..         
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00008610: 6f6f 745f 7370 6f74 735b 696e 7428 6375  oot_spots[int(cu
+00008620: 7272 656e 745f 726f 6f74 295d 203d 2073  rrent_root)] = s
+00008630: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00008640: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00008650: 7572 7265 6e74 5f72 6f6f 7429 5d0d 0a20  urrent_root)].. 
+00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008670: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008690: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000086a0: 6c5f 6375 7272 656e 745f 6365 6c6c 5f69  l_current_cell_i
+000086b0: 6473 5b69 6e74 2874 7261 636b 5f69 6429  ds[int(track_id)
+000086c0: 5d20 3d20 6375 7272 656e 745f 6365 6c6c  ] = current_cell
+000086d0: 5f69 6473 0d0a 2020 2020 2020 2020 2020  _ids..          
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00008700: 286c 656e 2863 7572 7265 6e74 5f63 656c  (len(current_cel
+00008710: 6c5f 6964 7329 293a 0d0a 2020 2020 2020  l_ids)):..      
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008740: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2020 2020 6b20 3d20 696e 7428          k = int(
+00008770: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
+00008780: 5b69 5d29 2020 2020 0d0a 2020 2020 2020  [i])    ..      
+00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087a0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000087b0: 6c5f 6469 6374 5f76 616c 7565 7320 3d20  l_dict_values = 
+000087c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000087d0: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008820: 2020 2020 2020 2020 2074 203d 2069 6e74           t = int
+00008830: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
+00008840: 7661 6c75 6573 5b73 656c 662e 6672 616d  values[self.fram
+00008850: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008880: 7a20 3d20 666c 6f61 7428 616c 6c5f 6469  z = float(all_di
+00008890: 6374 5f76 616c 7565 735b 7365 6c66 2e7a  ct_values[self.z
+000088a0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2079 203d 2066 6c6f 6174 2861 6c6c 5f64   y = float(all_d
+000088e0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000088f0: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 7820 3d20 666c 6f61 7428 616c 6c5f    x = float(all_
+00008930: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00008940: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 7370 6f74 5f63 656e 7472 6f69 6420 3d20  spot_centroid = 
+000089b0: 2872 6f75 6e64 287a 292f 7365 6c66 2e7a  (round(z)/self.z
+000089c0: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+000089d0: 6e64 2879 292f 7365 6c66 2e79 6361 6c69  nd(y)/self.ycali
+000089e0: 6272 6174 696f 6e2c 2072 6f75 6e64 2878  bration, round(x
+000089f0: 292f 7365 6c66 2e78 6361 6c69 6272 6174  )/self.xcalibrat
+00008a00: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
 00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008a80: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
-00008a90: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
-00008aa0: 5f69 645d 203d 205b 302c 2030 5d0d 0a20  _id] = [0, 0].. 
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00008ad0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00008ae0: 7279 203d 2046 616c 7365 0d0a 2020 2020  ry = False..    
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00008b10: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00008b20: 2069 6e20 7365 6c66 2e41 6c6c 5472 6163   in self.AllTrac
-00008b30: 6b49 6473 3a0d 0a20 2020 2020 2020 2020  kIds:..         
-00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008b60: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-00008b70: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00008b80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ba0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
-00008bb0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
-00008bc0: 4e6f 726d 616c 5472 6163 6b49 6473 3a20  NormalTrackIds: 
-00008bd0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bf0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-00008c00: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-00008c10: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00008c20: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c40: 2020 666f 7220 6c65 6166 2069 6e20 726f    for leaf in ro
-00008c50: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
+00008a20: 2020 2020 2020 2020 2020 6672 616d 655f            frame_
+00008a30: 7370 6f74 5f63 656e 7472 6f69 6420 3d20  spot_centroid = 
+00008a40: 2874 2c72 6f75 6e64 287a 292f 7365 6c66  (t,round(z)/self
+00008a50: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
+00008a60: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
+00008a70: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
+00008a80: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
+00008a90: 6174 696f 6e29 0d0a 0d0a 2020 2020 2020  ation)....      
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008ac0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
+00008ad0: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00008ae0: 6f74 5f63 656e 7472 6f69 645d 203d 206b  ot_centroid] = k
+00008af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00008b20: 655f 7472 6163 6b5f 6365 6e74 726f 6964  e_track_centroid
+00008b30: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
+00008b40: 726f 6964 5d20 3d20 7472 6163 6b5f 6964  roid] = track_id
+00008b50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b70: 2020 2020 2020 2020 6966 2073 7472 2874          if str(t
+00008b80: 2920 696e 2073 656c 662e 5f74 696d 6564  ) in self._timed
+00008b90: 5f63 656e 7472 6f69 643a 0d0a 2020 2020  _centroid:..    
+00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 2020 2074 7265 652c 2073 706f         tree, spo
+00008bd0: 745f 6365 6e74 726f 6964 7320 3d20 7365  t_centroids = se
+00008be0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+00008bf0: 6964 5b73 7472 2874 295d 0d0a 2020 2020  id[str(t)]..    
+00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c20: 2020 2020 2020 2073 706f 745f 6365 6e74         spot_cent
+00008c30: 726f 6964 732e 6170 7065 6e64 2873 706f  roids.append(spo
+00008c40: 745f 6365 6e74 726f 6964 290d 0a20 2020  t_centroid)..   
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008c80: 662e 5f73 6563 6f6e 645f 6368 616e 6e65  f._second_channe
-00008c90: 6c5f 7570 6461 7465 286c 6561 662c 2074  l_update(leaf, t
-00008ca0: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
+00008c70: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+00008c80: 7061 7469 616c 2e63 4b44 5472 6565 2873  patial.cKDTree(s
+00008c90: 706f 745f 6365 6e74 726f 6964 7329 0d0a  pot_centroids)..
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cc0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00008cd0: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
-00008ce0: 7065 6e64 286c 6561 6629 200d 0a20 2020  pend(leaf) ..   
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d10: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008d20: 5f70 726f 7065 7274 6965 735b 6c65 6166  _properties[leaf
-00008d30: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00008d40: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00008d50: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00008d60: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00008cc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008cd0: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
+00008ce0: 7374 7228 7429 5d20 3d20 7472 6565 2c20  str(t)] = tree, 
+00008cf0: 7370 6f74 5f63 656e 7472 6f69 6473 200d  spot_centroids .
+00008d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d20: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d50: 2020 2020 2020 2073 706f 745f 6365 6e74         spot_cent
+00008d60: 726f 6964 7320 3d20 5b5d 0d0a 2020 2020  roids = []..    
 00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00008d90: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00008da0: 6965 735b 6c65 6166 5d2e 7570 6461 7465  ies[leaf].update
-00008db0: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
-00008dc0: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
-00008dd0: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008e00: 736f 7572 6365 5f69 6420 696e 2061 6c6c  source_id in all
-00008e10: 5f73 6f75 7263 655f 6964 733a 0d0a 2020  _source_ids:..  
+00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d90: 2020 2020 2020 2073 706f 745f 6365 6e74         spot_cent
+00008da0: 726f 6964 732e 6170 7065 6e64 2873 706f  roids.append(spo
+00008db0: 745f 6365 6e74 726f 6964 290d 0a20 2020  t_centroid)..   
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+00008df0: 7061 7469 616c 2e63 4b44 5472 6565 2873  patial.cKDTree(s
+00008e00: 706f 745f 6365 6e74 726f 6964 7329 0d0a  pot_centroids)..
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e40: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
-00008e50: 616e 6e65 6c5f 7570 6461 7465 2873 6f75  annel_update(sou
-00008e60: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
-00008e70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00008ea0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00008eb0: 735b 736f 7572 6365 5f69 645d 2e75 7064  s[source_id].upd
-00008ec0: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00008ed0: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00008ee0: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
+00008e30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008e40: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
+00008e50: 7374 7228 7429 5d20 3d20 7472 6565 2c20  str(t)] = tree, 
+00008e60: 7370 6f74 5f63 656e 7472 6f69 6473 0d0a  spot_centroids..
+00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00008e90: 2020 2020 6465 6620 5f6d 6173 7465 725f      def _master_
+00008ea0: 7472 6163 6b5f 636f 6d70 7574 6572 2873  track_computer(s
+00008eb0: 656c 662c 2074 7261 636b 2c20 7472 6163  elf, track, trac
+00008ec0: 6b5f 6964 293a 0d0a 2020 2020 2020 2020  k_id):..        
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00008f20: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
-00008f30: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
-00008f40: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
-00008f50: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
-00008f60: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00008fa0: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
-00008fb0: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
-00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00008f00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00008f30: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f70: 2074 7261 636b 5f64 6973 706c 6163 656d   track_displacem
+00008f80: 656e 742c 746f 7461 6c5f 7472 6163 6b5f  ent,total_track_
+00008f90: 6469 7374 616e 6365 2c20 6d61 785f 7472  distance, max_tr
+00008fa0: 6163 6b5f 6469 7374 616e 6365 2c20 7472  ack_distance, tr
+00008fb0: 6163 6b5f 6475 7261 7469 6f6e 2020 3d20  ack_duration  = 
+00008fc0: 2073 656c 662e 5f67 6574 5f74 7261 636b   self._get_track
+00008fd0: 5f66 6561 7475 7265 7328 7472 6163 6b29  _features(track)
+00008fe0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009000: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
-00009010: 6e74 5f72 6f6f 7420 696e 2072 6f6f 745f  nt_root in root_
-00009020: 726f 6f74 3a0d 0a20 2020 2020 2020 2020  root:..         
-00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009050: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
-00009060: 7064 6174 6528 6375 7272 656e 745f 726f  pdate(current_ro
-00009070: 6f74 2c20 7472 6163 6b5f 6964 290d 0a20  ot, track_id).. 
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
-000090b0: 735b 696e 7428 6375 7272 656e 745f 726f  s[int(current_ro
-000090c0: 6f74 295d 203d 2073 656c 662e 756e 6971  ot)] = self.uniq
-000090d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000090e0: 6573 5b69 6e74 2863 7572 7265 6e74 5f72  es[int(current_r
-000090f0: 6f6f 7429 5d0d 0a20 2020 2020 2020 2020  oot)]..         
-00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00009120: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00009130: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
-00009140: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-00009150: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00009160: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00009170: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009190: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000091a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000091b0: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
-000091c0: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
-000091d0: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
-000091e0: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
-000091f0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009220: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009230: 6c66 2e61 6c6c 5f63 7572 7265 6e74 5f63  lf.all_current_c
-00009240: 656c 6c5f 6964 735b 696e 7428 7472 6163  ell_ids[int(trac
-00009250: 6b5f 6964 295d 203d 2063 7572 7265 6e74  k_id)] = current
-00009260: 5f63 656c 6c5f 6964 730d 0a20 2020 2020  _cell_ids..     
-00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009280: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00009000: 616c 6c5f 736f 7572 6365 5f69 6473 2c20  all_source_ids, 
+00009010: 616c 6c5f 7461 7267 6574 5f69 6473 203d  all_target_ids =
+00009020: 2020 7365 6c66 2e5f 6765 6e65 7261 7465    self._generate
+00009030: 5f67 656e 6572 6174 696f 6e73 2874 7261  _generations(tra
+00009040: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2072 6f6f 745f 726f 6f74 2c20 726f 6f74   root_root, root
+00009070: 5f73 706c 6974 732c 2072 6f6f 745f 6c65  _splits, root_le
+00009080: 6166 203d 2073 656c 662e 5f63 7265 6174  af = self._creat
+00009090: 655f 6765 6e65 7261 7469 6f6e 7328 616c  e_generations(al
+000090a0: 6c5f 736f 7572 6365 5f69 6473 2920 0d0a  l_source_ids) ..
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000090d0: 2e5f 6974 6572 6174 655f 7370 6c69 745f  ._iterate_split_
+000090e0: 646f 776e 2872 6f6f 745f 726f 6f74 2c20  down(root_root, 
+000090f0: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
+00009100: 7370 6c69 7473 290d 0a20 2020 2020 2020  splits)..       
+00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009120: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009140: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
+00009150: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
+00009160: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
+00009170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009180: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00009190: 6265 725f 6469 7669 6469 6e67 203d 206c  ber_dividing = l
+000091a0: 656e 2872 6f6f 745f 7370 6c69 7473 290d  en(root_splits).
+000091b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000091c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000091d0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+000091e0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00009210: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
+00009220: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
+00009230: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
+00009240: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
+00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009260: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+00009270: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
+00009280: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
 00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-000092b0: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
-000092c0: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
+000092a0: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+000092b0: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+000092c0: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
 000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-00009320: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
-00009330: 6473 5b69 5d29 2020 200d 0a20 2020 2020  ds[i])   ..     
-00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009350: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 2020 2020 2061 6c6c 5f64 6963 745f 7661       all_dict_va
-00009390: 6c75 6573 203d 2073 656c 662e 756e 6971  lues = self.uniq
-000093a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000093b0: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
-000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092f0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00009300: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+00009310: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009330: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00009340: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00009350: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
+00009360: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
+00009370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+000093a0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+000093b0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+000093c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000093f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009400: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2020 2020 2074 203d 2069 6e74 2866 6c6f       t = int(flo
-00009430: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009440: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
-00009450: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2020 2020 2020 2020 7a20 3d20              z = 
-00009480: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009490: 616c 7565 735b 7365 6c66 2e7a 706f 7369  alues[self.zposi
-000094a0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+00009420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009430: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00009440: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
+00009450: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
+00009460: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009480: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
+00009490: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
-000094d0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-000094e0: 7661 6c75 6573 5b73 656c 662e 7970 6f73  values[self.ypos
-000094f0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-00009520: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00009530: 5f76 616c 7565 735b 7365 6c66 2e78 706f  _values[self.xpo
-00009540: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009570: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00009580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009590: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
-000095a0: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
-000095b0: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
-000095c0: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
-000095d0: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
-000095e0: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
-000095f0: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
-00009600: 6f6e 2920 0d0a 0d0a 2020 2020 2020 2020  on) ....        
+000094c0: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+000094d0: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
+000094e0: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009510: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
+00009520: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00009530: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009550: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+00009560: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+00009570: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+00009580: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000095b0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+000095c0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+000095d0: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
+00009600: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
 00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009630: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-00009640: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-00009650: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
+00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009630: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00009640: 616e 6e65 6c5f 7570 6461 7465 286c 6561  annel_update(lea
+00009650: 662c 2074 7261 636b 5f69 6429 0d0a 2020  f, track_id)..  
 00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009680: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00009690: 7472 6163 6b5f 6365 6e74 726f 6964 5b66  track_centroid[f
-000096a0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-000096b0: 6964 5d20 3d20 7472 6163 6b5f 6964 0d0a  id] = track_id..
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 2020 200d 0a20 2020 2064 6566 205f 7365     ..    def _se
-000096f0: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
-00009700: 6174 6528 7365 6c66 2c20 6365 6c6c 5f69  ate(self, cell_i
-00009710: 642c 2074 7261 636b 5f69 6429 3a0d 0a20  d, track_id):.. 
-00009720: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00009730: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00009740: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-00009750: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00009760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009770: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00009780: 2020 2066 7261 6d65 203d 2073 656c 662e     frame = self.
-00009790: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000097a0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000097b0: 6964 295d 5b73 656c 662e 6672 616d 6569  id)][self.framei
-000097c0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-000097d0: 2020 2020 2020 2020 7a20 3d20 7365 6c66          z = self
-000097e0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000097f0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00009800: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00009810: 645f 6b65 795d 2f73 656c 662e 7a63 616c  d_key]/self.zcal
-00009820: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00009830: 2020 2020 2020 2020 2020 7920 3d20 7365            y = se
-00009840: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00009850: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00009860: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00009870: 7369 645f 6b65 795d 2f73 656c 662e 7963  sid_key]/self.yc
-00009880: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00009890: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-000098a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000098b0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000098c0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-000098d0: 706f 7369 645f 6b65 795d 2f73 656c 662e  posid_key]/self.
-000098e0: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
-000098f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009900: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
-00009910: 656c 5f73 706f 7473 2866 7261 6d65 2c20  el_spots(frame, 
-00009920: 7a2c 2079 2c20 782c 2063 656c 6c5f 6964  z, y, x, cell_id
-00009930: 2c20 7472 6163 6b5f 6964 290d 0a20 2020  , track_id)..   
-00009940: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00009950: 6669 6e61 6c5f 7472 6163 6b73 2873 656c  final_tracks(sel
-00009960: 662c 2074 7261 636b 2c20 7472 6163 6b5f  f, track, track_
-00009970: 6964 293a 0d0a 0d0a 2020 2020 2020 2020  id):....        
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
-000099a0: 5f69 6473 203d 2073 656c 662e 616c 6c5f  _ids = self.all_
-000099b0: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-000099c0: 5b69 6e74 2874 7261 636b 5f69 6429 5d0d  [int(track_id)].
-000099d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000099e0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000099f0: 7265 6e74 5f74 7261 636b 6c65 7473 203d  rent_tracklets =
-00009a00: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a20: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009a30: 7473 5f70 726f 7065 7274 6965 7320 3d20  ts_properties = 
-00009a40: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00009680: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00009690: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
+000096a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000096d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000096e0: 6c65 6166 5d2e 7570 6461 7465 287b 7365  leaf].update({se
+000096f0: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+00009700: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00009710: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009740: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00009750: 7065 7274 6965 735b 6c65 6166 5d2e 7570  perties[leaf].up
+00009760: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
+00009770: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
+00009780: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
+00009790: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000097c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000097d0: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
+000097e0: 7b73 656c 662e 6469 7370 6c61 6365 6d65  {self.displaceme
+000097f0: 6e74 5f6b 6579 203a 2074 7261 636b 5f64  nt_key : track_d
+00009800: 6973 706c 6163 656d 656e 747d 290d 0a20  isplacement}).. 
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00009840: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
+00009850: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
+00009860: 2e74 6f74 616c 5f74 7261 636b 5f64 6973  .total_track_dis
+00009870: 7461 6e63 655f 6b65 7920 3a20 746f 7461  tance_key : tota
+00009880: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+00009890: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000098c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000098d0: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
+000098e0: 7b73 656c 662e 6d61 785f 6469 7374 616e  {self.max_distan
+000098f0: 6365 5f74 7261 7665 6c65 645f 6b65 7920  ce_traveled_key 
+00009900: 3a20 6d61 785f 7472 6163 6b5f 6469 7374  : max_track_dist
+00009910: 616e 6365 7d29 0d0a 2020 2020 2020 2020  ance})..        
+00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009940: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00009950: 6572 7469 6573 5b6c 6561 665d 2e75 7064  erties[leaf].upd
+00009960: 6174 6528 7b73 656c 662e 7472 6163 6b5f  ate({self.track_
+00009970: 6475 7261 7469 6f6e 5f6b 6579 203a 2074  duration_key : t
+00009980: 7261 636b 5f64 7572 6174 696f 6e7d 290d  rack_duration}).
+00009990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
+000099e0: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
+000099f0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a10: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
+00009a20: 6f6e 645f 6368 616e 6e65 6c5f 7570 6461  ond_channel_upda
+00009a30: 7465 2873 6f75 7263 655f 6964 2c20 7472  te(source_id, tr
+00009a40: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
 00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009a70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009a80: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00009a90: 2863 7572 7265 6e74 5f63 656c 6c5f 6964  (current_cell_id
-00009aa0: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
-00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00009a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009a70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00009a80: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00009a90: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00009aa0: 6469 7669 6469 6e67 5f6b 6579 203a 2064  dividing_key : d
+00009ab0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+00009ac0: 7279 7d29 0d0a 2020 2020 2020 2020 2020  ry})..          
 00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 6b20 3d20 696e 7428 6375 7272      k = int(curr
-00009b00: 656e 745f 6365 6c6c 5f69 6473 5b69 5d29  ent_cell_ids[i])
-00009b10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-00009b40: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
-00009b50: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00009b60: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 756e 6971 7565 5f69 6420 3d20 7374 7228  unique_id = str(
-00009ba0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009bb0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-00009bc0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00009ae0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00009af0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00009b00: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+00009b10: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
+00009b20: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
+00009b30: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
+00009b40: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00009b70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00009b80: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+00009b90: 7570 6461 7465 287b 7365 6c66 2e64 6973  update({self.dis
+00009ba0: 706c 6163 656d 656e 745f 6b65 7920 3a20  placement_key : 
+00009bb0: 7472 6163 6b5f 6469 7370 6c61 6365 6d65  track_displaceme
+00009bc0: 6e74 7d29 0d0a 2020 2020 2020 2020 2020  nt})..          
 00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00009bf0: 5f74 7261 636b 5f69 6420 3d20 7374 7228  _track_id = str(
-00009c00: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009c10: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-00009c20: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2020 2020 2020 2020 7420 3d20 696e 7428          t = int(
-00009c50: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009c60: 616c 7565 735b 7365 6c66 2e66 7261 6d65  alues[self.frame
-00009c70: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
-00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c90: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-00009ca0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00009cb0: 745f 7661 6c75 6573 5b73 656c 662e 7a70  t_values[self.zp
-00009cc0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009be0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00009bf0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00009c00: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
+00009c10: 7570 6461 7465 287b 7365 6c66 2e74 6f74  update({self.tot
+00009c20: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+00009c30: 655f 6b65 7920 3a20 746f 7461 6c5f 7472  e_key : total_tr
+00009c40: 6163 6b5f 6469 7374 616e 6365 7d29 0d0a  ack_distance})..
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c70: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00009c80: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00009c90: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00009ca0: 287b 7365 6c66 2e6d 6178 5f64 6973 7461  ({self.max_dista
+00009cb0: 6e63 655f 7472 6176 656c 6564 5f6b 6579  nce_traveled_key
+00009cc0: 203a 206d 6178 5f74 7261 636b 5f64 6973   : max_track_dis
+00009cd0: 7461 6e63 657d 290d 0a20 2020 2020 2020  tance})..       
 00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cf0: 7920 3d20 666c 6f61 7428 616c 6c5f 6469  y = float(all_di
-00009d00: 6374 5f76 616c 7565 735b 7365 6c66 2e79  ct_values[self.y
-00009d10: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d40: 2078 203d 2066 6c6f 6174 2861 6c6c 5f64   x = float(all_d
-00009d50: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00009d60: 7870 6f73 6964 5f6b 6579 5d29 0d0a 0d0a  xposid_key])....
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-00009da0: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
-00009db0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009dc0: 6965 7320 3d20 7365 6c66 2e5f 7472 6163  ies = self._trac
-00009dd0: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
-00009de0: 6965 7328 7472 6163 6b2c 2020 616c 6c5f  ies(track,  all_
-00009df0: 6469 6374 5f76 616c 7565 732c 2074 2c20  dict_values, t, 
-00009e00: 7a2c 2079 2c20 782c 206b 2c20 6375 7272  z, y, x, k, curr
-00009e10: 656e 745f 7472 6163 6b5f 6964 2c20 756e  ent_track_id, un
-00009e20: 6971 7565 5f69 642c 2063 7572 7265 6e74  ique_id, current
-00009e30: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
-00009e40: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-00009e50: 6f70 6572 7469 6573 290d 0a20 2020 2020  operties)..     
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009e80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00009e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009ea0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009eb0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00009ec0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
-00009ed0: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
-00009ee0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00009ef0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009f00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009f10: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009f20: 5f70 726f 7065 7274 6965 7320 3d20 6e70  _properties = np
-00009f30: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00009f40: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-00009f50: 7274 6965 735b 7374 7228 7472 6163 6b5f  rties[str(track_
-00009f60: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
-00009f70: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fb0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00009fc0: 7261 636b 735b 7472 6163 6b5f 6964 5d20  racks[track_id] 
-00009fd0: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
-00009fe0: 6574 7320 2020 2020 0d0a 2020 2020 2020  ets     ..      
-00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a000: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000a010: 655f 7472 6163 6b5f 7072 6f70 6572 7469  e_track_properti
-0000a020: 6573 5b74 7261 636b 5f69 645d 203d 2063  es[track_id] = c
-0000a030: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-0000a040: 5f70 726f 7065 7274 6965 7320 2020 200d  _properties    .
-0000a050: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
-0000a060: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
-0000a070: 6965 7328 7365 6c66 2c20 7472 6163 6b2c  ies(self, track,
-0000a080: 2061 6c6c 5f64 6963 745f 7661 6c75 6573   all_dict_values
-0000a090: 2c20 742c 207a 2c20 792c 2078 2c20 6b2c  , t, z, y, x, k,
-0000a0a0: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
-0000a0b0: 642c 2075 6e69 7175 655f 6964 2c20 6375  d, unique_id, cu
-0000a0c0: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
-0000a0d0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000a0e0: 7473 5f70 726f 7065 7274 6965 7329 3a0d  ts_properties):.
-0000a0f0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a120: 2020 6765 6e5f 6964 203d 2069 6e74 2866    gen_id = int(f
-0000a130: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-0000a140: 6c75 6573 5b73 656c 662e 6765 6e65 7261  lues[self.genera
-0000a150: 7469 6f6e 6964 5f6b 6579 5d29 290d 0a20  tionid_key])).. 
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009d00: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00009d10: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00009d20: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00009d30: 7472 6163 6b5f 6475 7261 7469 6f6e 5f6b  track_duration_k
+00009d40: 6579 203a 2074 7261 636b 5f64 7572 6174  ey : track_durat
+00009d50: 696f 6e7d 290d 0a20 2020 2020 2020 2020  ion})..         
+00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d70: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009d80: 745f 6365 6c6c 5f69 6473 2e61 7070 656e  t_cell_ids.appen
+00009d90: 6428 736f 7572 6365 5f69 6429 0d0a 2020  d(source_id)..  
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00009dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009de0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00009df0: 7220 6375 7272 656e 745f 726f 6f74 2069  r current_root i
+00009e00: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e30: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
+00009e40: 616e 6e65 6c5f 7570 6461 7465 2863 7572  annel_update(cur
+00009e50: 7265 6e74 5f72 6f6f 742c 2074 7261 636b  rent_root, track
+00009e60: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e80: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
+00009e90: 6f74 5f73 706f 7473 5b69 6e74 2863 7572  ot_spots[int(cur
+00009ea0: 7265 6e74 5f72 6f6f 7429 5d20 3d20 7365  rent_root)] = se
+00009eb0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00009ec0: 726f 7065 7274 6965 735b 696e 7428 6375  roperties[int(cu
+00009ed0: 7272 656e 745f 726f 6f74 295d 0d0a 2020  rrent_root)]..  
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f00: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00009f10: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
+00009f20: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
+00009f30: 7365 6c66 2e64 6976 6964 696e 675f 6b65  self.dividing_ke
+00009f40: 7920 3a20 6469 7669 6469 6e67 5f74 7261  y : dividing_tra
+00009f50: 6a65 6374 6f72 797d 290d 0a20 2020 2020  jectory})..     
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009f80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00009f90: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+00009fa0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00009fb0: 662e 6e75 6d62 6572 5f64 6976 6964 696e  f.number_dividin
+00009fc0: 675f 6b65 7920 3a20 6e75 6d62 6572 5f64  g_key : number_d
+00009fd0: 6976 6964 696e 677d 290d 0a20 2020 2020  ividing})..     
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a000: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000a010: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+0000a020: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+0000a030: 662e 6469 7370 6c61 6365 6d65 6e74 5f6b  f.displacement_k
+0000a040: 6579 203a 2074 7261 636b 5f64 6973 706c  ey : track_displ
+0000a050: 6163 656d 656e 747d 290d 0a20 2020 2020  acement})..     
+0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a070: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000a080: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+0000a090: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+0000a0a0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+0000a0b0: 662e 746f 7461 6c5f 7472 6163 6b5f 6469  f.total_track_di
+0000a0c0: 7374 616e 6365 5f6b 6579 203a 2074 6f74  stance_key : tot
+0000a0d0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+0000a0e0: 657d 290d 0a20 2020 2020 2020 2020 2020  e})..           
+0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a100: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000a110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000a120: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
+0000a130: 7064 6174 6528 7b73 656c 662e 6d61 785f  pdate({self.max_
+0000a140: 6469 7374 616e 6365 5f74 7261 7665 6c65  distance_travele
+0000a150: 645f 6b65 7920 3a20 6d61 785f 7472 6163  d_key : max_trac
+0000a160: 6b5f 6469 7374 616e 6365 7d29 0d0a 2020  k_distance})..  
 0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2073 7065 6564 203d 2066 6c6f 6174     speed = float
-0000a190: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-0000a1a0: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
-0000a1b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 2061 6363 656c 6572 6174         accelerat
-0000a1e0: 696f 6e20 3d20 666c 6f61 7428 616c 6c5f  ion = float(all_
-0000a1f0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-0000a200: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-0000a210: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
-0000a240: 616e 676c 6520 3d20 666c 6f61 7428 616c  angle = float(al
-0000a250: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-0000a260: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-0000a270: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a190: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+0000a1a0: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
+0000a1b0: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
+0000a1c0: 7365 6c66 2e74 7261 636b 5f64 7572 6174  self.track_durat
+0000a1d0: 696f 6e5f 6b65 7920 3a20 7472 6163 6b5f  ion_key : track_
+0000a1e0: 6475 7261 7469 6f6e 7d29 0d0a 2020 2020  duration})..    
+0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a200: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a220: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
+0000a230: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
+0000a240: 696e 7428 7472 6163 6b5f 6964 295d 203d  int(track_id)] =
+0000a250: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+0000a260: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+0000a270: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 2020 2020 2072 6164 6961             radia
-0000a2a0: 6c5f 616e 676c 6520 3d20 666c 6f61 7428  l_angle = float(
-0000a2b0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-0000a2c0: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
-0000a2d0: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 2020 2020 2020 2020 2072 6164               rad
-0000a300: 6975 7320 3d20 666c 6f61 7428 616c 6c5f  ius = float(all_
-0000a310: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-0000a320: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000a2a0: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
+0000a2b0: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
+0000a2c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a310: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
+0000a320: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
+0000a330: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 2020 2076 6f6c 756d 655f 7069 7865 6c73     volume_pixels
-0000a360: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
-0000a370: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-0000a380: 662e 7175 616c 6974 795f 6b65 795d 2929  f.quality_key]))
-0000a390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2020 2020 746f 7461 6c5f 696e 7465        total_inte
-0000a3c0: 6e73 6974 7920 3d20 2066 6c6f 6174 2861  nsity =  float(a
-0000a3d0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-0000a3e0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000a3f0: 6974 795f 6b65 795d 290d 0a20 2020 2020  ity_key])..     
+0000a350: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a370: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+0000a380: 5f64 6963 745f 7661 6c75 6573 203d 2073  _dict_values = s
+0000a390: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+0000a3a0: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
-0000a450: 6c5f 6d61 736b 203d 2066 6c6f 6174 2861  l_mask = float(a
-0000a460: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-0000a470: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
-0000a480: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 2020  l_mask_key])..  
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 2020 7472 6163 6b5f 6469 7370 6c61 6365    track_displace
-0000a4c0: 6d65 6e74 2c74 6f74 616c 5f74 7261 636b  ment,total_track
-0000a4d0: 5f64 6973 7461 6e63 652c 206d 6178 5f74  _distance, max_t
-0000a4e0: 7261 636b 5f64 6973 7461 6e63 652c 2074  rack_distance, t
-0000a4f0: 7261 636b 5f64 7572 6174 696f 6e20 203d  rack_duration  =
-0000a500: 2020 7365 6c66 2e5f 6765 745f 7472 6163    self._get_trac
-0000a510: 6b5f 6665 6174 7572 6573 2874 7261 636b  k_features(track
-0000a520: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0000a410: 2020 2020 2020 2020 2020 2020 2074 203d               t =
+0000a420: 2069 6e74 2866 6c6f 6174 2861 6c6c 5f64   int(float(all_d
+0000a430: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+0000a440: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a470: 2020 2020 7a20 3d20 666c 6f61 7428 616c      z = float(al
+0000a480: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000a490: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+0000a4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4c0: 2020 2020 2079 203d 2066 6c6f 6174 2861       y = float(a
+0000a4d0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000a4e0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+0000a4f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 2020 2020 7820 3d20 666c 6f61 7428        x = float(
+0000a520: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+0000a530: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+0000a540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
-0000a5a0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
-0000a5b0: 6e20 616c 6c5f 6469 6374 5f76 616c 7565  n all_dict_value
-0000a5c0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a560: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000a590: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
+0000a5a0: 6964 203d 2028 742c 726f 756e 6428 7a29  id = (t,round(z)
+0000a5b0: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
+0000a5c0: 6f6e 2c20 726f 756e 6428 7929 2f73 656c  on, round(y)/sel
+0000a5d0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+0000a5e0: 726f 756e 6428 7829 2f73 656c 662e 7863  round(x)/self.xc
+0000a5f0: 616c 6962 7261 7469 6f6e 2920 0d0a 0d0a  alibration) ....
 0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
-0000a630: 636f 6d70 5f66 6972 7374 203d 2066 6c6f  comp_first = flo
-0000a640: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-0000a650: 6573 5b73 656c 662e 6563 6365 6e74 7269  es[self.eccentri
-0000a660: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
-0000a670: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-0000a6b0: 6d70 5f73 6563 6f6e 6420 3d20 666c 6f61  mp_second = floa
-0000a6c0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-0000a6d0: 735b 7365 6c66 2e65 6363 656e 7472 6963  s[self.eccentric
-0000a6e0: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
-0000a6f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a720: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
-0000a730: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-0000a740: 616c 7565 735b 7365 6c66 2e73 7572 6661  alues[self.surfa
-0000a750: 6365 5f61 7265 615f 6b65 795d 290d 0a20  ce_area_key]).. 
-0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a780: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
-0000a790: 7869 735f 6d61 736b 203d 2066 6c6f 6174  xis_mask = float
-0000a7a0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-0000a7b0: 5b73 656c 662e 6365 6c6c 6178 6973 5f6d  [self.cellaxis_m
-0000a7c0: 6173 6b5f 6b65 795d 290d 0a20 2020 2020  ask_key])..     
-0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a820: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000a850: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000a890: 705f 6669 7273 7420 3d20 2d31 0d0a 2020  p_first = -1..  
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-0000a8d0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-0000a8e0: 6e64 203d 202d 310d 0a20 2020 2020 2020  nd = -1..       
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a910: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
-0000a920: 6120 3d20 2d31 0d0a 2020 2020 2020 2020  a = -1..        
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a950: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
-0000a960: 736b 203d 202d 3120 2020 2020 0d0a 0d0a  sk = -1     ....
+0000a620: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000a630: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
+0000a640: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+0000a650: 645d 203d 206b 0d0a 2020 2020 2020 2020  d] = k..        
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a680: 2e75 6e69 7175 655f 7472 6163 6b5f 6365  .unique_track_ce
+0000a690: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
+0000a6a0: 745f 6365 6e74 726f 6964 5d20 3d20 7472  t_centroid] = tr
+0000a6b0: 6163 6b5f 6964 0d0a 2020 2020 2020 2020  ack_id..        
+0000a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000a6e0: 2064 6566 205f 7365 636f 6e64 5f63 6861   def _second_cha
+0000a6f0: 6e6e 656c 5f75 7064 6174 6528 7365 6c66  nnel_update(self
+0000a700: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
+0000a710: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
+0000a720: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a730: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000a740: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+0000a750: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000a760: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000a770: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+0000a780: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+0000a790: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+0000a7a0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+0000a7b0: 662e 6672 616d 6569 645f 6b65 795d 0d0a  f.frameid_key]..
+0000a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7d0: 7a20 3d20 7365 6c66 2e75 6e69 7175 655f  z = self.unique_
+0000a7e0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000a7f0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+0000a800: 6c66 2e7a 706f 7369 645f 6b65 795d 2f73  lf.zposid_key]/s
+0000a810: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+0000a820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a830: 2020 7920 3d20 7365 6c66 2e75 6e69 7175    y = self.uniqu
+0000a840: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000a850: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+0000a860: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+0000a870: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
+0000a880: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+0000a890: 2020 2020 7820 3d20 7365 6c66 2e75 6e69      x = self.uni
+0000a8a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000a8b0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+0000a8c0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+0000a8d0: 795d 2f73 656c 662e 7863 616c 6962 7261  y]/self.xcalibra
+0000a8e0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+0000a8f0: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+0000a900: 6e64 5f63 6861 6e6e 656c 5f73 706f 7473  nd_channel_spots
+0000a910: 2866 7261 6d65 2c20 7a2c 2079 2c20 782c  (frame, z, y, x,
+0000a920: 2063 656c 6c5f 6964 2c20 7472 6163 6b5f   cell_id, track_
+0000a930: 6964 290d 0a20 2020 2020 2020 200d 0a20  id)..        .. 
+0000a940: 2020 2064 6566 205f 6669 6e61 6c5f 7472     def _final_tr
+0000a950: 6163 6b73 2873 656c 662c 2074 7261 636b  acks(self, track
+0000a960: 5f69 6429 3a0d 0a0d 0a20 2020 2020 2020  _id):....       
 0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a990: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
-0000a9a0: 656e 7472 6f69 6420 3d20 2874 2c72 6f75  entroid = (t,rou
-0000a9b0: 6e64 287a 292f 7365 6c66 2e7a 6361 6c69  nd(z)/self.zcali
-0000a9c0: 6272 6174 696f 6e2c 2072 6f75 6e64 2879  bration, round(y
-0000a9d0: 292f 7365 6c66 2e79 6361 6c69 6272 6174  )/self.ycalibrat
-0000a9e0: 696f 6e2c 2072 6f75 6e64 2878 292f 7365  ion, round(x)/se
-0000a9f0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
-0000aa00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-0000aa30: 7565 5f73 706f 745f 6365 6e74 726f 6964  ue_spot_centroid
-0000aa40: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
-0000aa50: 726f 6964 5d20 3d20 6b0d 0a0d 0a20 2020  roid] = k....   
-0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa80: 2069 6620 6375 7272 656e 745f 7472 6163   if current_trac
-0000aa90: 6b5f 6964 2069 6e20 6375 7272 656e 745f  k_id in current_
-0000aaa0: 7472 6163 6b6c 6574 733a 0d0a 2020 2020  tracklets:..    
-0000aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aad0: 2020 2020 7472 6163 6b6c 6574 5f61 7272      tracklet_arr
-0000aae0: 6179 203d 2063 7572 7265 6e74 5f74 7261  ay = current_tra
-0000aaf0: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
-0000ab00: 7261 636b 5f69 645d 0d0a 2020 2020 2020  rack_id]..      
+0000a980: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+0000a990: 6c5f 6964 7320 3d20 7365 6c66 2e61 6c6c  l_ids = self.all
+0000a9a0: 5f63 7572 7265 6e74 5f63 656c 6c5f 6964  _current_cell_id
+0000a9b0: 735b 696e 7428 7472 6163 6b5f 6964 295d  s[int(track_id)]
+0000a9c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a9d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000a9e0: 7272 656e 745f 7472 6163 6b6c 6574 7320  rrent_tracklets 
+0000a9f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+0000aa20: 6574 735f 7072 6f70 6572 7469 6573 203d  ets_properties =
+0000aa30: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000aa70: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+0000aa80: 6e28 6375 7272 656e 745f 6365 6c6c 5f69  n(current_cell_i
+0000aa90: 6473 2929 3a0d 0a20 2020 2020 2020 2020  ds)):..         
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000aac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2020 206b 203d 2069 6e74 2863 7572       k = int(cur
+0000aaf0: 7265 6e74 5f63 656c 6c5f 6964 735b 695d  rent_cell_ids[i]
+0000ab00: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
 0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab30: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-0000ab40: 6574 5f61 7272 6179 203d 206e 702e 6172  et_array = np.ar
-0000ab50: 7261 7928 5b69 6e74 2866 6c6f 6174 2875  ray([int(float(u
-0000ab60: 6e69 7175 655f 6964 2929 2c20 742c 207a  nique_id)), t, z
-0000ab70: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
-0000ab80: 6f6e 2c20 792f 7365 6c66 2e79 6361 6c69  on, y/self.ycali
-0000ab90: 6272 6174 696f 6e2c 2078 2f73 656c 662e  bration, x/self.
-0000aba0: 7863 616c 6962 7261 7469 6f6e 5d29 0d0a  xcalibration])..
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+0000ab30: 6963 745f 7661 6c75 6573 203d 2073 656c  ict_values = sel
+0000ab40: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000ab50: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2075 6e69 7175 655f 6964 203d 2073 7472   unique_id = str
+0000ab90: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000aba0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000abb0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0000abe0: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
-0000abf0: 745f 7472 6163 6b5f 6964 5d20 3d20 6e70  t_track_id] = np
-0000ac00: 2e76 7374 6163 6b28 2874 7261 636b 6c65  .vstack((trackle
-0000ac10: 745f 6172 7261 792c 2063 7572 7265 6e74  t_array, current
-0000ac20: 5f74 7261 636b 6c65 745f 6172 7261 7929  _tracklet_array)
-0000ac30: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0000ac60: 7565 5f61 7272 6179 203d 2063 7572 7265  ue_array = curre
-0000ac70: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-0000ac80: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
-0000ac90: 7472 6163 6b5f 6964 5d0d 0a20 2020 2020  track_id]..     
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acc0: 2020 2063 7572 7265 6e74 5f76 616c 7565     current_value
-0000acd0: 5f61 7272 6179 203d 206e 702e 6172 7261  _array = np.arra
-0000ace0: 7928 5b74 2c20 696e 7428 666c 6f61 7428  y([t, int(float(
-0000acf0: 756e 6971 7565 5f69 6429 292c 2067 656e  unique_id)), gen
-0000ad00: 5f69 642c 2072 6164 6975 732c 2076 6f6c  _id, radius, vol
-0000ad10: 756d 655f 7069 7865 6c73 2c20 6563 6365  ume_pixels, ecce
-0000ad20: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-0000ad30: 7273 742c 2065 6363 656e 7472 6963 6974  rst, eccentricit
-0000ad40: 795f 636f 6d70 5f73 6563 6f6e 642c 2073  y_comp_second, s
-0000ad50: 7572 6661 6365 5f61 7265 612c 2074 6f74  urface_area, tot
-0000ad60: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
-0000ad70: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
-0000ad80: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
-0000ad90: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
-0000ada0: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
-0000adb0: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
-0000adc0: 6b2c 7472 6163 6b5f 6469 7370 6c61 6365  k,track_displace
-0000add0: 6d65 6e74 2c20 746f 7461 6c5f 7472 6163  ment, total_trac
-0000ade0: 6b5f 6469 7374 616e 6365 2c20 6d61 785f  k_distance, max_
-0000adf0: 7472 6163 6b5f 6469 7374 616e 6365 2c20  track_distance, 
-0000ae00: 7472 6163 6b5f 6475 7261 7469 6f6e 205d  track_duration ]
-0000ae10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+0000abe0: 745f 7472 6163 6b5f 6964 203d 2073 7472  t_track_id = str
+0000abf0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000ac00: 5b73 656c 662e 7472 6163 6b69 645f 6b65  [self.trackid_ke
+0000ac10: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac30: 2020 2020 2020 2020 2074 203d 2069 6e74           t = int
+0000ac40: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
+0000ac50: 7661 6c75 6573 5b73 656c 662e 6672 616d  values[self.fram
+0000ac60: 6569 645f 6b65 795d 2929 0d0a 2020 2020  eid_key]))..    
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac90: 7a20 3d20 666c 6f61 7428 616c 6c5f 6469  z = float(all_di
+0000aca0: 6374 5f76 616c 7565 735b 7365 6c66 2e7a  ct_values[self.z
+0000acb0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2079 203d 2066 6c6f 6174 2861 6c6c 5f64   y = float(all_d
+0000acf0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+0000ad00: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 7820 3d20 666c 6f61 7428 616c 6c5f    x = float(all_
+0000ad40: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+0000ad50: 2e78 706f 7369 645f 6b65 795d 290d 0a0d  .xposid_key])...
+0000ad60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+0000ad90: 636b 6c65 7473 2c20 6375 7272 656e 745f  cklets, current_
+0000ada0: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+0000adb0: 7469 6573 203d 2073 656c 662e 5f74 7261  ties = self._tra
+0000adc0: 636b 6c65 745f 616e 645f 7072 6f70 6572  cklet_and_proper
+0000add0: 7469 6573 2820 616c 6c5f 6469 6374 5f76  ties( all_dict_v
+0000ade0: 616c 7565 732c 2074 2c20 7a2c 2079 2c20  alues, t, z, y, 
+0000adf0: 782c 206b 2c20 6375 7272 656e 745f 7472  x, k, current_tr
+0000ae00: 6163 6b5f 6964 2c20 756e 6971 7565 5f69  ack_id, unique_i
+0000ae10: 642c 2063 7572 7265 6e74 5f74 7261 636b  d, current_track
+0000ae20: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
+0000ae30: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+0000ae40: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
 0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae60: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-0000ae70: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-0000ae80: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
-0000ae90: 6964 5d20 3d20 6e70 2e76 7374 6163 6b28  id] = np.vstack(
-0000aea0: 2876 616c 7565 5f61 7272 6179 2c20 6375  (value_array, cu
-0000aeb0: 7272 656e 745f 7661 6c75 655f 6172 7261  rrent_value_arra
-0000aec0: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aee0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000aef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-0000af20: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
-0000af30: 203d 206e 702e 6172 7261 7928 5b69 6e74   = np.array([int
-0000af40: 2866 6c6f 6174 2875 6e69 7175 655f 6964  (float(unique_id
-0000af50: 2929 2c20 742c 207a 2f73 656c 662e 7a63  )), t, z/self.zc
-0000af60: 616c 6962 7261 7469 6f6e 2c20 792f 7365  alibration, y/se
-0000af70: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-0000af80: 2078 2f73 656c 662e 7863 616c 6962 7261   x/self.xcalibra
-0000af90: 7469 6f6e 5d29 0d0a 2020 2020 2020 2020  tion])..        
-0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afc0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-0000afd0: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
-0000afe0: 6964 5d20 3d20 6375 7272 656e 745f 7472  id] = current_tr
-0000aff0: 6163 6b6c 6574 5f61 7272 6179 200d 0a0d  acklet_array ...
-0000b000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b020: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000b030: 5f76 616c 7565 5f61 7272 6179 203d 206e  _value_array = n
-0000b040: 702e 6172 7261 7928 5b74 2c20 696e 7428  p.array([t, int(
-0000b050: 666c 6f61 7428 756e 6971 7565 5f69 6429  float(unique_id)
-0000b060: 292c 2067 656e 5f69 642c 2072 6164 6975  ), gen_id, radiu
-0000b070: 732c 2076 6f6c 756d 655f 7069 7865 6c73  s, volume_pixels
-0000b080: 2c20 2065 6363 656e 7472 6963 6974 795f  ,  eccentricity_
-0000b090: 636f 6d70 5f66 6972 7374 2c20 6563 6365  comp_first, ecce
-0000b0a0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-0000b0b0: 636f 6e64 2c20 7375 7266 6163 655f 6172  cond, surface_ar
-0000b0c0: 6561 2c20 2074 6f74 616c 5f69 6e74 656e  ea,  total_inten
-0000b0d0: 7369 7479 2c20 7370 6565 642c 206d 6f74  sity, speed, mot
-0000b0e0: 696f 6e5f 616e 676c 652c 2061 6363 656c  ion_angle, accel
-0000b0f0: 6572 6174 696f 6e2c 2064 6973 7461 6e63  eration, distanc
-0000b100: 655f 6365 6c6c 5f6d 6173 6b2c 2072 6164  e_cell_mask, rad
-0000b110: 6961 6c5f 616e 676c 652c 2063 656c 6c5f  ial_angle, cell_
-0000b120: 6178 6973 5f6d 6173 6b2c 7472 6163 6b5f  axis_mask,track_
-0000b130: 6469 7370 6c61 6365 6d65 6e74 2c20 746f  displacement, to
-0000b140: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
-0000b150: 6365 2c20 6d61 785f 7472 6163 6b5f 6469  ce, max_track_di
-0000b160: 7374 616e 6365 2c20 7472 6163 6b5f 6475  stance, track_du
-0000b170: 7261 7469 6f6e 205d 290d 0a20 2020 2020  ration ])..     
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-0000b1b0: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
-0000b1c0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-0000b1d0: 5d20 3d20 6375 7272 656e 745f 7661 6c75  ] = current_valu
-0000b1e0: 655f 6172 7261 790d 0a0d 0a20 2020 2020  e_array....     
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b210: 6574 7572 6e20 6375 7272 656e 745f 7472  eturn current_tr
-0000b220: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
-0000b230: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-0000b240: 7274 6965 7320 2020 2020 0d0a 0d0a 2020  rties     ....  
-0000b250: 2020 6465 6620 5f6d 6173 7465 725f 7370    def _master_sp
-0000b260: 6f74 5f63 6f6d 7075 7465 7228 7365 6c66  ot_computer(self
-0000b270: 2c20 6672 616d 6529 3a0d 0a20 2020 2020  , frame):..     
-0000b280: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000b290: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-0000b2a0: 696e 2066 7261 6d65 2e66 696e 6461 6c6c  in frame.findall
-0000b2b0: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
+0000ae60: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+0000ae90: 5f74 7261 636b 6c65 7473 203d 206e 702e  _tracklets = np.
+0000aea0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+0000aeb0: 7472 6163 6b6c 6574 735b 7374 7228 7472  tracklets[str(tr
+0000aec0: 6163 6b5f 6964 295d 2c20 6474 7970 653d  ack_id)], dtype=
+0000aed0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aef0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+0000af00: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+0000af10: 7274 6965 7320 3d20 6e70 2e61 7361 7272  rties = np.asarr
+0000af20: 6179 2863 7572 7265 6e74 5f74 7261 636b  ay(current_track
+0000af30: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+0000af40: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
+0000af50: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+0000af60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000af70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000af80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000af90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000afa0: 662e 756e 6971 7565 5f74 7261 636b 735b  f.unique_tracks[
+0000afb0: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
+0000afc0: 656e 745f 7472 6163 6b6c 6574 7320 2020  ent_tracklets   
+0000afd0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aff0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+0000b000: 6b5f 7072 6f70 6572 7469 6573 5b74 7261  k_properties[tra
+0000b010: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
+0000b020: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+0000b030: 7274 6965 7320 2020 200d 0a0d 0a20 2020  rties    ....   
+0000b040: 2064 6566 205f 7472 6163 6b6c 6574 5f61   def _tracklet_a
+0000b050: 6e64 5f70 726f 7065 7274 6965 7328 7365  nd_properties(se
+0000b060: 6c66 2c61 6c6c 5f64 6963 745f 7661 6c75  lf,all_dict_valu
+0000b070: 6573 2c20 742c 207a 2c20 792c 2078 2c20  es, t, z, y, x, 
+0000b080: 6b2c 2063 7572 7265 6e74 5f74 7261 636b  k, current_track
+0000b090: 5f69 642c 2075 6e69 7175 655f 6964 2c20  _id, unique_id, 
+0000b0a0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+0000b0b0: 732c 2063 7572 7265 6e74 5f74 7261 636b  s, current_track
+0000b0c0: 6c65 7473 5f70 726f 7065 7274 6965 7329  lets_properties)
+0000b0d0: 3a0d 0a20 2020 2020 2020 2020 2020 0d0a  :..           ..
+0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b100: 2020 2020 6765 6e5f 6964 203d 2069 6e74      gen_id = int
+0000b110: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
+0000b120: 7661 6c75 6573 5b73 656c 662e 6765 6e65  values[self.gene
+0000b130: 7261 7469 6f6e 6964 5f6b 6579 5d29 290d  rationid_key])).
+0000b140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b160: 2020 2020 2073 7065 6564 203d 2066 6c6f       speed = flo
+0000b170: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000b180: 6573 5b73 656c 662e 7370 6565 645f 6b65  es[self.speed_ke
+0000b190: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 2020 2020 2020 2061 6363 656c 6572           acceler
+0000b1c0: 6174 696f 6e20 3d20 666c 6f61 7428 616c  ation = float(al
+0000b1d0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000b1e0: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+0000b1f0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+0000b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b210: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
+0000b220: 6e5f 616e 676c 6520 3d20 666c 6f61 7428  n_angle = float(
+0000b230: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+0000b240: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+0000b250: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b270: 2020 2020 2020 2020 2020 2020 2072 6164               rad
+0000b280: 6961 6c5f 616e 676c 6520 3d20 666c 6f61  ial_angle = floa
+0000b290: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+0000b2a0: 735b 7365 6c66 2e72 6164 6961 6c5f 616e  s[self.radial_an
+0000b2b0: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
 0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000b2e0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000b2f0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
-0000b300: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-0000b310: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b2e0: 6164 6975 7320 3d20 666c 6f61 7428 616c  adius = float(al
+0000b2f0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000b300: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
+0000b310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b330: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000b340: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000b350: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000b360: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
-0000b370: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0000b330: 2020 2020 2076 6f6c 756d 655f 7069 7865       volume_pixe
+0000b340: 6c73 203d 2069 6e74 2866 6c6f 6174 2861  ls = int(float(a
+0000b350: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000b360: 656c 662e 7175 616c 6974 795f 6b65 795d  elf.quality_key]
+0000b370: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 7261 6469 7573 203d 2066 6c6f 6174    radius = float
-0000b3c0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000b3d0: 7365 6c66 2e72 6164 6975 735f 6b65 7929  self.radius_key)
-0000b3e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b390: 2020 2020 2020 2020 746f 7461 6c5f 696e          total_in
+0000b3a0: 7465 6e73 6974 7920 3d20 2066 6c6f 6174  tensity =  float
+0000b3b0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000b3c0: 5b73 656c 662e 746f 7461 6c5f 696e 7465  [self.total_inte
+0000b3d0: 6e73 6974 795f 6b65 795d 290d 0a20 2020  nsity_key])..   
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 2071 7561 6c69 7479 203d 2066 6c6f     quality = flo
-0000b410: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b420: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
-0000b430: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b450: 2020 2020 2020 746f 7461 6c5f 696e 7465        total_inte
-0000b460: 6e73 6974 7920 3d20 666c 6f61 7428 5370  nsity = float(Sp
-0000b470: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b480: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000b490: 795f 6b65 7929 290d 0a20 2020 2020 2020  y_key))..       
+0000b400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+0000b430: 656c 6c5f 6d61 736b 203d 2066 6c6f 6174  ell_mask = float
+0000b440: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000b450: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+0000b460: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
 0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 2020 2020 2020 206d 6561 6e5f 696e           mean_in
-0000b4c0: 7465 6e73 6974 7920 3d20 666c 6f61 7428  tensity = float(
-0000b4d0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b4e0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-0000b4f0: 7479 5f6b 6579 2929 0d0a 0d0a 2020 2020  ty_key))....    
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b520: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-0000b530: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000b540: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+0000b4b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2069 6620 7365 6c66 2e73 7572 6661     if self.surfa
+0000b4f0: 6365 5f61 7265 615f 6b65 7920 696e 2061  ce_area_key in a
+0000b500: 6c6c 5f64 6963 745f 7661 6c75 6573 2e6b  ll_dict_values.k
+0000b510: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000b570: 656c 6c69 645f 6b65 793a 2069 6e74 2866  ellid_key: int(f
-0000b580: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b590: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-0000b5a0: 6b65 7929 2929 2c20 0d0a 2020 2020 2020  key))), ..      
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b5d0: 6c66 2e66 7261 6d65 6964 5f6b 6579 203a  lf.frameid_key :
-0000b5e0: 2069 6e74 2866 6c6f 6174 2853 706f 746f   int(float(Spoto
-0000b5f0: 626a 6563 742e 6765 7428 7365 6c66 2e66  bject.get(self.f
-0000b600: 7261 6d65 6964 5f6b 6579 2929 292c 0d0a  rameid_key))),..
-0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b630: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
-0000b640: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000b650: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b660: 7a70 6f73 6964 5f6b 6579 2929 2c0d 0a20  zposid_key)),.. 
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2073 656c 662e 7970 6f73 6964 5f6b     self.yposid_k
-0000b6a0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000b6b0: 626a 6563 742e 6765 7428 7365 6c66 2e79  bject.get(self.y
-0000b6c0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
-0000b700: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000b710: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
-0000b720: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b570: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000b580: 705f 6669 7273 7420 3d20 666c 6f61 7428  p_first = float(
+0000b590: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+0000b5a0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+0000b5b0: 795f 636f 6d70 5f66 6972 7374 6b65 795d  y_comp_firstkey]
+0000b5c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+0000b5f0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000b600: 7365 636f 6e64 203d 2066 6c6f 6174 2861  second = float(a
+0000b610: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000b620: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+0000b630: 5f63 6f6d 705f 7365 636f 6e64 6b65 795d  _comp_secondkey]
+0000b640: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2020 2020 2020 2020 2020 2020 2020 7375                su
+0000b670: 7266 6163 655f 6172 6561 203d 2066 6c6f  rface_area = flo
+0000b680: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000b690: 6573 5b73 656c 662e 7375 7266 6163 655f  es[self.surface_
+0000b6a0: 6172 6561 5f6b 6579 5d29 0d0a 2020 2020  area_key])..    
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6d0: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+0000b6e0: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
+0000b6f0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000b700: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+0000b710: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2073 656c 662e 746f 7461 6c5f 696e 7465   self.total_inte
-0000b760: 6e73 6974 795f 6b65 7920 3a20 746f 7461  nsity_key : tota
-0000b770: 6c5f 696e 7465 6e73 6974 792c 0d0a 2020  l_intensity,..  
+0000b740: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
-0000b7b0: 6e73 6974 795f 6b65 7920 3a20 6d65 616e  nsity_key : mean
-0000b7c0: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
-0000b800: 203a 2072 6164 6975 732c 0d0a 2020 2020   : radius,..    
-0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000b840: 203a 2071 7561 6c69 7479 2c0d 0a20 2020   : quality,..   
+0000b790: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000b7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+0000b7d0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000b7e0: 6972 7374 203d 202d 310d 0a20 2020 2020  irst = -1..     
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
+0000b820: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
+0000b830: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
-0000b880: 656c 6c5f 6d61 736b 5f6b 6579 3a20 2866  ell_mask_key: (f
-0000b890: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b8a0: 6765 7428 7365 6c66 2e64 6973 7461 6e63  get(self.distanc
-0000b8b0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 7929  e_cell_mask_key)
-0000b8c0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000b860: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+0000b870: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
+0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8a0: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
+0000b8b0: 3d20 2d31 2020 2020 200d 0a0d 0a20 2020  = -1     ....   
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8e0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-0000b8f0: 6971 7565 6964 5f6b 6579 203a 2073 7472  iqueid_key : str
-0000b900: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000b910: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-0000b920: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000b950: 7261 636b 6c65 7469 645f 6b65 7920 3a20  rackletid_key : 
-0000b960: 7374 7228 5370 6f74 6f62 6a65 6374 2e67  str(Spotobject.g
-0000b970: 6574 2873 656c 662e 7472 6163 6b6c 6574  et(self.tracklet
-0000b980: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b9b0: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
-0000b9c0: 5f6b 6579 203a 2073 7472 2853 706f 746f  _key : str(Spoto
-0000b9d0: 626a 6563 742e 6765 7428 7365 6c66 2e67  bject.get(self.g
-0000b9e0: 656e 6572 6174 696f 6e69 645f 6b65 7929  enerationid_key)
-0000b9f0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000b8e0: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
+0000b8f0: 726f 6964 203d 2028 742c 726f 756e 6428  roid = (t,round(
+0000b900: 7a29 2f73 656c 662e 7a63 616c 6962 7261  z)/self.zcalibra
+0000b910: 7469 6f6e 2c20 726f 756e 6428 7929 2f73  tion, round(y)/s
+0000b920: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+0000b930: 2c20 726f 756e 6428 7829 2f73 656c 662e  , round(x)/self.
+0000b940: 7863 616c 6962 7261 7469 6f6e 2920 0d0a  xcalibration) ..
+0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b970: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000b980: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
+0000b990: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+0000b9a0: 645d 203d 206b 0d0a 0d0a 2020 2020 2020  d] = k....      
+0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b9d0: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
+0000b9e0: 6420 696e 2063 7572 7265 6e74 5f74 7261  d in current_tra
+0000b9f0: 636b 6c65 7473 3a0d 0a20 2020 2020 2020  cklets:..       
 0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000ba20: 636b 6964 5f6b 6579 203a 2073 7472 2853  ckid_key : str(S
-0000ba30: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000ba40: 6c66 2e74 7261 636b 6964 5f6b 6579 2929  lf.trackid_key))
-0000ba50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba20: 2074 7261 636b 6c65 745f 6172 7261 7920   tracklet_array 
+0000ba30: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
+0000ba40: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
+0000ba50: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
 0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba70: 2020 2020 2020 2073 656c 662e 6d6f 7469         self.moti
-0000ba80: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 2028  on_angle_key : (
-0000ba90: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000baa0: 2e67 6574 2873 656c 662e 6d6f 7469 6f6e  .get(self.motion
-0000bab0: 5f61 6e67 6c65 5f6b 6579 2929 292c 0d0a  _angle_key))),..
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 7365 6c66 2e73 7065 6564 5f6b      self.speed_k
-0000baf0: 6579 203a 2028 666c 6f61 7428 5370 6f74  ey : (float(Spot
-0000bb00: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000bb10: 7370 6565 645f 6b65 7929 2929 2c0d 0a20  speed_key))),.. 
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 2020 2073 656c 662e 6163 6365 6c65 7261     self.accelera
-0000bb50: 7469 6f6e 5f6b 6579 203a 2028 666c 6f61  tion_key : (floa
-0000bb60: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000bb70: 2873 656c 662e 6163 6365 6c65 7261 7469  (self.accelerati
-0000bb80: 6f6e 5f6b 6579 2929 292c 0d0a 2020 2020  on_key))),..    
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000ba80: 7572 7265 6e74 5f74 7261 636b 6c65 745f  urrent_tracklet_
+0000ba90: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
+0000baa0: 285b 696e 7428 666c 6f61 7428 756e 6971  ([int(float(uniq
+0000bab0: 7565 5f69 6429 292c 2074 2c20 7a2f 7365  ue_id)), t, z/se
+0000bac0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+0000bad0: 2079 2f73 656c 662e 7963 616c 6962 7261   y/self.ycalibra
+0000bae0: 7469 6f6e 2c20 782f 7365 6c66 2e78 6361  tion, x/self.xca
+0000baf0: 6c69 6272 6174 696f 6e5d 290d 0a20 2020  libration])..   
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+0000bb30: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
+0000bb40: 7261 636b 5f69 645d 203d 206e 702e 7673  rack_id] = np.vs
+0000bb50: 7461 636b 2828 7472 6163 6b6c 6574 5f61  tack((tracklet_a
+0000bb60: 7272 6179 2c20 6375 7272 656e 745f 7472  rray, current_tr
+0000bb70: 6163 6b6c 6574 5f61 7272 6179 2929 0d0a  acklet_array))..
+0000bb80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbb0: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
-0000bbc0: 655f 6b65 793a 2066 6c6f 6174 2853 706f  e_key: float(Spo
-0000bbd0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bbe0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
-0000bbf0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000bba0: 2020 2020 2020 2020 2020 7661 6c75 655f            value_
+0000bbb0: 6172 7261 7920 3d20 6375 7272 656e 745f  array = current_
+0000bbc0: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+0000bbd0: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
+0000bbe0: 636b 5f69 645d 0d0a 2020 2020 2020 2020  ck_id]..        
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc10: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000bc40: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-0000bc50: 7920 696e 2053 706f 746f 626a 6563 742e  y in Spotobject.
-0000bc60: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000bc90: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-0000bca0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-0000bcb0: 6c5f 6964 295d 2e75 7064 6174 6528 7b0d  l_id)].update({.
-0000bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
-0000bd20: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000bd30: 6669 7273 746b 6579 203a 2066 6c6f 6174  firstkey : float
-0000bd40: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bd50: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-0000bd60: 795f 636f 6d70 5f66 6972 7374 6b65 7929  y_comp_firstkey)
-0000bd70: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
+0000bc20: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
+0000bc30: 742c 2069 6e74 2866 6c6f 6174 2875 6e69  t, int(float(uni
+0000bc40: 7175 655f 6964 2929 2c20 6765 6e5f 6964  que_id)), gen_id
+0000bc50: 2c20 7261 6469 7573 2c20 766f 6c75 6d65  , radius, volume
+0000bc60: 5f70 6978 656c 732c 2065 6363 656e 7472  _pixels, eccentr
+0000bc70: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+0000bc80: 2c20 6563 6365 6e74 7269 6369 7479 5f63  , eccentricity_c
+0000bc90: 6f6d 705f 7365 636f 6e64 2c20 7375 7266  omp_second, surf
+0000bca0: 6163 655f 6172 6561 2c20 746f 7461 6c5f  ace_area, total_
+0000bcb0: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
+0000bcc0: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
+0000bcd0: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
+0000bce0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000bcf0: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
+0000bd00: 6365 6c6c 5f61 7869 735f 6d61 736b 2c74  cell_axis_mask,t
+0000bd10: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+0000bd20: 742c 2074 6f74 616c 5f74 7261 636b 5f64  t, total_track_d
+0000bd30: 6973 7461 6e63 652c 206d 6178 5f74 7261  istance, max_tra
+0000bd40: 636b 5f64 6973 7461 6e63 652c 2074 7261  ck_distance, tra
+0000bd50: 636b 5f64 7572 6174 696f 6e20 5d29 0d0a  ck_duration ])..
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bdd0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-0000bde0: 6d70 5f73 6563 6f6e 646b 6579 203a 2066  mp_secondkey : f
-0000bdf0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000be00: 6765 7428 7365 6c66 2e65 6363 656e 7472  get(self.eccentr
-0000be10: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000be20: 646b 6579 2929 2c0d 0a20 2020 2020 2020  dkey)),..       
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+0000bdc0: 6574 735f 7072 6f70 6572 7469 6573 5b63  ets_properties[c
+0000bdd0: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+0000bde0: 203d 206e 702e 7673 7461 636b 2828 7661   = np.vstack((va
+0000bdf0: 6c75 655f 6172 7261 792c 2063 7572 7265  lue_array, curre
+0000be00: 6e74 5f76 616c 7565 5f61 7272 6179 2929  nt_value_array))
+0000be10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be30: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
-0000be90: 6561 5f6b 6579 203a 2066 6c6f 6174 2853  ea_key : float(S
-0000bea0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000beb0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000bec0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+0000be70: 7261 636b 6c65 745f 6172 7261 7920 3d20  racklet_array = 
+0000be80: 6e70 2e61 7272 6179 285b 696e 7428 666c  np.array([int(fl
+0000be90: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
+0000bea0: 2074 2c20 7a2f 7365 6c66 2e7a 6361 6c69   t, z/self.zcali
+0000beb0: 6272 6174 696f 6e2c 2079 2f73 656c 662e  bration, y/self.
+0000bec0: 7963 616c 6962 7261 7469 6f6e 2c20 782f  ycalibration, x/
+0000bed0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000bee0: 6e5d 290d 0a20 2020 2020 2020 2020 2020  n])..           
 0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-0000bf30: 736b 5f6b 6579 3a20 666c 6f61 7428 5370  sk_key: float(Sp
-0000bf40: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bf50: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-0000bf60: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfc0: 2020 207d 290d 0a20 2020 2020 2020 2020     })..         
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c020: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c040: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 656c 6966 2073 656c 662e 756e 6971 7565  elif self.unique
-0000c070: 6964 5f6b 6579 206e 6f74 2069 6e20 5370  id_key not in Sp
-0000c080: 6f74 6f62 6a65 6374 2e6b 6579 7328 293a  otobject.keys():
-0000c090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000bf00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0000bf10: 7265 6e74 5f74 7261 636b 6c65 7473 5b63  rent_tracklets[c
+0000bf20: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+0000bf30: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
+0000bf40: 6c65 745f 6172 7261 7920 0d0a 0d0a 2020  let_array ....  
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 2020 2020 6375 7272 656e 745f 7661        current_va
+0000bf80: 6c75 655f 6172 7261 7920 3d20 6e70 2e61  lue_array = np.a
+0000bf90: 7272 6179 285b 742c 2069 6e74 2866 6c6f  rray([t, int(flo
+0000bfa0: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
+0000bfb0: 6765 6e5f 6964 2c20 7261 6469 7573 2c20  gen_id, radius, 
+0000bfc0: 766f 6c75 6d65 5f70 6978 656c 732c 2020  volume_pixels,  
+0000bfd0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000bfe0: 705f 6669 7273 742c 2065 6363 656e 7472  p_first, eccentr
+0000bff0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+0000c000: 642c 2073 7572 6661 6365 5f61 7265 612c  d, surface_area,
+0000c010: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+0000c020: 792c 2073 7065 6564 2c20 6d6f 7469 6f6e  y, speed, motion
+0000c030: 5f61 6e67 6c65 2c20 6163 6365 6c65 7261  _angle, accelera
+0000c040: 7469 6f6e 2c20 6469 7374 616e 6365 5f63  tion, distance_c
+0000c050: 656c 6c5f 6d61 736b 2c20 7261 6469 616c  ell_mask, radial
+0000c060: 5f61 6e67 6c65 2c20 6365 6c6c 5f61 7869  _angle, cell_axi
+0000c070: 735f 6d61 736b 2c74 7261 636b 5f64 6973  s_mask,track_dis
+0000c080: 706c 6163 656d 656e 742c 2074 6f74 616c  placement, total
+0000c090: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
+0000c0a0: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
+0000c0b0: 6e63 652c 2074 7261 636b 5f64 7572 6174  nce, track_durat
+0000c0c0: 696f 6e20 5d29 0d0a 2020 2020 2020 2020  ion ])..        
 0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000c100: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000c110: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
-0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c140: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000c150: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
-0000c160: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c170: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000c180: 7479 5f63 6832 5f6b 6579 290d 0a20 2020  ty_ch2_key)..   
-0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
-0000c1d0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
-0000c1e0: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-0000c1f0: 7369 7479 5f63 6832 5f6b 6579 290d 0a20  sity_ch2_key).. 
-0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c230: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 2020 2020 2020 2020 2020 2020 2020 544f                TO
-0000c270: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
-0000c280: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c290: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000c2a0: 6974 795f 6368 315f 6b65 7929 0d0a 2020  ity_ch1_key)..  
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000c2f0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
-0000c300: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
-0000c310: 6e73 6974 795f 6368 315f 6b65 7929 0d0a  nsity_ch1_key)..
-0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+0000c100: 735f 7072 6f70 6572 7469 6573 5b63 7572  s_properties[cur
+0000c110: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
+0000c120: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
+0000c130: 7272 6179 0d0a 0d0a 2020 2020 2020 2020  rray....        
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c160: 726e 2063 7572 7265 6e74 5f74 7261 636b  rn current_track
+0000c170: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
+0000c180: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+0000c190: 6573 2020 2020 200d 0a0d 0a20 2020 2064  es     ....    d
+0000c1a0: 6566 205f 6d61 7374 6572 5f73 706f 745f  ef _master_spot_
+0000c1b0: 636f 6d70 7574 6572 2873 656c 662c 2066  computer(self, f
+0000c1c0: 7261 6d65 293a 0d0a 2020 2020 2020 2020  rame):..        
+0000c1d0: 2020 0d0a 2020 2020 2020 2020 2020 666f    ..          fo
+0000c1e0: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
+0000c1f0: 6672 616d 652e 6669 6e64 616c 6c28 2753  frame.findall('S
+0000c200: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+0000c210: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000c220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c230: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000c240: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000c250: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000c260: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000c270: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000c280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c290: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000c2a0: 2e75 6e69 7175 6569 645f 6b65 7920 696e  .uniqueid_key in
+0000c2b0: 2053 706f 746f 626a 6563 742e 6b65 7973   Spotobject.keys
+0000c2c0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0000c2d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000c300: 6164 6975 7320 3d20 666c 6f61 7428 5370  adius = float(Sp
+0000c310: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c320: 662e 7261 6469 7573 5f6b 6579 2929 0d0a  f.radius_key))..
 0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
-0000c350: 5553 203d 2066 6c6f 6174 2853 706f 746f  US = float(Spoto
-0000c360: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
-0000c370: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
-0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 7175 616c 6974 7920 3d20 666c 6f61 7428  quality = float(
+0000c360: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c370: 656c 662e 7175 616c 6974 795f 6b65 7929  elf.quality_key)
+0000c380: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
-0000c3b0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000c3c0: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
-0000c3d0: 6c69 7479 5f6b 6579 2929 2020 2020 200d  lity_key))     .
-0000c3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c3a0: 2020 2074 6f74 616c 5f69 6e74 656e 7369     total_intensi
+0000c3b0: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
+0000c3c0: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000c3d0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000c3e0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000c410: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
-0000c420: 6c6f 6174 2854 4f54 414c 5f49 4e54 454e  loat(TOTAL_INTEN
-0000c430: 5349 5459 290d 0a20 2020 2020 2020 2020  SITY)..         
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 6d65 616e 5f69 6e74 656e        mean_inten
+0000c410: 7369 7479 203d 2066 6c6f 6174 2853 706f  sity = float(Spo
+0000c420: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000c430: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+0000c440: 6b65 7929 290d 0a0d 0a20 2020 2020 2020  key))....       
 0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000c470: 5920 3d20 666c 6f61 7428 4d45 414e 5f49  Y = float(MEAN_I
-0000c480: 4e54 454e 5349 5459 290d 0a20 2020 2020  NTENSITY)..     
-0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000c470: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000c480: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+0000c490: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
 0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-0000c4c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000c4d0: 6573 5b63 656c 6c5f 6964 5d20 3d20 7b0d  es[cell_id] = {.
-0000c4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c510: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
-0000c520: 7428 6365 6c6c 5f69 6429 2c20 0d0a 2020  t(cell_id), ..  
-0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0000c560: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
-0000c570: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000c580: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
-0000c590: 6964 5f6b 6579 2929 292c 0d0a 2020 2020  id_key))),..    
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5c0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
-0000c5d0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-0000c5e0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c5f0: 656c 662e 7a70 6f73 6964 5f6b 6579 2929  elf.zposid_key))
-0000c600: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c630: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
-0000c640: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000c650: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
-0000c660: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
-0000c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+0000c4c0: 6964 5f6b 6579 3a20 696e 7428 666c 6f61  id_key: int(floa
+0000c4d0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c4e0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000c4f0: 2929 292c 200d 0a20 2020 2020 2020 2020  ))), ..         
+0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c520: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+0000c530: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000c540: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
+0000c550: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c580: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000c590: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000c5a0: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000c5b0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000c5f0: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000c600: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
+0000c610: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c640: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000c650: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c660: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000c670: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
 0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c690: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
-0000c6a0: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000c6b0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000c6c0: 662e 7870 6f73 6964 5f6b 6579 2929 2c0d  f.xposid_key)),.
-0000c6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c700: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000c710: 795f 6b65 7920 3a20 544f 5441 4c5f 494e  y_key : TOTAL_IN
-0000c720: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
-0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c750: 2020 2020 2020 7365 6c66 2e6d 6561 6e5f        self.mean_
-0000c760: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
-0000c770: 4d45 414e 5f49 4e54 454e 5349 5459 2c0d  MEAN_INTENSITY,.
-0000c780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c7b0: 662e 7261 6469 7573 5f6b 6579 203a 2052  f.radius_key : R
-0000c7c0: 4144 4955 532c 0d0a 2020 2020 2020 2020  ADIUS,..        
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7f0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
-0000c800: 5f6b 6579 203a 2051 5541 4c49 5459 0d0a  _key : QUALITY..
-0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c6a0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000c6b0: 7479 5f6b 6579 203a 2074 6f74 616c 5f69  ty_key : total_i
+0000c6c0: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
+0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c6f0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000c700: 7479 5f6b 6579 203a 206d 6561 6e5f 696e  ty_key : mean_in
+0000c710: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
+0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c730: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c740: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+0000c750: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
+0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c770: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c780: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000c790: 7175 616c 6974 792c 0d0a 2020 2020 2020  quality,..      
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000c7c0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000c7d0: 5f6d 6173 6b5f 6b65 793a 2028 666c 6f61  _mask_key: (floa
+0000c7e0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000c7f0: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
+0000c800: 656c 6c5f 6d61 736b 5f6b 6579 2929 292c  ell_mask_key))),
+0000c810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c830: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0000c840: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c850: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c880: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-0000c890: 6566 205f 7370 6f74 5f63 6f6d 7075 7465  ef _spot_compute
-0000c8a0: 7228 7365 6c66 2c20 6672 616d 6529 3a0d  r(self, frame):.
-0000c8b0: 0a0d 0a20 2020 2020 2020 2020 2066 6f72  ...          for
-0000c8c0: 2053 706f 746f 626a 6563 7420 696e 2066   Spotobject in f
-0000c8d0: 7261 6d65 2e66 696e 6461 6c6c 2827 5370  rame.findall('Sp
-0000c8e0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000c900: 2043 7265 6174 6520 6f62 6a65 6374 2077   Create object w
-0000c910: 6974 6820 756e 6971 7565 2063 656c 6c20  ith unique cell 
-0000c920: 4944 0d0a 2020 2020 2020 2020 2020 2020  ID..            
-0000c930: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000c940: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
-0000c950: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
-0000c960: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
-0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c980: 2020 2020 2320 4765 7420 7468 6520 545a      # Get the TZ
-0000c990: 5958 206c 6f63 6174 696f 6e20 6f66 2074  YX location of t
-0000c9a0: 6865 2063 656c 6c73 2069 6e20 7468 6174  he cells in that
-0000c9b0: 2066 7261 6d65 0d0a 2020 2020 2020 2020   frame..        
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9d0: 6966 2073 656c 662e 6465 7465 6374 6f72  if self.detector
-0000c9e0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
-0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ca10: 6620 5370 6f74 6f62 6a65 6374 2e67 6574  f Spotobject.get
-0000ca20: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000ca30: 6e73 6974 795f 6368 325f 6b65 7929 2069  nsity_ch2_key) i
-0000ca40: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000ca80: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000ca90: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000caa0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000cab0: 5f63 6832 5f6b 6579 2929 0d0a 2020 2020  _ch2_key))..    
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
-0000caf0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000cb00: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
-0000cb10: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
-0000cb20: 325f 6b65 7929 290d 0a20 2020 2020 2020  2_key))..       
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb40: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000c830: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000c840: 6569 645f 6b65 7920 3a20 7374 7228 5370  eid_key : str(Sp
+0000c850: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c860: 662e 756e 6971 7565 6964 5f6b 6579 2929  f.uniqueid_key))
+0000c870: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000c8a0: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+0000c8b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000c8c0: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
+0000c8d0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c900: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+0000c910: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
+0000c920: 6374 2e67 6574 2873 656c 662e 6765 6e65  ct.get(self.gene
+0000c930: 7261 7469 6f6e 6964 5f6b 6579 2929 2c0d  rationid_key)),.
+0000c940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+0000c970: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
+0000c980: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000c990: 7472 6163 6b69 645f 6b65 7929 292c 0d0a  trackid_key)),..
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9c0: 2020 2020 7365 6c66 2e6d 6f74 696f 6e5f      self.motion_
+0000c9d0: 616e 676c 655f 6b65 7920 3a20 2866 6c6f  angle_key : (flo
+0000c9e0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000c9f0: 7428 7365 6c66 2e6d 6f74 696f 6e5f 616e  t(self.motion_an
+0000ca00: 676c 655f 6b65 7929 2929 2c0d 0a20 2020  gle_key))),..   
+0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca30: 2073 656c 662e 7370 6565 645f 6b65 7920   self.speed_key 
+0000ca40: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
+0000ca50: 6563 742e 6765 7428 7365 6c66 2e73 7065  ect.get(self.spe
+0000ca60: 6564 5f6b 6579 2929 292c 0d0a 2020 2020  ed_key))),..    
+0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000caa0: 6e5f 6b65 7920 3a20 2866 6c6f 6174 2853  n_key : (float(S
+0000cab0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000cac0: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+0000cad0: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000cb00: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
+0000cb10: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
+0000cb20: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000cb30: 6469 616c 5f61 6e67 6c65 5f6b 6579 2929  dial_angle_key))
+0000cb40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb70: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000cb80: 454e 5349 5459 203d 202d 310d 0a20 2020  ENSITY = -1..   
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbb0: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
-0000cbc0: 5459 203d 202d 3120 2020 2020 2020 0d0a  TY = -1       ..
-0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbe0: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
-0000cbf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc10: 2020 2020 2020 2069 6620 5370 6f74 6f62         if Spotob
-0000cc20: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
-0000cc30: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0000cc40: 315f 6b65 7929 2069 7320 6e6f 7420 4e6f  1_key) is not No
-0000cc50: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc70: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000cc80: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
-0000cc90: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000cca0: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
-0000ccb0: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
-0000ccc0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000cb60: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb80: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000cb90: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000cba0: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
+0000cbb0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000cbe0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000cbf0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000cc00: 6429 5d2e 7570 6461 7465 287b 0d0a 2020  d)].update({..  
+0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
+0000cc70: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+0000cc80: 7374 6b65 7920 3a20 666c 6f61 7428 5370  stkey : float(Sp
+0000cc90: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000cca0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+0000ccb0: 6f6d 705f 6669 7273 746b 6579 2929 2c0d  omp_firstkey)),.
+0000ccc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cce0: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
-0000ccf0: 5f49 4e54 454e 5349 5459 203d 2066 6c6f  _INTENSITY = flo
-0000cd00: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000cd10: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
-0000cd20: 6e73 6974 795f 6368 315f 6b65 7929 290d  nsity_ch1_key)).
-0000cd30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
-0000cd90: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
+0000cd20: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000cd30: 7365 636f 6e64 6b65 7920 3a20 666c 6f61  secondkey : floa
+0000cd40: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000cd50: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
+0000cd60: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+0000cd70: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000cdc0: 414e 5f49 4e54 454e 5349 5459 203d 202d  AN_INTENSITY = -
-0000cdd0: 3120 2020 2020 2020 2020 0d0a 0d0a 2020  1         ....  
-0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 2020 2020 2020 2020 5241 4449 5553 203d          RADIUS =
-0000ce20: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000ce30: 742e 6765 7428 7365 6c66 2e72 6164 6975  t.get(self.radiu
-0000ce40: 735f 6b65 7929 290d 0a20 2020 2020 2020  s_key))..       
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cdd0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+0000cde0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000cdf0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000ce00: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000ce10: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 2051 5541 4c49 5459 203d 2066 6c6f 6174   QUALITY = float
-0000ce70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000ce80: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000ce90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000cea0: 2020 2020 2020 2020 2020 2020 7465 7374              test
-0000ceb0: 6c6f 6361 7469 6f6e 203d 2028 666c 6f61  location = (floa
-0000cec0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000ced0: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
-0000cee0: 2929 2c20 666c 6f61 7428 5370 6f74 6f62  )), float(Spotob
-0000cef0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
-0000cf00: 6f73 6964 5f6b 6579 2929 2c20 2066 6c6f  osid_key)),  flo
-0000cf10: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000cf20: 7428 7365 6c66 2e78 706f 7369 645f 6b65  t(self.xposid_ke
-0000cf30: 7929 2929 0d0a 2020 2020 2020 2020 2020  y)))..          
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-0000cf50: 616d 6520 3d20 5370 6f74 6f62 6a65 6374  ame = Spotobject
-0000cf60: 2e67 6574 2873 656c 662e 6672 616d 6569  .get(self.framei
-0000cf70: 645f 6b65 7929 0d0a 2020 2020 2020 2020  d_key)..        
+0000ce60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ce70: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+0000ce80: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
+0000ce90: 626a 6563 742e 6765 7428 7365 6c66 2e63  bject.get(self.c
+0000cea0: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+0000ceb0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000cfa0: 736b 2c20 6d61 736b 6365 6e74 726f 6964  sk, maskcentroid
-0000cfb0: 203d 2073 656c 662e 5f67 6574 5f62 6f75   = self._get_bou
-0000cfc0: 6e64 6172 795f 6469 7374 2866 7261 6d65  ndary_dist(frame
-0000cfd0: 2c20 7465 7374 6c6f 6361 7469 6f6e 290d  , testlocation).
-0000cfe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cff0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000cf90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000cfa0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000cfb0: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
+0000cfc0: 6b65 7920 6e6f 7420 696e 2053 706f 746f  key not in Spoto
+0000cfd0: 626a 6563 742e 6b65 7973 2829 3a0d 0a20  bject.keys():.. 
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-0000d020: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000d030: 656c 6c5f 6964 5d20 3d20 7b0d 0a20 2020  ell_id] = {..   
-0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d050: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
-0000d060: 6c6c 6964 5f6b 6579 3a20 696e 7428 6365  llid_key: int(ce
-0000d070: 6c6c 5f69 6429 2c20 0d0a 2020 2020 2020  ll_id), ..      
+0000d010: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d040: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000d050: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000d060: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-0000d0a0: 6964 5f6b 6579 203a 2069 6e74 2866 6c6f  id_key : int(flo
-0000d0b0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000d0c0: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
-0000d0d0: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
+0000d090: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000d0a0: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
+0000d0b0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000d0c0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000d0d0: 6368 325f 6b65 7929 0d0a 2020 2020 2020  ch2_key)..      
 0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0f0: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
-0000d100: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000d110: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000d120: 7a70 6f73 6964 5f6b 6579 2929 2c0d 0a20  zposid_key)),.. 
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d150: 7970 6f73 6964 5f6b 6579 203a 2066 6c6f  yposid_key : flo
-0000d160: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000d170: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
-0000d180: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d100: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000d110: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
+0000d120: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000d130: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000d140: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+0000d180: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1a0: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
-0000d1b0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000d1c0: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
-0000d1d0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1f0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
-0000d200: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000d210: 7920 3a20 544f 5441 4c5f 494e 5445 4e53  y : TOTAL_INTENS
-0000d220: 4954 592c 0d0a 2020 2020 2020 2020 2020  ITY,..          
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
-0000d250: 6e73 6974 795f 6b65 7920 3a20 4d45 414e  nsity_key : MEAN
-0000d260: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000d1c0: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
+0000d1d0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000d1e0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000d1f0: 5f63 6831 5f6b 6579 290d 0a20 2020 2020  _ch1_key)..     
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d220: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000d230: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000d240: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000d250: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000d260: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
 0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d280: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000d290: 6469 7573 5f6b 6579 203a 2052 4144 4955  dius_key : RADIU
-0000d2a0: 532c 0d0a 2020 2020 2020 2020 2020 2020  S,..            
-0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000d2d0: 203a 2051 5541 4c49 5459 2c0d 0a20 2020   : QUALITY,..   
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+0000d2a0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000d2b0: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
+0000d2c0: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
-0000d300: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000d310: 5f6b 6579 3a20 666c 6f61 7428 6469 7374  _key: float(dist
-0000d320: 616e 6365 5f63 656c 6c5f 6d61 736b 292c  ance_cell_mask),
-0000d330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d340: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d350: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-0000d360: 7a5f 6b65 793a 2066 6c6f 6174 286d 6173  z_key: float(mas
-0000d370: 6b63 656e 7472 6f69 645b 305d 292c 0d0a  kcentroid[0]),..
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d3a0: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-0000d3b0: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-0000d3c0: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000d3f0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-0000d400: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
-0000d410: 7472 6f69 645b 325d 2920 0d0a 2020 2020  troid[2]) ..    
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 2020 2020 7d0d 0a20 2020 2020 2020 0d0a      }..       ..
-0000d440: 2020 2020 6465 6620 5f67 6574 5f6d 6173      def _get_mas
-0000d450: 7465 725f 786d 6c5f 6461 7461 2873 656c  ter_xml_data(sel
-0000d460: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-0000d470: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
-0000d480: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
-0000d490: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d4b0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000d4c0: 636f 6e74 656e 7420 3d20 7365 6c66 2e78  content = self.x
-0000d4d0: 6d6c 5f63 6f6e 7465 6e74 0d0a 2020 2020  ml_content..    
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2020 7365 6c66 2e78 6d6c 5f74 7265 6520    self.xml_tree 
-0000d500: 3d20 6574 2e70 6172 7365 2873 656c 662e  = et.parse(self.
-0000d510: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
-0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d530: 2073 656c 662e 786d 6c5f 726f 6f74 203d   self.xml_root =
-0000d540: 2073 656c 662e 786d 6c5f 7472 6565 2e67   self.xml_tree.g
-0000d550: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
+0000d2f0: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
+0000d300: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000d310: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
+0000d320: 795f 6b65 7929 2920 2020 2020 0d0a 2020  y_key))     ..  
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d350: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000d360: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000d370: 7428 544f 5441 4c5f 494e 5445 4e53 4954  t(TOTAL_INTENSIT
+0000d380: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
+0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000d3c0: 2066 6c6f 6174 284d 4541 4e5f 494e 5445   float(MEAN_INTE
+0000d3d0: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d400: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000d410: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000d420: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000d460: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+0000d470: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4a0: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000d4b0: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000d4c0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000d4d0: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000d4e0: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d510: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000d520: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000d530: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000d540: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
+0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000d580: 5f6e 616d 6520 3d20 2773 6563 6f6e 645f  _name = 'second_
-0000d590: 6368 616e 6e65 6c5f 2720 2b20 6f73 2e70  channel_' + os.p
-0000d5a0: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
-0000d5b0: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
-0000d5c0: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
-0000d5d0: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5f0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
-0000d600: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
-0000d610: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
-0000d620: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d640: 656c 662e 5f63 7265 6174 655f 6368 616e  elf._create_chan
-0000d650: 6e65 6c5f 7472 6565 2829 0d0a 0d0a 2020  nel_tree()....  
-0000d660: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000d670: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
-0000d680: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-0000d690: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
-0000d6a0: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-0000d6b0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000d6c0: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
-0000d6d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d6e0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000d6f0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000d700: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000d710: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000d720: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000d730: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
-0000d740: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
-0000d750: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
-0000d760: 5f70 6f69 6e74 735f 7469 6d65 7320 3d20  _points_times = 
-0000d770: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-0000d780: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d790: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d7a0: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
-0000d7b0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000d7c0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000d7d0: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000d7e0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000d7f0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-0000d800: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-0000d810: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
-0000d820: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d830: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-0000d840: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000d850: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000d860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d870: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000d880: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000d890: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000d8a0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000d8b0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000d8c0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000d8d0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000d8e0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0000d8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d900: 5370 6f74 6f62 6a65 6374 7320 3d20 7365  Spotobjects = se
-0000d910: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000d920: 696e 6428 274d 6f64 656c 2729 2e66 696e  ind('Model').fin
-0000d930: 6428 2741 6c6c 5370 6f74 7327 290d 0a20  d('AllSpots').. 
-0000d940: 2020 2020 2020 2020 2020 2023 2045 7874             # Ext
-0000d950: 7261 6374 2074 6865 2074 7261 636b 7320  ract the tracks 
-0000d960: 6672 6f6d 2078 6d6c 0d0a 2020 2020 2020  from xml..      
-0000d970: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-0000d980: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000d990: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
-0000d9a0: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
-0000d9b0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000d9c0: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
-0000d9d0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000d9e0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000d9f0: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
-0000da00: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
-0000da10: 2020 2073 656c 662e 7863 616c 6962 7261     self.xcalibra
-0000da20: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000da30: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000da40: 7069 7865 6c77 6964 7468 2229 290d 0a20  pixelwidth")).. 
-0000da50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000da60: 7963 616c 6962 7261 7469 6f6e 203d 2066  ycalibration = f
-0000da70: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000da80: 6773 2e67 6574 2822 7069 7865 6c68 6569  gs.get("pixelhei
-0000da90: 6768 7422 2929 0d0a 2020 2020 2020 2020  ght"))..        
-0000daa0: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
-0000dab0: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000dac0: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000dad0: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
-0000dae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000daf0: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
-0000db00: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
-0000db10: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
-0000db20: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
-0000db30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000db40: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
-0000db50: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000db60: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
-0000db70: 6773 2229 2e66 696e 6428 2244 6574 6563  gs").find("Detec
-0000db80: 746f 7253 6574 7469 6e67 7322 290d 0a20  torSettings").. 
-0000db90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000dba0: 6261 7369 6373 6574 7469 6e67 7320 3d20  basicsettings = 
-0000dbb0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000dbc0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
-0000dbd0: 292e 6669 6e64 2822 4261 7369 6353 6574  ).find("BasicSet
-0000dbe0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
-0000dbf0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000dc00: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
-0000dc10: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
-0000dc20: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
-0000dc30: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
-0000dc40: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000dc50: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
-0000dc60: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-0000dc70: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-0000dc80: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
-0000dc90: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-0000dca0: 6e64 203d 2069 6e74 2866 6c6f 6174 2873  nd = int(float(s
-0000dcb0: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
-0000dcc0: 732e 6765 7428 2274 656e 6422 2929 2920  s.get("tend"))) 
-0000dcd0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000dce0: 2020 2020 2070 7269 6e74 2827 4974 6572       print('Iter
-0000dcf0: 6174 696e 6720 6f76 6572 2073 706f 7473  ating over spots
-0000dd00: 2069 6e20 6672 616d 6527 290d 0a20 2020   in frame')..   
-0000dd10: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000dd20: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0000dd30: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
-0000dd40: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000dd50: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
-0000dd60: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
-0000dd70: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
-0000dd80: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
-0000dd90: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
-0000dda0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
-0000ddb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000ddc0: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
-0000ddd0: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
-0000dde0: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
-0000ddf0: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
-0000de00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000de10: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-0000de20: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-0000de30: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-0000de40: 662e 5f6d 6173 7465 725f 7370 6f74 5f63  f._master_spot_c
-0000de50: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
-0000de60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000de70: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-0000de80: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-0000de90: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000deb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000dee0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-0000def0: 2022 436f 6c6c 6563 7469 6e67 2053 706f   "Collecting Spo
-0000df00: 7473 220d 0a20 2020 2020 2020 2020 2020  ts"..           
-0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df20: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000df30: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000df40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d580: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+0000d590: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000d5a0: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000d5b0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000d5f0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000d600: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000d610: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000d650: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000d660: 6579 203a 2054 4f54 414c 5f49 4e54 454e  ey : TOTAL_INTEN
+0000d670: 5349 5459 2c0d 0a20 2020 2020 2020 2020  SITY,..         
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6a0: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+0000d6b0: 656e 7369 7479 5f6b 6579 203a 204d 4541  ensity_key : MEA
+0000d6c0: 4e5f 494e 5445 4e53 4954 592c 0d0a 2020  N_INTENSITY,..  
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000d700: 6164 6975 735f 6b65 7920 3a20 5241 4449  adius_key : RADI
+0000d710: 5553 2c0d 0a20 2020 2020 2020 2020 2020  US,..           
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2073 656c 662e 7175 616c 6974 795f 6b65   self.quality_ke
+0000d750: 7920 3a20 5155 414c 4954 590d 0a20 2020  y : QUALITY..   
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 207d 0d0a 2020 2020 2020 200d       }..       .
+0000d790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d7a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d7b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7d0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+0000d7e0: 5f73 706f 745f 636f 6d70 7574 6572 2873  _spot_computer(s
+0000d7f0: 656c 662c 2066 7261 6d65 293a 0d0a 0d0a  elf, frame):....
+0000d800: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+0000d810: 6f74 6f62 6a65 6374 2069 6e20 6672 616d  otobject in fram
+0000d820: 652e 6669 6e64 616c 6c28 2753 706f 7427  e.findall('Spot'
+0000d830: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000d840: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+0000d850: 6561 7465 206f 626a 6563 7420 7769 7468  eate object with
+0000d860: 2075 6e69 7175 6520 6365 6c6c 2049 440d   unique cell ID.
+0000d870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d880: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000d890: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000d8a0: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000d8b0: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8d0: 2023 2047 6574 2074 6865 2054 5a59 5820   # Get the TZYX 
+0000d8e0: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
+0000d8f0: 6365 6c6c 7320 696e 2074 6861 7420 6672  cells in that fr
+0000d900: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+0000d910: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d920: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000d930: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
+0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d950: 2020 2020 2020 2020 2020 2020 6966 2053              if S
+0000d960: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000d970: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000d980: 7479 5f63 6832 5f6b 6579 2920 6973 206e  ty_ch2_key) is n
+0000d990: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9c0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
+0000d9d0: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000d9e0: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
+0000d9f0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0000da00: 325f 6b65 7929 290d 0a20 2020 2020 2020  2_key))..       
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000da40: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000da50: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
+0000da60: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
+0000da70: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000da80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
+0000dad0: 4954 5920 3d20 2d31 0d0a 2020 2020 2020  ITY = -1..      
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db00: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000db10: 3d20 2d31 2020 2020 2020 200d 0a20 2020  = -1       ..   
+0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db30: 2020 2020 2065 6c73 653a 2020 2020 2020       else:      
+0000db40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db60: 2020 2020 6966 2053 706f 746f 626a 6563      if Spotobjec
+0000db70: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
+0000db80: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
+0000db90: 6579 2920 6973 206e 6f74 204e 6f6e 653a  ey) is not None:
+0000dba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbc0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000dbd0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000dbe0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000dbf0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
+0000dc00: 6e73 6974 795f 6368 315f 6b65 7929 290d  nsity_ch1_key)).
+0000dc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
+0000dc40: 5445 4e53 4954 5920 3d20 666c 6f61 7428  TENSITY = float(
+0000dc50: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000dc60: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000dc70: 7479 5f63 6831 5f6b 6579 2929 0d0a 2020  ty_ch1_key))..  
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000dca0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000dcd0: 414c 5f49 4e54 454e 5349 5459 203d 202d  AL_INTENSITY = -
+0000dce0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
+0000dd10: 494e 5445 4e53 4954 5920 3d20 2d31 2020  INTENSITY = -1  
+0000dd20: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd40: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd60: 2020 2020 2052 4144 4955 5320 3d20 666c       RADIUS = fl
+0000dd70: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000dd80: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000dd90: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 5155                QU
+0000ddb0: 414c 4954 5920 3d20 666c 6f61 7428 5370  ALITY = float(Sp
+0000ddc0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000ddd0: 662e 7175 616c 6974 795f 6b65 7929 290d  f.quality_key)).
+0000dde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ddf0: 2020 2020 2020 2020 2074 6573 746c 6f63           testloc
+0000de00: 6174 696f 6e20 3d20 2866 6c6f 6174 2853  ation = (float(S
+0000de10: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000de20: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000de30: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000de40: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000de50: 645f 6b65 7929 292c 2020 666c 6f61 7428  d_key)),  float(
+0000de60: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000de70: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
+0000de80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000de90: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+0000dea0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000deb0: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
+0000dec0: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
+0000ded0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+0000dee0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+0000def0: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
+0000df00: 7365 6c66 2e5f 6765 745f 626f 756e 6461  self._get_bounda
+0000df10: 7279 5f64 6973 7428 6672 616d 652c 2074  ry_dist(frame, t
+0000df20: 6573 746c 6f63 6174 696f 6e29 0d0a 2020  estlocation)..  
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df80: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000df90: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
-0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfb0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000df70: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000df80: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
+0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfa0: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+0000dfb0: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
+0000dfc0: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
 0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfe0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000dff0: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
-0000e000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e010: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
-0000e020: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
-0000e030: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e060: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000e070: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
-0000e080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0a0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000e0b0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000e0c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0f0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000e100: 722e 7661 6c75 6520 3d20 2073 656c 662e  r.value =  self.
-0000e110: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e130: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
-0000e140: 756c 7428 2920 2020 200d 0a0d 0a20 2020  ult()    ....   
-0000e150: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0000e160: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
-0000e170: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
-0000e180: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-0000e190: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
-0000e1a0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-0000e1b0: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
-0000e1c0: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
-0000e1d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e1e0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000e1f0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000e220: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
-0000e230: 6374 696e 6720 5472 6163 6b73 220d 0a20  cting Tracks".. 
-0000e240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e250: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000e260: 2e72 616e 6765 203d 2028 302c 206c 656e  .range = (0, len
-0000e270: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-0000e280: 7261 636b 5f69 6473 2929 0d0a 2020 2020  rack_ids))..    
-0000e290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e2a0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000e2b0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
-0000e2c0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
-0000e2d0: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
-0000e2e0: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
-0000e310: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
-0000e320: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
-0000e330: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e340: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
-0000e350: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-0000e360: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
-0000e370: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e380: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
-0000e390: 7075 7465 7228 7472 6163 6b2c 2074 7261  puter(track, tra
-0000e3a0: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-0000e3b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e3c0: 2e63 6f75 6e74 202b 3d20 310d 0a20 2020  .count += 1..   
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3e0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000e3f0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000e400: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000e410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e420: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-0000e430: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
-0000e440: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000e450: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-0000e460: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-0000e470: 6f6e 653a 2020 0d0a 2020 2020 2020 2020  one:  ..        
-0000e480: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000e490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e4a0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
-0000e4b0: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
-0000e4c0: 6e65 6c5f 786d 6c28 290d 0a20 2020 2020  nel_xml()..     
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4e0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000e4f0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-0000e500: 6e20 7365 6c66 2e67 7261 7068 5f73 706c  n self.graph_spl
-0000e510: 6974 2e69 7465 6d73 2829 3a0d 0a20 2020  it.items():..   
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e530: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
-0000e560: 7261 636b 5f69 6420 3d20 2069 6e74 2866  rack_id =  int(f
-0000e570: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-0000e580: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e590: 7469 6573 5b69 6e74 2866 6c6f 6174 286b  ties[int(float(k
-0000e5a0: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-0000e5b0: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5d0: 2020 2020 2020 2070 6172 656e 745f 7472         parent_tr
-0000e5e0: 6163 6b5f 6964 203d 2069 6e74 2866 6c6f  ack_id = int(flo
-0000e5f0: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
-0000e600: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000e610: 6573 5b69 6e74 2866 6c6f 6174 2876 2929  es[int(float(v))
-0000e620: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
-0000e630: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2073 656c 662e 6772 6170 685f       self.graph_
-0000e660: 7472 6163 6b73 5b64 6175 6768 7465 725f  tracks[daughter_
-0000e670: 7472 6163 6b5f 6964 5d20 3d20 7061 7265  track_id] = pare
-0000e680: 6e74 5f74 7261 636b 5f69 640d 0a0d 0a20  nt_track_id.... 
-0000e690: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000e6a0: 2827 6765 7474 696e 6720 6174 7472 6962  ('getting attrib
-0000e6b0: 7574 6573 2729 2020 2020 2020 2020 2020  utes')          
-0000e6c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e6d0: 2020 2020 7365 6c66 2e5f 6765 745f 6174      self._get_at
-0000e6e0: 7472 6962 7574 6573 2829 0d0a 2020 2020  tributes()..    
-0000e6f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e700: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-0000e710: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
-0000e720: 2066 6f72 2069 6e64 6578 2c20 7472 6163   for index, trac
-0000e730: 6b5f 6964 2069 6e20 656e 756d 6572 6174  k_id in enumerat
-0000e740: 6528 7365 6c66 2e66 696c 7465 7265 645f  e(self.filtered_
-0000e750: 7472 6163 6b5f 6964 7329 3a0d 0a20 2020  track_ids):..   
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000e790: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000e7a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e7d0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000e7e0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-0000e7f0: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
-0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000e830: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000e840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e870: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8a0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000e8b0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000e8c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e920: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000e930: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e960: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000e970: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000e9b0: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-0000e9c0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
-0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000e9f0: 636b 203d 2073 656c 662e 6669 6c74 6572  ck = self.filter
-0000ea00: 6564 5f74 7261 636b 735b 696e 6465 785d  ed_tracks[index]
-0000ea10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000ea40: 6669 6e61 6c5f 7472 6163 6b73 2874 7261  final_tracks(tra
-0000ea50: 636b 2c20 7472 6163 6b5f 6964 2920 0d0a  ck, track_id) ..
-0000ea60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000ea70: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea90: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
-0000eaa0: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
-0000ead0: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000eb00: 2020 7365 6c66 2e5f 7465 6d70 6f72 616c    self._temporal
-0000eb10: 5f70 6c6f 7473 5f74 7261 636b 6d61 7465  _plots_trackmate
-0000eb20: 2829 2020 2020 2020 2020 0d0a 0d0a 0d0a  ()        ......
-0000eb30: 2020 2020 6465 6620 5f63 7265 6174 655f      def _create_
-0000eb40: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
-0000eb50: 6d6c 2873 656c 6629 3a0d 0a20 2020 2020  ml(self):..     
-0000eb60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000eb70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000eb80: 7428 2754 7261 6e73 6665 7272 696e 6720  t('Transferring 
-0000eb90: 584d 4c27 2920 2020 0d0a 2020 2020 2020  XML')   ..      
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-0000ebb0: 616e 6e65 6c5f 6669 6c74 6572 6564 5f74  annel_filtered_t
-0000ebc0: 7261 636b 7320 3d20 5b5d 2020 2020 2020  racks = []      
-0000ebd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000ebe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ebf0: 5370 6f74 6f62 6a65 6374 2069 6e20 7365  Spotobject in se
-0000ec00: 6c66 2e78 6d6c 5f72 6f6f 742e 6974 6572  lf.xml_root.iter
-0000ec10: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
-0000ec40: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
-0000ec50: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-0000ec60: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec80: 2020 2069 6620 6365 6c6c 5f69 6420 696e     if cell_id in
-0000ec90: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000eca0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000ecb0: 7469 6573 2e6b 6579 7328 293a 2020 2020  ties.keys():    
-0000ecc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 2020 2020 2020 2020 6e65 775f 706f 7369          new_posi
-0000ed10: 7469 6f6e 7820 3d20 2073 656c 662e 6368  tionx =  self.ch
-0000ed20: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000ed30: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000ed40: 6c5f 6964 5d5b 7365 6c66 2e78 706f 7369  l_id][self.xposi
-0000ed50: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000ed80: 706f 7369 7469 6f6e 7920 3d20 2073 656c  positiony =  sel
-0000ed90: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000eda0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000edb0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e79  [cell_id][self.y
-0000edc0: 706f 7369 645f 6b65 795d 0d0a 2020 2020  posid_key]..    
-0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 6e65 775f 706f 7369 7469 6f6e 7a20 3d20  new_positionz = 
-0000ee00: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000ee10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000ee20: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000ee30: 6c66 2e7a 706f 7369 645f 6b65 795d 0d0a  lf.zposid_key]..
-0000ee40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee60: 2020 2020 2020 6e65 775f 746f 7461 6c5f        new_total_
-0000ee70: 696e 7465 6e73 6974 7920 3d20 7365 6c66  intensity = self
-0000ee80: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000ee90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000eea0: 6365 6c6c 5f69 645d 5b73 656c 662e 746f  cell_id][self.to
-0000eeb0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000eec0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eee0: 2020 2020 2020 2020 6e65 775f 6d65 616e          new_mean
-0000eef0: 5f69 6e74 656e 7369 7479 203d 2073 656c  _intensity = sel
-0000ef00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000ef10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000ef20: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e6d  [cell_id][self.m
-0000ef30: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
-0000ef40: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
-0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef60: 2020 2020 2020 2020 2020 6e65 775f 7261            new_ra
-0000ef70: 6469 7573 203d 2073 656c 662e 6368 616e  dius = self.chan
-0000ef80: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000ef90: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000efa0: 6964 5d5b 7365 6c66 2e72 6164 6975 735f  id][self.radius_
-0000efb0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 2020 2020 2020 2020 2020 6e65 775f 7175            new_qu
-0000efe0: 616c 6974 7920 3d20 7365 6c66 2e63 6861  ality = self.cha
-0000eff0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000f000: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000f010: 5f69 645d 5b73 656c 662e 7175 616c 6974  _id][self.qualit
-0000f020: 795f 6b65 795d 0d0a 2020 2020 2020 2020  y_key]..        
-0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f040: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000f050: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000f060: 736b 203d 2073 656c 662e 6368 616e 6e65  sk = self.channe
-0000f070: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000f080: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000f090: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
-0000f0a0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 0d0a  cell_mask_key]..
-0000f0b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0d0: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
-0000f0e0: 2e73 6574 2873 656c 662e 7870 6f73 6964  .set(self.xposid
-0000f0f0: 5f6b 6579 2c20 7374 7228 6e65 775f 706f  _key, str(new_po
-0000f100: 7369 7469 6f6e 7829 2920 2020 2020 0d0a  sitionx))     ..
-0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f130: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000f140: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
-0000f150: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
-0000f160: 7469 6f6e 7929 290d 0a20 2020 2020 2020  tiony))..       
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000f190: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000f1a0: 2e7a 706f 7369 645f 6b65 792c 2073 7472  .zposid_key, str
-0000f1b0: 286e 6577 5f70 6f73 6974 696f 6e7a 2929  (new_positionz))
-0000f1c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1e0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000f1f0: 6374 2e73 6574 2873 656c 662e 746f 7461  ct.set(self.tota
-0000f200: 6c5f 696e 7465 6e73 6974 795f 6b65 792c  l_intensity_key,
-0000f210: 2073 7472 286e 6577 5f74 6f74 616c 5f69   str(new_total_i
-0000f220: 6e74 656e 7369 7479 2929 2020 2020 200d  ntensity))     .
-0000f230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f250: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000f260: 7365 7428 7365 6c66 2e6d 6561 6e5f 696e  set(self.mean_in
-0000f270: 7465 6e73 6974 795f 6b65 792c 2073 7472  tensity_key, str
-0000f280: 286e 6577 5f6d 6561 6e5f 696e 7465 6e73  (new_mean_intens
-0000f290: 6974 7929 290d 0a20 2020 2020 2020 2020  ity))..         
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2b0: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
-0000f2c0: 626a 6563 742e 7365 7428 7365 6c66 2e72  bject.set(self.r
-0000f2d0: 6164 6975 735f 6b65 792c 2073 7472 286e  adius_key, str(n
-0000f2e0: 6577 5f72 6164 6975 7329 2920 2020 2020  ew_radius))     
-0000f2f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f310: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
-0000f320: 2e73 6574 2873 656c 662e 7175 616c 6974  .set(self.qualit
-0000f330: 795f 6b65 792c 2073 7472 286e 6577 5f71  y_key, str(new_q
-0000f340: 7561 6c69 7479 2929 0d0a 2020 2020 2020  uality))..      
-0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f360: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-0000f370: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
-0000f380: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
-0000f390: 6d61 736b 5f6b 6579 2c20 7374 7228 6e65  mask_key, str(ne
-0000f3a0: 775f 6469 7374 616e 6365 5f63 656c 6c5f  w_distance_cell_
-0000f3b0: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3d0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-0000f3e0: 6b5f 6964 203d 2073 656c 662e 6368 616e  k_id = self.chan
-0000f3f0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000f400: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-0000f410: 656c 6c5f 6964 295d 5b73 656c 662e 7472  ell_id)][self.tr
-0000f420: 6163 6b69 645f 6b65 795d 0d0a 2020 2020  ackid_key]..    
-0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f450: 6368 616e 6e65 6c5f 6669 6c74 6572 6564  channel_filtered
-0000f460: 5f74 7261 636b 732e 6170 7065 6e64 2874  _tracks.append(t
-0000f470: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f490: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4b0: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
-0000f4c0: 652e 7772 6974 6528 6f73 2e70 6174 682e  e.write(os.path.
-0000f4d0: 6a6f 696e 2873 656c 662e 6368 616e 6e65  join(self.channe
-0000f4e0: 6c5f 786d 6c5f 7061 7468 2c20 7365 6c66  l_xml_path, self
-0000f4f0: 2e63 6861 6e6e 656c 5f78 6d6c 5f6e 616d  .channel_xml_nam
-0000f500: 6529 2920 0d0a 0d0a 2020 2020 6465 6620  e)) ....    def 
-0000f510: 5f67 6574 5f78 6d6c 5f64 6174 6128 7365  _get_xml_data(se
-0000f520: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
-0000f530: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-0000f540: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000f550: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-0000f560: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-0000f570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000f580: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f590: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
-0000f5a0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
-0000f5b0: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
-0000f5c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f5d0: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
-0000f5e0: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
-0000f5f0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-0000f600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f610: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
-0000f620: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
-0000f630: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000f640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f650: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
-0000f660: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
-0000f670: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
-0000f680: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
-0000f690: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
-0000f6a0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
-0000f6b0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
-0000f6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f6d0: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
-0000f6e0: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
-0000f6f0: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
-0000f700: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000f710: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000f720: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
-0000f730: 7265 6528 290d 0a20 2020 2020 2020 2020  ree()..         
-0000f740: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000f750: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
-0000f760: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000f770: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
-0000f780: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000dfe0: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
+0000dff0: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
+0000e000: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000e010: 656c 662e 6672 616d 6569 645f 6b65 7929  elf.frameid_key)
+0000e020: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e040: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000e050: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000e060: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000e070: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e090: 2020 2020 2020 2020 7365 6c66 2e79 706f          self.ypo
+0000e0a0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000e0b0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000e0c0: 656c 662e 7970 6f73 6964 5f6b 6579 2929  elf.yposid_key))
+0000e0d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e0f0: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000e100: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000e110: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000e120: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e140: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+0000e150: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
+0000e160: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000e170: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000e180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e190: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000e1a0: 7479 5f6b 6579 203a 204d 4541 4e5f 494e  ty_key : MEAN_IN
+0000e1b0: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1d0: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
+0000e1e0: 735f 6b65 7920 3a20 5241 4449 5553 2c0d  s_key : RADIUS,.
+0000e1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e200: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e210: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000e220: 5155 414c 4954 592c 0d0a 2020 2020 2020  QUALITY,..      
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e240: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
+0000e250: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+0000e260: 793a 2066 6c6f 6174 2864 6973 7461 6e63  y: float(distanc
+0000e270: 655f 6365 6c6c 5f6d 6173 6b29 2c0d 0a20  e_cell_mask),.. 
+0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e2a0: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
+0000e2b0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000e2c0: 6e74 726f 6964 5b30 5d29 2c0d 0a20 2020  ntroid[0]),..   
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2e0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000e2f0: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
+0000e300: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000e310: 726f 6964 5b31 5d29 2c0d 0a20 2020 2020  roid[1]),..     
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+0000e340: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
+0000e350: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+0000e360: 6964 5b32 5d29 200d 0a20 2020 2020 2020  id[2]) ..       
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e380: 207d 0d0a 2020 2020 2020 200d 0a20 2020   }..       ..   
+0000e390: 2064 6566 205f 6765 745f 6d61 7374 6572   def _get_master
+0000e3a0: 5f78 6d6c 5f64 6174 6128 7365 6c66 293a  _xml_data(self):
+0000e3b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000e3c0: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000e3d0: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000e3e0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000e3f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e400: 2e63 6861 6e6e 656c 5f78 6d6c 5f63 6f6e  .channel_xml_con
+0000e410: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
+0000e420: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
+0000e430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e440: 656c 662e 786d 6c5f 7472 6565 203d 2065  elf.xml_tree = e
+0000e450: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000e460: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000e470: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e480: 6c66 2e78 6d6c 5f72 6f6f 7420 3d20 7365  lf.xml_root = se
+0000e490: 6c66 2e78 6d6c 5f74 7265 652e 6765 7472  lf.xml_tree.getr
+0000e4a0: 6f6f 7428 290d 0a20 2020 2020 2020 2020  oot()..         
+0000e4b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e4c0: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
+0000e4d0: 6d65 203d 2027 7365 636f 6e64 5f63 6861  me = 'second_cha
+0000e4e0: 6e6e 656c 5f27 202b 206f 732e 7061 7468  nnel_' + os.path
+0000e4f0: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
+0000e500: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
+0000e510: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
+0000e520: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
+0000e530: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e540: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000e550: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
+0000e560: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
+0000e570: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000e580: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e590: 2e5f 6372 6561 7465 5f63 6861 6e6e 656c  ._create_channel
+0000e5a0: 5f74 7265 6528 290d 0a0d 0a20 2020 2020  _tree()....     
+0000e5b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000e5c0: 7565 5f6f 626a 6563 7473 203d 207b 7d0d  ue_objects = {}.
+0000e5d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000e5e0: 662e 756e 6971 7565 5f70 726f 7065 7274  f.unique_propert
+0000e5f0: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+0000e600: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+0000e610: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000e620: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000e630: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
+0000e640: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000e650: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000e660: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000e670: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0000e680: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
+0000e690: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000e6a0: 2020 2073 656c 662e 7370 6c69 745f 706f     self.split_po
+0000e6b0: 696e 7473 5f74 696d 6573 203d 205b 5d0d  ints_times = [].
+0000e6c0: 0a0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
+0000e6d0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000e6e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e6f0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000e700: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000e710: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000e720: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000e730: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000e740: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000e750: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000e760: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000e770: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000e780: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000e790: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000e7a0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000e7b0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000e7c0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
+0000e7d0: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
+0000e7e0: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
+0000e7f0: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+0000e800: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
+0000e810: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
+0000e820: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000e830: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000e840: 2020 2020 2020 2020 7365 6c66 2e53 706f          self.Spo
+0000e850: 746f 626a 6563 7473 203d 2073 656c 662e  tobjects = self.
+0000e860: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000e870: 2827 4d6f 6465 6c27 292e 6669 6e64 2827  ('Model').find('
+0000e880: 416c 6c53 706f 7473 2729 0d0a 2020 2020  AllSpots')..    
+0000e890: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000e8a0: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
+0000e8b0: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
+0000e8c0: 2020 2073 656c 662e 7472 6163 6b73 203d     self.tracks =
+0000e8d0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000e8e0: 742e 6669 6e64 2822 4d6f 6465 6c22 292e  t.find("Model").
+0000e8f0: 6669 6e64 2822 416c 6c54 7261 636b 7322  find("AllTracks"
+0000e900: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000e910: 656c 662e 7365 7474 696e 6773 203d 2073  elf.settings = s
+0000e920: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000e930: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000e940: 2e66 696e 6428 2249 6d61 6765 4461 7461  .find("ImageData
+0000e950: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000e960: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000e970: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000e980: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000e990: 656c 7769 6474 6822 2929 0d0a 2020 2020  elwidth"))..    
+0000e9a0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
+0000e9b0: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000e9c0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000e9d0: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
+0000e9e0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000e9f0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+0000ea00: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
+0000ea10: 7365 7474 696e 6773 2e67 6574 2822 766f  settings.get("vo
+0000ea20: 7865 6c64 6570 7468 2229 290d 0a20 2020  xeldepth"))..   
+0000ea30: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0000ea40: 616c 6962 7261 7469 6f6e 203d 2069 6e74  alibration = int
+0000ea50: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
+0000ea60: 696e 6773 2e67 6574 2822 7469 6d65 696e  ings.get("timein
+0000ea70: 7465 7276 616c 2229 2929 0d0a 2020 2020  terval")))..    
+0000ea80: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000ea90: 6563 746f 7273 6574 7469 6e67 7320 3d20  ectorsettings = 
+0000eaa0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000eab0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000eac0: 292e 6669 6e64 2822 4465 7465 6374 6f72  ).find("Detector
+0000ead0: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
+0000eae0: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+0000eaf0: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
+0000eb00: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000eb10: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000eb20: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
+0000eb30: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
+0000eb40: 2020 7365 6c66 2e64 6574 6563 746f 7263    self.detectorc
+0000eb50: 6861 6e6e 656c 203d 2069 6e74 2866 6c6f  hannel = int(flo
+0000eb60: 6174 2873 656c 662e 6465 7465 6374 6f72  at(self.detector
+0000eb70: 7365 7474 696e 6773 2e67 6574 2822 5441  settings.get("TA
+0000eb80: 5247 4554 5f43 4841 4e4e 454c 2229 2929  RGET_CHANNEL")))
+0000eb90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000eba0: 6c66 2e74 7374 6172 7420 3d20 696e 7428  lf.tstart = int(
+0000ebb0: 666c 6f61 7428 7365 6c66 2e62 6173 6963  float(self.basic
+0000ebc0: 7365 7474 696e 6773 2e67 6574 2822 7473  settings.get("ts
+0000ebd0: 7461 7274 2229 2929 0d0a 2020 2020 2020  tart")))..      
+0000ebe0: 2020 2020 2020 7365 6c66 2e74 656e 6420        self.tend 
+0000ebf0: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000ec00: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
+0000ec10: 6574 2822 7465 6e64 2229 2929 2020 2020  et("tend")))    
+0000ec20: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000ec30: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
+0000ec40: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
+0000ec50: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
+0000ec60: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+0000ec70: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+0000ec80: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
+0000ec90: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0000eca0: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+0000ecb0: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+0000ecc0: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+0000ecd0: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+0000ece0: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+0000ecf0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+0000ed00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000ed10: 2020 2020 2020 2066 6f72 2066 7261 6d65         for frame
+0000ed20: 2069 6e20 7365 6c66 2e53 706f 746f 626a   in self.Spotobj
+0000ed30: 6563 7473 2e66 696e 6461 6c6c 2827 5370  ects.findall('Sp
+0000ed40: 6f74 7349 6e46 7261 6d65 2729 3a0d 0a20  otsInFrame'):.. 
+0000ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed60: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000ed70: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+0000ed80: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+0000ed90: 6d61 7374 6572 5f73 706f 745f 636f 6d70  master_spot_comp
+0000eda0: 7574 6572 2c20 6672 616d 6529 290d 0a20  uter, frame)).. 
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000edc0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000edd0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000ede0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee20: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000ee30: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000ee40: 6f6c 6c65 6374 696e 6720 5370 6f74 7322  ollecting Spots"
+0000ee50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee70: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000ee80: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eeb0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eed0: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+0000eee0: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
+0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef00: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000ef30: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000ef40: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+0000ef50: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
+0000ef60: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+0000ef70: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+0000ef80: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efb0: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
+0000efc0: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eff0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000f000: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000f010: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f030: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f040: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000f050: 616c 7565 203d 2020 7365 6c66 2e63 6f75  alue =  self.cou
+0000f060: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f080: 2020 2020 2020 2020 722e 7265 7375 6c74          r.result
+0000f090: 2829 2020 2020 0d0a 0d0a 2020 2020 2020  ()    ....      
+0000f0a0: 2020 2020 2020 7072 696e 7428 6627 4974        print(f'It
+0000f0b0: 6572 6174 696e 6720 6f76 6572 2074 7261  erating over tra
+0000f0c0: 636b 7320 7b6c 656e 2873 656c 662e 6669  cks {len(self.fi
+0000f0d0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000f0e0: 297d 2729 2020 0d0a 2020 2020 2020 2020  )}')  ..        
+0000f0f0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000f100: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+0000f110: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
+0000f120: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000f130: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000f140: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000f150: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f160: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+0000f170: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
+0000f180: 6e67 2054 7261 636b 7322 0d0a 2020 2020  ng Tracks"..    
+0000f190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f1a0: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+0000f1b0: 6e67 6520 3d20 2830 2c20 6c65 6e28 7365  nge = (0, len(se
+0000f1c0: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+0000f1d0: 6b5f 6964 7329 290d 0a20 2020 2020 2020  k_ids))..       
+0000f1e0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f1f0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000f200: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000f210: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
+0000f220: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
+0000f230: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
+0000f240: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000f250: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
+0000f260: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
+0000f270: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000f280: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+0000f290: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+0000f2a0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000f2b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f2c0: 2020 2020 2020 2073 656c 662e 5f6d 6173         self._mas
+0000f2d0: 7465 725f 7472 6163 6b5f 636f 6d70 7574  ter_track_comput
+0000f2e0: 6572 2874 7261 636b 2c20 7472 6163 6b5f  er(track, track_
+0000f2f0: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+0000f300: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000f310: 756e 7420 2b3d 2031 0d0a 2020 2020 2020  unt += 1..      
+0000f320: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f330: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000f340: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000f350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f360: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f370: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000f380: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+0000f390: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000f3a0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+0000f3b0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000f3c0: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+0000f3d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3f0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+0000f400: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
+0000f410: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f430: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000f440: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+0000f450: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
+0000f460: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4a0: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
+0000f4b0: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
+0000f4c0: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
+0000f4d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000f4e0: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
+0000f4f0: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000f500: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
+0000f530: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000f540: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+0000f550: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000f560: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
+0000f570: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000f580: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5a0: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
+0000f5b0: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
+0000f5c0: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
+0000f5d0: 7472 6163 6b5f 6964 0d0a 0d0a 2020 2020  track_id....    
+0000f5e0: 2020 2020 2020 2020 7072 696e 7428 2767          print('g
+0000f5f0: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+0000f600: 7327 2920 2020 2020 2020 2020 2020 2020  s')             
+0000f610: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f620: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
+0000f630: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
+0000f640: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f650: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000f660: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000f670: 7220 696e 6465 782c 2074 7261 636b 5f69  r index, track_i
+0000f680: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
+0000f690: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000f6a0: 636b 5f69 6473 293a 0d0a 2020 2020 2020  ck_ids):..      
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f6d0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000f6e0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000f6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f720: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+0000f730: 203d 2022 4a75 7374 206f 6e65 206d 6f72   = "Just one mor
+0000f740: 6520 7468 696e 6722 0d0a 2020 2020 2020  e thing"..      
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f770: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000f780: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
 0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
-0000f7b0: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
-0000f7c0: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
-0000f7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f7e0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000f7f0: 7465 725f 786d 6c5f 7472 6565 203d 2065  ter_xml_tree = e
-0000f800: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
-0000f810: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f830: 656c 662e 6d61 7374 6572 5f78 6d6c 5f72  elf.master_xml_r
-0000f840: 6f6f 7420 3d20 7365 6c66 2e6d 6173 7465  oot = self.maste
-0000f850: 725f 786d 6c5f 7472 6565 2e67 6574 726f  r_xml_tree.getro
-0000f860: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
-0000f870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f880: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
-0000f890: 6520 3d20 276d 6173 7465 725f 2720 2b20  e = 'master_' + 
-0000f8a0: 7365 6c66 2e6d 6173 7465 725f 6578 7472  self.master_extr
-0000f8b0: 615f 6e61 6d65 2020 2b20 6f73 2e70 6174  a_name  + os.pat
-0000f8c0: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
-0000f8d0: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
-0000f8e0: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
-0000f8f0: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-0000f920: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
-0000f930: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
-0000f940: 7061 7468 2920 2020 2020 200d 0a20 2020  path)      ..   
-0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f960: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000f970: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000f980: 655f 6f62 6a65 6374 7320 3d20 7b7d 0d0a  e_objects = {}..
-0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f9a0: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
-0000f9b0: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-0000f9c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f9d0: 662e 416c 6c54 7261 636b 4964 7320 3d20  f.AllTrackIds = 
-0000f9e0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000f9f0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000fa00: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
-0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa20: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000fa30: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000fa40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000fa50: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
-0000fa60: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
-0000fa70: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000fa80: 706c 6974 5f70 6f69 6e74 735f 7469 6d65  plit_points_time
-0000fa90: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-0000faa0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fab0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fad0: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
-0000fae0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000faf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fb00: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-0000fb10: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
-0000fb20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb30: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-0000fb40: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000fb50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fb60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000fb70: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
-0000fb80: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000fb90: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fbb0: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-0000fbc0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000fbd0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fbf0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000fc00: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000fc10: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000fc20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000fc30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000fc40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fc50: 656c 662e 5370 6f74 6f62 6a65 6374 7320  elf.Spotobjects 
-0000fc60: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000fc70: 6e74 2e66 696e 6428 274d 6f64 656c 2729  nt.find('Model')
-0000fc80: 2e66 696e 6428 2741 6c6c 5370 6f74 7327  .find('AllSpots'
-0000fc90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fca0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-0000fcb0: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
-0000fcc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fcd0: 2020 7365 6c66 2e74 7261 636b 7320 3d20    self.tracks = 
-0000fce0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000fcf0: 2e66 696e 6428 224d 6f64 656c 2229 2e66  .find("Model").f
-0000fd00: 696e 6428 2241 6c6c 5472 6163 6b73 2229  ind("AllTracks")
+0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+0000f7c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7f0: 2020 206c 656e 2873 656c 662e 6669 6c74     len(self.filt
+0000f800: 6572 6564 5f74 7261 636b 5f69 6473 292c  ered_track_ids),
+0000f810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f830: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0000f840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f860: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000f870: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000f880: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f8b0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+0000f8c0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8f0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000f900: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
+0000f910: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+0000f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f930: 2020 2020 2020 2020 2020 7472 6163 6b20            track 
+0000f940: 3d20 7365 6c66 2e66 696c 7465 7265 645f  = self.filtered_
+0000f950: 7472 6163 6b73 5b69 6e64 6578 5d20 2020  tracks[index]   
+0000f960: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f980: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
+0000f990: 616c 5f74 7261 636b 7328 7472 6163 6b5f  al_tracks(track_
+0000f9a0: 6964 2920 0d0a 0d0a 2020 2020 2020 2020  id) ....        
+0000f9b0: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
+0000f9c0: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
+0000f9d0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000f9e0: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
+0000f9f0: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
+0000fa00: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+0000fa10: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
+0000fa20: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
+0000fa30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000fa40: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0000fa50: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
+0000fa60: 636b 6d61 7465 2829 2020 2020 2020 2020  ckmate()        
+0000fa70: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f63  ......    def _c
+0000fa80: 7265 6174 655f 7365 636f 6e64 5f63 6861  reate_second_cha
+0000fa90: 6e6e 656c 5f78 6d6c 2873 656c 6629 3a0d  nnel_xml(self):.
+0000faa0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+0000fab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fac0: 2020 7072 696e 7428 2754 7261 6e73 6665    print('Transfe
+0000fad0: 7272 696e 6720 584d 4c27 2920 2020 0d0a  rring XML')   ..
+0000fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faf0: 2020 2020 6368 616e 6e65 6c5f 6669 6c74      channel_filt
+0000fb00: 6572 6564 5f74 7261 636b 7320 3d20 5b5d  ered_tracks = []
+0000fb10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
+0000fb40: 2069 6e20 7365 6c66 2e78 6d6c 5f72 6f6f   in self.xml_roo
+0000fb50: 742e 6974 6572 2827 5370 6f74 2729 3a0d  t.iter('Spot'):.
+0000fb60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb70: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000fb80: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+0000fb90: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000fba0: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+0000fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbc0: 2020 2020 2020 2020 2069 6620 6365 6c6c           if cell
+0000fbd0: 5f69 6420 696e 2073 656c 662e 6368 616e  _id in self.chan
+0000fbe0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000fbf0: 7072 6f70 6572 7469 6573 2e6b 6579 7328  properties.keys(
+0000fc00: 293a 2020 2020 2020 2020 0d0a 2020 2020  ):        ..    
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000fc50: 775f 706f 7369 7469 6f6e 7820 3d20 2073  w_positionx =  s
+0000fc60: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000fc70: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000fc80: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000fc90: 2e78 706f 7369 645f 6b65 795d 0d0a 2020  .xposid_key]..  
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcc0: 2020 6e65 775f 706f 7369 7469 6f6e 7920    new_positiony 
+0000fcd0: 3d20 2073 656c 662e 6368 616e 6e65 6c5f  =  self.channel_
+0000fce0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000fcf0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000fd00: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
 0000fd10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fd20: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
-0000fd30: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000fd40: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000fd50: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
-0000fd60: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
-0000fd70: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
-0000fd80: 6573 697a 6520 3d20 2869 6e74 2866 6c6f  esize = (int(flo
-0000fd90: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000fda0: 2e67 6574 2822 6e66 7261 6d65 7322 2929  .get("nframes"))
-0000fdb0: 292c 696e 7428 666c 6f61 7428 7365 6c66  ),int(float(self
-0000fdc0: 2e73 6574 7469 6e67 732e 6765 7428 226e  .settings.get("n
-0000fdd0: 736c 6963 6573 2229 2929 2c69 6e74 2866  slices"))),int(f
-0000fde0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000fdf0: 6773 2e67 6574 2822 6865 6967 6874 2229  gs.get("height")
-0000fe00: 2929 2c20 2069 6e74 2866 6c6f 6174 2873  )),  int(float(s
-0000fe10: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000fe20: 2822 7769 6474 6822 2929 2929 0d0a 2020  ("width"))))..  
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000fe40: 696e 7428 6627 584d 4c20 6669 6c65 206d  int(f'XML file m
-0000fe50: 6164 6520 7573 696e 6720 696d 6167 6520  ade using image 
-0000fe60: 6f66 207b 7365 6c66 2e69 6d61 6765 7369  of {self.imagesi
-0000fe70: 7a65 7d27 290d 0a20 2020 2020 2020 2020  ze}')..         
-0000fe80: 2020 2020 2020 2073 656c 662e 7863 616c         self.xcal
-0000fe90: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
-0000fea0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000feb0: 6574 2822 7069 7865 6c77 6964 7468 2229  et("pixelwidth")
-0000fec0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fed0: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
-0000fee0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000fef0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000ff00: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 2020 2020 2020 6e65 775f 706f 7369 7469        new_positi
+0000fd40: 6f6e 7a20 3d20 2073 656c 662e 6368 616e  onz =  self.chan
+0000fd50: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000fd60: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000fd70: 6964 5d5b 7365 6c66 2e7a 706f 7369 645f  id][self.zposid_
+0000fd80: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fda0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000fdb0: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
+0000fdc0: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
+0000fdd0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000fde0: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000fdf0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000fe00: 6974 795f 6b65 795d 0d0a 2020 2020 2020  ity_key]..      
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000fe30: 775f 6d65 616e 5f69 6e74 656e 7369 7479  w_mean_intensity
+0000fe40: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000fe50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000fe60: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000fe70: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000fe80: 6974 795f 6b65 795d 0d0a 0d0a 2020 2020  ity_key]....    
+0000fe90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000feb0: 6e65 775f 7261 6469 7573 203d 2073 656c  new_radius = sel
+0000fec0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000fed0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000fee0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e72  [cell_id][self.r
+0000fef0: 6164 6975 735f 6b65 795d 0d0a 2020 2020  adius_key]..    
+0000ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff20: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-0000ff30: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
-0000ff40: 6574 7469 6e67 732e 6765 7428 2276 6f78  ettings.get("vox
-0000ff50: 656c 6465 7074 6822 2929 0d0a 2020 2020  eldepth"))..    
-0000ff60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ff70: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
-0000ff80: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
-0000ff90: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
-0000ffa0: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ffc0: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
-0000ffd0: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-0000ffe0: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-0000fff0: 7474 696e 6773 2229 2e66 696e 6428 2244  ttings").find("D
-00010000: 6574 6563 746f 7253 6574 7469 6e67 7322  etectorSettings"
-00010010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010020: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
-00010030: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-00010040: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-00010050: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-00010060: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
-00010070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010080: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
-00010090: 616e 6e65 6c20 3d20 696e 7428 666c 6f61  annel = int(floa
-000100a0: 7428 7365 6c66 2e64 6574 6563 746f 7273  t(self.detectors
-000100b0: 6574 7469 6e67 732e 6765 7428 2254 4152  ettings.get("TAR
-000100c0: 4745 545f 4348 414e 4e45 4c22 2929 290d  GET_CHANNEL"))).
-000100d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100e0: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
-000100f0: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-00010100: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-00010110: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
-00010120: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010130: 662e 7465 6e64 203d 2069 6e74 2866 6c6f  f.tend = int(flo
-00010140: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-00010150: 7469 6e67 732e 6765 7428 2274 656e 6422  tings.get("tend"
-00010160: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-00010170: 2020 2020 2073 656c 662e 5f67 6574 5f62       self._get_b
-00010180: 6f75 6e64 6172 795f 706f 696e 7473 2829  oundary_points()
-00010190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000101a0: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
-000101b0: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
-000101c0: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
-000101d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000101e0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
-000101f0: 2020 2020 2020 2020 2020 6675 7475 7265            future
-00010200: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-00010210: 2020 2020 2020 2020 2020 7769 7468 2063            with c
-00010220: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-00010230: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
-00010240: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
-00010250: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
-00010260: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
-00010270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010280: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00010290: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
-000102a0: 7261 6d65 2069 6e20 7365 6c66 2e53 706f  rame in self.Spo
-000102b0: 746f 626a 6563 7473 2e66 696e 6461 6c6c  tobjects.findall
-000102c0: 2827 5370 6f74 7349 6e46 7261 6d65 2729  ('SpotsInFrame')
-000102d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
-00010300: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
-00010310: 656c 662e 5f73 706f 745f 636f 6d70 7574  elf._spot_comput
-00010320: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
-00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010340: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-00010350: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00010360: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000103b0: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-000103c0: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
-000103d0: 2053 706f 7473 220d 0a20 2020 2020 2020   Spots"..       
-000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010400: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-00010410: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010440: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-00010450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010460: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00010470: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
-00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-000104d0: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-000104e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000104f0: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
-00010500: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-00010510: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
-00010520: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 6e65 775f 7175 616c 6974 7920 3d20 7365  new_quality = se
+0000ff30: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000ff40: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000ff50: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000ff60: 7175 616c 6974 795f 6b65 795d 0d0a 2020  quality_key]..  
+0000ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2020 6e65 775f 6469 7374 616e 6365 5f63    new_distance_c
+0000ffa0: 656c 6c5f 6d61 736b 203d 2073 656c 662e  ell_mask = self.
+0000ffb0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+0000ffc0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000ffd0: 656c 6c5f 6964 5d5b 7365 6c66 2e64 6973  ell_id][self.dis
+0000ffe0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+0000fff0: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
+00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010010: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+00010020: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+00010030: 7870 6f73 6964 5f6b 6579 2c20 7374 7228  xposid_key, str(
+00010040: 6e65 775f 706f 7369 7469 6f6e 7829 2920  new_positionx)) 
+00010050: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
+00010080: 6a65 6374 2e73 6574 2873 656c 662e 7970  ject.set(self.yp
+00010090: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
+000100a0: 775f 706f 7369 7469 6f6e 7929 290d 0a20  w_positiony)).. 
+000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+000100e0: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
+000100f0: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
+00010100: 696f 6e7a 2929 0d0a 0d0a 2020 2020 2020  ionz))....      
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+00010130: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
+00010140: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+00010150: 795f 6b65 792c 2073 7472 286e 6577 5f74  y_key, str(new_t
+00010160: 6f74 616c 5f69 6e74 656e 7369 7479 2929  otal_intensity))
+00010170: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010190: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+000101a0: 626a 6563 742e 7365 7428 7365 6c66 2e6d  bject.set(self.m
+000101b0: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+000101c0: 792c 2073 7472 286e 6577 5f6d 6561 6e5f  y, str(new_mean_
+000101d0: 696e 7465 6e73 6974 7929 290d 0a20 2020  intensity))..   
+000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
+00010210: 7365 6c66 2e72 6164 6975 735f 6b65 792c  self.radius_key,
+00010220: 2073 7472 286e 6577 5f72 6164 6975 7329   str(new_radius)
+00010230: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+00010260: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+00010270: 7175 616c 6974 795f 6b65 792c 2073 7472  quality_key, str
+00010280: 286e 6577 5f71 7561 6c69 7479 2929 0d0a  (new_quality))..
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102b0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+000102c0: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
+000102d0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2c20  _cell_mask_key, 
+000102e0: 7374 7228 6e65 775f 6469 7374 616e 6365  str(new_distance
+000102f0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 7472 6163 6b5f 6964 203d 2073 656c    track_id = sel
+00010330: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00010340: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00010350: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00010360: 656c 662e 7472 6163 6b69 645f 6b65 795d  elf.trackid_key]
+00010370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010390: 2020 2020 2020 6368 616e 6e65 6c5f 6669        channel_fi
+000103a0: 6c74 6572 6564 5f74 7261 636b 732e 6170  ltered_tracks.ap
+000103b0: 7065 6e64 2874 7261 636b 5f69 6429 0d0a  pend(track_id)..
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000103f0: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+00010400: 6d6c 5f74 7265 652e 7772 6974 6528 6f73  ml_tree.write(os
+00010410: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00010420: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
+00010430: 2c20 7365 6c66 2e63 6861 6e6e 656c 5f78  , self.channel_x
+00010440: 6d6c 5f6e 616d 6529 2920 0d0a 0d0a 2020  ml_name)) ....  
+00010450: 2020 6465 6620 5f67 6574 5f78 6d6c 5f64    def _get_xml_d
+00010460: 6174 6128 7365 6c66 293a 0d0a 0d0a 2020  ata(self):....  
+00010470: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00010480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010490: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+000104a0: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+000104b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104d0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
+000104e0: 5f63 6f6e 7465 6e74 203d 2073 656c 662e  _content = self.
+000104f0: 786d 6c5f 636f 6e74 656e 740d 0a20 2020  xml_content..   
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 2020 2073 656c 662e 786d 6c5f 7472 6565     self.xml_tree
+00010520: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
+00010530: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
 00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010550: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-00010560: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
-00010570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010550: 2020 7365 6c66 2e78 6d6c 5f72 6f6f 7420    self.xml_root 
+00010560: 3d20 7365 6c66 2e78 6d6c 5f74 7265 652e  = self.xml_tree.
+00010570: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
 00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010590: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000105a0: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-000105b0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000105f0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-00010600: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
-00010640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010650: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
-00010660: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
-00010670: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
-00010680: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
-00010690: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-000106a0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-000106b0: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-000106c0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-000106d0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-000106e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000106f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010700: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-00010710: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
-00010720: 2054 7261 636b 7322 0d0a 2020 2020 2020   Tracks"..      
-00010730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010740: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-00010750: 7261 6e67 6520 3d20 2830 2c20 6c65 6e28  range = (0, len(
-00010760: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-00010770: 6163 6b5f 6964 7329 290d 0a20 2020 2020  ack_ids))..     
-00010780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010790: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000107a0: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
-000107b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000107c0: 2020 2020 2020 2020 2020 2020 206d 6178               max
-000107d0: 5f6c 656e 6774 6820 3d20 3020 2020 200d  _length = 0    .
-000107e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000107f0: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
-00010800: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
-00010810: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 2074 7261 636b 5f69 6420 3d20 696e 7428   track_id = int(
-00010840: 7472 6163 6b2e 6765 7428 7365 6c66 2e74  track.get(self.t
-00010850: 7261 636b 6964 5f6b 6579 2929 0d0a 2020  rackid_key))..  
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
-00010880: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-00010890: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
-000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108b0: 2020 2020 2020 2064 6967 6974 5f6c 656e         digit_len
-000108c0: 6774 6820 3d20 6c65 6e28 7374 7228 7472  gth = len(str(tr
-000108d0: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
-000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108f0: 2020 2020 2020 6966 2064 6967 6974 5f6c        if digit_l
-00010900: 656e 6774 6820 3e20 6d61 785f 6c65 6e67  ength > max_leng
-00010910: 7468 3a0d 0a20 2020 2020 2020 2020 2020  th:..           
-00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010930: 2020 2020 206d 6178 5f6c 656e 6774 6820       max_length 
-00010940: 3d20 6469 6769 745f 6c65 6e67 7468 0d0a  = digit_length..
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 7365 6c66 2e6d 6178 5f74 7261 636b 5f64  self.max_track_d
-00010970: 6967 6974 203d 206d 6178 5f6c 656e 6774  igit = max_lengt
-00010980: 6820 2020 2020 2020 2020 2020 2020 2020  h               
-00010990: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000109a0: 2020 2066 6f72 2074 7261 636b 2069 6e20     for track in 
-000109b0: 7365 6c66 2e74 7261 636b 732e 6669 6e64  self.tracks.find
-000109c0: 616c 6c28 2754 7261 636b 2729 3a0d 0a20  all('Track'):.. 
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
-000109f0: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
-00010a00: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a20: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
-00010a30: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-00010a40: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a60: 2020 2020 2073 656c 662e 5f74 7261 636b       self._track
-00010a70: 5f63 6f6d 7075 7465 7228 7472 6163 6b2c  _computer(track,
-00010a80: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
-00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010aa0: 2020 2020 7365 6c66 2e63 6f75 6e74 202b      self.count +
-00010ab0: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-00010ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010ad0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010ae0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010b10: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
-00010b20: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
-00010b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010b40: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
-00010b50: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
-00010b60: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
-00010b90: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
-00010ba0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
-00010bb0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00010bc0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-00010bd0: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
-00010be0: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
-00010bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010c00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
-00010c30: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
-00010c40: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-00010c50: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00010c60: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-00010c70: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
-00010c80: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
-00010cb0: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
-00010cc0: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
-00010cd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00010ce0: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
-00010cf0: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
-00010d00: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00010d30: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
-00010d40: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
-00010d50: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-00010d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010d70: 2020 7365 6c66 2e5f 6765 745f 6174 7472    self._get_attr
-00010d80: 6962 7574 6573 2829 0d0a 2020 2020 2020  ibutes()..      
-00010d90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010da0: 662e 6175 746f 656e 636f 6465 725f 6d6f  f.autoencoder_mo
-00010db0: 6465 6c20 616e 6420 7365 6c66 2e73 6567  del and self.seg
-00010dc0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-00010dd0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00010de0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010df0: 7428 2747 6574 7469 6e67 2061 7574 6f65  t('Getting autoe
-00010e00: 6e63 6f64 6572 2063 6c6f 7564 7327 290d  ncoder clouds').
-00010e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010e20: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-00010e30: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
-00010e40: 7373 2829 0d0a 2020 2020 2020 2020 2020  ss()..          
-00010e50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00010e60: 6e74 2827 4372 6561 7469 6e67 206d 6173  nt('Creating mas
-00010e70: 7465 7220 786d 6c27 290d 0a20 2020 2020  ter xml')..     
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2020 7365 6c66 2e5f 6372 6561 7465 5f6d    self._create_m
-00010ea0: 6173 7465 725f 786d 6c28 290d 0a20 2020  aster_xml()..   
-00010eb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010ec0: 662e 636f 756e 7420 3d20 3020 0d0a 2020  f.count = 0 ..  
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010ee0: 7220 696e 6465 782c 2074 7261 636b 5f69  r index, track_i
-00010ef0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
-00010f00: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-00010f10: 636b 5f69 6473 293a 0d0a 2020 2020 2020  ck_ids):..      
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010f40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00010f50: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-00010f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010f90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-00010fa0: 203d 2022 4a75 7374 206f 6e65 206d 6f72   = "Just one mor
-00010fb0: 6520 7468 696e 6722 0d0a 2020 2020 2020  e thing"..      
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010ff0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
-00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00011030: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2020 206c 656e 2873 656c 662e 6669 6c74     len(self.filt
-00011070: 6572 6564 5f74 7261 636b 5f69 6473 292c  ered_track_ids),
-00011080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-000110b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110d0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000110e0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
-000110f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011120: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-00011130: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010590: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+000105a0: 6c5f 6e61 6d65 203d 2027 7365 636f 6e64  l_name = 'second
+000105b0: 5f63 6861 6e6e 656c 5f27 202b 206f 732e  _channel_' + os.
+000105c0: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
+000105d0: 2e70 6174 682e 6261 7365 6e61 6d65 2873  .path.basename(s
+000105e0: 656c 662e 786d 6c5f 7061 7468 2929 5b30  elf.xml_path))[0
+000105f0: 5d20 2b20 272e 786d 6c27 0d0a 2020 2020  ] + '.xml'..    
+00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010610: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+00010620: 6d6c 5f70 6174 6820 3d20 6f73 2e70 6174  ml_path = os.pat
+00010630: 682e 6469 726e 616d 6528 7365 6c66 2e78  h.dirname(self.x
+00010640: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
+00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010660: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
+00010670: 6e6e 656c 5f74 7265 6528 290d 0a20 2020  nnel_tree()..   
+00010680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010690: 7365 6c66 2e61 7574 6f65 6e63 6f64 6572  self.autoencoder
+000106a0: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
+000106b0: 6e65 2061 6e64 2073 656c 662e 7365 675f  ne and self.seg_
+000106c0: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+000106d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000106e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000106f0: 6d61 7374 6572 5f78 6d6c 5f63 6f6e 7465  master_xml_conte
+00010700: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+00010710: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+00010720: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010730: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
+00010740: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
+00010750: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+00010780: 5f78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  _xml_root = self
+00010790: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
+000107a0: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107c0: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+000107d0: 6d6c 5f6e 616d 6520 3d20 276d 6173 7465  ml_name = 'maste
+000107e0: 725f 2720 2b20 7365 6c66 2e6d 6173 7465  r_' + self.maste
+000107f0: 725f 6578 7472 615f 6e61 6d65 2020 2b20  r_extra_name  + 
+00010800: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+00010810: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+00010820: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+00010830: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
+00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010850: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+00010860: 725f 786d 6c5f 7061 7468 203d 206f 732e  r_xml_path = os.
+00010870: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
+00010880: 662e 786d 6c5f 7061 7468 2920 2020 2020  f.xml_path)     
+00010890: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000108a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000108b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000108c0: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
+000108d0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+000108e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000108f0: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
+00010900: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00010910: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+00010920: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+00010930: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+00010940: 6976 6964 696e 6754 7261 636b 4964 7320  ividingTrackIds 
+00010950: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00010960: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+00010970: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
+00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010990: 7365 6c66 2e61 6c6c 5f74 7261 636b 5f70  self.all_track_p
+000109a0: 726f 7065 7274 6965 7320 3d20 5b5d 0d0a  roperties = []..
+000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109c0: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
+000109d0: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010a00: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00010a10: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00010a20: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
+00010a30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010a40: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
+00010a50: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+00010a60: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
+00010a70: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+00010a80: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
+00010a90: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+00010aa0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010ac0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+00010ad0: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+00010ae0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+00010af0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+00010b00: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+00010b10: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+00010b20: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+00010b30: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+00010b40: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
+00010b50: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
+00010b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00010b80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010b90: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
+00010ba0: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
+00010bb0: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
+00010bc0: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
+00010bd0: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
+00010be0: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
+00010bf0: 6374 2074 6865 2074 7261 636b 7320 6672  ct the tracks fr
+00010c00: 6f6d 2078 6d6c 0d0a 2020 2020 2020 2020  om xml..        
+00010c10: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00010c20: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
+00010c30: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
+00010c40: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
+00010c50: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
+00010c60: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00010c70: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+00010c80: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+00010c90: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+00010ca0: 496d 6167 6544 6174 6122 290d 0a20 2020  ImageData")..   
+00010cb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010cc0: 662e 696d 6167 6573 697a 6520 3d20 2869  f.imagesize = (i
+00010cd0: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
+00010ce0: 7474 696e 6773 2e67 6574 2822 6e66 7261  ttings.get("nfra
+00010cf0: 6d65 7322 2929 292c 696e 7428 666c 6f61  mes"))),int(floa
+00010d00: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+00010d10: 6765 7428 226e 736c 6963 6573 2229 2929  get("nslices")))
+00010d20: 2c69 6e74 2866 6c6f 6174 2873 656c 662e  ,int(float(self.
+00010d30: 7365 7474 696e 6773 2e67 6574 2822 6865  settings.get("he
+00010d40: 6967 6874 2229 2929 2c20 2069 6e74 2866  ight"))),  int(f
+00010d50: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+00010d60: 6773 2e67 6574 2822 7769 6474 6822 2929  gs.get("width"))
+00010d70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00010d80: 2020 2020 7072 696e 7428 6627 584d 4c20      print(f'XML 
+00010d90: 6669 6c65 206d 6164 6520 7573 696e 6720  file made using 
+00010da0: 696d 6167 6520 6f66 207b 7365 6c66 2e69  image of {self.i
+00010db0: 6d61 6765 7369 7a65 7d27 290d 0a20 2020  magesize}')..   
+00010dc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010dd0: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
+00010de0: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+00010df0: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
+00010e00: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
+00010e10: 2020 2020 2020 2020 2073 656c 662e 7963           self.yc
+00010e20: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+00010e30: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+00010e40: 2e67 6574 2822 7069 7865 6c68 6569 6768  .get("pixelheigh
+00010e50: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
+00010e60: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
+00010e70: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+00010e80: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+00010e90: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
+00010ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010eb0: 2020 7365 6c66 2e74 6361 6c69 6272 6174    self.tcalibrat
+00010ec0: 696f 6e20 3d20 696e 7428 666c 6f61 7428  ion = int(float(
+00010ed0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+00010ee0: 7428 2274 696d 6569 6e74 6572 7661 6c22  t("timeinterval"
+00010ef0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+00010f00: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+00010f10: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
+00010f20: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+00010f30: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+00010f40: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
+00010f50: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+00010f60: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+00010f70: 7369 6373 6574 7469 6e67 7320 3d20 7365  sicsettings = se
+00010f80: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+00010f90: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+00010fa0: 6669 6e64 2822 4261 7369 6353 6574 7469  find("BasicSetti
+00010fb0: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
+00010fc0: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+00010fd0: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
+00010fe0: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
+00010ff0: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
+00011000: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
+00011010: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
+00011020: 2020 2020 2020 2073 656c 662e 7473 7461         self.tsta
+00011030: 7274 203d 2069 6e74 2866 6c6f 6174 2873  rt = int(float(s
+00011040: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
+00011050: 732e 6765 7428 2274 7374 6172 7422 2929  s.get("tstart"))
+00011060: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011070: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
+00011080: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+00011090: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+000110a0: 2274 656e 6422 2929 290d 0a20 2020 2020  "tend")))..     
+000110b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000110c0: 5f67 6574 5f62 6f75 6e64 6172 795f 706f  _get_boundary_po
+000110d0: 696e 7473 2829 0d0a 2020 2020 2020 2020  ints()..        
+000110e0: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
+000110f0: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
+00011100: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
+00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011120: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011140: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
 00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011170: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
-00011180: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 2020 2020 2020 7472 6163 6b20            track 
-000111b0: 3d20 7365 6c66 2e66 696c 7465 7265 645f  = self.filtered_
-000111c0: 7472 6163 6b73 5b69 6e64 6578 5d20 2020  tracks[index]   
-000111d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
-00011200: 616c 5f74 7261 636b 7328 7472 6163 6b2c  al_tracks(track,
-00011210: 2074 7261 636b 5f69 6429 200d 0a0d 0a20   track_id) .... 
-00011220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011230: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
-00011240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011250: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
-00011260: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
-00011290: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000112c0: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
-000112d0: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
-000112e0: 6b6d 6174 6528 290d 0a20 2020 2020 2020  kmate()..       
-000112f0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00011300: 2064 6566 205f 6372 6561 7465 5f6d 6173   def _create_mas
-00011310: 7465 725f 786d 6c28 7365 6c66 293a 0d0a  ter_xml(self):..
-00011320: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00011330: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011340: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
-00011350: 2069 6e20 7365 6c66 2e6d 6173 7465 725f   in self.master_
-00011360: 786d 6c5f 726f 6f74 2e69 7465 7228 2753  xml_root.iter('S
-00011370: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
-00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011390: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
-000113a0: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
-000113b0: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
-000113c0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+00011160: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
+00011170: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
+00011180: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
+00011190: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
+000111a0: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
+000111b0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
+000111c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111e0: 2066 6f72 2066 7261 6d65 2069 6e20 7365   for frame in se
+000111f0: 6c66 2e53 706f 746f 626a 6563 7473 2e66  lf.Spotobjects.f
+00011200: 696e 6461 6c6c 2827 5370 6f74 7349 6e46  indall('SpotsInF
+00011210: 7261 6d65 2729 3a0d 0a20 2020 2020 2020  rame'):..       
+00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011230: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+00011240: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+00011250: 626d 6974 2873 656c 662e 5f73 706f 745f  bmit(self._spot_
+00011260: 636f 6d70 7574 6572 2c20 6672 616d 6529  computer, frame)
+00011270: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011280: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00011290: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+000112a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00011300: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+00011310: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
+00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+00011350: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011380: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 6c65 6e28 6675 7475 7265 7329      len(futures)
+000113c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113e0: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
-000113f0: 6964 2069 6e20 7365 6c66 2e75 6e69 7175  id in self.uniqu
-00011400: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00011410: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011440: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00011470: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-00011480: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00011490: 6365 6c6c 5f69 645d 2e6b 6579 7328 293a  cell_id].keys():
-000114a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-000114d0: 706f 746f 626a 6563 742e 7365 7428 6b2c  potobject.set(k,
-000114e0: 2073 7472 2873 656c 662e 756e 6971 7565   str(self.unique
-000114f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011500: 5b63 656c 6c5f 6964 5d5b 6b5d 2929 2020  [cell_id][k]))  
-00011510: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00011540: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00011550: 6173 7465 725f 786d 6c5f 7472 6565 2e77  aster_xml_tree.w
-00011560: 7269 7465 286f 732e 7061 7468 2e6a 6f69  rite(os.path.joi
-00011570: 6e28 7365 6c66 2e6d 6173 7465 725f 786d  n(self.master_xm
-00011580: 6c5f 7061 7468 2c20 7365 6c66 2e6d 6173  l_path, self.mas
-00011590: 7465 725f 786d 6c5f 6e61 6d65 2929 0d0a  ter_xml_name))..
-000115a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00011600: 0a20 2020 2064 6566 205f 6173 7369 676e  .    def _assign
-00011610: 5f63 6c75 7374 6572 5f63 6c61 7373 2873  _cluster_class(s
-00011620: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-00011630: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011640: 2020 2020 2020 2020 7365 6c66 2e61 7865          self.axe
-00011650: 7320 3d20 7365 6c66 2e61 7865 732e 7265  s = self.axes.re
-00011660: 706c 6163 6528 2254 222c 2022 2229 0d0a  place("T", "")..
+000113e0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011410: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00011420: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
+00011430: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011440: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
+00011450: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
+00011460: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
+00011470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000114a0: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
+000114b0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000114e0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+000114f0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+00011500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011530: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+00011540: 616c 7565 203d 2020 7365 6c66 2e63 6f75  alue =  self.cou
+00011550: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
+00011580: 7375 6c74 2829 0d0a 2020 2020 2020 2020  sult()..        
+00011590: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+000115a0: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
+000115b0: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
+000115c0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+000115d0: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
+000115e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000115f0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+00011600: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00011610: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+00011620: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011640: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00011650: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+00011660: 6563 7469 6e67 2054 7261 636b 7322 0d0a  ecting Tracks"..
 00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011680: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011690: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000116a0: 756e 742c 2074 696d 655f 6b65 7920 696e  unt, time_key in
-000116b0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
-000116c0: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
-000116d0: 6b65 7973 2829 293a 0d0a 2020 2020 2020  keys()):..      
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011710: 2020 7472 6565 2c20 7370 6f74 5f63 656e    tree, spot_cen
-00011720: 7472 6f69 6473 203d 2073 656c 662e 5f74  troids = self._t
-00011730: 696d 6564 5f63 656e 7472 6f69 645b 7469  imed_centroid[ti
-00011740: 6d65 5f6b 6579 5d0d 0a20 2020 2020 2020  me_key]..       
-00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011760: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-00011770: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-00011780: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117a0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000117b0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-000117c0: 2022 4175 746f 656e 636f 6465 7220 666f   "Autoencoder fo
-000117d0: 7220 7265 6669 6e69 6e67 2070 6f69 6e74  r refining point
-000117e0: 2063 6c6f 7564 7322 0d0a 2020 2020 2020   clouds"..      
-000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011800: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00011810: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-00011820: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
-00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-000118b0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-000118c0: 6f69 642e 6b65 7973 2829 2920 2b20 312c  oid.keys()) + 1,
-000118d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011900: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00011910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011930: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00011940: 6172 2e76 616c 7565 203d 2020 636f 756e  ar.value =  coun
-00011950: 7420 0d0a 2020 2020 2020 2020 2020 2020  t ..            
-00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011970: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00011980: 735f 6261 722e 7368 6f77 2829 0d0a 0d0a  s_bar.show()....
-00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
-000119b0: 6572 5f65 7661 6c20 3d20 436c 7573 7465  er_eval = Cluste
-000119c0: 7269 6e67 2873 656c 662e 6163 6365 6c65  ring(self.accele
-000119d0: 7261 746f 722c 2073 656c 662e 6465 7669  rator, self.devi
-000119e0: 6365 732c 2073 656c 662e 7365 675f 696d  ces, self.seg_im
-000119f0: 6167 655b 696e 7428 7469 6d65 5f6b 6579  age[int(time_key
-00011a00: 292c 3a5d 2c20 2073 656c 662e 6178 6573  ),:],  self.axes
-00011a10: 2c20 7365 6c66 2e6e 756d 5f70 6f69 6e74  , self.num_point
-00011a20: 732c 2073 656c 662e 6175 746f 656e 636f  s, self.autoenco
-00011a30: 6465 725f 6d6f 6465 6c2c 206b 6579 203d  der_model, key =
-00011a40: 2074 696d 655f 6b65 792c 2070 726f 6772   time_key, progr
-00011a50: 6573 735f 6261 723d 7365 6c66 2e70 726f  ess_bar=self.pro
-00011a60: 6772 6573 735f 6261 722c 2062 6174 6368  gress_bar, batch
-00011a70: 5f73 697a 6520 3d20 7365 6c66 2e62 6174  _size = self.bat
-00011a80: 6368 5f73 697a 652c 2073 6361 6c65 5f7a  ch_size, scale_z
-00011a90: 3d73 656c 662e 7363 616c 655f 7a2c 2073  =self.scale_z, s
-00011aa0: 6361 6c65 5f78 793d 2073 656c 662e 7363  cale_xy= self.sc
-00011ab0: 616c 655f 7879 2c20 6365 6e74 6572 203d  ale_xy, center =
-00011ac0: 2073 656c 662e 6365 6e74 6572 2920 2020   self.center)   
-00011ad0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2063 6c75 7374 6572 5f65 7661 6c2e 5f63   cluster_eval._c
-00011b00: 7265 6174 655f 636c 7573 7465 725f 6c61  reate_cluster_la
-00011b10: 6265 6c73 2829 0d0a 2020 2020 2020 2020  bels()..        
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b30: 2020 2074 696d 6564 5f63 6c75 7374 6572     timed_cluster
-00011b40: 5f6c 6162 656c 203d 2063 6c75 7374 6572  _label = cluster
-00011b50: 5f65 7661 6c2e 7469 6d65 645f 636c 7573  _eval.timed_clus
-00011b60: 7465 725f 6c61 6265 6c20 0d0a 2020 2020  ter_label ..    
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2020 2020 2020 206f 7574 7075 745f 6c61         output_la
-00011b90: 6265 6c73 2c20 206f 7574 7075 745f 636c  bels,  output_cl
-00011ba0: 7573 7465 725f 6365 6e74 726f 6964 2c20  uster_centroid, 
-00011bb0: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
-00011bc0: 656e 7472 6963 6974 792c 206f 7574 7075  entricity, outpu
-00011bd0: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
-00011be0: 6563 746f 722c 206f 7574 7075 745f 6c61  ector, output_la
-00011bf0: 7267 6573 745f 6569 6765 6e76 616c 7565  rgest_eigenvalue
-00011c00: 2c20 6f75 7470 7574 5f64 696d 656e 7369  , output_dimensi
-00011c10: 6f6e 732c 206f 7574 7075 745f 636c 6f75  ons, output_clou
-00011c20: 645f 7375 7266 6163 655f 6172 6561 203d  d_surface_area =
-00011c30: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
-00011c40: 6162 656c 5b74 696d 655f 6b65 795d 0d0a  abel[time_key]..
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00011c70: 5f31 203d 2031 0d0a 2020 2020 2020 2020  _1 = 1..        
-00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c90: 2020 2073 6361 6c65 5f32 203d 2031 0d0a     scale_2 = 1..
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00011cc0: 2069 6e20 7261 6e67 6528 6c65 6e28 6f75   in range(len(ou
-00011cd0: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
-00011ce0: 7472 6f69 6429 293a 0d0a 2020 2020 2020  troid)):..      
-00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d00: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00011d10: 6e74 726f 6964 203d 206f 7574 7075 745f  ntroid = output_
-00011d20: 636c 7573 7465 725f 6365 6e74 726f 6964  cluster_centroid
-00011d30: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d50: 2020 2020 2020 2020 2071 7561 6c69 7479           quality
-00011d60: 203d 206f 7574 7075 745f 6c61 7267 6573   = output_larges
-00011d70: 745f 6569 6765 6e76 616c 7565 5b69 5d0d  t_eigenvalue[i].
-00011d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011680: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00011690: 735f 6261 722e 7261 6e67 6520 3d20 2830  s_bar.range = (0
+000116a0: 2c20 6c65 6e28 7365 6c66 2e66 696c 7465  , len(self.filte
+000116b0: 7265 645f 7472 6163 6b5f 6964 7329 290d  red_track_ids)).
+000116c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000116d0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+000116e0: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+000116f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011700: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011710: 2020 206d 6178 5f6c 656e 6774 6820 3d20     max_length = 
+00011720: 3020 2020 200d 0a20 2020 2020 2020 2020  0    ..         
+00011730: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
+00011740: 2069 6e20 7365 6c66 2e74 7261 636b 732e   in self.tracks.
+00011750: 6669 6e64 616c 6c28 2754 7261 636b 2729  findall('Track')
+00011760: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00011770: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+00011780: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
+00011790: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+000117a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000117b0: 2020 2020 2020 2020 6966 2074 7261 636b          if track
+000117c0: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
+000117d0: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
+000117e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117f0: 2020 2020 2020 2020 2020 2020 2064 6967               dig
+00011800: 6974 5f6c 656e 6774 6820 3d20 6c65 6e28  it_length = len(
+00011810: 7374 7228 7472 6163 6b5f 6964 2929 0d0a  str(track_id))..
+00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011830: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00011840: 6967 6974 5f6c 656e 6774 6820 3e20 6d61  igit_length > ma
+00011850: 785f 6c65 6e67 7468 3a0d 0a20 2020 2020  x_length:..     
+00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011870: 2020 2020 2020 2020 2020 206d 6178 5f6c             max_l
+00011880: 656e 6774 6820 3d20 6469 6769 745f 6c65  ength = digit_le
+00011890: 6e67 7468 0d0a 2020 2020 2020 2020 2020  ngth..          
+000118a0: 2020 2020 2020 7365 6c66 2e6d 6178 5f74        self.max_t
+000118b0: 7261 636b 5f64 6967 6974 203d 206d 6178  rack_digit = max
+000118c0: 5f6c 656e 6774 6820 2020 2020 2020 2020  _length         
+000118d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000118e0: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+000118f0: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+00011900: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+00011910: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00011920: 2020 2020 2020 2020 2074 7261 636b 5f69           track_i
+00011930: 6420 3d20 696e 7428 7472 6163 6b2e 6765  d = int(track.ge
+00011940: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
+00011950: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+00011960: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+00011970: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+00011980: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00011990: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000119a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000119b0: 5f74 7261 636b 5f63 6f6d 7075 7465 7228  _track_computer(
+000119c0: 7472 6163 6b2c 2074 7261 636b 5f69 6429  track, track_id)
+000119d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000119e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000119f0: 6f75 6e74 202b 3d20 310d 0a20 2020 2020  ount += 1..     
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+00011a20: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+00011a30: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00011a60: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
+00011a70: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+00011a80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011a90: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00011aa0: 6520 6973 206e 6f74 204e 6f6e 653a 2020  e is not None:  
+00011ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011ac0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00011ad0: 7265 6174 655f 7365 636f 6e64 5f63 6861  reate_second_cha
+00011ae0: 6e6e 656c 5f78 6d6c 2829 0d0a 2020 2020  nnel_xml()..    
+00011af0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b10: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
+00011b20: 662e 6772 6170 685f 7370 6c69 742e 6974  f.graph_split.it
+00011b30: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b70: 2064 6175 6768 7465 725f 7472 6163 6b5f   daughter_track_
+00011b80: 6964 203d 2020 696e 7428 666c 6f61 7428  id =  int(float(
+00011b90: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+00011ba0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011bb0: 696e 7428 666c 6f61 7428 6b29 295d 5b73  int(float(k))][s
+00011bc0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+00011bd0: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bf0: 2020 7061 7265 6e74 5f74 7261 636b 5f69    parent_track_i
+00011c00: 6420 3d20 696e 7428 666c 6f61 7428 7374  d = int(float(st
+00011c10: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
+00011c20: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011c30: 7428 666c 6f61 7428 7629 295d 5b73 656c  t(float(v))][sel
+00011c40: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
+00011c50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 7365 6c66 2e67 7261 7068 5f74 7261 636b  self.graph_track
+00011c80: 735b 6461 7567 6874 6572 5f74 7261 636b  s[daughter_track
+00011c90: 5f69 645d 203d 2070 6172 656e 745f 7472  _id] = parent_tr
+00011ca0: 6163 6b5f 6964 0d0a 2020 2020 2020 2020  ack_id..        
+00011cb0: 2020 2020 2020 2020 7365 6c66 2e5f 6765          self._ge
+00011cc0: 745f 6174 7472 6962 7574 6573 2829 0d0a  t_attributes()..
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ce0: 6966 2073 656c 662e 6175 746f 656e 636f  if self.autoenco
+00011cf0: 6465 725f 6d6f 6465 6c20 616e 6420 7365  der_model and se
+00011d00: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
+00011d10: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 7072 696e 7428 2747 6574 7469 6e67    print('Getting
+00011d40: 2061 7574 6f65 6e63 6f64 6572 2063 6c6f   autoencoder clo
+00011d50: 7564 7327 290d 0a20 2020 2020 2020 2020  uds')..         
+00011d60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011d70: 6c66 2e5f 6173 7369 676e 5f63 6c75 7374  lf._assign_clust
+00011d80: 6572 5f63 6c61 7373 2829 0d0a 2020 2020  er_class()..    
 00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
-00011db0: 795f 636f 6d70 5f66 6972 7374 797a 203d  y_comp_firstyz =
-00011dc0: 206f 7574 7075 745f 636c 6f75 645f 6563   output_cloud_ec
-00011dd0: 6365 6e74 7269 6369 7479 5b69 5d0d 0a20  centricity[i].. 
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e00: 2020 2065 7373 656e 7472 6963 6974 795f     essentricity_
-00011e10: 6469 6d65 6e73 696f 6e20 3d20 6f75 7470  dimension = outp
-00011e20: 7574 5f64 696d 656e 7369 6f6e 735b 695d  ut_dimensions[i]
-00011e30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
-00011e60: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00011e70: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ea0: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
-00011eb0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00011ec0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011ef0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00011f00: 6d65 6e73 696f 6e5b 315d 203d 3d20 313a  mension[1] == 1:
-00011f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f40: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
-00011f50: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
-00011f60: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
-00011f90: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00011fa0: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
-00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
-00011fe0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00011ff0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00011da0: 2020 2070 7269 6e74 2827 4372 6561 7469     print('Creati
+00011db0: 6e67 206d 6173 7465 7220 786d 6c27 290d  ng master xml').
+00011dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011dd0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+00011de0: 6561 7465 5f6d 6173 7465 725f 786d 6c28  eate_master_xml(
+00011df0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011e00: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+00011e10: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
+00011e20: 2020 2020 666f 7220 696e 6465 782c 2074      for index, t
+00011e30: 7261 636b 5f69 6420 696e 2065 6e75 6d65  rack_id in enume
+00011e40: 7261 7465 2873 656c 662e 6669 6c74 6572  rate(self.filter
+00011e50: 6564 5f74 7261 636b 5f69 6473 293a 0d0a  ed_track_ids):..
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e80: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+00011e90: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+00011ea0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011ed0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00011ee0: 2e6c 6162 656c 203d 2022 4a75 7374 206f  .label = "Just o
+00011ef0: 6e65 206d 6f72 6520 7468 696e 6722 0d0a  ne more thing"..
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f20: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00011f30: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+00011f40: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f70: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
+00011fb0: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+00011fc0: 5f69 6473 292c 0d0a 2020 2020 2020 2020  _ids),..        
+00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ff0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
 00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012020: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00012030: 6d65 6e73 696f 6e5b 315d 203d 3d20 303a  mension[1] == 0:
-00012040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012020: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00012030: 2e73 686f 7728 290d 0a20 2020 2020 2020  .show()..       
+00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012070: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
-00012080: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-00012090: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-000120c0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-000120d0: 696f 6e5b 305d 203d 3d20 313a 0d0a 2020  ion[0] == 1:..  
+00012060: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
+00012070: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
+00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120a0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+000120b0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
+000120c0: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
+000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00012110: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
-00012120: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012150: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00012160: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00012170: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000120f0: 7472 6163 6b20 3d20 7365 6c66 2e66 696c  track = self.fil
+00012100: 7465 7265 645f 7472 6163 6b73 5b69 6e64  tered_tracks[ind
+00012110: 6578 5d20 2020 200d 0a20 2020 2020 2020  ex]    ..       
+00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012140: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
+00012150: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
+00012160: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012170: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
 00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121a0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-000121b0: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-000121c0: 6f6e 2020 0d0a 0d0a 2020 2020 2020 2020  on  ....        
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-000121f0: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
-00012200: 6e73 696f 6e5b 305d 203d 3d20 313a 0d0a  nsion[0] == 1:..
-00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00012240: 5f31 203d 2073 656c 662e 7963 616c 6962  _1 = self.ycalib
-00012250: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012280: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
-00012290: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
-000122a0: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
-000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
+000121a0: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
+000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121c0: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
+000121d0: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012200: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
+00012210: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
+00012220: 6d61 7465 2829 0d0a 2020 2020 2020 2020  mate()..        
+00012230: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00012240: 6465 6620 5f63 7265 6174 655f 6d61 7374  def _create_mast
+00012250: 6572 5f78 6d6c 2873 656c 6629 3a0d 0a20  er_xml(self):.. 
+00012260: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00012270: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012280: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
+00012290: 696e 2073 656c 662e 6d61 7374 6572 5f78  in self.master_x
+000122a0: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
+000122b0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
 000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122d0: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
-000122e0: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
-000122f0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00012300: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+000122d0: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
+000122e0: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
+000122f0: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
+00012300: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
 00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012320: 2020 2020 2020 2020 2020 2069 6620 6573             if es
-00012330: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
-00012340: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
-00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012320: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
+00012330: 6420 696e 2073 656c 662e 756e 6971 7565  d in self.unique
+00012340: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00012350: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
 00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012370: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00012380: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
-00012390: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123c0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-000123d0: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
-000123e0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012380: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+000123b0: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
+000123c0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+000123d0: 656c 6c5f 6964 5d2e 6b65 7973 2829 3a0d  ell_id].keys():.
+000123e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012410: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
-00012420: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
-00012430: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2020 2020 2020 2020 2020 2069 6620 6573             if es
-00012460: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
-00012470: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
-00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-000124b0: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
-000124c0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00012500: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
-00012510: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
+00012400: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+00012410: 6f74 6f62 6a65 6374 2e73 6574 286b 2c20  otobject.set(k, 
+00012420: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+00012430: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00012440: 6365 6c6c 5f69 645d 5b6b 5d29 2920 2020  cell_id][k]))   
+00012450: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012470: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00012480: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+00012490: 7374 6572 5f78 6d6c 5f74 7265 652e 7772  ster_xml_tree.wr
+000124a0: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
+000124b0: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
+000124c0: 5f70 6174 682c 2073 656c 662e 6d61 7374  _path, self.mast
+000124d0: 6572 5f78 6d6c 5f6e 616d 6529 290d 0a20  er_xml_name)).. 
+000124e0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012510: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
-00012550: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
-00012560: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00012540: 2020 2020 6465 6620 5f61 7373 6967 6e5f      def _assign_
+00012550: 636c 7573 7465 725f 636c 6173 7328 7365  cluster_class(se
+00012560: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
+00012570: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012580: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
+00012590: 203d 2073 656c 662e 6178 6573 2e72 6570   = self.axes.rep
+000125a0: 6c61 6365 2822 5422 2c20 2222 290d 0a20  lace("T", "").. 
 000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125c0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00012620: 6c6c 5f61 7869 7320 3d20 6f75 7470 7574  ll_axis = output
-00012630: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
-00012640: 6374 6f72 5b69 5d0d 0a20 2020 2020 2020  ctor[i]..       
-00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012660: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-00012670: 6661 6365 5f61 7265 6120 3d20 6f75 7470  face_area = outp
-00012680: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
-00012690: 5f61 7265 615b 695d 202a 2073 656c 662e  _area[i] * self.
-000126a0: 7a63 616c 6962 7261 7469 6f6e 202a 2073  zcalibration * s
-000126b0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-000126c0: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
-000126d0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126f0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
-00012700: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
-00012710: 7279 2863 656e 7472 6f69 6429 0d0a 2020  ry(centroid)..  
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000125d0: 2020 2020 2020 2020 2066 6f72 2063 6f75           for cou
+000125e0: 6e74 2c20 7469 6d65 5f6b 6579 2069 6e20  nt, time_key in 
+000125f0: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
+00012600: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
+00012610: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
+00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012630: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012650: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
+00012660: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
+00012670: 6d65 645f 6365 6e74 726f 6964 5b74 696d  med_centroid[tim
+00012680: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
+00012690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126a0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+000126b0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+000126c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+000126f0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
+00012700: 2241 7574 6f65 6e63 6f64 6572 2066 6f72  "Autoencoder for
+00012710: 2072 6566 696e 696e 6720 706f 696e 7420   refining point 
+00012720: 636c 6f75 6473 220d 0a20 2020 2020 2020  clouds"..       
 00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2020 7261 6469 7573 203d 2071 7561 6c69    radius = quali
-00012750: 7479 202a 206d 6174 682e 706f 7728 7365  ty * math.pow(se
-00012760: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
-00012770: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-00012780: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
-00012790: 6272 6174 696f 6e2c 2031 2e30 2f33 2e30  bration, 1.0/3.0
-000127a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012740: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00012750: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
+00012760: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00012770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127a0: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
 000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127c0: 2020 2020 2020 2069 6620 6469 7374 203c         if dist <
-000127d0: 2071 7561 6c69 7479 3a0d 0a20 2020 2020   quality:..     
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012800: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
-00012810: 656e 7472 6f69 6420 3d20 7370 6f74 5f63  entroid = spot_c
-00012820: 656e 7472 6f69 6473 5b69 6e64 6578 5d0d  entroids[index].
-00012830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-00012860: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
-00012870: 203d 2028 696e 7428 7469 6d65 5f6b 6579   = (int(time_key
-00012880: 292c 636c 6f73 6573 745f 6365 6e74 726f  ),closest_centro
-00012890: 6964 5b30 5d2c 2063 6c6f 7365 7374 5f63  id[0], closest_c
-000128a0: 656e 7472 6f69 645b 315d 2c20 636c 6f73  entroid[1], clos
-000128b0: 6573 745f 6365 6e74 726f 6964 5b32 5d29  est_centroid[2])
-000128c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127e0: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
+000127f0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
+00012800: 6964 2e6b 6579 7328 2929 202b 2031 2c0d  id.keys()) + 1,.
+00012810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012840: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00012880: 722e 7661 6c75 6520 3d20 2063 6f75 6e74  r.value =  count
+00012890: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000128a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128b0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+000128c0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
 000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-000128f0: 6f73 6573 745f 6365 6c6c 5f69 6420 3d20  osest_cell_id = 
-00012900: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012910: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
-00012920: 7370 6f74 5f63 656e 7472 6f69 645d 0d0a  spot_centroid]..
-00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012950: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
-00012960: 5f76 6563 746f 7220 3d20 5b20 666c 6f61  _vector = [ floa
-00012970: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00012980: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00012990: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-000129a0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
-000129b0: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
-000129c0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000129d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000129e0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-000129f0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-00012a00: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
-00012a10: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
-00012a20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012a30: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012a40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00012a50: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
-00012a60: 795d 2920 5d0d 0a20 2020 2020 2020 2020  y]) ]..         
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00012aa0: 6b20 3d20 616e 6775 6c61 725f 6368 616e  k = angular_chan
-00012ab0: 6765 2863 656c 6c5f 6178 6973 2c20 6d61  ge(cell_axis, ma
-00012ac0: 736b 5f76 6563 746f 7229 0d0a 2020 2020  sk_vector)..    
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012b30: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012b40: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012b50: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00012b60: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-00012b70: 736b 5f6b 6579 203a 2063 656c 6c5f 6178  sk_key : cell_ax
-00012b80: 6973 5f6d 6173 6b7d 290d 0a20 2020 2020  is_mask})..     
+000128e0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
+000128f0: 725f 6576 616c 203d 2043 6c75 7374 6572  r_eval = Cluster
+00012900: 696e 6728 7365 6c66 2e61 6363 656c 6572  ing(self.acceler
+00012910: 6174 6f72 2c20 7365 6c66 2e64 6576 6963  ator, self.devic
+00012920: 6573 2c20 7365 6c66 2e73 6567 5f69 6d61  es, self.seg_ima
+00012930: 6765 5b69 6e74 2874 696d 655f 6b65 7929  ge[int(time_key)
+00012940: 2c3a 5d2c 2020 7365 6c66 2e61 7865 732c  ,:],  self.axes,
+00012950: 2073 656c 662e 6e75 6d5f 706f 696e 7473   self.num_points
+00012960: 2c20 7365 6c66 2e61 7574 6f65 6e63 6f64  , self.autoencod
+00012970: 6572 5f6d 6f64 656c 2c20 6b65 7920 3d20  er_model, key = 
+00012980: 7469 6d65 5f6b 6579 2c20 7072 6f67 7265  time_key, progre
+00012990: 7373 5f62 6172 3d73 656c 662e 7072 6f67  ss_bar=self.prog
+000129a0: 7265 7373 5f62 6172 2c20 6261 7463 685f  ress_bar, batch_
+000129b0: 7369 7a65 203d 2073 656c 662e 6261 7463  size = self.batc
+000129c0: 685f 7369 7a65 2c20 7363 616c 655f 7a3d  h_size, scale_z=
+000129d0: 7365 6c66 2e73 6361 6c65 5f7a 2c20 7363  self.scale_z, sc
+000129e0: 616c 655f 7879 3d20 7365 6c66 2e73 6361  ale_xy= self.sca
+000129f0: 6c65 5f78 792c 2063 656e 7465 7220 3d20  le_xy, center = 
+00012a00: 7365 6c66 2e63 656e 7465 7229 2020 2020  self.center)    
+00012a10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a30: 636c 7573 7465 725f 6576 616c 2e5f 6372  cluster_eval._cr
+00012a40: 6561 7465 5f63 6c75 7374 6572 5f6c 6162  eate_cluster_lab
+00012a50: 656c 7328 290d 0a20 2020 2020 2020 2020  els()..         
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a70: 2020 7469 6d65 645f 636c 7573 7465 725f    timed_cluster_
+00012a80: 6c61 6265 6c20 3d20 636c 7573 7465 725f  label = cluster_
+00012a90: 6576 616c 2e74 696d 6564 5f63 6c75 7374  eval.timed_clust
+00012aa0: 6572 5f6c 6162 656c 200d 0a20 2020 2020  er_label ..     
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 2020 2020 2020 6f75 7470 7574 5f6c 6162        output_lab
+00012ad0: 656c 732c 2020 6f75 7470 7574 5f63 6c75  els,  output_clu
+00012ae0: 7374 6572 5f63 656e 7472 6f69 642c 206f  ster_centroid, o
+00012af0: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
+00012b00: 6e74 7269 6369 7479 2c20 6f75 7470 7574  ntricity, output
+00012b10: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
+00012b20: 6374 6f72 2c20 6f75 7470 7574 5f6c 6172  ctor, output_lar
+00012b30: 6765 7374 5f65 6967 656e 7661 6c75 652c  gest_eigenvalue,
+00012b40: 206f 7574 7075 745f 6469 6d65 6e73 696f   output_dimensio
+00012b50: 6e73 2c20 6f75 7470 7574 5f63 6c6f 7564  ns, output_cloud
+00012b60: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
+00012b70: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
+00012b80: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
 00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2020 2020 2069 6620 7365 6c66 2e75         if self.u
-00012bc0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00012bd0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00012be0: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
-00012bf0: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
-00012c00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c30: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012c40: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012c50: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012c60: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012c70: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-00012c80: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-00012c90: 203a 2065 6363 656e 7472 6963 6974 795f   : eccentricity_
-00012ca0: 636f 6d70 5f66 6972 7374 797a 5b30 5d20  comp_firstyz[0] 
-00012cb0: 2a20 7363 616c 655f 317d 290d 0a20 2020  * scale_1})..   
+00012ba0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00012bb0: 3120 3d20 310d 0a20 2020 2020 2020 2020  1 = 1..         
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 7363 616c 655f 3220 3d20 310d 0a20    scale_2 = 1.. 
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+00012c00: 696e 2072 616e 6765 286c 656e 286f 7574  in range(len(out
+00012c10: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
+00012c20: 726f 6964 2929 3a0d 0a20 2020 2020 2020  roid)):..       
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 2020 2020 2020 2020 2020 2020 2063 656e               cen
+00012c50: 7472 6f69 6420 3d20 6f75 7470 7574 5f63  troid = output_c
+00012c60: 6c75 7374 6572 5f63 656e 7472 6f69 645b  luster_centroid[
+00012c70: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 2020 2020 2020 7175 616c 6974 7920          quality 
+00012ca0: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
+00012cb0: 5f65 6967 656e 7661 6c75 655b 695d 0d0a  _eigenvalue[i]..
 00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00012d00: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012d10: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00012d20: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00012d30: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00012d40: 705f 7365 636f 6e64 6b65 7920 3a20 6563  p_secondkey : ec
-00012d50: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00012d60: 6669 7273 7479 7a5b 315d 202a 2073 6361  firstyz[1] * sca
-00012d70: 6c65 5f32 7d29 0d0a 2020 2020 2020 2020  le_2})..        
+00012ce0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+00012cf0: 5f63 6f6d 705f 6669 7273 7479 7a20 3d20  _comp_firstyz = 
+00012d00: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
+00012d10: 656e 7472 6963 6974 795b 695d 0d0a 2020  entricity[i]..  
+00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 6573 7365 6e74 7269 6369 7479 5f64    essentricity_d
+00012d50: 696d 656e 7369 6f6e 203d 206f 7574 7075  imension = outpu
+00012d60: 745f 6469 6d65 6e73 696f 6e73 5b69 5d20  t_dimensions[i] 
+00012d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012db0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00012dc0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00012dd0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-00012de0: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
-00012df0: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
-00012e00: 7266 6163 655f 6172 6561 7d29 0d0a 2020  rface_area})..  
+00012d90: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00012da0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00012db0: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012de0: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
+00012df0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00012e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e40: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00012e50: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00012e60: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00012e70: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00012e80: 2e71 7561 6c69 7479 5f6b 6579 203a 2071  .quality_key : q
-00012e90: 7561 6c69 7479 7d29 0d0a 2020 2020 2020  uality})..      
-00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00012e30: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00012e40: 656e 7369 6f6e 5b31 5d20 3d3d 2031 3a0d  ension[1] == 1:.
+00012e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e80: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
+00012e90: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
+00012ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012ed0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012ee0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00012ef0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00012f00: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
-00012f10: 6975 735f 6b65 7920 3a20 7261 6469 7573  ius_key : radius
-00012f20: 207d 290d 0a20 2020 2020 2020 2020 2020   })..           
-00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
+00012ed0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
+00012ee0: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
+00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f10: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
+00012f20: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00012f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00012f60: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00012f70: 656e 7369 6f6e 5b31 5d20 3d3d 2030 3a0d  ension[1] == 0:.
+00012f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00012fd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012fe0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00012ff0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00013000: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013010: 705f 6669 7273 746b 6579 203a 202d 317d  p_firstkey : -1}
-00013020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012fb0: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
+00012fc0: 662e 7863 616c 6962 7261 7469 6f6e 2020  f.xcalibration  
+00012fd0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ff0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+00013000: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+00013010: 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20 2020  on[0] == 1:..   
+00013020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013060: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00013070: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00013080: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00013090: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-000130a0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-000130b0: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
+00013040: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
+00013050: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
+00013060: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013090: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
+000130a0: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
+000130b0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
 000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000130f0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00013100: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00013110: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00013120: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
-00013130: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
-00013140: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
+000130e0: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
+000130f0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00013100: 6e20 200d 0a0d 0a20 2020 2020 2020 2020  n  ....         
+00013110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013120: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00013130: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00013140: 7369 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20  sion[0] == 1:.. 
 00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00013180: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00013190: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-000131a0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-000131b0: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
-000131c0: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00013180: 3120 3d20 7365 6c66 2e79 6361 6c69 6272  1 = self.ycalibr
+00013190: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131c0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+000131d0: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+000131e0: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
 000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00013210: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00013220: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00013230: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00013240: 7261 6469 7573 5f6b 6579 203a 202d 3120  radius_key : -1 
-00013250: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 2020 2020 2020 200d 0a0d 0a0d 0a0d 0a0d         .........
-00013290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013210: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00013220: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
+00013230: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
+00013240: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013260: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00013270: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00013280: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
+00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132d0: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
-000132e0: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
-000132f0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013320: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
-00013330: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00013340: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
-00013350: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013360: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
-00013370: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
-00013380: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
-00013390: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
-000133a0: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-000133b0: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
-000133c0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-000133d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000133e0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-000133f0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
-00013400: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
-00013410: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
-00013420: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
-00013430: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
-00013440: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00013450: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
-00013460: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
-00013470: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
-00013480: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
-00013490: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
-000134a0: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
-000134b0: 2020 2020 2020 2020 2020 2020 2020 5820                X 
-000134c0: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
-000134d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000134e0: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
-000134f0: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
-00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013510: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
-00013520: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00013530: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
-00013540: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-00013550: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
-00013560: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
-00013570: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-00013580: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
-00013590: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000135a0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-000135b0: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
-000135c0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000135d0: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
-000135e0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
-000135f0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00013600: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
-00013610: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-00013620: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013630: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
-00013640: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
-00013650: 2020 2020 2020 2020 2020 2020 2020 6563                ec
-00013660: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013670: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
-00013680: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
-00013690: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000136a0: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
-000136b0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-000136c0: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
-000136d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000136e0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-000136f0: 656e 7369 7479 203d 2074 7261 636b 6c65  ensity = trackle
-00013700: 745f 7072 6f70 6572 7469 6573 5b3a 2c38  t_properties[:,8
-00013710: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013720: 2020 2073 7065 6564 203d 2074 7261 636b     speed = track
-00013730: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00013740: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
-00013750: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
-00013760: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-00013770: 7065 7274 6965 735b 3a2c 3130 5d0d 0a20  perties[:,10].. 
-00013780: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00013790: 6363 656c 6572 6174 696f 6e20 3d20 7472  cceleration = tr
-000137a0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-000137b0: 735b 3a2c 3131 5d0d 0a20 2020 2020 2020  s[:,11]..       
-000137c0: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-000137d0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7472  e_cell_mask = tr
-000137e0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-000137f0: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
-00013800: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
-00013810: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
-00013820: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
-00013830: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013840: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-00013850: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
-00013860: 7065 7274 6965 735b 3a2c 3134 5d0d 0a20  perties[:,14].. 
-00013870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00013880: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
-00013890: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
-000138a0: 7065 7274 6965 735b 3a2c 3135 5d0d 0a20  perties[:,15].. 
-000138b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000138c0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-000138d0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
-000138e0: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-000138f0: 7065 7274 6965 735b 3a2c 3136 5d0d 0a20  perties[:,16].. 
-00013900: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013910: 2020 2020 2020 2020 2020 2020 206d 6178               max
-00013920: 5f74 7261 636b 5f64 6973 7461 6e63 6520  _track_distance 
-00013930: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00013940: 7274 6965 735b 3a2c 3137 5d0d 0a20 2020  rties[:,17]..   
-00013950: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00013960: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00013970: 6b5f 6475 7261 7469 6f6e 203d 2074 7261  k_duration = tra
-00013980: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00013990: 5b3a 2c31 385d 0d0a 0d0a 0d0a 2020 2020  [:,18]......    
-000139a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000139b0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-000139c0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-000139d0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
-000139e0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-000139f0: 2020 2075 6e69 7175 655f 636c 7573 7465     unique_cluste
-00013a00: 725f 7072 6f70 6572 7469 6573 5f74 7261  r_properties_tra
-00013a10: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
-00013a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013a30: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
-00013a40: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00013a50: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00013a60: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013a70: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00013a80: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-00013a90: 3d20 7b7d 0d0a 0d0a 2020 2020 2020 2020  = {}....        
-00013aa0: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
-00013ab0: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
-00013ac0: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-00013ad0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00013ae0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-00013af0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00013b00: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
-00013b10: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00013b20: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00013b30: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00013b40: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00013b50: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00013b60: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-00013b70: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00013b80: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00013b90: 2020 2020 6578 7061 6e64 6564 5f74 696d      expanded_tim
-00013ba0: 6520 3d20 6e70 2e7a 6572 6f73 2873 656c  e = np.zeros(sel
-00013bb0: 662e 7465 6e64 202d 2073 656c 662e 7473  f.tend - self.ts
-00013bc0: 7461 7274 202b 2031 290d 0a20 2020 2020  tart + 1)..     
-00013bd0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
-00013be0: 5f73 616d 706c 6520 3d20 6578 7061 6e64  _sample = expand
-00013bf0: 6564 5f74 696d 652e 7368 6170 655b 305d  ed_time.shape[0]
-00013c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013c10: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00013c20: 286c 656e 2865 7870 616e 6465 645f 7469  (len(expanded_ti
-00013c30: 6d65 2929 3a0d 0a20 2020 2020 2020 2020  me)):..         
-00013c40: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00013c50: 7061 6e64 6564 5f74 696d 655b 695d 203d  panded_time[i] =
-00013c60: 2069 200d 0a20 2020 2020 2020 2020 2020   i ..           
-00013c70: 2020 2020 2066 6f72 2063 7572 7265 6e74       for current
-00013c80: 5f75 6e69 7175 655f 6964 2069 6e20 756e  _unique_id in un
-00013c90: 6971 7565 5f69 6473 5f73 6574 3a0d 0a20  ique_ids_set:.. 
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00013cc0: 2020 2020 2020 2065 7870 616e 6465 645f         expanded_
-00013cd0: 696e 7465 6e73 6974 7920 3d20 6e70 2e7a  intensity = np.z
-00013ce0: 6572 6f73 2873 656c 662e 7465 6e64 202d  eros(self.tend -
-00013cf0: 2073 656c 662e 7473 7461 7274 202b 2031   self.tstart + 1
-00013d00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013d10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013d20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 6375 7272 656e 745f 7469 6d65 203d 205b  current_time = [
-00013d50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013d60: 2020 2020 2020 6375 7272 656e 745f 7a20        current_z 
-00013d70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00013d80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013d90: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00013da0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013db0: 656e 745f 7820 3d20 5b5d 0d0a 2020 2020  ent_x = []..    
-00013dc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013dd0: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
-00013de0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00013df0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013e00: 745f 7261 6469 7573 203d 205b 5d0d 0a20  t_radius = [].. 
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
-00013e30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00013e40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013e50: 745f 7370 6565 6420 3d20 5b5d 0d0a 2020  t_speed = []..  
-00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e70: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
-00013e80: 616e 676c 6520 3d20 5b5d 0d0a 2020 2020  angle = []..    
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013ea0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00013eb0: 696f 6e20 3d20 5b5d 0d0a 2020 2020 2020  ion = []..      
-00013ec0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013ed0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
-00013ee0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+000132b0: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+000132c0: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
+000132d0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00013310: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+00013320: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013350: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+00013360: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+00013370: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013390: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+000133a0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+000133b0: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
+000133c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133e0: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+000133f0: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
+00013400: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013430: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00013440: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+00013450: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013480: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+00013490: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+000134a0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013500: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013530: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013550: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+00013560: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
+00013570: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
+00013580: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
+00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135a0: 2020 2020 2020 2020 2020 2020 7375 7266              surf
+000135b0: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
+000135c0: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
+000135d0: 6172 6561 5b69 5d20 2a20 7365 6c66 2e7a  area[i] * self.z
+000135e0: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
+000135f0: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
+00013600: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
+00013610: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013630: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
+00013640: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
+00013650: 7928 6365 6e74 726f 6964 290d 0a20 2020  y(centroid)..   
+00013660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013680: 2072 6164 6975 7320 3d20 7175 616c 6974   radius = qualit
+00013690: 7920 2a20 6d61 7468 2e70 6f77 2873 656c  y * math.pow(sel
+000136a0: 662e 7a63 616c 6962 7261 7469 6f6e 202a  f.zcalibration *
+000136b0: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+000136c0: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
+000136d0: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
+000136e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013700: 2020 2020 2020 6966 2064 6973 7420 3c20        if dist < 
+00013710: 7175 616c 6974 793a 0d0a 2020 2020 2020  quality:..      
+00013720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013740: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
+00013750: 6e74 726f 6964 203d 2073 706f 745f 6365  ntroid = spot_ce
+00013760: 6e74 726f 6964 735b 696e 6465 785d 0d0a  ntroids[index]..
+00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000137a0: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+000137b0: 3d20 2869 6e74 2874 696d 655f 6b65 7929  = (int(time_key)
+000137c0: 2c63 6c6f 7365 7374 5f63 656e 7472 6f69  ,closest_centroi
+000137d0: 645b 305d 2c20 636c 6f73 6573 745f 6365  d[0], closest_ce
+000137e0: 6e74 726f 6964 5b31 5d2c 2063 6c6f 7365  ntroid[1], close
+000137f0: 7374 5f63 656e 7472 6f69 645b 325d 290d  st_centroid[2]).
+00013800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013820: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
+00013830: 7365 7374 5f63 656c 6c5f 6964 203d 2073  sest_cell_id = s
+00013840: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00013850: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
+00013860: 706f 745f 6365 6e74 726f 6964 5d0d 0a20  pot_centroid].. 
+00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013890: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
+000138a0: 7665 6374 6f72 203d 205b 2066 6c6f 6174  vector = [ float
+000138b0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000138c0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000138d0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+000138e0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
+000138f0: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
+00013900: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00013910: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00013920: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
+00013930: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
+00013940: 656e 7472 6f69 645f 795f 6b65 795d 292c  entroid_y_key]),
+00013950: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00013960: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00013970: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00013980: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
+00013990: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+000139a0: 5d29 205d 0d0a 2020 2020 2020 2020 2020  ]) ]..          
+000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139d0: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
+000139e0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
+000139f0: 6528 6365 6c6c 5f61 7869 732c 206d 6173  e(cell_axis, mas
+00013a00: 6b5f 7665 6374 6f72 290d 0a20 2020 2020  k_vector)..     
+00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a60: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00013a70: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00013a80: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00013a90: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00013aa0: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
+00013ab0: 6b5f 6b65 7920 3a20 6365 6c6c 5f61 7869  k_key : cell_axi
+00013ac0: 735f 6d61 736b 7d29 0d0a 2020 2020 2020  s_mask})..      
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013af0: 2020 2020 2020 6966 2073 656c 662e 756e        if self.un
+00013b00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00013b10: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00013b20: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
+00013b30: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
+00013b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b70: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00013b80: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00013b90: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00013ba0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00013bb0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00013bc0: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
+00013bd0: 3a20 6563 6365 6e74 7269 6369 7479 5f63  : eccentricity_c
+00013be0: 6f6d 705f 6669 7273 7479 7a5b 305d 202a  omp_firstyz[0] *
+00013bf0: 2073 6361 6c65 5f31 7d29 0d0a 2020 2020   scale_1})..    
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00013c40: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00013c50: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00013c60: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
+00013c70: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013c80: 5f73 6563 6f6e 646b 6579 203a 2065 6363  _secondkey : ecc
+00013c90: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00013ca0: 6972 7374 797a 5b31 5d20 2a20 7363 616c  irstyz[1] * scal
+00013cb0: 655f 327d 290d 0a20 2020 2020 2020 2020  e_2})..         
+00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013cf0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00013d00: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00013d10: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+00013d20: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
+00013d30: 655f 6172 6561 5f6b 6579 203a 2073 7572  e_area_key : sur
+00013d40: 6661 6365 5f61 7265 617d 290d 0a20 2020  face_area})..   
+00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d80: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00013d90: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00013da0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00013db0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00013dc0: 7175 616c 6974 795f 6b65 7920 3a20 7175  quality_key : qu
+00013dd0: 616c 6974 797d 290d 0a20 2020 2020 2020  ality})..       
+00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013e10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00013e20: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00013e30: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00013e40: 7064 6174 6528 7b73 656c 662e 7261 6469  pdate({self.radi
+00013e50: 7573 5f6b 6579 203a 2072 6164 6975 7320  us_key : radius 
+00013e60: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e90: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ec0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00013f10: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013f20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00013f30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013f40: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00013f50: 6f6d 705f 7365 636f 6e64 203d 205b 5d0d  omp_second = [].
-00013f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f70: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
-00013f80: 6163 655f 6172 6561 203d 205b 5d0d 0a0d  ace_area = []...
-00013f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013fa0: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00013fb0: 616c 5f61 6e67 6c65 203d 205b 5d0d 0a20  al_angle = [].. 
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
-00013fe0: 7869 735f 6d61 736b 203d 205b 5d20 0d0a  xis_mask = [] ..
-00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014000: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-00014010: 5f64 6973 706c 6163 656d 656e 7420 3d20  _displacement = 
-00014020: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00014030: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00014040: 6f74 616c 5f74 7261 636b 5f64 6973 7461  otal_track_dista
-00014050: 6e63 6520 3d20 5b5d 0d0a 2020 2020 2020  nce = []..      
-00014060: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00014070: 7265 6e74 5f6d 6178 5f74 7261 636b 5f64  rent_max_track_d
-00014080: 6973 7461 6e63 6520 3d20 5b5d 0d0a 2020  istance = []..  
+00013f00: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00013f10: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00013f20: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00013f30: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
+00013f40: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013f50: 5f66 6972 7374 6b65 7920 3a20 2d31 7d29  _firstkey : -1})
+00013f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00013fa0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00013fb0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00013fc0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00013fd0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+00013fe0: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
+00013ff0: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014020: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014030: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014040: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00014050: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00014060: 7064 6174 6528 7b73 656c 662e 7375 7266  pdate({self.surf
+00014070: 6163 655f 6172 6561 5f6b 6579 203a 202d  ace_area_key : -
+00014080: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
 00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2063 7572 7265 6e74 5f74 7261 636b 5f64   current_track_d
-000140b0: 7572 6174 696f 6e20 3d20 5b5d 0d0a 2020  uration = []..  
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000140e0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-000140f0: 616e 6765 2874 696d 652e 7368 6170 655b  ange(time.shape[
-00014100: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140b0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000140c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000140d0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+000140e0: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+000140f0: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
+00014100: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
 00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014120: 6966 2063 7572 7265 6e74 5f75 6e69 7175  if current_uniqu
-00014130: 655f 6964 203d 3d20 756e 6971 7565 5f69  e_id == unique_i
-00014140: 6473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ds[j]:..        
-00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014160: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00014170: 5f74 696d 652e 6170 7065 6e64 2874 696d  _time.append(tim
-00014180: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-00014190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000141b0: 7a2e 6170 7065 6e64 285a 5b6a 5d29 0d0a  z.append(Z[j])..
-000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014140: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014150: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014160: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
+00014170: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
+00014180: 6164 6975 735f 6b65 7920 3a20 2d31 207d  adius_key : -1 }
+00014190: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000141a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141c0: 2020 2020 2020 0d0a 0d0a 0d0a 0d0a 0d0a        ..........
 000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 2063 7572 7265 6e74 5f79 2e61 7070 656e   current_y.appen
-000141f0: 6428 595b 6a5d 290d 0a20 2020 2020 2020  d(Y[j])..       
+000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014210: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014220: 745f 782e 6170 7065 6e64 2858 5b6a 5d29  t_x.append(X[j])
-00014230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014210: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00014220: 6c66 2e72 6f6f 745f 7370 6f74 732e 6974  lf.root_spots.it
+00014230: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
 00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014250: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
-00014260: 6e73 6974 795b 696e 7428 7469 6d65 5b6a  nsity[int(time[j
-00014270: 5d29 5d20 3d20 696e 7465 6e73 6974 795b  ])] = intensity[
-00014280: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
-00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142a0: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
-000142b0: 656e 7369 7479 2e61 7070 656e 6428 696e  ensity.append(in
-000142c0: 7465 6e73 6974 795b 6a5d 290d 0a20 2020  tensity[j])..   
-000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000142f0: 7272 656e 745f 7261 6469 7573 2e61 7070  rrent_radius.app
-00014300: 656e 6428 7261 6469 7573 5b6a 5d29 0d0a  end(radius[j])..
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014330: 2063 7572 7265 6e74 5f76 6f6c 756d 652e   current_volume.
-00014340: 6170 7065 6e64 2876 6f6c 756d 655b 6a5d  append(volume[j]
-00014350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
-00014380: 642e 6170 7065 6e64 2873 7065 6564 5b6a  d.append(speed[j
-00014390: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143b0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
-000143c0: 696f 6e5f 616e 676c 652e 6170 7065 6e64  ion_angle.append
-000143d0: 286d 6f74 696f 6e5f 616e 676c 655b 6a5d  (motion_angle[j]
-000143e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00014410: 6c65 7261 7469 6f6e 2e61 7070 656e 6428  leration.append(
-00014420: 6163 6365 6c65 7261 7469 6f6e 5b6a 5d29  acceleration[j])
-00014430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00014460: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00014470: 7065 6e64 2864 6973 7461 6e63 655f 6365  pend(distance_ce
-00014480: 6c6c 5f6d 6173 6b5b 6a5d 290d 0a20 2020  ll_mask[j])..   
-00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144a0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000144b0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-000144c0: 7479 5f63 6f6d 705f 6669 7273 742e 6170  ty_comp_first.ap
-000144d0: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
-000144e0: 795f 636f 6d70 5f66 6972 7374 5b6a 5d29  y_comp_first[j])
-000144f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014510: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-00014520: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00014530: 6f6e 642e 6170 7065 6e64 2865 6363 656e  ond.append(eccen
-00014540: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00014550: 6f6e 645b 6a5d 290d 0a20 2020 2020 2020  ond[j])..       
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014580: 745f 7375 7266 6163 655f 6172 6561 2e61  t_surface_area.a
-00014590: 7070 656e 6428 7375 7266 6163 655f 6172  ppend(surface_ar
-000145a0: 6561 5b6a 5d29 0d0a 2020 2020 2020 2020  ea[j])..        
-000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000145d0: 5f72 6164 6961 6c5f 616e 676c 652e 6170  _radial_angle.ap
-000145e0: 7065 6e64 2872 6164 6961 6c5f 616e 676c  pend(radial_angl
-000145f0: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014620: 6365 6c6c 5f61 7869 735f 6d61 736b 2e61  cell_axis_mask.a
-00014630: 7070 656e 6428 6365 6c6c 5f61 7869 735f  ppend(cell_axis_
-00014640: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
-00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00014670: 6e74 5f74 7261 636b 5f64 6973 706c 6163  nt_track_displac
-00014680: 656d 656e 742e 6170 7065 6e64 2874 7261  ement.append(tra
-00014690: 636b 5f64 6973 706c 6163 656d 656e 745b  ck_displacement[
-000146a0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 2020 2020 2020 6375 7272 656e 745f 746f        current_to
-000146d0: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
-000146e0: 6365 2e61 7070 656e 6428 746f 7461 6c5f  ce.append(total_
-000146f0: 7472 6163 6b5f 6469 7374 616e 6365 5b6a  track_distance[j
-00014700: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2063 7572 7265 6e74 5f6d 6178       current_max
-00014730: 5f74 7261 636b 5f64 6973 7461 6e63 652e  _track_distance.
-00014740: 6170 7065 6e64 286d 6178 5f74 7261 636b  append(max_track
-00014750: 5f64 6973 7461 6e63 655b 6a5d 290d 0a20  _distance[j]).. 
-00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 6375 7272 656e 745f 7472 6163 6b5f 6475  current_track_du
-00014790: 7261 7469 6f6e 2e61 7070 656e 6428 7472  ration.append(tr
-000147a0: 6163 6b5f 6475 7261 7469 6f6e 5b6a 5d29  ack_duration[j])
-000147b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000147e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000147f0: 6e74 5f74 696d 6520 3d20 6e70 2e61 7361  nt_time = np.asa
-00014800: 7272 6179 2863 7572 7265 6e74 5f74 696d  rray(current_tim
-00014810: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00014820: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-00014830: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00014840: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
-00014850: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00014860: 696e 7465 6e73 6974 792c 2064 7479 7065  intensity, dtype
-00014870: 3d6e 702e 666c 6f61 7433 3229 0d0a 0d0a  =np.float32)....
-00014880: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014890: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
-000148a0: 6164 6975 7320 3d20 6e70 2e61 7361 7272  adius = np.asarr
-000148b0: 6179 2863 7572 7265 6e74 5f72 6164 6975  ay(current_radiu
-000148c0: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-000148d0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-000148e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000148f0: 5f76 6f6c 756d 6520 3d20 6e70 2e61 7361  _volume = np.asa
-00014900: 7272 6179 2863 7572 7265 6e74 5f76 6f6c  rray(current_vol
-00014910: 756d 652c 2064 7479 7065 3d6e 702e 666c  ume, dtype=np.fl
-00014920: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00014930: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00014940: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
-00014950: 636f 6d70 5f66 6972 7374 203d 206e 702e  comp_first = np.
-00014960: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00014970: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00014980: 705f 6669 7273 742c 2064 7479 7065 3d6e  p_first, dtype=n
-00014990: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000149b0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-000149c0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
-000149d0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-000149e0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-000149f0: 795f 636f 6d70 5f73 6563 6f6e 642c 2064  y_comp_second, d
-00014a00: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00014a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014a20: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
-00014a30: 6661 6365 5f61 7265 6120 3d20 6e70 2e61  face_area = np.a
-00014a40: 7361 7272 6179 2863 7572 7265 6e74 5f73  sarray(current_s
-00014a50: 7572 6661 6365 5f61 7265 612c 2064 7479  urface_area, dty
-00014a60: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00014a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014a80: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
-00014a90: 6564 203d 206e 702e 6173 6172 7261 7928  ed = np.asarray(
-00014aa0: 6375 7272 656e 745f 7370 6565 642c 2064  current_speed, d
-00014ab0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00014ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014ad0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
-00014ae0: 696f 6e5f 616e 676c 6520 3d20 6e70 2e61  ion_angle = np.a
-00014af0: 7361 7272 6179 2863 7572 7265 6e74 5f6d  sarray(current_m
-00014b00: 6f74 696f 6e5f 616e 676c 652c 2064 7479  otion_angle, dty
-00014b10: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b30: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
-00014b40: 6572 6174 696f 6e20 3d20 6e70 2e61 7361  eration = np.asa
-00014b50: 7272 6179 2863 7572 7265 6e74 5f61 6363  rray(current_acc
-00014b60: 656c 6572 6174 696f 6e2c 2064 7479 7065  eleration, dtype
-00014b70: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-00014b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b90: 2063 7572 7265 6e74 5f64 6973 7461 6e63   current_distanc
-00014ba0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 6e70  e_cell_mask = np
-00014bb0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00014bc0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00014bd0: 6173 6b2c 2064 7479 7065 3d6e 702e 666c  ask, dtype=np.fl
-00014be0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00014bf0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00014c00: 6e74 5f72 6164 6961 6c5f 616e 676c 6520  nt_radial_angle 
-00014c10: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00014c20: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
-00014c30: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00014c40: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-00014c50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00014c60: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b20  _cell_axis_mask 
-00014c70: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00014c80: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-00014c90: 6173 6b2c 2064 7479 7065 3d6e 702e 666c  ask, dtype=np.fl
-00014ca0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
-00014cb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cd0: 6375 7272 656e 745f 7472 6163 6b5f 6469  current_track_di
-00014ce0: 7370 6c61 6365 6d65 6e74 203d 206e 702e  splacement = np.
-00014cf0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00014d00: 7472 6163 6b5f 6469 7370 6c61 6365 6d65  track_displaceme
-00014d10: 6e74 2c20 6474 7970 653d 6e70 2e66 6c6f  nt, dtype=np.flo
-00014d20: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014d30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014d40: 745f 746f 7461 6c5f 7472 6163 6b5f 6469  t_total_track_di
-00014d50: 7374 616e 6365 203d 206e 702e 6173 6172  stance = np.asar
-00014d60: 7261 7928 6375 7272 656e 745f 746f 7461  ray(current_tota
-00014d70: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
-00014d80: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00014d90: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00014da0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014db0: 6d61 785f 7472 6163 6b5f 6469 7374 616e  max_track_distan
-00014dc0: 6365 203d 206e 702e 6173 6172 7261 7928  ce = np.asarray(
-00014dd0: 6375 7272 656e 745f 6d61 785f 7472 6163  current_max_trac
-00014de0: 6b5f 6469 7374 616e 6365 2c20 6474 7970  k_distance, dtyp
-00014df0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e10: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
-00014e20: 6475 7261 7469 6f6e 203d 206e 702e 6173  duration = np.as
-00014e30: 6172 7261 7928 6375 7272 656e 745f 7472  array(current_tr
-00014e40: 6163 6b5f 6475 7261 7469 6f6e 2c20 6474  ack_duration, dt
-00014e50: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00014e60: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00014e70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00014e80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ea0: 2020 6966 2070 6f69 6e74 5f73 616d 706c    if point_sampl
-00014eb0: 6520 3e20 303a 0d0a 2020 2020 2020 2020  e > 0:..        
-00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ed0: 2020 2020 2020 2020 7866 5f73 616d 706c          xf_sampl
-00014ee0: 6520 3d20 6666 7466 7265 7128 706f 696e  e = fftfreq(poin
-00014ef0: 745f 7361 6d70 6c65 2c20 7365 6c66 2e74  t_sample, self.t
-00014f00: 6361 6c69 6272 6174 696f 6e29 0d0a 2020  calibration)..  
-00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f20: 2020 2020 2020 2020 2020 2020 2020 6666                ff
-00014f30: 7473 7472 6970 5f73 616d 706c 6520 3d20  tstrip_sample = 
-00014f40: 6666 7428 6578 7061 6e64 6564 5f69 6e74  fft(expanded_int
-00014f50: 656e 7369 7479 290d 0a20 2020 2020 2020  ensity)..       
-00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f70: 2020 2020 2020 2020 2066 6674 746f 7461           ffttota
-00014f80: 6c5f 7361 6d70 6c65 203d 206e 702e 6162  l_sample = np.ab
-00014f90: 7328 6666 7473 7472 6970 5f73 616d 706c  s(fftstrip_sampl
-00014fa0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fc0: 2020 2020 7866 5f73 616d 706c 6520 3d20      xf_sample = 
-00014fd0: 7866 5f73 616d 706c 655b 3020 3a20 6c65  xf_sample[0 : le
-00014fe0: 6e28 7866 5f73 616d 706c 6529 202f 2f20  n(xf_sample) // 
-00014ff0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
+00014250: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00014260: 6f6f 745f 7370 6f74 735b 6b5d 203d 2073  oot_spots[k] = s
+00014270: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00014280: 7072 6f70 6572 7469 6573 5b6b 5d20 2020  properties[k]   
+00014290: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000142a0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+000142b0: 6620 5f63 6f6d 7075 7465 5f70 6865 6e6f  f _compute_pheno
+000142c0: 7479 7065 7328 7365 6c66 293a 0d0a 0d0a  types(self):....
+000142d0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+000142e0: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
+000142f0: 7565 5f74 7261 636b 732e 6974 656d 7328  ue_tracks.items(
+00014300: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00014310: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00014320: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+00014330: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
+00014340: 2020 2020 7472 6163 6b6c 6574 5f70 726f      tracklet_pro
+00014350: 7065 7274 6965 7320 3d20 7365 6c66 2e75  perties = self.u
+00014360: 6e69 7175 655f 7472 6163 6b5f 7072 6f70  nique_track_prop
+00014370: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
+00014380: 2020 2020 2020 2020 2020 2074 7261 636b             track
+00014390: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
+000143a0: 7472 6163 6b73 5b6b 5d0d 0a20 2020 2020  tracks[k]..     
+000143b0: 2020 2020 2020 2020 2020 205a 203d 2074             Z = t
+000143c0: 7261 636b 735b 3a2c 325d 0d0a 2020 2020  racks[:,2]..    
+000143d0: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
+000143e0: 7472 6163 6b73 5b3a 2c33 5d0d 0a20 2020  tracks[:,3]..   
+000143f0: 2020 2020 2020 2020 2020 2020 2058 203d               X =
+00014400: 2074 7261 636b 735b 3a2c 345d 0d0a 2020   tracks[:,4]..  
+00014410: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00014420: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
+00014430: 6f70 6572 7469 6573 5b3a 2c30 5d0d 0a20  operties[:,0].. 
+00014440: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00014450: 6e69 7175 655f 6964 7320 3d20 7472 6163  nique_ids = trac
+00014460: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00014470: 3a2c 315d 0d0a 2020 2020 2020 2020 2020  :,1]..          
+00014480: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
+00014490: 5f73 6574 203d 2073 6574 2875 6e69 7175  _set = set(uniqu
+000144a0: 655f 6964 7329 0d0a 2020 2020 2020 2020  e_ids)..        
+000144b0: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+000144c0: 6f6e 5f69 6473 203d 2074 7261 636b 6c65  on_ids = trackle
+000144d0: 745f 7072 6f70 6572 7469 6573 5b3a 2c32  t_properties[:,2
+000144e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000144f0: 2020 2072 6164 6975 7320 3d20 7472 6163     radius = trac
+00014500: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00014510: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
+00014520: 2020 2020 2020 766f 6c75 6d65 203d 2074        volume = t
+00014530: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00014540: 6573 5b3a 2c34 5d0d 0a20 2020 2020 2020  es[:,4]..       
+00014550: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
+00014560: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00014570: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00014580: 6572 7469 6573 5b3a 2c35 5d0d 0a20 2020  erties[:,5]..   
+00014590: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+000145a0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+000145b0: 6563 6f6e 6420 3d20 7472 6163 6b6c 6574  econd = tracklet
+000145c0: 5f70 726f 7065 7274 6965 735b 3a2c 365d  _properties[:,6]
+000145d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000145e0: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+000145f0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00014600: 7469 6573 5b3a 2c37 5d0d 0a20 2020 2020  ties[:,7]..     
+00014610: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014620: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+00014630: 6e73 6974 7920 3d20 7472 6163 6b6c 6574  nsity = tracklet
+00014640: 5f70 726f 7065 7274 6965 735b 3a2c 385d  _properties[:,8]
+00014650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014660: 2020 7370 6565 6420 3d20 7472 6163 6b6c    speed = trackl
+00014670: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00014680: 395d 0d0a 2020 2020 2020 2020 2020 2020  9]..            
+00014690: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
+000146a0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000146b0: 6572 7469 6573 5b3a 2c31 305d 0d0a 2020  erties[:,10]..  
+000146c0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
+000146d0: 6365 6c65 7261 7469 6f6e 203d 2074 7261  celeration = tra
+000146e0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000146f0: 5b3a 2c31 315d 0d0a 2020 2020 2020 2020  [:,11]..        
+00014700: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+00014710: 5f63 656c 6c5f 6d61 736b 203d 2074 7261  _cell_mask = tra
+00014720: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00014730: 5b3a 2c31 325d 0d0a 2020 2020 2020 2020  [:,12]..        
+00014740: 2020 2020 2020 2020 7261 6469 616c 5f61          radial_a
+00014750: 6e67 6c65 203d 2074 7261 636b 6c65 745f  ngle = tracklet_
+00014760: 7072 6f70 6572 7469 6573 5b3a 2c31 335d  properties[:,13]
+00014770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014780: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
+00014790: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000147a0: 6572 7469 6573 5b3a 2c31 345d 0d0a 2020  erties[:,14]..  
+000147b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000147c0: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
+000147d0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+000147e0: 6572 7469 6573 5b3a 2c31 355d 0d0a 2020  erties[:,15]..  
+000147f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014800: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00014810: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+00014820: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00014830: 6572 7469 6573 5b3a 2c31 365d 0d0a 2020  erties[:,16]..  
+00014840: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014850: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00014860: 7472 6163 6b5f 6469 7374 616e 6365 203d  track_distance =
+00014870: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00014880: 7469 6573 5b3a 2c31 375d 0d0a 2020 2020  ties[:,17]..    
+00014890: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000148a0: 2020 2020 2020 2020 2020 2074 7261 636b             track
+000148b0: 5f64 7572 6174 696f 6e20 3d20 7472 6163  _duration = trac
+000148c0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+000148d0: 3a2c 3138 5d0d 0a0d 0a0d 0a20 2020 2020  :,18]......     
+000148e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000148f0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00014900: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+00014910: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
+00014920: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014930: 2020 756e 6971 7565 5f63 6c75 7374 6572    unique_cluster
+00014940: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00014950: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
+00014960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014970: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
+00014980: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
+00014990: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+000149a0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000149b0: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+000149c0: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
+000149d0: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
+000149e0: 2020 2020 2020 2075 6e69 7175 655f 7368         unique_sh
+000149f0: 6170 655f 7072 6f70 6572 7469 6573 5f74  ape_properties_t
+00014a00: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
+00014a10: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00014a20: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+00014a30: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00014a40: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00014a50: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014a60: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
+00014a70: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+00014a80: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00014a90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014aa0: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+00014ab0: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+00014ac0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00014ad0: 2020 2065 7870 616e 6465 645f 7469 6d65     expanded_time
+00014ae0: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
+00014af0: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
+00014b00: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
+00014b10: 2020 2020 2020 2020 2020 706f 696e 745f            point_
+00014b20: 7361 6d70 6c65 203d 2065 7870 616e 6465  sample = expande
+00014b30: 645f 7469 6d65 2e73 6861 7065 5b30 5d0d  d_time.shape[0].
+00014b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b50: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00014b60: 6c65 6e28 6578 7061 6e64 6564 5f74 696d  len(expanded_tim
+00014b70: 6529 293a 0d0a 2020 2020 2020 2020 2020  e)):..          
+00014b80: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00014b90: 616e 6465 645f 7469 6d65 5b69 5d20 3d20  anded_time[i] = 
+00014ba0: 6920 0d0a 2020 2020 2020 2020 2020 2020  i ..            
+00014bb0: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
+00014bc0: 756e 6971 7565 5f69 6420 696e 2075 6e69  unique_id in uni
+00014bd0: 7175 655f 6964 735f 7365 743a 0d0a 2020  que_ids_set:..  
+00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bf0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00014c00: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
+00014c10: 6e74 656e 7369 7479 203d 206e 702e 7a65  ntensity = np.ze
+00014c20: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
+00014c30: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
+00014c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014c50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00014c60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014c70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014c80: 7572 7265 6e74 5f74 696d 6520 3d20 5b5d  urrent_time = []
+00014c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014ca0: 2020 2020 2063 7572 7265 6e74 5f7a 203d       current_z =
+00014cb0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00014cc0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00014cd0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00014ce0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014cf0: 6e74 5f78 203d 205b 5d0d 0a20 2020 2020  nt_x = []..     
+00014d00: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00014d10: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
+00014d20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00014d30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014d40: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d60: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
+00014d70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00014d80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014d90: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+00014dc0: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00014de0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00014df0: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
+00014e00: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00014e10: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00014e20: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e40: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00014e50: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
+00014e60: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00014e70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014e80: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00014e90: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
+00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014eb0: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00014ec0: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
+00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ee0: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
+00014ef0: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f10: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00014f20: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
+00014f50: 6469 7370 6c61 6365 6d65 6e74 203d 205b  displacement = [
+00014f60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00014f70: 2020 2020 2020 6375 7272 656e 745f 746f        current_to
+00014f80: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
+00014f90: 6365 203d 205b 5d0d 0a20 2020 2020 2020  ce = []..       
+00014fa0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00014fb0: 656e 745f 6d61 785f 7472 6163 6b5f 6469  ent_max_track_di
+00014fc0: 7374 616e 6365 203d 205b 5d0d 0a20 2020  stance = []..   
+00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fe0: 6375 7272 656e 745f 7472 6163 6b5f 6475  current_track_du
+00014ff0: 7261 7469 6f6e 203d 205b 5d0d 0a20 2020  ration = []..   
 00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
-00015020: 706c 6520 3d20 6666 7474 6f74 616c 5f73  ple = ffttotal_s
-00015030: 616d 706c 655b 3020 3a20 6c65 6e28 6666  ample[0 : len(ff
-00015040: 7474 6f74 616c 5f73 616d 706c 6529 202f  ttotal_sample) /
-00015050: 2f20 325d 0d0a 0d0a 2020 2020 2020 2020  / 2]....        
-00015060: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00015070: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00015080: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00015090: 745f 756e 6971 7565 5f69 645d 203d 2065  t_unique_id] = e
-000150a0: 7870 616e 6465 645f 7469 6d65 2c20 6578  xpanded_time, ex
-000150b0: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-000150c0: 2c20 7866 5f73 616d 706c 652c 2066 6674  , xf_sample, fft
-000150d0: 746f 7461 6c5f 7361 6d70 6c65 0d0a 2020  total_sample..  
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
-00015100: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00015110: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00015120: 7565 5f69 645d 203d 2020 6375 7272 656e  ue_id] =  curren
-00015130: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
-00015140: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00015150: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-00015160: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00015170: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
-00015180: 2063 7572 7265 6e74 5f74 696d 652c 2063   current_time, c
-00015190: 7572 7265 6e74 5f7a 2c20 6375 7272 656e  urrent_z, curren
-000151a0: 745f 792c 2063 7572 7265 6e74 5f78 2c20  t_y, current_x, 
-000151b0: 6375 7272 656e 745f 7261 6469 7573 2c20  current_radius, 
-000151c0: 6375 7272 656e 745f 766f 6c75 6d65 2c20  current_volume, 
-000151d0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-000151e0: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
-000151f0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00015200: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00015210: 642c 2063 7572 7265 6e74 5f73 7572 6661  d, current_surfa
-00015220: 6365 5f61 7265 610d 0a20 2020 2020 2020  ce_area..       
-00015230: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00015240: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00015250: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00015260: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00015270: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
-00015280: 2c20 6375 7272 656e 745f 7370 6565 642c  , current_speed,
-00015290: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
-000152a0: 616e 676c 652c 2063 7572 7265 6e74 5f61  angle, current_a
-000152b0: 6363 656c 6572 6174 696f 6e2c 2063 7572  cceleration, cur
-000152c0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
-000152d0: 6c6c 5f6d 6173 6b2c 2063 7572 7265 6e74  ll_mask, current
-000152e0: 5f72 6164 6961 6c5f 616e 676c 652c 2063  _radial_angle, c
-000152f0: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-00015300: 5f6d 6173 6b2c 2063 7572 7265 6e74 5f74  _mask, current_t
-00015310: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
-00015320: 742c 2063 7572 7265 6e74 5f74 6f74 616c  t, current_total
-00015330: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
-00015340: 2063 7572 7265 6e74 5f6d 6178 5f74 7261   current_max_tra
-00015350: 636b 5f64 6973 7461 6e63 652c 2063 7572  ck_distance, cur
-00015360: 7265 6e74 5f74 7261 636b 5f64 7572 6174  rent_track_durat
-00015370: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00015380: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015390: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
-000153a0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
-000153b0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
-000153c0: 7175 655f 6964 3a75 6e69 7175 655f 6666  que_id:unique_ff
-000153d0: 745f 7072 6f70 6572 7469 6573 5f74 7261  t_properties_tra
-000153e0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
-000153f0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
-00015400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015410: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
-00015420: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
-00015430: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
-00015440: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00015450: 643a 756e 6971 7565 5f63 6c75 7374 6572  d:unique_cluster
-00015460: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00015470: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00015480: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
-00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154a0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
-000154b0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
-000154c0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-000154d0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-000154e0: 3a75 6e69 7175 655f 7368 6170 655f 7072  :unique_shape_pr
-000154f0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00015500: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00015510: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
-00015520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015530: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-00015540: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-00015550: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
-00015560: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
-00015570: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
-00015580: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00015590: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-000155a0: 6964 5d7d 290d 0a0d 0a20 2020 2064 6566  id]})....    def
-000155b0: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
-000155c0: 5f73 706f 7473 2873 656c 662c 2066 7261  _spots(self, fra
-000155d0: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
-000155e0: 6c5f 6964 2c20 7472 6163 6b5f 6964 293a  l_id, track_id):
-000155f0: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-00015600: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
-00015610: 2063 656e 7472 6f69 6473 2c20 6c61 6265   centroids, labe
-00015620: 6c73 2c20 766f 6c75 6d65 2c20 696e 7465  ls, volume, inte
-00015630: 6e73 6974 795f 6d65 616e 2c20 696e 7465  nsity_mean, inte
-00015640: 6e73 6974 795f 746f 7461 6c2c 2062 6f75  nsity_total, bou
-00015650: 6e64 696e 675f 626f 7865 7320 3d20 7365  nding_boxes = se
-00015660: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
-00015670: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
-00015680: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
-00015690: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
-000156a0: 2070 6978 656c 7465 7374 6c6f 6361 7469   pixeltestlocati
-000156b0: 6f6e 203d 2028 7a2c 792c 7829 0d0a 2020  on = (z,y,x)..  
-000156c0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
-000156d0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
-000156e0: 7279 2870 6978 656c 7465 7374 6c6f 6361  ry(pixeltestloca
-000156f0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
-00015700: 2020 2020 2020 2062 626f 7820 3d20 626f         bbox = bo
-00015710: 756e 6469 6e67 5f62 6f78 6573 5b69 6e64  unding_boxes[ind
-00015720: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
-00015730: 2073 697a 657a 203d 2061 6273 2862 626f   sizez = abs(bbo
-00015740: 785b 305d 202d 2062 626f 785b 335d 290d  x[0] - bbox[3]).
-00015750: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00015760: 6579 203d 2061 6273 2862 626f 785b 315d  ey = abs(bbox[1]
-00015770: 202d 2062 626f 785b 345d 290d 0a20 2020   - bbox[4])..   
-00015780: 2020 2020 2020 2020 2073 697a 6578 203d           sizex =
-00015790: 2061 6273 2862 626f 785b 325d 202d 2062   abs(bbox[2] - b
-000157a0: 626f 785b 355d 2920 0d0a 2020 2020 2020  box[5]) ..      
-000157b0: 2020 2020 2020 7665 746f 5f76 6f6c 756d        veto_volum
-000157c0: 6520 3d20 7369 7a65 7820 2a20 7369 7a65  e = sizex * size
-000157d0: 7920 2a20 7369 7a65 7a0d 0a20 2020 2020  y * sizez..     
-000157e0: 2020 2020 2020 2076 6574 6f5f 7261 6469         veto_radi
-000157f0: 7573 203d 206d 6174 682e 706f 7728 3320  us = math.pow(3 
-00015800: 2a20 7665 746f 5f76 6f6c 756d 6520 2f20  * veto_volume / 
-00015810: 2834 202a 206d 6174 682e 7069 292c 2031  (4 * math.pi), 1
-00015820: 2e30 202f 2033 2e30 290d 0a0d 0a20 2020  .0 / 3.0)....   
-00015830: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
-00015840: 6e20 3d20 2863 656e 7472 6f69 6473 5b69  n = (centroids[i
-00015850: 6e64 6578 5d5b 305d 202a 2073 656c 662e  ndex][0] * self.
-00015860: 7a63 616c 6962 7261 7469 6f6e 2c20 6365  zcalibration, ce
-00015870: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
-00015880: 5d2a 7365 6c66 2e79 6361 6c69 6272 6174  ]*self.ycalibrat
-00015890: 696f 6e2c 2063 656e 7472 6f69 6473 5b69  ion, centroids[i
-000158a0: 6e64 6578 5d5b 325d 2a73 656c 662e 7863  ndex][2]*self.xc
-000158b0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
-000158c0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
-000158d0: 203d 206d 6174 682e 706f 7728 766f 6c75   = math.pow(volu
-000158e0: 6d65 5b69 6e64 6578 5d2c 2031 2e30 2f33  me[index], 1.0/3
-000158f0: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
-00015900: 2052 4144 4955 5320 3d20 6d61 7468 2e70   RADIUS = math.p
-00015910: 6f77 2876 6f6c 756d 655b 696e 6465 785d  ow(volume[index]
-00015920: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
-00015930: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
-00015940: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
-00015950: 7a63 616c 6962 7261 7469 6f6e 2c20 312e  zcalibration, 1.
-00015960: 302f 332e 3029 200d 0a0d 0a20 2020 2020  0/3.0) ....     
-00015970: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00015980: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
-00015990: 656e 7472 6f69 6420 3d20 7365 6c66 2e5f  entroid = self._
-000159a0: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
-000159b0: 7428 6672 616d 652c 206c 6f63 6174 696f  t(frame, locatio
-000159c0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-000159d0: 6966 2064 6973 7420 3c3d 2032 202a 2076  if dist <= 2 * v
-000159e0: 6574 6f5f 7261 6469 7573 3a0d 0a20 2020  eto_radius:..   
-000159f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015a00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-00015a10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015a20: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a40: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
-00015a50: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
-00015a60: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
-00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a80: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00015a90: 203a 2069 6e74 2866 7261 6d65 292c 0d0a   : int(frame),..
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ab0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
-00015ac0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-00015ad0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-00015ae0: 5b30 5d2a 2073 656c 662e 7a63 616c 6962  [0]* self.zcalib
-00015af0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
-00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b10: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-00015b20: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
-00015b30: 6964 735b 696e 6465 785d 5b31 5d2a 2073  ids[index][1]* s
-00015b40: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00015b50: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00015b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015b70: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
-00015b80: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
-00015b90: 6465 785d 5b32 5d2a 2073 656c 662e 7863  dex][2]* self.xc
-00015ba0: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
-00015bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bc0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00015bd0: 6964 5f6b 6579 3a20 696e 7428 7472 6163  id_key: int(trac
-00015be0: 6b5f 6964 292c 0d0a 2020 2020 2020 2020  k_id),..        
-00015bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c00: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-00015c10: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
-00015c20: 7428 696e 7465 6e73 6974 795f 746f 7461  t(intensity_tota
-00015c30: 6c5b 696e 6465 785d 2929 2c0d 0a20 2020  l[index])),..   
-00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c50: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
-00015c60: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
-00015c70: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
-00015c80: 6d65 616e 5b69 6e64 6578 5d29 292c 0d0a  mean[index])),..
-00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ca0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00015cb0: 6975 735f 6b65 7920 3a20 2866 6c6f 6174  ius_key : (float
-00015cc0: 2852 4144 4955 5329 292c 0d0a 2020 2020  (RADIUS)),..    
-00015cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ce0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
-00015cf0: 5f6b 6579 203a 2028 666c 6f61 7428 5155  _key : (float(QU
-00015d00: 414c 4954 5929 292c 0d0a 2020 2020 2020  ALITY)),..      
-00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d20: 2020 7365 6c66 2e64 6973 7461 6e63 655f    self.distance_
-00015d30: 6365 6c6c 5f6d 6173 6b5f 6b65 793a 2066  cell_mask_key: f
-00015d40: 6c6f 6174 2864 6973 7461 6e63 655f 6365  loat(distance_ce
-00015d50: 6c6c 5f6d 6173 6b29 2c0d 0a20 2020 2020  ll_mask),..     
-00015d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d70: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
-00015d80: 726f 6964 5f7a 5f6b 6579 3a20 666c 6f61  roid_z_key: floa
-00015d90: 7428 6d61 736b 6365 6e74 726f 6964 5b30  t(maskcentroid[0
-00015da0: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
-00015db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015dc0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
-00015dd0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-00015de0: 6365 6e74 726f 6964 5b31 5d29 2c0d 0a20  centroid[1]),.. 
-00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e00: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-00015e10: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
-00015e20: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
-00015e30: 6964 5b32 5d29 200d 0a0d 0a20 2020 2020  id[2]) ....     
-00015e40: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00015e50: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00015e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015e70: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00015e80: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00015e90: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-00015ea0: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
-00015eb0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015ec0: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015ee0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-00015ef0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015f00: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
-00015f10: 6528 7b73 656c 662e 746f 7461 6c5f 696e  e({self.total_in
-00015f20: 7465 6e73 6974 795f 6b65 793a 202d 317d  tensity_key: -1}
-00015f30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015f40: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00015f50: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-00015f60: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-00015f70: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
-00015f80: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-00015f90: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
-00015fa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015fb0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-00015fc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015fd0: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
-00015fe0: 7465 287b 7365 6c66 2e72 6164 6975 735f  te({self.radius_
-00015ff0: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
-00016000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016010: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-00016020: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00016030: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
-00016040: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
-00016050: 5f6b 6579 3a20 2d31 7d29 0d0a 0d0a 0d0a  _key: -1})......
-00016060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016080: 2020 200d 0a20 2020 2064 6566 205f 6469     ..    def _di
-00016090: 6374 5f75 7064 6174 6528 7365 6c66 2c20  ct_update(self, 
-000160a0: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
-000160b0: 6964 733a 204c 6973 742c 2020 6365 6c6c  ids: List,  cell
-000160c0: 5f69 643a 2069 6e74 2c20 7472 6163 6b5f  _id: int, track_
-000160d0: 6964 3a20 696e 742c 2073 6f75 7263 655f  id: int, source_
-000160e0: 6964 3a20 696e 742c 2074 6172 6765 745f  id: int, target_
-000160f0: 6964 3a20 696e 7429 3a0d 0a0d 0a20 0d0a  id: int):.... ..
-00016100: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
-00016110: 6f6e 5f69 6420 3d20 7365 6c66 2e67 656e  on_id = self.gen
-00016120: 6572 6174 696f 6e5f 6469 6374 5b63 656c  eration_dict[cel
-00016130: 6c5f 6964 5d0d 0a20 2020 2020 2020 2074  l_id]..        t
-00016140: 7261 636b 6c65 745f 6964 203d 2073 656c  racklet_id = sel
-00016150: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-00016160: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
-00016170: 200d 0a0d 0a20 2020 2020 2020 2075 6e69   ....        uni
-00016180: 7175 655f 6964 203d 2073 7472 2874 7261  que_id = str(tra
-00016190: 636b 5f69 6429 202b 2020 7374 7228 6765  ck_id) +  str(ge
-000161a0: 6e65 7261 7469 6f6e 5f69 6429 202b 2073  neration_id) + s
-000161b0: 7472 2874 7261 636b 6c65 745f 6964 290d  tr(tracklet_id).
-000161c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000161d0: 2020 2076 6563 5f6d 6173 6b20 3d20 5b66     vec_mask = [f
-000161e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000161f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00016200: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00016210: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-00016220: 5f78 5f6b 6579 5d29 2c20 666c 6f61 7428  _x_key]), float(
-00016230: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016240: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016250: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00016260: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-00016270: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
-00016280: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016290: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000162a0: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
-000162b0: 6e74 726f 6964 5f7a 5f6b 6579 5d29 205d  ntroid_z_key]) ]
-000162c0: 0d0a 0d0a 2020 2020 2020 2020 7665 635f  ....        vec_
-000162d0: 6365 6c6c 203d 205b 666c 6f61 7428 7365  cell = [float(se
-000162e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000162f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00016300: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
-00016310: 7369 645f 6b65 795d 2920 2c20 0d0a 2020  sid_key]) , ..  
-00016320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016330: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00016340: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016350: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016360: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
-00016370: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00016380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016390: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-000163a0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000163b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000163c0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-000163d0: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a0d  zposid_key])]...
-000163e0: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
-000163f0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
-00016400: 7665 635f 6d61 736b 2c20 7665 635f 6365  vec_mask, vec_ce
-00016410: 6c6c 290d 0a0d 0a20 2020 2020 2020 2073  ll)....        s
-00016420: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016430: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00016440: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00016450: 7b73 656c 662e 7261 6469 616c 5f61 6e67  {self.radial_ang
-00016460: 6c65 5f6b 6579 203a 2061 6e67 6c65 7d29  le_key : angle})
-00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016480: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00016490: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
-000164a0: 6964 732e 6170 7065 6e64 2873 7472 2875  ids.append(str(u
-000164b0: 6e69 7175 655f 6964 2929 0d0a 2020 2020  nique_id))..    
-000164c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000164d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000164e0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-000164f0: 6461 7465 287b 7365 6c66 2e75 6e69 7175  date({self.uniqu
-00016500: 6569 645f 6b65 7920 3a20 7374 7228 756e  eid_key : str(un
-00016510: 6971 7565 5f69 6429 7d29 0d0a 2020 2020  ique_id)})..    
-00016520: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00016530: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016540: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00016550: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
-00016560: 6c65 7469 645f 6b65 7920 3a20 7374 7228  letid_key : str(
-00016570: 7472 6163 6b6c 6574 5f69 6429 7d29 200d  tracklet_id)}) .
-00016580: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00016590: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000165a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000165b0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-000165c0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
-000165d0: 203a 2073 7472 2867 656e 6572 6174 696f   : str(generatio
-000165e0: 6e5f 6964 297d 2920 0d0a 2020 2020 2020  n_id)}) ..      
-000165f0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016600: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016610: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016620: 7465 287b 7365 6c66 2e74 7261 636b 6964  te({self.trackid
-00016630: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
-00016640: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
-00016650: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016660: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016670: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00016680: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
-00016690: 676c 655f 6b65 7920 3a20 302e 307d 290d  gle_key : 0.0}).
-000166a0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-000166b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000166c0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000166d0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-000166e0: 7370 6565 645f 6b65 7920 3a20 302e 307d  speed_key : 0.0}
-000166f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00016700: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016710: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00016720: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00016730: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-00016740: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
-00016750: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00016760: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016770: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00016780: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
-00016790: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-000167a0: 7374 6b65 7920 3a20 2d31 7d29 0d0a 2020  stkey : -1})..  
-000167b0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000167c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000167d0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000167e0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-000167f0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00016800: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
-00016810: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00016820: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016830: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00016840: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00016850: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-00016860: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00016870: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00016880: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00016890: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-000168a0: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
-000168b0: 5f6d 6173 6b5f 6b65 7920 3a20 2d31 7d29  _mask_key : -1})
-000168c0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
-000168d0: 6f75 7263 655f 6964 2069 7320 6e6f 7420  ource_id is not 
-000168e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000168f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00016900: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016910: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00016920: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
-00016930: 6964 5f6b 6579 203a 2069 6e74 2873 6f75  id_key : int(sou
-00016940: 7263 655f 6964 297d 290d 0a20 2020 2020  rce_id)})..     
-00016950: 2020 2020 2020 2076 6563 5f31 203d 205b         vec_1 = [
-00016960: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00016970: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016980: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00016990: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-000169a0: 2920 2d20 666c 6f61 7428 7365 6c66 2e75  ) - float(self.u
-000169b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000169c0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-000169d0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-000169e0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00016a10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016a20: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00016a30: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
-00016a40: 6964 5f6b 6579 5d29 202d 2066 6c6f 6174  id_key]) - float
-00016a50: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00016a60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00016a70: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00016a80: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
-00016a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-00016ab0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00016ac0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016ad0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00016ae0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
-00016af0: 2d20 2066 6c6f 6174 2873 656c 662e 756e  -  float(self.un
-00016b00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016b10: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00016b20: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00016b30: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
-00016b40: 2020 2020 2073 7065 6564 203d 206e 702e       speed = np.
-00016b50: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
-00016b60: 312c 2076 6563 5f31 2929 2f73 656c 662e  1, vec_1))/self.
-00016b70: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
-00016b80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00016b90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00016ba0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00016bb0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00016bc0: 2e73 7065 6564 5f6b 6579 203a 2073 7065  .speed_key : spe
-00016bd0: 6564 7d29 0d0a 0d0a 2020 2020 2020 2020  ed})....        
-00016be0: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-00016bf0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00016c00: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
-00016c10: 3129 0d0a 0d0a 2020 2020 2020 2020 2020  1)....          
-00016c20: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016c30: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016c40: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016c50: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
-00016c60: 616e 676c 655f 6b65 7920 3a20 6d6f 7469  angle_key : moti
-00016c70: 6f6e 5f61 6e67 6c65 7d29 200d 0a0d 0a20  on_angle}) .... 
-00016c80: 2020 2020 2020 2020 2020 2069 6620 736f             if so
-00016c90: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
-00016ca0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00016cb0: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-00016cc0: 2020 2020 2020 2020 2070 7265 5f73 6f75           pre_sou
-00016cd0: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
-00016ce0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
-00016cf0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
-00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d10: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016d20: 2020 2020 2020 2076 6563 5f32 203d 205b         vec_2 = [
-00016d30: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00016d40: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016d50: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00016d60: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00016d70: 2920 2d20 3220 2a20 666c 6f61 7428 7365  ) - 2 * float(se
-00016d80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016d90: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-00016da0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
-00016db0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
-00016dc0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00016dd0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016de0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
-00016df0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00016e00: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-00016e30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016e40: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00016e50: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
-00016e60: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
-00016e70: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016e80: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016e90: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00016ea0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00016eb0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-00016ec0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016ed0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-00016ee0: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
-00016ef0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f10: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00016f20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016f30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016f40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
-00016f50: 706f 7369 645f 6b65 795d 2920 2d20 2032  posid_key]) -  2
-00016f60: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
-00016f70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016f80: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00016f90: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00016fa0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
-00016fb0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016fc0: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
-00016fd0: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
-00016fe0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00016ff0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017000: 2020 2020 2020 2061 6363 203d 206e 702e         acc = np.
-00017010: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
-00017020: 322c 2076 6563 5f32 2929 2f73 656c 662e  2, vec_2))/self.
-00017030: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
-00017040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017050: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00017060: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00017070: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00017080: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00017090: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-000170a0: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
-000170b0: 3a20 6163 637d 290d 0a20 2020 2020 2020  : acc})..       
-000170c0: 2065 6c69 6620 736f 7572 6365 5f69 6420   elif source_id 
-000170d0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-000170e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000170f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00017100: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00017110: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
-00017120: 6f72 6569 645f 6b65 7920 3a20 4e6f 6e65  oreid_key : None
-00017130: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
-00017140: 200d 0a0d 0a20 2020 2020 2020 2069 6620   ....        if 
-00017150: 7461 7267 6574 5f69 6420 6973 206e 6f74  target_id is not
-00017160: 204e 6f6e 653a 2020 2020 2020 200d 0a20   None:       .. 
-00017170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017180: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00017190: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000171a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000171b0: 662e 6166 7465 7269 645f 6b65 7920 3a20  f.afterid_key : 
-000171c0: 696e 7428 7461 7267 6574 5f69 6429 7d29  int(target_id)})
-000171d0: 200d 0a20 2020 2020 2020 2065 6c69 6620   ..        elif 
-000171e0: 7461 7267 6574 5f69 6420 6973 204e 6f6e  target_id is Non
-000171f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00017200: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00017210: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00017220: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00017230: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
-00017240: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
-00017250: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00017260: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
-00017270: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
-00017280: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
-00017290: 2920 2020 200d 0a0d 0a0d 0a20 2020 2064  )    ......    d
-000172a0: 6566 205f 7465 6d70 6f72 616c 5f70 6c6f  ef _temporal_plo
-000172b0: 7473 5f74 7261 636b 6d61 7465 2873 656c  ts_trackmate(sel
-000172c0: 6629 3a0d 0a20 2020 200d 0a20 2020 200d  f):..    ..    .
-000172d0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
-000172e0: 2020 2020 2020 2073 656c 662e 4174 7472         self.Attr
-000172f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00017300: 2020 2020 2020 2073 7461 7274 7469 6d65         starttime
-00017310: 203d 2069 6e74 286d 696e 2873 656c 662e   = int(min(self.
-00017320: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
-00017330: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
-00017340: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00017350: 6e64 7469 6d65 203d 2069 6e74 286d 6178  ndtime = int(max
-00017360: 2873 656c 662e 416c 6c56 616c 7565 735b  (self.AllValues[
-00017370: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00017380: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-00017390: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000173a0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-000173b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000173c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000173d0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
-000173e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000173f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00017400: 7469 635f 7661 725f 6469 7370 5f7a 203d  tic_var_disp_z =
-00017410: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00017420: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00017430: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
-00017440: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00017450: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017460: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
-00017470: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00017480: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017490: 6963 5f6d 6561 6e5f 6469 7370 5f78 203d  ic_mean_disp_x =
-000174a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000174b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000174c0: 635f 7661 725f 6469 7370 5f78 203d 205b  c_var_disp_x = [
-000174d0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000174e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000174f0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
-00017500: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017510: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017520: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00017530: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017540: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017550: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
-00017560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017570: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00017580: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
-00017590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000175a0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-000175b0: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
-000175c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000175d0: 662e 6d69 746f 7469 635f 7661 725f 6163  f.mitotic_var_ac
-000175e0: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-000175f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00017600: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
-00017610: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
-00017620: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017630: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00017640: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
-00017650: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
-00017660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017670: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00017680: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
-00017690: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
-000176a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000176b0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-000176c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-000176d0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000176e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000176f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00017700: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
-00017710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017720: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00017730: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
-00017740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017750: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00017760: 6d65 616e 5f64 6973 705f 7920 3d20 5b5d  mean_disp_y = []
-00017770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017780: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00017790: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
-000177a0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000177b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000177c0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-000177d0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-000177e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000177f0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00017800: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
-00017810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017820: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00017830: 616e 5f72 6164 6975 7320 3d20 5b5d 0d0a  an_radius = []..
-00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017850: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00017860: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00017870: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017880: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00017890: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
-000178a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000178b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000178c0: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
-000178d0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000178e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000178f0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f61  n_mitotic_mean_a
-00017900: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00017910: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017920: 6e5f 6d69 746f 7469 635f 7661 725f 6163  n_mitotic_var_ac
-00017930: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-00017940: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00017950: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00017960: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00017970: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
-00017980: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017990: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000179a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000179b0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000179c0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000179d0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000179e0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000179f0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00017a00: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017a10: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00017a20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00017a30: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00017a40: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017a50: 5f6d 6561 6e5f 6469 7370 5f7a 203d 205b  _mean_disp_z = [
-00017a60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017a70: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00017a80: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
-00017a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017aa0: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
-00017ab0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
-00017ac0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00017ad0: 6c6c 5f76 6172 5f64 6973 705f 7920 3d20  ll_var_disp_y = 
-00017ae0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00017af0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00017b00: 6561 6e5f 6469 7370 5f78 203d 205b 5d0d  ean_disp_x = [].
-00017b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b20: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00017b30: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
-00017b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017b50: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
-00017b60: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00017b70: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017b80: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00017b90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017ba0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00017bb0: 6e5f 7370 6565 6420 3d20 5b5d 0d0a 2020  n_speed = []..  
-00017bc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017bd0: 6c66 2e61 6c6c 5f76 6172 5f73 7065 6564  lf.all_var_speed
-00017be0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017bf0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017c00: 6c5f 6d65 616e 5f61 6363 203d 205b 5d0d  l_mean_acc = [].
-00017c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c20: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
-00017c30: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-00017c40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00017c50: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
-00017c60: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00017c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c80: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00017c90: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00017ca0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017cb0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017cc0: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
-00017cd0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cf0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
-00017d00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00017d10: 3d20 5b5d 0d0a 0d0a 0d0a 2020 2020 2020  = []......      
-00017d20: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00017d30: 6f74 735f 7472 6163 6b73 203d 207b 7d0d  ots_tracks = {}.
-00017d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d50: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00017d60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00017d70: 726f 7065 7274 6965 732e 6974 656d 7328  roperties.items(
-00017d80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00017d90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 2020 616c 6c5f 7370 6f74 7320 3d20 7365    all_spots = se
-00017dc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00017dd0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-00017de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017df0: 2020 2020 6966 2073 656c 662e 7472 6163      if self.trac
-00017e00: 6b69 645f 6b65 7920 696e 2061 6c6c 5f73  kid_key in all_s
-00017e10: 706f 7473 3a0d 0a20 2020 2020 2020 2020  pots:..         
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00017e40: 735b 6b5d 203d 2061 6c6c 5f73 706f 7473  s[k] = all_spots
-00017e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017e60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00017e70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00017e80: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-00017e90: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00017ea0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-00017eb0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-00017ec0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-00017ed0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-00017ee0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-00017ef0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00017f20: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00017f30: 6e20 7471 646d 2872 616e 6765 2873 7461  n tqdm(range(sta
-00017f40: 7274 7469 6d65 2c20 656e 6474 696d 6529  rttime, endtime)
-00017f50: 2c20 746f 7461 6c3d 656e 6474 696d 6520  , total=endtime 
-00017f60: 2d20 7374 6172 7474 696d 6529 3a0d 0a20  - starttime):.. 
-00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017f90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00017fa0: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-00017fb0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-00017fc0: 6c66 2e5f 636f 6d70 7574 655f 7465 6d70  lf._compute_temp
-00017fd0: 6f72 616c 2c20 692c 2061 6c6c 5f73 706f  oral, i, all_spo
-00017fe0: 7473 5f74 7261 636b 7329 290d 0a20 0d0a  ts_tracks)).. ..
-00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018000: 2020 2020 5b72 2e72 6573 756c 7428 2920      [r.result() 
-00018010: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
-00018020: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
-00018030: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
-00018040: 295d 0d0a 0d0a 0d0a 2020 2020 6465 6620  )]......    def 
-00018050: 5f63 6f6d 7075 7465 5f74 656d 706f 7261  _compute_tempora
-00018060: 6c28 7365 6c66 2c20 692c 2061 6c6c 5f73  l(self, i, all_s
-00018070: 706f 7473 5f74 7261 636b 7329 3a20 2020  pots_tracks):   
-00018080: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00018090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180a0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-000180b0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-000180c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000180d0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-000180e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000180f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00018100: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00018110: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00018120: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00018130: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00018140: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
-00018150: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00018160: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00018170: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-00018180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018190: 2020 2020 206d 6974 6f74 6963 5f64 6972       mitotic_dir
-000181a0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000181b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000181c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000181d0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-000181e0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-000181f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018200: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00018210: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00018220: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018230: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00018240: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00018250: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018260: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00018270: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00018280: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00018290: 7469 635f 7261 6469 7573 203d 205b 5d0d  tic_radius = [].
-000182a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000182b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000182c0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182e0: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
+00015010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015020: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+00015030: 6e67 6528 7469 6d65 2e73 6861 7065 5b30  nge(time.shape[0
+00015040: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00015050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015060: 6620 6375 7272 656e 745f 756e 6971 7565  f current_unique
+00015070: 5f69 6420 3d3d 2075 6e69 7175 655f 6964  _id == unique_id
+00015080: 735b 6a5d 3a0d 0a20 2020 2020 2020 2020  s[j]:..         
+00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000150b0: 7469 6d65 2e61 7070 656e 6428 7469 6d65  time.append(time
+000150c0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150e0: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
+000150f0: 2e61 7070 656e 6428 5a5b 6a5d 290d 0a20  .append(Z[j]).. 
+00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015120: 6375 7272 656e 745f 792e 6170 7065 6e64  current_y.append
+00015130: 2859 5b6a 5d29 0d0a 2020 2020 2020 2020  (Y[j])..        
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00015160: 5f78 2e61 7070 656e 6428 585b 6a5d 290d  _x.append(X[j]).
+00015170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
+000151a0: 7369 7479 5b69 6e74 2874 696d 655b 6a5d  sity[int(time[j]
+000151b0: 295d 203d 2069 6e74 656e 7369 7479 5b6a  )] = intensity[j
+000151c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151e0: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
+000151f0: 6e73 6974 792e 6170 7065 6e64 2869 6e74  nsity.append(int
+00015200: 656e 7369 7479 5b6a 5d29 0d0a 2020 2020  ensity[j])..    
+00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015220: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00015230: 7265 6e74 5f72 6164 6975 732e 6170 7065  rent_radius.appe
+00015240: 6e64 2872 6164 6975 735b 6a5d 290d 0a20  nd(radius[j]).. 
+00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015270: 6375 7272 656e 745f 766f 6c75 6d65 2e61  current_volume.a
+00015280: 7070 656e 6428 766f 6c75 6d65 5b6a 5d29  ppend(volume[j])
+00015290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000152a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152b0: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
+000152c0: 2e61 7070 656e 6428 7370 6565 645b 6a5d  .append(speed[j]
+000152d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000152e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152f0: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
+00015300: 6f6e 5f61 6e67 6c65 2e61 7070 656e 6428  on_angle.append(
+00015310: 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a 5d29  motion_angle[j])
+00015320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015340: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
+00015350: 6572 6174 696f 6e2e 6170 7065 6e64 2861  eration.append(a
+00015360: 6363 656c 6572 6174 696f 6e5b 6a5d 290d  cceleration[j]).
+00015370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015390: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
+000153a0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+000153b0: 656e 6428 6469 7374 616e 6365 5f63 656c  end(distance_cel
+000153c0: 6c5f 6d61 736b 5b6a 5d29 0d0a 2020 2020  l_mask[j])..    
+000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153e0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000153f0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00015400: 795f 636f 6d70 5f66 6972 7374 2e61 7070  y_comp_first.app
+00015410: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
+00015420: 5f63 6f6d 705f 6669 7273 745b 6a5d 290d  _comp_first[j]).
+00015430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015450: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00015460: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00015470: 6e64 2e61 7070 656e 6428 6563 6365 6e74  nd.append(eccent
+00015480: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00015490: 6e64 5b6a 5d29 0d0a 2020 2020 2020 2020  nd[j])..        
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000154c0: 5f73 7572 6661 6365 5f61 7265 612e 6170  _surface_area.ap
+000154d0: 7065 6e64 2873 7572 6661 6365 5f61 7265  pend(surface_are
+000154e0: 615b 6a5d 290d 0a20 2020 2020 2020 2020  a[j])..         
+000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015500: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00015510: 7261 6469 616c 5f61 6e67 6c65 2e61 7070  radial_angle.app
+00015520: 656e 6428 7261 6469 616c 5f61 6e67 6c65  end(radial_angle
+00015530: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00015540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015550: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00015560: 656c 6c5f 6178 6973 5f6d 6173 6b2e 6170  ell_axis_mask.ap
+00015570: 7065 6e64 2863 656c 6c5f 6178 6973 5f6d  pend(cell_axis_m
+00015580: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
+00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000155b0: 745f 7472 6163 6b5f 6469 7370 6c61 6365  t_track_displace
+000155c0: 6d65 6e74 2e61 7070 656e 6428 7472 6163  ment.append(trac
+000155d0: 6b5f 6469 7370 6c61 6365 6d65 6e74 5b6a  k_displacement[j
+000155e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015600: 2020 2020 2063 7572 7265 6e74 5f74 6f74       current_tot
+00015610: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+00015620: 652e 6170 7065 6e64 2874 6f74 616c 5f74  e.append(total_t
+00015630: 7261 636b 5f64 6973 7461 6e63 655b 6a5d  rack_distance[j]
+00015640: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2020 2020 6375 7272 656e 745f 6d61 785f      current_max_
+00015670: 7472 6163 6b5f 6469 7374 616e 6365 2e61  track_distance.a
+00015680: 7070 656e 6428 6d61 785f 7472 6163 6b5f  ppend(max_track_
+00015690: 6469 7374 616e 6365 5b6a 5d29 0d0a 2020  distance[j])..  
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000156c0: 7572 7265 6e74 5f74 7261 636b 5f64 7572  urrent_track_dur
+000156d0: 6174 696f 6e2e 6170 7065 6e64 2874 7261  ation.append(tra
+000156e0: 636b 5f64 7572 6174 696f 6e5b 6a5d 290d  ck_duration[j]).
+000156f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015710: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00015720: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00015730: 745f 7469 6d65 203d 206e 702e 6173 6172  t_time = np.asar
+00015740: 7261 7928 6375 7272 656e 745f 7469 6d65  ray(current_time
+00015750: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00015760: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00015770: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00015780: 696e 7465 6e73 6974 7920 3d20 6e70 2e61  intensity = np.a
+00015790: 7361 7272 6179 2863 7572 7265 6e74 5f69  sarray(current_i
+000157a0: 6e74 656e 7369 7479 2c20 6474 7970 653d  ntensity, dtype=
+000157b0: 6e70 2e66 6c6f 6174 3332 290d 0a0d 0a0d  np.float32).....
+000157c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000157d0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
+000157e0: 6469 7573 203d 206e 702e 6173 6172 7261  dius = np.asarra
+000157f0: 7928 6375 7272 656e 745f 7261 6469 7573  y(current_radius
+00015800: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00015810: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00015820: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00015830: 766f 6c75 6d65 203d 206e 702e 6173 6172  volume = np.asar
+00015840: 7261 7928 6375 7272 656e 745f 766f 6c75  ray(current_volu
+00015850: 6d65 2c20 6474 7970 653d 6e70 2e66 6c6f  me, dtype=np.flo
+00015860: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00015870: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00015880: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00015890: 6f6d 705f 6669 7273 7420 3d20 6e70 2e61  omp_first = np.a
+000158a0: 7361 7272 6179 2863 7572 7265 6e74 5f65  sarray(current_e
+000158b0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000158c0: 5f66 6972 7374 2c20 6474 7970 653d 6e70  _first, dtype=np
+000158d0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+000158e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000158f0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00015900: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
+00015910: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00015920: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00015930: 5f63 6f6d 705f 7365 636f 6e64 2c20 6474  _comp_second, dt
+00015940: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00015950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015960: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
+00015970: 6163 655f 6172 6561 203d 206e 702e 6173  ace_area = np.as
+00015980: 6172 7261 7928 6375 7272 656e 745f 7375  array(current_su
+00015990: 7266 6163 655f 6172 6561 2c20 6474 7970  rface_area, dtyp
+000159a0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
+000159b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000159c0: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
+000159d0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
+000159e0: 7572 7265 6e74 5f73 7065 6564 2c20 6474  urrent_speed, dt
+000159f0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00015a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015a10: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
+00015a20: 6f6e 5f61 6e67 6c65 203d 206e 702e 6173  on_angle = np.as
+00015a30: 6172 7261 7928 6375 7272 656e 745f 6d6f  array(current_mo
+00015a40: 7469 6f6e 5f61 6e67 6c65 2c20 6474 7970  tion_angle, dtyp
+00015a50: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a70: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
+00015a80: 7261 7469 6f6e 203d 206e 702e 6173 6172  ration = np.asar
+00015a90: 7261 7928 6375 7272 656e 745f 6163 6365  ray(current_acce
+00015aa0: 6c65 7261 7469 6f6e 2c20 6474 7970 653d  leration, dtype=
+00015ab0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
+00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
+00015ae0: 5f63 656c 6c5f 6d61 736b 203d 206e 702e  _cell_mask = np.
+00015af0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00015b00: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00015b10: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
+00015b20: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00015b30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00015b40: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
+00015b50: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00015b60: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00015b70: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00015b80: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00015b90: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00015ba0: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
+00015bb0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00015bc0: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
+00015bd0: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
+00015be0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00015bf0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00015c00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00015c10: 7572 7265 6e74 5f74 7261 636b 5f64 6973  urrent_track_dis
+00015c20: 706c 6163 656d 656e 7420 3d20 6e70 2e61  placement = np.a
+00015c30: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
+00015c40: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+00015c50: 742c 2064 7479 7065 3d6e 702e 666c 6f61  t, dtype=np.floa
+00015c60: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00015c70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00015c80: 5f74 6f74 616c 5f74 7261 636b 5f64 6973  _total_track_dis
+00015c90: 7461 6e63 6520 3d20 6e70 2e61 7361 7272  tance = np.asarr
+00015ca0: 6179 2863 7572 7265 6e74 5f74 6f74 616c  ay(current_total
+00015cb0: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
+00015cc0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00015cd0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00015ce0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
+00015cf0: 6178 5f74 7261 636b 5f64 6973 7461 6e63  ax_track_distanc
+00015d00: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
+00015d10: 7572 7265 6e74 5f6d 6178 5f74 7261 636b  urrent_max_track
+00015d20: 5f64 6973 7461 6e63 652c 2064 7479 7065  _distance, dtype
+00015d30: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d50: 2063 7572 7265 6e74 5f74 7261 636b 5f64   current_track_d
+00015d60: 7572 6174 696f 6e20 3d20 6e70 2e61 7361  uration = np.asa
+00015d70: 7272 6179 2863 7572 7265 6e74 5f74 7261  rray(current_tra
+00015d80: 636b 5f64 7572 6174 696f 6e2c 2064 7479  ck_duration, dty
+00015d90: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+00015da0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00015db0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015dc0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015de0: 2069 6620 706f 696e 745f 7361 6d70 6c65   if point_sample
+00015df0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00015e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e10: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
+00015e20: 203d 2066 6674 6672 6571 2870 6f69 6e74   = fftfreq(point
+00015e30: 5f73 616d 706c 652c 2073 656c 662e 7463  _sample, self.tc
+00015e40: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e60: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00015e70: 7374 7269 705f 7361 6d70 6c65 203d 2066  strip_sample = f
+00015e80: 6674 2865 7870 616e 6465 645f 696e 7465  ft(expanded_inte
+00015e90: 6e73 6974 7929 0d0a 2020 2020 2020 2020  nsity)..        
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015eb0: 2020 2020 2020 2020 6666 7474 6f74 616c          ffttotal
+00015ec0: 5f73 616d 706c 6520 3d20 6e70 2e61 6273  _sample = np.abs
+00015ed0: 2866 6674 7374 7269 705f 7361 6d70 6c65  (fftstrip_sample
+00015ee0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f00: 2020 2078 665f 7361 6d70 6c65 203d 2078     xf_sample = x
+00015f10: 665f 7361 6d70 6c65 5b30 203a 206c 656e  f_sample[0 : len
+00015f20: 2878 665f 7361 6d70 6c65 2920 2f2f 2032  (xf_sample) // 2
+00015f30: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
+00015f60: 6c65 203d 2066 6674 746f 7461 6c5f 7361  le = ffttotal_sa
+00015f70: 6d70 6c65 5b30 203a 206c 656e 2866 6674  mple[0 : len(fft
+00015f80: 746f 7461 6c5f 7361 6d70 6c65 2920 2f2f  total_sample) //
+00015f90: 2032 5d0d 0a0d 0a20 2020 2020 2020 2020   2]....         
+00015fa0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00015fb0: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
+00015fc0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00015fd0: 5f75 6e69 7175 655f 6964 5d20 3d20 6578  _unique_id] = ex
+00015fe0: 7061 6e64 6564 5f74 696d 652c 2065 7870  panded_time, exp
+00015ff0: 616e 6465 645f 696e 7465 6e73 6974 792c  anded_intensity,
+00016000: 2078 665f 7361 6d70 6c65 2c20 6666 7474   xf_sample, fftt
+00016010: 6f74 616c 5f73 616d 706c 650d 0a20 2020  otal_sample..   
+00016020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016030: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
+00016040: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00016050: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00016060: 655f 6964 5d20 3d20 2063 7572 7265 6e74  e_id] =  current
+00016070: 5f74 696d 650d 0a20 2020 2020 2020 2020  _time..         
+00016080: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00016090: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+000160a0: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+000160b0: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
+000160c0: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
+000160d0: 7272 656e 745f 7a2c 2063 7572 7265 6e74  rrent_z, current
+000160e0: 5f79 2c20 6375 7272 656e 745f 782c 2063  _y, current_x, c
+000160f0: 7572 7265 6e74 5f72 6164 6975 732c 2063  urrent_radius, c
+00016100: 7572 7265 6e74 5f76 6f6c 756d 652c 2063  urrent_volume, c
+00016110: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00016120: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
+00016130: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00016140: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00016150: 2c20 6375 7272 656e 745f 7375 7266 6163  , current_surfac
+00016160: 655f 6172 6561 0d0a 2020 2020 2020 2020  e_area..        
+00016170: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00016180: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
+00016190: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+000161a0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+000161b0: 203d 2063 7572 7265 6e74 5f74 696d 652c   = current_time,
+000161c0: 2063 7572 7265 6e74 5f73 7065 6564 2c20   current_speed, 
+000161d0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+000161e0: 6e67 6c65 2c20 6375 7272 656e 745f 6163  ngle, current_ac
+000161f0: 6365 6c65 7261 7469 6f6e 2c20 6375 7272  celeration, curr
+00016200: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00016210: 6c5f 6d61 736b 2c20 6375 7272 656e 745f  l_mask, current_
+00016220: 7261 6469 616c 5f61 6e67 6c65 2c20 6375  radial_angle, cu
+00016230: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
+00016240: 6d61 736b 2c20 6375 7272 656e 745f 7472  mask, current_tr
+00016250: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
+00016260: 2c20 6375 7272 656e 745f 746f 7461 6c5f  , current_total_
+00016270: 7472 6163 6b5f 6469 7374 616e 6365 2c20  track_distance, 
+00016280: 6375 7272 656e 745f 6d61 785f 7472 6163  current_max_trac
+00016290: 6b5f 6469 7374 616e 6365 2c20 6375 7272  k_distance, curr
+000162a0: 656e 745f 7472 6163 6b5f 6475 7261 7469  ent_track_durati
+000162b0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000162c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000162d0: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+000162e0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
+000162f0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
+00016300: 7565 5f69 643a 756e 6971 7565 5f66 6674  ue_id:unique_fft
+00016310: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00016320: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00016330: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
+00016340: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016350: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
+00016360: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
+00016370: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+00016380: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00016390: 3a75 6e69 7175 655f 636c 7573 7465 725f  :unique_cluster_
+000163a0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+000163b0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+000163c0: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
+000163d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000163e0: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
+000163f0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+00016400: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
+00016410: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
+00016420: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00016430: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00016440: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+00016450: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
+00016460: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00016470: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+00016480: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00016490: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
+000164a0: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
+000164b0: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+000164c0: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+000164d0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+000164e0: 645d 7d29 0d0a 0d0a 2020 2020 6465 6620  d]})....    def 
+000164f0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+00016500: 7370 6f74 7328 7365 6c66 2c20 6672 616d  spots(self, fram
+00016510: 652c 207a 2c20 792c 2078 2c20 6365 6c6c  e, z, y, x, cell
+00016520: 5f69 642c 2074 7261 636b 5f69 6429 3a0d  _id, track_id):.
+00016530: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+00016540: 2020 2020 2020 2020 2020 7472 6565 2c20            tree, 
+00016550: 6365 6e74 726f 6964 732c 206c 6162 656c  centroids, label
+00016560: 732c 2076 6f6c 756d 652c 2069 6e74 656e  s, volume, inten
+00016570: 7369 7479 5f6d 6561 6e2c 2069 6e74 656e  sity_mean, inten
+00016580: 7369 7479 5f74 6f74 616c 2c20 626f 756e  sity_total, boun
+00016590: 6469 6e67 5f62 6f78 6573 203d 2073 656c  ding_boxes = sel
+000165a0: 662e 5f74 696d 6564 5f63 6861 6e6e 656c  f._timed_channel
+000165b0: 5f73 6567 5f69 6d61 6765 5b73 7472 2869  _seg_image[str(i
+000165c0: 6e74 2866 6c6f 6174 2866 7261 6d65 2929  nt(float(frame))
+000165d0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+000165e0: 7069 7865 6c74 6573 746c 6f63 6174 696f  pixeltestlocatio
+000165f0: 6e20 3d20 287a 2c79 2c78 290d 0a20 2020  n = (z,y,x)..   
+00016600: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
+00016610: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
+00016620: 7928 7069 7865 6c74 6573 746c 6f63 6174  y(pixeltestlocat
+00016630: 696f 6e29 0d0a 0d0a 0d0a 2020 2020 2020  ion)......      
+00016640: 2020 2020 2020 6262 6f78 203d 2062 6f75        bbox = bou
+00016650: 6e64 696e 675f 626f 7865 735b 696e 6465  nding_boxes[inde
+00016660: 785d 0d0a 2020 2020 2020 2020 2020 2020  x]..            
+00016670: 7369 7a65 7a20 3d20 6162 7328 6262 6f78  sizez = abs(bbox
+00016680: 5b30 5d20 2d20 6262 6f78 5b33 5d29 0d0a  [0] - bbox[3])..
+00016690: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+000166a0: 7920 3d20 6162 7328 6262 6f78 5b31 5d20  y = abs(bbox[1] 
+000166b0: 2d20 6262 6f78 5b34 5d29 0d0a 2020 2020  - bbox[4])..    
+000166c0: 2020 2020 2020 2020 7369 7a65 7820 3d20          sizex = 
+000166d0: 6162 7328 6262 6f78 5b32 5d20 2d20 6262  abs(bbox[2] - bb
+000166e0: 6f78 5b35 5d29 200d 0a20 2020 2020 2020  ox[5]) ..       
+000166f0: 2020 2020 2076 6574 6f5f 766f 6c75 6d65       veto_volume
+00016700: 203d 2073 697a 6578 202a 2073 697a 6579   = sizex * sizey
+00016710: 202a 2073 697a 657a 0d0a 2020 2020 2020   * sizez..      
+00016720: 2020 2020 2020 7665 746f 5f72 6164 6975        veto_radiu
+00016730: 7320 3d20 6d61 7468 2e70 6f77 2833 202a  s = math.pow(3 *
+00016740: 2076 6574 6f5f 766f 6c75 6d65 202f 2028   veto_volume / (
+00016750: 3420 2a20 6d61 7468 2e70 6929 2c20 312e  4 * math.pi), 1.
+00016760: 3020 2f20 332e 3029 0d0a 0d0a 2020 2020  0 / 3.0)....    
+00016770: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
+00016780: 203d 2028 6365 6e74 726f 6964 735b 696e   = (centroids[in
+00016790: 6465 785d 5b30 5d20 2a20 7365 6c66 2e7a  dex][0] * self.z
+000167a0: 6361 6c69 6272 6174 696f 6e2c 2063 656e  calibration, cen
+000167b0: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
+000167c0: 2a73 656c 662e 7963 616c 6962 7261 7469  *self.ycalibrati
+000167d0: 6f6e 2c20 6365 6e74 726f 6964 735b 696e  on, centroids[in
+000167e0: 6465 785d 5b32 5d2a 7365 6c66 2e78 6361  dex][2]*self.xca
+000167f0: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
+00016800: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
+00016810: 3d20 6d61 7468 2e70 6f77 2876 6f6c 756d  = math.pow(volum
+00016820: 655b 696e 6465 785d 2c20 312e 302f 332e  e[index], 1.0/3.
+00016830: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00016840: 5241 4449 5553 203d 206d 6174 682e 706f  RADIUS = math.po
+00016850: 7728 766f 6c75 6d65 5b69 6e64 6578 5d20  w(volume[index] 
+00016860: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
+00016870: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
+00016880: 6272 6174 696f 6e20 2a20 7365 6c66 2e7a  bration * self.z
+00016890: 6361 6c69 6272 6174 696f 6e2c 2031 2e30  calibration, 1.0
+000168a0: 2f33 2e30 2920 0d0a 0d0a 2020 2020 2020  /3.0) ....      
+000168b0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+000168c0: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
+000168d0: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
+000168e0: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
+000168f0: 2866 7261 6d65 2c20 6c6f 6361 7469 6f6e  (frame, location
+00016900: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00016910: 6620 6469 7374 203c 3d20 3220 2a20 7665  f dist <= 2 * ve
+00016920: 746f 5f72 6164 6975 733a 0d0a 2020 2020  to_radius:..    
+00016930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016940: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+00016950: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016960: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+00016970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016980: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+00016990: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
+000169a0: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
+000169b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000169c0: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
+000169d0: 3a20 696e 7428 6672 616d 6529 2c0d 0a20  : int(frame),.. 
+000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169f0: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
+00016a00: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+00016a10: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00016a20: 305d 2a20 7365 6c66 2e7a 6361 6c69 6272  0]* self.zcalibr
+00016a30: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+00016a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a50: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
+00016a60: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
+00016a70: 6473 5b69 6e64 6578 5d5b 315d 2a20 7365  ds[index][1]* se
+00016a80: 6c66 2e79 6361 6c69 6272 6174 696f 6e29  lf.ycalibration)
+00016a90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00016aa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016ab0: 7870 6f73 6964 5f6b 6579 203a 2066 6c6f  xposid_key : flo
+00016ac0: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
+00016ad0: 6578 5d5b 325d 2a20 7365 6c66 2e78 6361  ex][2]* self.xca
+00016ae0: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
+00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b00: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+00016b10: 645f 6b65 793a 2069 6e74 2874 7261 636b  d_key: int(track
+00016b20: 5f69 6429 2c0d 0a20 2020 2020 2020 2020  _id),..         
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016b40: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+00016b50: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
+00016b60: 2869 6e74 656e 7369 7479 5f74 6f74 616c  (intensity_total
+00016b70: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
+00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b90: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
+00016ba0: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
+00016bb0: 6c6f 6174 2869 6e74 656e 7369 7479 5f6d  loat(intensity_m
+00016bc0: 6561 6e5b 696e 6465 785d 2929 2c0d 0a20  ean[index])),.. 
+00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016be0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00016bf0: 7573 5f6b 6579 203a 2028 666c 6f61 7428  us_key : (float(
+00016c00: 5241 4449 5553 2929 2c0d 0a20 2020 2020  RADIUS)),..     
+00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c20: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+00016c30: 6b65 7920 3a20 2866 6c6f 6174 2851 5541  key : (float(QUA
+00016c40: 4c49 5459 2929 2c0d 0a20 2020 2020 2020  LITY)),..       
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
+00016c70: 656c 6c5f 6d61 736b 5f6b 6579 3a20 666c  ell_mask_key: fl
+00016c80: 6f61 7428 6469 7374 616e 6365 5f63 656c  oat(distance_cel
+00016c90: 6c5f 6d61 736b 292c 0d0a 2020 2020 2020  l_mask),..      
+00016ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016cb0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+00016cc0: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
+00016cd0: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
+00016ce0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00016cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016d00: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
+00016d10: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+00016d20: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d40: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
+00016d50: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
+00016d60: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
+00016d70: 645b 325d 2920 0d0a 0d0a 2020 2020 2020  d[2]) ....      
+00016d80: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+00016d90: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00016dc0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00016dd0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00016de0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+00016df0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00016e00: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
+00016e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016e20: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00016e30: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016e40: 5b63 656c 6c5f 6964 5d2e 7570 6461 7465  [cell_id].update
+00016e50: 287b 7365 6c66 2e74 6f74 616c 5f69 6e74  ({self.total_int
+00016e60: 656e 7369 7479 5f6b 6579 3a20 2d31 7d29  ensity_key: -1})
+00016e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016e80: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
+00016e90: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+00016ea0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+00016eb0: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00016ec0: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
+00016ed0: 6579 3a20 2d31 7d29 0d0a 2020 2020 2020  ey: -1})..      
+00016ee0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016ef0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00016f00: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016f10: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
+00016f20: 6528 7b73 656c 662e 7261 6469 7573 5f6b  e({self.radius_k
+00016f30: 6579 3a20 2d31 7d29 0d0a 2020 2020 2020  ey: -1})..      
+00016f40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016f50: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00016f60: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016f70: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
+00016f80: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
+00016f90: 6b65 793a 202d 317d 290d 0a0d 0a0d 0a0d  key: -1}).......
+00016fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fc0: 2020 0d0a 2020 2020 6465 6620 5f64 6963    ..    def _dic
+00016fd0: 745f 7570 6461 7465 2873 656c 662c 2075  t_update(self, u
+00016fe0: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
+00016ff0: 6473 3a20 4c69 7374 2c20 2063 656c 6c5f  ds: List,  cell_
+00017000: 6964 3a20 696e 742c 2074 7261 636b 5f69  id: int, track_i
+00017010: 643a 2069 6e74 2c20 736f 7572 6365 5f69  d: int, source_i
+00017020: 643a 2069 6e74 2c20 7461 7267 6574 5f69  d: int, target_i
+00017030: 643a 2069 6e74 293a 0d0a 0d0a 200d 0a20  d: int):.... .. 
+00017040: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
+00017050: 6e5f 6964 203d 2073 656c 662e 6765 6e65  n_id = self.gene
+00017060: 7261 7469 6f6e 5f64 6963 745b 6365 6c6c  ration_dict[cell
+00017070: 5f69 645d 0d0a 2020 2020 2020 2020 7472  _id]..        tr
+00017080: 6163 6b6c 6574 5f69 6420 3d20 7365 6c66  acklet_id = self
+00017090: 2e74 7261 636b 6c65 745f 6469 6374 5b63  .tracklet_dict[c
+000170a0: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
+000170b0: 0d0a 0d0a 2020 2020 2020 2020 756e 6971  ....        uniq
+000170c0: 7565 5f69 6420 3d20 7374 7228 7472 6163  ue_id = str(trac
+000170d0: 6b5f 6964 2920 2b20 2073 7472 2867 656e  k_id) +  str(gen
+000170e0: 6572 6174 696f 6e5f 6964 2920 2b20 7374  eration_id) + st
+000170f0: 7228 7472 6163 6b6c 6574 5f69 6429 0d0a  r(tracklet_id)..
+00017100: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00017110: 2020 7665 635f 6d61 736b 203d 205b 666c    vec_mask = [fl
+00017120: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00017130: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00017140: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00017150: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00017160: 785f 6b65 795d 292c 2066 6c6f 6174 2873  x_key]), float(s
+00017170: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00017180: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00017190: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
+000171a0: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
+000171b0: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
+000171c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000171d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000171e0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+000171f0: 7472 6f69 645f 7a5f 6b65 795d 2920 5d0d  troid_z_key]) ].
+00017200: 0a0d 0a20 2020 2020 2020 2076 6563 5f63  ...        vec_c
+00017210: 656c 6c20 3d20 5b66 6c6f 6174 2873 656c  ell = [float(sel
+00017220: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00017230: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00017240: 6c5f 6964 295d 5b73 656c 662e 7870 6f73  l_id)][self.xpos
+00017250: 6964 5f6b 6579 5d29 202c 200d 0a20 2020  id_key]) , ..   
+00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017270: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+00017280: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00017290: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000172a0: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
+000172b0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000172d0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+000172e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000172f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00017300: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
+00017310: 706f 7369 645f 6b65 795d 295d 0d0a 0d0a  posid_key])]....
+00017320: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
+00017330: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
+00017340: 6563 5f6d 6173 6b2c 2076 6563 5f63 656c  ec_mask, vec_cel
+00017350: 6c29 0d0a 0d0a 2020 2020 2020 2020 7365  l)....        se
+00017360: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00017370: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00017380: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00017390: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
+000173a0: 655f 6b65 7920 3a20 616e 676c 657d 2920  e_key : angle}) 
+000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173c0: 2020 200d 0a0d 0a20 2020 2020 2020 2075     ....        u
+000173d0: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
+000173e0: 6473 2e61 7070 656e 6428 7374 7228 756e  ds.append(str(un
+000173f0: 6971 7565 5f69 6429 290d 0a20 2020 2020  ique_id))..     
+00017400: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00017410: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00017420: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00017430: 6174 6528 7b73 656c 662e 756e 6971 7565  ate({self.unique
+00017440: 6964 5f6b 6579 203a 2073 7472 2875 6e69  id_key : str(uni
+00017450: 7175 655f 6964 297d 290d 0a20 2020 2020  que_id)})..     
+00017460: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00017470: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00017480: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00017490: 6174 6528 7b73 656c 662e 7472 6163 6b6c  ate({self.trackl
+000174a0: 6574 6964 5f6b 6579 203a 2073 7472 2874  etid_key : str(t
+000174b0: 7261 636b 6c65 745f 6964 297d 2920 0d0a  racklet_id)}) ..
+000174c0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000174d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000174e0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+000174f0: 5d2e 7570 6461 7465 287b 7365 6c66 2e67  ].update({self.g
+00017500: 656e 6572 6174 696f 6e69 645f 6b65 7920  enerationid_key 
+00017510: 3a20 7374 7228 6765 6e65 7261 7469 6f6e  : str(generation
+00017520: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
+00017530: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00017540: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00017550: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00017560: 6528 7b73 656c 662e 7472 6163 6b69 645f  e({self.trackid_
+00017570: 6b65 7920 3a20 7374 7228 7472 6163 6b5f  key : str(track_
+00017580: 6964 297d 290d 0a20 2020 2020 2020 2073  id)})..        s
+00017590: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000175a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000175b0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000175c0: 7b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  {self.motion_ang
+000175d0: 6c65 5f6b 6579 203a 2030 2e30 7d29 0d0a  le_key : 0.0})..
+000175e0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000175f0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017600: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00017610: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00017620: 7065 6564 5f6b 6579 203a 2030 2e30 7d29  peed_key : 0.0})
+00017630: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00017640: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00017650: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00017660: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00017670: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+00017680: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
+00017690: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+000176a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000176b0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+000176c0: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
+000176d0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+000176e0: 746b 6579 203a 202d 317d 290d 0a20 2020  tkey : -1})..   
+000176f0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00017700: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00017710: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00017720: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
+00017730: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+00017740: 636f 6e64 6b65 7920 3a20 2d31 7d29 0d0a  condkey : -1})..
+00017750: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00017760: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017770: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00017780: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
+00017790: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
+000177a0: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
+000177b0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000177c0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000177d0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000177e0: 287b 7365 6c66 2e63 656c 6c61 7869 735f  ({self.cellaxis_
+000177f0: 6d61 736b 5f6b 6579 203a 202d 317d 290d  mask_key : -1}).
+00017800: 0a0d 0a20 2020 2020 2020 2069 6620 736f  ...        if so
+00017810: 7572 6365 5f69 6420 6973 206e 6f74 204e  urce_id is not N
+00017820: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00017830: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00017840: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00017850: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00017860: 7465 287b 7365 6c66 2e62 6566 6f72 6569  te({self.beforei
+00017870: 645f 6b65 7920 3a20 696e 7428 736f 7572  d_key : int(sour
+00017880: 6365 5f69 6429 7d29 0d0a 2020 2020 2020  ce_id)})..      
+00017890: 2020 2020 2020 7665 635f 3120 3d20 5b66        vec_1 = [f
+000178a0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000178b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000178c0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000178d0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+000178e0: 202d 2066 6c6f 6174 2873 656c 662e 756e   - float(self.un
+000178f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00017900: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+00017910: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+00017920: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
+00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017940: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
+00017950: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00017960: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00017970: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
+00017980: 645f 6b65 795d 2920 2d20 666c 6f61 7428  d_key]) - float(
+00017990: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000179a0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000179b0: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
+000179c0: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
+000179d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179e0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+000179f0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00017a00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00017a10: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00017a20: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
+00017a30: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
+00017a40: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017a50: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00017a60: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00017a70: 6b65 795d 295d 0d0a 2020 2020 2020 2020  key])]..        
+00017a80: 2020 2020 7370 6565 6420 3d20 6e70 2e73      speed = np.s
+00017a90: 7172 7428 6e70 2e64 6f74 2876 6563 5f31  qrt(np.dot(vec_1
+00017aa0: 2c20 7665 635f 3129 292f 7365 6c66 2e74  , vec_1))/self.t
+00017ab0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00017ac0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00017ad0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00017ae0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00017af0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00017b00: 7370 6565 645f 6b65 7920 3a20 7370 6565  speed_key : spee
+00017b10: 647d 290d 0a0d 0a20 2020 2020 2020 2020  d})....         
+00017b20: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
+00017b30: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
+00017b40: 2876 6563 5f6d 6173 6b2c 2076 6563 5f31  (vec_mask, vec_1
+00017b50: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00017b60: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00017b70: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00017b80: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00017b90: 6528 7b73 656c 662e 6d6f 7469 6f6e 5f61  e({self.motion_a
+00017ba0: 6e67 6c65 5f6b 6579 203a 206d 6f74 696f  ngle_key : motio
+00017bb0: 6e5f 616e 676c 657d 2920 0d0a 0d0a 2020  n_angle}) ....  
+00017bc0: 2020 2020 2020 2020 2020 6966 2073 6f75            if sou
+00017bd0: 7263 655f 6964 2069 6e20 7365 6c66 2e65  rce_id in self.e
+00017be0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+00017bf0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
+00017c00: 2020 2020 2020 2020 7072 655f 736f 7572          pre_sour
+00017c10: 6365 5f69 6420 3d20 7365 6c66 2e65 6467  ce_id = self.edg
+00017c20: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
+00017c30: 736f 7572 6365 5f69 645d 0d0a 2020 2020  source_id]..    
+00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017c60: 2020 2020 2020 7665 635f 3220 3d20 5b66        vec_2 = [f
+00017c70: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00017c80: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00017c90: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00017ca0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00017cb0: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
+00017cc0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00017cd0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00017ce0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
+00017cf0: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
+00017d00: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00017d10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00017d20: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
+00017d30: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00017d40: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
+00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d60: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
+00017d70: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00017d80: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00017d90: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
+00017da0: 6b65 795d 2920 2d20 3220 2a20 666c 6f61  key]) - 2 * floa
+00017db0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00017dc0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00017dd0: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+00017de0: 6c66 2e79 706f 7369 645f 6b65 795d 2920  lf.yposid_key]) 
+00017df0: 2b20 666c 6f61 7428 7365 6c66 2e75 6e69  + float(self.uni
+00017e00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017e10: 6965 735b 696e 7428 7072 655f 736f 7572  ies[int(pre_sour
+00017e20: 6365 5f69 6429 5d5b 7365 6c66 2e79 706f  ce_id)][self.ypo
+00017e30: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e50: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+00017e60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00017e70: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00017e80: 656c 6c5f 6964 295d 5b73 656c 662e 7a70  ell_id)][self.zp
+00017e90: 6f73 6964 5f6b 6579 5d29 202d 2020 3220  osid_key]) -  2 
+00017ea0: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
+00017eb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017ec0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+00017ed0: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00017ee0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
+00017ef0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00017f00: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
+00017f10: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
+00017f20: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
+00017f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017f40: 2020 2020 2020 6163 6320 3d20 6e70 2e73        acc = np.s
+00017f50: 7172 7428 6e70 2e64 6f74 2876 6563 5f32  qrt(np.dot(vec_2
+00017f60: 2c20 7665 635f 3229 292f 7365 6c66 2e74  , vec_2))/self.t
+00017f70: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017fa0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00017fb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00017fc0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00017fd0: 2e75 7064 6174 6528 7b73 656c 662e 6163  .update({self.ac
+00017fe0: 6365 6c65 7261 7469 6f6e 5f6b 6579 203a  celeration_key :
+00017ff0: 2061 6363 7d29 0d0a 2020 2020 2020 2020   acc})..        
+00018000: 656c 6966 2073 6f75 7263 655f 6964 2069  elif source_id i
+00018010: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00018020: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00018030: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00018040: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00018050: 7064 6174 6528 7b73 656c 662e 6265 666f  pdate({self.befo
+00018060: 7265 6964 5f6b 6579 203a 204e 6f6e 657d  reid_key : None}
+00018070: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
+00018080: 0d0a 0d0a 2020 2020 2020 2020 6966 2074  ....        if t
+00018090: 6172 6765 745f 6964 2069 7320 6e6f 7420  arget_id is not 
+000180a0: 4e6f 6e65 3a20 2020 2020 2020 0d0a 2020  None:       ..  
+000180b0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000180c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000180d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000180e0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000180f0: 2e61 6674 6572 6964 5f6b 6579 203a 2069  .afterid_key : i
+00018100: 6e74 2874 6172 6765 745f 6964 297d 2920  nt(target_id)}) 
+00018110: 0d0a 2020 2020 2020 2020 656c 6966 2074  ..        elif t
+00018120: 6172 6765 745f 6964 2069 7320 4e6f 6e65  arget_id is None
+00018130: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00018140: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00018150: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00018160: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00018170: 7b73 656c 662e 6166 7465 7269 645f 6b65  {self.afterid_ke
+00018180: 7920 3a20 4e6f 6e65 7d29 0d0a 2020 2020  y : None})..    
+00018190: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000181a0: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
+000181b0: 6861 6e6e 656c 5f75 7064 6174 6528 6365  hannel_update(ce
+000181c0: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
+000181d0: 2020 2020 0d0a 0d0a 0d0a 2020 2020 6465      ......    de
+000181e0: 6620 5f74 656d 706f 7261 6c5f 706c 6f74  f _temporal_plot
+000181f0: 735f 7472 6163 6b6d 6174 6528 7365 6c66  s_trackmate(self
+00018200: 293a 0d0a 2020 2020 0d0a 2020 2020 0d0a  ):..    ..    ..
+00018210: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00018220: 2020 2020 2020 7365 6c66 2e41 7474 7220        self.Attr 
+00018230: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00018240: 2020 2020 2020 7374 6172 7474 696d 6520        starttime 
+00018250: 3d20 696e 7428 6d69 6e28 7365 6c66 2e41  = int(min(self.A
+00018260: 6c6c 5661 6c75 6573 5b73 656c 662e 6672  llValues[self.fr
+00018270: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+00018280: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00018290: 6474 696d 6520 3d20 696e 7428 6d61 7828  dtime = int(max(
+000182a0: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
+000182b0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+000182c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000182d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000182e0: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
 000182f0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00018300: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018310: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00018320: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018340: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00018350: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018360: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00018370: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018390: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
-000183a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000183b0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-000183c0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-000183d0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000183e0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018400: 2020 616c 6c5f 7261 6469 7573 203d 205b    all_radius = [
-00018410: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00018420: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
-00018430: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00018440: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-00018450: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00018460: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00018470: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018480: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00018490: 2020 2020 2020 2020 2020 2020 2020 616c                al
-000184a0: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-000184b0: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a0d  mask = [].......
-000184c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000184d0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-000184e0: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
-000184f0: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
-00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018510: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018530: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00018540: 5f74 696d 6520 3d20 616c 6c5f 7370 6f74  _time = all_spot
-00018550: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018560: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
-00018570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018580: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00018590: 6963 203d 2061 6c6c 5f73 706f 7473 5f74  ic = all_spots_t
-000185a0: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-000185b0: 7669 6469 6e67 5f6b 6579 5d0d 0a20 2020  viding_key]..   
-000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185f0: 2020 2020 2020 6966 2069 203d 3d20 696e        if i == in
-00018600: 7428 6375 7272 656e 745f 7469 6d65 293a  t(current_time):
-00018610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018630: 2020 2020 6966 206d 6974 6f74 6963 3a0d      if mitotic:.
-00018640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018660: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00018670: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
-00018680: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00018690: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
-000186a0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186c0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000186d0: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
-000186e0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000186f0: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
-00018700: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018730: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00018740: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
-00018750: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018760: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018790: 2020 2020 2020 2020 6966 2061 6c6c 5f73          if all_s
-000187a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000187b0: 656c 662e 7261 6469 7573 5f6b 6579 5d20  elf.radius_key] 
-000187c0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 206d 6974 6f74 6963 5f72 6164 6975 732e   mitotic_radius.
-00018800: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018810: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018820: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018850: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00018860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018880: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00018890: 7261 6469 7573 2e61 7070 656e 6428 4e6f  radius.append(No
-000188a0: 6e65 2920 2020 2020 2020 0d0a 2020 2020  ne)       ..    
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188d0: 2020 2020 6d69 746f 7469 635f 7370 6565      mitotic_spee
-000188e0: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-000188f0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018900: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018930: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
-00018940: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00018950: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00018960: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00018970: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018990: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000189a0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-000189b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000189c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000189d0: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-000189e0: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a10: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00018a20: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018a30: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018a40: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018a50: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-00018a60: 6173 6b5f 6b65 795d 290d 0a0d 0a0d 0a20  ask_key])...... 
-00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
-00018aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ac0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018ad0: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
-00018ae0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00018af0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
-00018b00: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b30: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00018b40: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
-00018b50: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00018b60: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00018b70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00018ba0: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
-00018bb0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018bc0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
-00018bd0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c00: 2020 2020 2069 6620 616c 6c5f 7370 6f74       if all_spot
-00018c10: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018c20: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
-00018c30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00018c60: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
-00018c70: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00018c80: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018c90: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cc0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018300: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018310: 7469 635f 6d65 616e 5f64 6973 705f 7a20  tic_mean_disp_z 
+00018320: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00018330: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018340: 6963 5f76 6172 5f64 6973 705f 7a20 3d20  ic_var_disp_z = 
+00018350: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00018360: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018370: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
+00018380: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00018390: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000183a0: 635f 7661 725f 6469 7370 5f79 203d 205b  c_var_disp_y = [
+000183b0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000183c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000183d0: 635f 6d65 616e 5f64 6973 705f 7820 3d20  c_mean_disp_x = 
+000183e0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000183f0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018400: 5f76 6172 5f64 6973 705f 7820 3d20 5b5d  _var_disp_x = []
+00018410: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018420: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018430: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
+00018440: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00018450: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018460: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
+00018470: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018480: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018490: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
+000184a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000184b0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+000184c0: 725f 7370 6565 6420 3d20 5b5d 0d0a 0d0a  r_speed = []....
+000184d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184e0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+000184f0: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
+00018500: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018510: 2e6d 6974 6f74 6963 5f76 6172 5f61 6363  .mitotic_var_acc
+00018520: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00018530: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018540: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
+00018550: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00018560: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00018570: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018580: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+00018590: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 0d0a  _change = []....
+000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185b0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+000185c0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+000185d0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
+000185e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000185f0: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
+00018600: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00018610: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00018620: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018630: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018640: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
+00018650: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00018660: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00018670: 6973 705f 7a20 3d20 5b5d 0d0a 0d0a 2020  isp_z = []....  
+00018680: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018690: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000186a0: 6561 6e5f 6469 7370 5f79 203d 205b 5d0d  ean_disp_y = [].
+000186b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000186c0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000186d0: 635f 7661 725f 6469 7370 5f79 203d 205b  c_var_disp_y = [
+000186e0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000186f0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018700: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00018710: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00018720: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018730: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00018740: 705f 7820 3d20 5b5d 0d0a 0d0a 2020 2020  p_x = []....    
+00018750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018760: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00018770: 6e5f 7261 6469 7573 203d 205b 5d0d 0a20  n_radius = [].. 
+00018780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018790: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000187a0: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
+000187b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000187c0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000187d0: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
+000187e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000187f0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018800: 746f 7469 635f 7661 725f 7370 6565 6420  totic_var_speed 
+00018810: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00018820: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018830: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6163  _mitotic_mean_ac
+00018840: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+00018850: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018860: 5f6d 6974 6f74 6963 5f76 6172 5f61 6363  _mitotic_var_acc
+00018870: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00018880: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018890: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+000188a0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+000188b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+000188c0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000188d0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6972  _mitotic_var_dir
+000188e0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+000188f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00018900: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018910: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00018920: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018930: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018940: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018950: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
+00018960: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00018970: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00018980: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018990: 6d65 616e 5f64 6973 705f 7a20 3d20 5b5d  mean_disp_z = []
+000189a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000189b0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+000189c0: 6973 705f 7a20 3d20 5b5d 0d0a 0d0a 2020  isp_z = []....  
+000189d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000189e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+000189f0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00018a00: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018a10: 6c5f 7661 725f 6469 7370 5f79 203d 205b  l_var_disp_y = [
+00018a20: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00018a30: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00018a40: 616e 5f64 6973 705f 7820 3d20 5b5d 0d0a  an_disp_x = []..
+00018a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a60: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018a70: 705f 7820 3d20 5b5d 0d0a 0d0a 2020 2020  p_x = []....    
+00018a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018a90: 2e61 6c6c 5f6d 6561 6e5f 7261 6469 7573  .all_mean_radius
+00018aa0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018ab0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018ac0: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
+00018ad0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018ae0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00018af0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00018b00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018b10: 662e 616c 6c5f 7661 725f 7370 6565 6420  f.all_var_speed 
+00018b20: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00018b30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018b40: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
+00018b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b60: 7365 6c66 2e61 6c6c 5f76 6172 5f61 6363  self.all_var_acc
+00018b70: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00018b80: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00018b90: 6c5f 6d65 616e 5f64 6972 6563 7469 6f6e  l_mean_direction
+00018ba0: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bc0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
+00018bd0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00018be0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00018bf0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018c00: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+00018c10: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
+00018c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018c30: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
+00018c40: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00018c50: 205b 5d0d 0a0d 0a0d 0a20 2020 2020 2020   []......       
+00018c60: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
+00018c70: 7473 5f74 7261 636b 7320 3d20 7b7d 0d0a  ts_tracks = {}..
+00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c90: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
+00018ca0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00018cb0: 6f70 6572 7469 6573 2e69 7465 6d73 2829  operties.items()
+00018cc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018cd0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018d00: 6974 6f74 6963 5f72 6164 6975 732e 6170  itotic_radius.ap
-00018d10: 7065 6e64 284e 6f6e 6529 2020 2020 2020  pend(None)      
-00018d20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d40: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018d50: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
-00018d60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018d70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018d80: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
-00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018db0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00018dc0: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
-00018dd0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00018de0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-00018df0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
-00018e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e20: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
-00018e30: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00018e40: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018e50: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018e60: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00018e70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00018e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e90: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00018ea0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00018eb0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-00018ec0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00018ed0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
-00018ee0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00018ef0: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
-00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f10: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00018f20: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
-00018f30: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00018f40: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00018f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f70: 2020 2020 616c 6c5f 6469 7370 5f79 2e61      all_disp_y.a
-00018f80: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018f90: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
-00018fa0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00018fd0: 6c6c 5f64 6973 705f 782e 6170 7065 6e64  ll_disp_x.append
-00018fe0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00018ff0: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
-00019000: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019020: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-00019030: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00019040: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
-00019050: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
-00019060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019070: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00019080: 6c5f 7261 6469 7573 2e61 7070 656e 6428  l_radius.append(
-00019090: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000190a0: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
-000190b0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00018cf0: 2061 6c6c 5f73 706f 7473 203d 2073 656c   all_spots = sel
+00018d00: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00018d10: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d30: 2020 2069 6620 7365 6c66 2e74 7261 636b     if self.track
+00018d40: 6964 5f6b 6579 2069 6e20 616c 6c5f 7370  id_key in all_sp
+00018d50: 6f74 733a 0d0a 2020 2020 2020 2020 2020  ots:..          
+00018d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d70: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00018d80: 5b6b 5d20 3d20 616c 6c5f 7370 6f74 730d  [k] = all_spots.
+00018d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018da0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00018db0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00018dc0: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
+00018dd0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00018de0: 2020 2020 2077 6974 6820 636f 6e63 7572       with concur
+00018df0: 7265 6e74 2e66 7574 7572 6573 2e54 6872  rent.futures.Thr
+00018e00: 6561 6450 6f6f 6c45 7865 6375 746f 7228  eadPoolExecutor(
+00018e10: 6d61 785f 776f 726b 6572 7320 3d20 6f73  max_workers = os
+00018e20: 2e63 7075 5f63 6f75 6e74 2829 2920 6173  .cpu_count()) as
+00018e30: 2065 7865 6375 746f 723a 0d0a 2020 2020   executor:..    
+00018e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00018e60: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00018e70: 2074 7164 6d28 7261 6e67 6528 7374 6172   tqdm(range(star
+00018e80: 7474 696d 652c 2065 6e64 7469 6d65 292c  ttime, endtime),
+00018e90: 2074 6f74 616c 3d65 6e64 7469 6d65 202d   total=endtime -
+00018ea0: 2073 7461 7274 7469 6d65 293a 0d0a 2020   starttime):..  
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ec0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00018ed0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+00018ee0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+00018ef0: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+00018f00: 662e 5f63 6f6d 7075 7465 5f74 656d 706f  f._compute_tempo
+00018f10: 7261 6c2c 2069 2c20 616c 6c5f 7370 6f74  ral, i, all_spot
+00018f20: 735f 7472 6163 6b73 2929 0d0a 200d 0a20  s_tracks)).. .. 
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 2020 205b 722e 7265 7375 6c74 2829 2066     [r.result() f
+00018f50: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
+00018f60: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
+00018f70: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
+00018f80: 5d0d 0a0d 0a0d 0a20 2020 2064 6566 205f  ]......    def _
+00018f90: 636f 6d70 7574 655f 7465 6d70 6f72 616c  compute_temporal
+00018fa0: 2873 656c 662c 2069 2c20 616c 6c5f 7370  (self, i, all_sp
+00018fb0: 6f74 735f 7472 6163 6b73 293a 2020 2020  ots_tracks):    
+00018fc0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fe0: 2020 6d69 746f 7469 635f 6469 7370 5f7a    mitotic_disp_z
+00018ff0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00019000: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00019010: 6963 5f64 6973 705f 7920 3d20 5b5d 0d0a  ic_disp_y = []..
+00019020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019030: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00019040: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00019050: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00019060: 6f74 6963 5f72 6164 6975 7320 3d20 5b5d  otic_radius = []
+00019070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019080: 2020 2020 2020 6d69 746f 7469 635f 7370        mitotic_sp
+00019090: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
+000190a0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000190b0: 746f 7469 635f 6163 6320 3d20 5b5d 0d0a  totic_acc = []..
 000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190d0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
-00019110: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
-00019120: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000190d0: 2020 2020 6d69 746f 7469 635f 6469 7265      mitotic_dire
+000190e0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+000190f0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00019100: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00019110: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00019120: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
 00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019140: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
-00019150: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00019160: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00019170: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191a0: 2061 6c6c 5f61 6363 2e61 7070 656e 6428   all_acc.append(
-000191b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000191c0: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-000191d0: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
+00019140: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00019150: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+00019160: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00019170: 5f6d 6974 6f74 6963 5f64 6973 705f 7920  _mitotic_disp_y 
+00019180: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00019190: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+000191a0: 746f 7469 635f 6469 7370 5f78 203d 205b  totic_disp_x = [
+000191b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000191c0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+000191d0: 6963 5f72 6164 6975 7320 3d20 5b5d 0d0a  ic_radius = []..
 000191e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019200: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00019210: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
-00019220: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00019230: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-00019240: 6c65 5f6b 6579 5d29 2020 200d 0a20 2020  le_key])   ..   
-00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019260: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019270: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-00019280: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
-00019290: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-000192a0: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-000192b0: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+000191f0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00019200: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00019210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019220: 6e6f 6e5f 6d69 746f 7469 635f 6163 6320  non_mitotic_acc 
+00019230: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00019240: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00019250: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00019260: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019280: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00019290: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000192a0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
+000192b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000192f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019300: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00019310: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
-00019320: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00019330: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00019340: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00019350: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00019360: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-00019370: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
-00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019390: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
-000193a0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-000193b0: 6628 6d69 746f 7469 635f 6469 7370 5f78  f(mitotic_disp_x
-000193c0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000193d0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-000193e0: 746f 7469 635f 6469 7370 5f7a 203d 206e  totic_disp_z = n
-000193f0: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
-00019400: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00019410: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019420: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00019430: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00019440: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
-00019450: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00019460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019470: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00019480: 635f 6469 7370 5f78 203d 206e 702e 6162  c_disp_x = np.ab
-00019490: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
-000194a0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-000194b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000194c0: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
-000194d0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-000194e0: 6628 616c 6c5f 6469 7370 5f7a 2929 0d0a  f(all_disp_z))..
-000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
-00019510: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00019520: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
-00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 2020 616c 6c5f 6469 7370 5f78 203d 206e    all_disp_x = n
-00019550: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
-00019560: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 0d0a  l_disp_x))......
-00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192d0: 2020 616c 6c5f 6469 7370 5f7a 203d 205b    all_disp_z = [
+000192e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000192f0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00019300: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+00019310: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00019320: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019340: 2061 6c6c 5f72 6164 6975 7320 3d20 5b5d   all_radius = []
+00019350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019360: 2020 2020 2020 616c 6c5f 7370 6565 6420        all_speed 
+00019370: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00019380: 2020 2020 2020 2020 2020 616c 6c5f 6163            all_ac
+00019390: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+000193a0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000193b0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+000193c0: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+000193d0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000193e0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000193f0: 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a 0d0a  ask = []........
+00019400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019410: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+00019420: 696e 2061 6c6c 5f73 706f 7473 5f74 7261  in all_spots_tra
+00019430: 636b 732e 6974 656d 7328 293a 0d0a 2020  cks.items():..  
+00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019450: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019470: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00019480: 7469 6d65 203d 2061 6c6c 5f73 706f 7473  time = all_spots
+00019490: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+000194a0: 6672 616d 6569 645f 6b65 795d 0d0a 2020  frameid_key]..  
+000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000194d0: 6320 3d20 616c 6c5f 7370 6f74 735f 7472  c = all_spots_tr
+000194e0: 6163 6b73 5b6b 5d5b 7365 6c66 2e64 6976  acks[k][self.div
+000194f0: 6964 696e 675f 6b65 795d 0d0a 2020 2020  iding_key]..    
+00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019510: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019530: 2020 2020 2069 6620 6920 3d3d 2069 6e74       if i == int
+00019540: 2863 7572 7265 6e74 5f74 696d 6529 3a0d  (current_time):.
+00019550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019570: 2020 2069 6620 6d69 746f 7469 633a 0d0a     if mitotic:..
 00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019590: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000195a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000195b0: 6c66 2e74 696d 652e 6170 7065 6e64 2869  lf.time.append(i
-000195c0: 202a 2073 656c 662e 7463 616c 6962 7261   * self.tcalibra
-000195d0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
-000195e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000195f0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00019600: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-00019610: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
-00019620: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00019630: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019640: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00019650: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
-00019660: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
-00019670: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
-00019680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019690: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-000196a0: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
-000196b0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
-000196c0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-000196d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000196e0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-000196f0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00019700: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-00019710: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019720: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00019730: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
-00019740: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00019750: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00019760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019770: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00019780: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
-00019790: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-000197a0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000195b0: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
+000195c0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000195d0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+000195e0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019600: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00019610: 6f74 6963 5f64 6973 705f 792e 6170 7065  otic_disp_y.appe
+00019620: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00019630: 636b 735b 6b5d 5b73 656c 662e 7970 6f73  cks[k][self.ypos
+00019640: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019670: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
+00019680: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00019690: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000196a0: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
+000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196d0: 2020 2020 2020 2069 6620 616c 6c5f 7370         if all_sp
+000196e0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000196f0: 6c66 2e72 6164 6975 735f 6b65 795d 203e  lf.radius_key] >
+00019700: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019730: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
+00019740: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00019750: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
+00019760: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
+00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197c0: 2020 2066 696c 7465 7265 645f 7661 6c75     filtered_valu
-000197d0: 6573 203d 205b 7661 6c20 666f 7220 7661  es = [val for va
-000197e0: 6c20 696e 206d 6974 6f74 6963 5f72 6164  l in mitotic_rad
-000197f0: 6975 7320 6966 2076 616c 2069 7320 6e6f  ius if val is no
-00019800: 7420 4e6f 6e65 5d0d 0a20 2020 2020 2020  t None]..       
-00019810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019820: 662e 6d69 746f 7469 635f 6d65 616e 5f72  f.mitotic_mean_r
-00019830: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00019840: 6d65 616e 2866 696c 7465 7265 645f 7661  mean(filtered_va
-00019850: 6c75 6573 2929 0d0a 2020 2020 2020 2020  lues))..        
-00019860: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00019870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019880: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00019890: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
-000198a0: 286e 702e 7374 6428 6669 6c74 6572 6564  (np.std(filtered
-000198b0: 5f76 616c 7565 7329 290d 0a20 2020 2020  _values))..     
-000198c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000198d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000198f0: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
-00019900: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00019910: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00019940: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
-00019950: 702e 7374 6428 6d69 746f 7469 635f 7370  p.std(mitotic_sp
-00019960: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00019970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019980: 662e 6d69 746f 7469 635f 6d65 616e 5f61  f.mitotic_mean_a
-00019990: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-000199a0: 6e28 6d69 746f 7469 635f 6163 6329 290d  n(mitotic_acc)).
-000199b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000199c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000199d0: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
-000199e0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-000199f0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00019a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019a10: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00019a20: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00019a30: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00019a40: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
-00019a50: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
+000197c0: 2020 2020 2020 206d 6974 6f74 6963 5f72         mitotic_r
+000197d0: 6164 6975 732e 6170 7065 6e64 284e 6f6e  adius.append(Non
+000197e0: 6529 2020 2020 2020 200d 0a20 2020 2020  e)       ..     
+000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019810: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
+00019820: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00019830: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00019840: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
+00019850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019870: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
+00019880: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
+00019890: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+000198a0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+000198b0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198d0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000198e0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+000198f0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00019900: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00019910: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
+00019920: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
+00019930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00019960: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00019970: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00019980: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00019990: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000199a0: 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020  sk_key])......  
+000199b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199d0: 6966 206e 6f74 206d 6974 6f74 6963 3a0d  if not mitotic:.
+000199e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00019a10: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
+00019a20: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00019a30: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
+00019a40: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a70: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00019a80: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00019a90: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00019aa0: 2e73 7464 286d 6974 6f74 6963 5f64 6972  .std(mitotic_dir
-00019ab0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00019ac0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019ad0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00019ae0: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
-00019af0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00019b00: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00019b10: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00019b20: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00019b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019b40: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00019b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00019b60: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00019b70: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
-00019b80: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
-00019b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ba0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00019bb0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00019bc0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-00019bd0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00019be0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-00019bf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019c00: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00019c10: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00019c20: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00019c30: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
-00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c50: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00019c60: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-00019c70: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00019c80: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
-00019c90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019ca0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019cb0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00019cc0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-00019cd0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00019ce0: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-00019cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019d00: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019d10: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00019d20: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00019d30: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
+00019a70: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+00019a80: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
+00019a90: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00019aa0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00019ab0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ad0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00019ae0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
+00019af0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00019b00: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+00019b10: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b40: 2020 2020 6966 2061 6c6c 5f73 706f 7473      if all_spots
+00019b50: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00019b60: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
+00019b70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b90: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00019ba0: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
+00019bb0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00019bc0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00019bd0: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
+00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c00: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c30: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00019c40: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
+00019c50: 656e 6428 4e6f 6e65 2920 2020 2020 2020  end(None)       
+00019c60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c80: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00019c90: 5f6d 6974 6f74 6963 5f73 7065 6564 2e61  _mitotic_speed.a
+00019ca0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00019cb0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
+00019cc0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
+00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cf0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00019d00: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+00019d10: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00019d20: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+00019d30: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00019d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d50: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00019d60: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-00019d70: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00019d80: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
-00019d90: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019da0: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
-00019db0: 645f 7661 6c75 6573 203d 205b 7661 6c20  d_values = [val 
-00019dc0: 666f 7220 7661 6c20 696e 206e 6f6e 5f6d  for val in non_m
-00019dd0: 6974 6f74 6963 5f72 6164 6975 7320 6966  itotic_radius if
-00019de0: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
-00019df0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00019e00: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019e10: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
-00019e20: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
-00019e30: 616e 2866 696c 7465 7265 645f 7661 6c75  an(filtered_valu
-00019e40: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
-00019e50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00019e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e70: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00019e80: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00019e90: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
-00019ea0: 6564 5f76 616c 7565 7329 290d 0a0d 0a20  ed_values)).... 
-00019eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ec0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00019ed0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
-00019ee0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00019ef0: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
-00019f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019f10: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019f20: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00019f30: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00019f40: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00019f50: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-00019f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019f70: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00019f80: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-00019f90: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-00019fa0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
-00019fb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019fc0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00019fd0: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-00019fe0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
-00019ff0: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
-0001a000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a010: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-0001a020: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-0001a030: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-0001a040: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-0001a050: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-0001a060: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-0001a070: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-0001a080: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-0001a090: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-0001a0a0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-0001a0b0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-0001a0c0: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
-0001a0d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a0e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-0001a0f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-0001a100: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0001a110: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-0001a120: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-0001a130: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-0001a140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a150: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-0001a160: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
-0001a170: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-0001a180: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-0001a190: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-0001a1a0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
-0001a1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a1c0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-0001a1d0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
-0001a1e0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-0001a1f0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-0001a200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001a210: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
-0001a220: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-0001a230: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
-0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a250: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-0001a260: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-0001a270: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
-0001a280: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001a290: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-0001a2a0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
-0001a2b0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-0001a2c0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-0001a2d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a2e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-0001a2f0: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
-0001a300: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
-0001a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a320: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-0001a330: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-0001a340: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
-0001a350: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0001a360: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
-0001a370: 6564 5f76 616c 7565 7320 3d20 5b76 616c  ed_values = [val
-0001a380: 2066 6f72 2076 616c 2069 6e20 616c 6c5f   for val in all_
-0001a390: 7261 6469 7573 2069 6620 7661 6c20 6973  radius if val is
-0001a3a0: 206e 6f74 204e 6f6e 655d 0d0a 2020 2020   not None]..    
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3c0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
-0001a3d0: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
-0001a3e0: 6561 6e28 6669 6c74 6572 6564 5f76 616c  ean(filtered_val
-0001a3f0: 7565 7329 290d 0a20 2020 2020 2020 2020  ues))..         
-0001a400: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a420: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
-0001a430: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
-0001a440: 7464 2866 696c 7465 7265 645f 7661 6c75  td(filtered_valu
-0001a450: 6573 2929 0d0a 0d0a 2020 2020 2020 2020  es))....        
-0001a460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001a470: 2e61 6c6c 5f6d 6561 6e5f 7370 6565 642e  .all_mean_speed.
-0001a480: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-0001a490: 6c6c 5f73 7065 6564 2929 0d0a 2020 2020  ll_speed))..    
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4b0: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
-0001a4c0: 6564 2e61 7070 656e 6428 6e70 2e73 7464  ed.append(np.std
-0001a4d0: 2861 6c6c 5f73 7065 6564 2929 0d0a 0d0a  (all_speed))....
-0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4f0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-0001a500: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
-0001a510: 6d65 616e 2861 6c6c 5f61 6363 2929 0d0a  mean(all_acc))..
-0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a530: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-0001a540: 5f61 6363 2e61 7070 656e 6428 6e70 2e73  _acc.append(np.s
-0001a550: 7464 2861 6c6c 5f61 6363 2929 0d0a 0d0a  td(all_acc))....
-0001a560: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a570: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-0001a580: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-0001a590: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-0001a5a0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7265  np.mean(all_dire
-0001a5b0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-0001a5c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a5d0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-0001a5e0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-0001a5f0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-0001a600: 7374 6428 616c 6c5f 6469 7265 6374 696f  std(all_directio
-0001a610: 6e61 6c5f 6368 616e 6765 2929 0d0a 0d0a  nal_change))....
-0001a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a630: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-0001a640: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-0001a650: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
-0001a660: 6561 6e28 616c 6c5f 6469 7374 616e 6365  ean(all_distance
-0001a670: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-0001a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a690: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-0001a6a0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0001a6b0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
-0001a6c0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-0001a6d0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a700: 0d0a 6465 6620 626f 756e 6461 7279 5f70  ..def boundary_p
-0001a710: 6f69 6e74 7328 6d61 736b 2c20 7863 616c  oints(mask, xcal
-0001a720: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
-0001a730: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
-0001a740: 7469 6f6e 293a 0d0a 0d0a 2020 2020 6e64  tion):....    nd
-0001a750: 696d 203d 206c 656e 286d 6173 6b2e 7368  im = len(mask.sh
-0001a760: 6170 6529 0d0a 2020 2020 7469 6d65 645f  ape)..    timed_
-0001a770: 6d61 736b 203d 207b 7d0d 0a20 2020 206d  mask = {}..    m
-0001a780: 6173 6b20 3d20 6d61 736b 203e 2030 0d0a  ask = mask > 0..
-0001a790: 2020 2020 6d61 736b 203d 206d 6173 6b2e      mask = mask.
-0001a7a0: 6173 7479 7065 2827 7569 6e74 3827 290d  astype('uint8').
-0001a7b0: 0a20 2020 2023 2059 5820 7368 6170 6564  .    # YX shaped
-0001a7c0: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
-0001a7d0: 6e64 696d 203d 3d20 323a 0d0a 2020 2020  ndim == 2:..    
-0001a7e0: 2020 2020 0d0a 2020 2020 2020 2020 626f      ..        bo
-0001a7f0: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
-0001a800: 756e 6461 7269 6573 286d 6173 6b29 0d0a  undaries(mask)..
-0001a810: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
-0001a820: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
-0001a830: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-0001a840: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
-0001a850: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001a860: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-0001a870: 203e 2030 290d 0a20 2020 2020 2020 2072   > 0)..        r
-0001a880: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
-0001a890: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
-0001a8a0: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
-0001a8b0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-0001a8c0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
-0001a8d0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-0001a8e0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
-0001a8f0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
-0001a900: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-0001a910: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-0001a920: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-0001a930: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-0001a940: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
-0001a950: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-0001a960: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-0001a970: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
-0001a980: 696f 6e0d 0a0d 0a20 2020 2020 2020 2074  ion....        t
-0001a990: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
-0001a9a0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
-0001a9b0: 6573 290d 0a20 2020 2020 2020 2023 2054  es)..        # T
-0001a9c0: 6869 7320 6f62 6a65 6374 2063 6f6e 7461  his object conta
-0001a9d0: 696e 7320 6c69 7374 206f 6620 616c 6c20  ins list of all 
-0001a9e0: 7468 6520 706f 696e 7473 2066 6f72 2061  the points for a
-0001a9f0: 6c6c 2074 6865 206c 6162 656c 7320 696e  ll the labels in
-0001aa00: 2074 6865 204d 6173 6b20 696d 6167 6520   the Mask image 
-0001aa10: 7769 7468 2074 6865 206c 6162 656c 2069  with the label i
-0001aa20: 6420 616e 6420 766f 6c75 6d65 206f 6620  d and volume of 
-0001aa30: 6561 6368 206c 6162 656c 0d0a 2020 2020  each label..    
-0001aa40: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-0001aa50: 7472 2830 295d 203d 205b 7472 6565 2c20  tr(0)] = [tree, 
-0001aa60: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-0001aa70: 656e 7472 6f69 645d 0d0a 0d0a 2020 2020  entroid]....    
-0001aa80: 2320 5459 5820 7368 6170 6564 206f 626a  # TYX shaped obj
-0001aa90: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-0001aaa0: 203d 3d20 333a 0d0a 0d0a 0d0a 2020 2020   == 3:......    
-0001aab0: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
-0001aac0: 6d28 7261 6e67 6528 302c 206d 6173 6b2e  m(range(0, mask.
-0001aad0: 7368 6170 655b 305d 2929 3a0d 0a20 2020  shape[0])):..   
-0001aae0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0001ab00: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
-0001ab10: 6f75 6e64 6172 6965 7328 6d61 736b 5b69  oundaries(mask[i
-0001ab20: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
-0001ab30: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
-0001ab40: 726f 6964 203d 2028 302c 2920 2b20 636f  roid = (0,) + co
-0001ab50: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
-0001ab60: 6f75 6e64 6172 7929 200d 0a20 2020 2020  oundary) ..     
-0001ab70: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-0001ab80: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
-0001ab90: 756e 6461 7279 203e 2030 290d 0a20 2020  undary > 0)..   
-0001aba0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-0001abb0: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
-0001abc0: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
-0001abd0: 7261 7928 696e 6469 6365 732c 2064 7479  ray(indices, dty
-0001abe0: 7065 3d6e 702e 666c 6f61 7433 3229 292e  pe=np.float32)).
-0001abf0: 636f 7079 2829 0d0a 0d0a 2020 2020 2020  copy()....      
-0001ac00: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-0001ac10: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
-0001ac20: 7265 616c 5f69 6e64 6963 6573 2929 3a0d  real_indices)):.
-0001ac30: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001ac40: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-0001ac50: 6365 735b 6a5d 5b30 5d20 3d20 7265 616c  ces[j][0] = real
-0001ac60: 5f69 6e64 6963 6573 5b6a 5d5b 305d 202a  _indices[j][0] *
-0001ac70: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
+00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d60: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
+00019d70: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00019d80: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00019d90: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+00019da0: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+00019db0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dd0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00019de0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00019df0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00019e00: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00019e10: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
+00019e20: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+00019e30: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
+00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e50: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00019e60: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
+00019e70: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00019e80: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+00019e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019eb0: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
+00019ec0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00019ed0: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
+00019ee0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+00019ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f00: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00019f10: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
+00019f20: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00019f30: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
+00019f40: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00019f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f60: 2020 2020 2020 2020 2069 6620 616c 6c5f           if all_
+00019f70: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00019f80: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+00019f90: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00019fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fb0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00019fc0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
+00019fd0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00019fe0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00019ff0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+0001a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a010: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a040: 2020 2020 2061 6c6c 5f72 6164 6975 732e       all_radius.
+0001a050: 6170 7065 6e64 284e 6f6e 6529 2020 2020  append(None)    
+0001a060: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a080: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
+0001a090: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+0001a0a0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+0001a0b0: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
+0001a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0e0: 616c 6c5f 6163 632e 6170 7065 6e64 2861  all_acc.append(a
+0001a0f0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+0001a100: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
+0001a110: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
+0001a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a130: 2020 2020 2020 2020 2020 2020 2020 616c                al
+0001a140: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
+0001a150: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
+0001a160: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+0001a170: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+0001a180: 655f 6b65 795d 2920 2020 0d0a 2020 2020  e_key])   ..    
+0001a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1a0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+0001a1b0: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
+0001a1c0: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
+0001a1d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+0001a1e0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0001a1f0: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a20  ll_mask_key]).. 
+0001a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a220: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001a230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a240: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+0001a250: 705f 7a20 3d20 6e70 2e61 6273 286e 702e  p_z = np.abs(np.
+0001a260: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
+0001a270: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
+0001a280: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+0001a290: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
+0001a2a0: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
+0001a2b0: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
+0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2d0: 206d 6974 6f74 6963 5f64 6973 705f 7820   mitotic_disp_x 
+0001a2e0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+0001a2f0: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
+0001a300: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001a310: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+0001a320: 6f74 6963 5f64 6973 705f 7a20 3d20 6e70  otic_disp_z = np
+0001a330: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
+0001a340: 5f6d 6974 6f74 6963 5f64 6973 705f 7a29  _mitotic_disp_z)
+0001a350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a360: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+0001a370: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
+0001a380: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
+0001a390: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+0001a3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a3b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+0001a3c0: 5f64 6973 705f 7820 3d20 6e70 2e61 6273  _disp_x = np.abs
+0001a3d0: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
+0001a3e0: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
+0001a3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a400: 2020 2020 2061 6c6c 5f64 6973 705f 7a20       all_disp_z 
+0001a410: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+0001a420: 2861 6c6c 5f64 6973 705f 7a29 290d 0a20  (all_disp_z)).. 
+0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a440: 2020 2061 6c6c 5f64 6973 705f 7920 3d20     all_disp_y = 
+0001a450: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
+0001a460: 6c6c 5f64 6973 705f 7929 290d 0a20 2020  ll_disp_y))..   
+0001a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a480: 2061 6c6c 5f64 6973 705f 7820 3d20 6e70   all_disp_x = np
+0001a490: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
+0001a4a0: 5f64 6973 705f 7829 290d 0a0d 0a0d 0a20  _disp_x))...... 
+0001a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001a4e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001a4f0: 662e 7469 6d65 2e61 7070 656e 6428 6920  f.time.append(i 
+0001a500: 2a20 7365 6c66 2e74 6361 6c69 6272 6174  * self.tcalibrat
+0001a510: 696f 6e29 0d0a 0d0a 0d0a 2020 2020 2020  ion)......      
+0001a520: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a530: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+0001a540: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+0001a550: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+0001a560: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+0001a570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a580: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+0001a590: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+0001a5a0: 6428 6d69 746f 7469 635f 6469 7370 5f7a  d(mitotic_disp_z
+0001a5b0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+0001a5c0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0001a5d0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+0001a5e0: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+0001a5f0: 6e28 6d69 746f 7469 635f 6469 7370 5f79  n(mitotic_disp_y
+0001a600: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001a610: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+0001a620: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
+0001a630: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+0001a640: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
+0001a650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a660: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+0001a670: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+0001a680: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+0001a690: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6b0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+0001a6c0: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+0001a6d0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+0001a6e0: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
+0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a700: 2020 6669 6c74 6572 6564 5f76 616c 7565    filtered_value
+0001a710: 7320 3d20 5b76 616c 2066 6f72 2076 616c  s = [val for val
+0001a720: 2069 6e20 6d69 746f 7469 635f 7261 6469   in mitotic_radi
+0001a730: 7573 2069 6620 7661 6c20 6973 206e 6f74  us if val is not
+0001a740: 204e 6f6e 655d 0d0a 2020 2020 2020 2020   None]..        
+0001a750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a760: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7261  .mitotic_mean_ra
+0001a770: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
+0001a780: 6561 6e28 6669 6c74 6572 6564 5f76 616c  ean(filtered_val
+0001a790: 7565 7329 290d 0a20 2020 2020 2020 2020  ues))..         
+0001a7a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7c0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+0001a7d0: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
+0001a7e0: 6e70 2e73 7464 2866 696c 7465 7265 645f  np.std(filtered_
+0001a7f0: 7661 6c75 6573 2929 0d0a 2020 2020 2020  values))..      
+0001a800: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a820: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+0001a830: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
+0001a840: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+0001a850: 6963 5f73 7065 6564 2929 0d0a 2020 2020  ic_speed))..    
+0001a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a870: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+0001a880: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+0001a890: 2e73 7464 286d 6974 6f74 6963 5f73 7065  .std(mitotic_spe
+0001a8a0: 6564 2929 0d0a 0d0a 2020 2020 2020 2020  ed))....        
+0001a8b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a8c0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6163  .mitotic_mean_ac
+0001a8d0: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
+0001a8e0: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
+0001a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a900: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+0001a910: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
+0001a920: 6e70 2e73 7464 286d 6974 6f74 6963 5f61  np.std(mitotic_a
+0001a930: 6363 2929 0d0a 0d0a 2020 2020 2020 2020  cc))....        
+0001a940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a950: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+0001a960: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+0001a970: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+0001a980: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+0001a990: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9b0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+0001a9c0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+0001a9d0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+0001a9e0: 7374 6428 6d69 746f 7469 635f 6469 7265  std(mitotic_dire
+0001a9f0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+0001aa00: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001aa10: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+0001aa20: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
+0001aa30: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+0001aa40: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+0001aa50: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+0001aa60: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+0001aa70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001aa80: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+0001aa90: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0001aaa0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+0001aab0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+0001aac0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aae0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+0001aaf0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
+0001ab00: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+0001ab10: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+0001ab20: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+0001ab30: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001ab40: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+0001ab50: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+0001ab60: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+0001ab70: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
+0001ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab90: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+0001aba0: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
+0001abb0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+0001abc0: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+0001abd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001abe0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+0001abf0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+0001ac00: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
+0001ac10: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+0001ac20: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
+0001ac30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ac40: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+0001ac50: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
+0001ac60: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+0001ac70: 7469 635f 6469 7370 5f78 2929 0d0a 2020  tic_disp_x))..  
 0001ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac90: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-0001aca0: 6a5d 5b31 5d20 3d20 7265 616c 5f69 6e64  j][1] = real_ind
-0001acb0: 6963 6573 5b6a 5d5b 315d 202a 2078 6361  ices[j][1] * xca
-0001acc0: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
-0001acd0: 2020 2020 2020 2020 2020 2020 2074 7265               tre
-0001ace0: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
-0001acf0: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
-0001ad00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001ad10: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
-0001ad20: 7374 7228 6929 5d20 3d20 5b74 7265 652c  str(i)] = [tree,
-0001ad30: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
-0001ad40: 6365 6e74 726f 6964 5d0d 0a20 2020 2020  centroid]..     
-0001ad50: 2020 2020 2020 200d 0a20 2020 2023 2054         ..    # T
-0001ad60: 5a59 5820 7368 6170 6564 206f 626a 6563  ZYX shaped objec
-0001ad70: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
-0001ad80: 3d20 343a 0d0a 2020 2020 2020 2020 7072  = 4:..        pr
-0001ad90: 696e 7428 274d 616b 696e 6720 6d61 736b  int('Making mask
-0001ada0: 2069 6e20 3444 2729 0d0a 2020 2020 2020   in 4D')..      
-0001adb0: 2020 626f 756e 6461 7279 203d 206e 702e    boundary = np.
-0001adc0: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
-0001add0: 2020 2020 5b6d 6173 6b2e 7368 6170 655b      [mask.shape[
-0001ade0: 305d 2c20 6d61 736b 2e73 6861 7065 5b31  0], mask.shape[1
-0001adf0: 5d2c 206d 6173 6b2e 7368 6170 655b 325d  ], mask.shape[2]
-0001ae00: 2c20 6d61 736b 2e73 6861 7065 5b33 5d5d  , mask.shape[3]]
-0001ae10: 2c20 6474 7970 653d 6e70 2e75 696e 7438  , dtype=np.uint8
-0001ae20: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-0001ae30: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001ae40: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
-0001ae50: 655b 305d 293a 0d0a 2020 2020 2020 2020  e[0]):..        
-0001ae60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001ae70: 2020 626f 756e 6461 7279 5b69 2c3a 5d20    boundary[i,:] 
-0001ae80: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
-0001ae90: 7328 6d61 736b 5b69 2c3a 5d29 0d0a 2020  s(mask[i,:])..  
-0001aea0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
-0001aeb0: 6365 6e74 726f 6964 203d 2063 6f6d 7075  centroid = compu
-0001aec0: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
-0001aed0: 6461 7279 5b69 2c3a 5d29 200d 0a20 2020  dary[i,:]) ..   
-0001aee0: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-0001aef0: 203d 206e 702e 7768 6572 6528 626f 756e   = np.where(boun
-0001af00: 6461 7279 5b69 2c3a 5d20 3e20 3029 0d0a  dary[i,:] > 0)..
-0001af10: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001af20: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-0001af30: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-0001af40: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
-0001af50: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
-0001af60: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-0001af70: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-0001af80: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
-0001af90: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
-0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afb0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-0001afc0: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
-0001afd0: 6365 735b 6a5d 5b30 5d20 2a20 7a63 616c  ces[j][0] * zcal
-0001afe0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-0001aff0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001b000: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-0001b010: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-0001b020: 6a5d 5b31 5d20 2a20 7963 616c 6962 7261  j][1] * ycalibra
-0001b030: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-0001b040: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-0001b050: 6e64 6963 6573 5b6a 5d5b 325d 203d 2072  ndices[j][2] = r
-0001b060: 6561 6c5f 696e 6469 6365 735b 6a5d 5b32  eal_indices[j][2
-0001b070: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
-0001b080: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001b090: 7472 6565 203d 2073 7061 7469 616c 2e63  tree = spatial.c
-0001b0a0: 4b44 5472 6565 2872 6561 6c5f 696e 6469  KDTree(real_indi
-0001b0b0: 6365 7329 0d0a 2020 2020 2020 2020 2020  ces)..          
-0001b0c0: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
-0001b0d0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
-0001b0e0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
-0001b0f0: 7472 6f69 645d 0d0a 2020 2020 7072 696e  troid]..    prin
-0001b100: 7428 2743 6f6d 7075 7465 6420 7468 6520  t('Computed the 
-0001b110: 626f 756e 6461 7279 2070 6f69 6e74 7327  boundary points'
-0001b120: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
-0001b130: 7469 6d65 645f 6d61 736b 2c20 626f 756e  timed_mask, boun
-0001b140: 6461 7279 2020 2020 2020 2020 0d0a 0d0a  dary        ....
-0001b150: 6465 6620 636f 6d70 7574 655f 6365 6e74  def compute_cent
-0001b160: 726f 6964 2862 696e 6172 795f 696d 6167  roid(binary_imag
-0001b170: 6529 3a0d 0a20 2020 2023 2045 6e73 7572  e):..    # Ensur
-0001b180: 6520 6269 6e61 7279 2069 6d61 6765 2069  e binary image i
-0001b190: 7320 6120 4e75 6d50 7920 6172 7261 790d  s a NumPy array.
-0001b1a0: 0a20 2020 2062 696e 6172 795f 696d 6167  .    binary_imag
-0001b1b0: 6520 3d20 6e70 2e61 7272 6179 2862 696e  e = np.array(bin
-0001b1c0: 6172 795f 696d 6167 6529 0d0a 0d0a 2020  ary_image)....  
-0001b1d0: 2020 7768 6974 655f 7069 7865 6c73 203d    white_pixels =
-0001b1e0: 206e 702e 7768 6572 6528 6269 6e61 7279   np.where(binary
-0001b1f0: 5f69 6d61 6765 203d 3d20 3129 0d0a 2020  _image == 1)..  
-0001b200: 2020 6e75 6d5f 7069 7865 6c73 203d 206c    num_pixels = l
-0001b210: 656e 2877 6869 7465 5f70 6978 656c 735b  en(white_pixels[
-0001b220: 305d 290d 0a0d 0a20 2020 2023 2043 6f6d  0])....    # Com
-0001b230: 7075 7465 2074 6865 2063 656e 7472 6f69  pute the centroi
-0001b240: 6420 6f66 2074 6865 2077 6869 7465 2070  d of the white p
-0001b250: 6978 656c 7320 696e 2074 6865 2062 6f75  ixels in the bou
-0001b260: 6e64 6172 7920 696d 6167 650d 0a20 2020  ndary image..   
-0001b270: 2063 656e 7472 6f69 6420 3d20 6e70 2e7a   centroid = np.z
-0001b280: 6572 6f73 2862 696e 6172 795f 696d 6167  eros(binary_imag
-0001b290: 652e 6e64 696d 290d 0a20 2020 2066 6f72  e.ndim)..    for
-0001b2a0: 2064 696d 2069 6e20 7261 6e67 6528 6269   dim in range(bi
-0001b2b0: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
-0001b2c0: 3a0d 0a20 2020 2020 2020 2063 656e 7472  :..        centr
-0001b2d0: 6f69 645b 6469 6d5d 203d 2077 6869 7465  oid[dim] = white
-0001b2e0: 5f70 6978 656c 735b 6469 6d5d 2e73 756d  _pixels[dim].sum
-0001b2f0: 2829 202f 206e 756d 5f70 6978 656c 730d  () / num_pixels.
-0001b300: 0a0d 0a20 2020 2072 6574 7572 6e20 6365  ...    return ce
-0001b310: 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a 200d  ntroid........ .
-0001b320: 0a0d 0a64 6566 2067 6574 5f63 7376 5f64  ...def get_csv_d
-0001b330: 6174 6128 6373 7629 3a0d 0a0d 0a20 2020  ata(csv):....   
-0001b340: 2020 2020 2064 6174 6173 6574 203d 2070       dataset = p
-0001b350: 642e 7265 6164 5f63 7376 280d 0a20 2020  d.read_csv(..   
-0001b360: 2020 2020 2020 2020 2063 7376 2c20 6465           csv, de
-0001b370: 6c69 6d69 7465 723d 222c 222c 2065 6e63  limiter=",", enc
-0001b380: 6f64 696e 673d 2275 6e69 636f 6465 5f65  oding="unicode_e
-0001b390: 7363 6170 6522 2c20 6c6f 775f 6d65 6d6f  scape", low_memo
-0001b3a0: 7279 3d46 616c 7365 0d0a 2020 2020 2020  ry=False..      
-0001b3b0: 2020 295b 333a 5d0d 0a20 2020 2020 2020    )[3:]..       
-0001b3c0: 2064 6174 6173 6574 5f69 6e64 6578 203d   dataset_index =
-0001b3d0: 2064 6174 6173 6574 2e69 6e64 6578 0d0a   dataset.index..
-0001b3e0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-0001b3f0: 6174 6173 6574 2c20 6461 7461 7365 745f  ataset, dataset_
-0001b400: 696e 6465 780d 0a20 2020 200d 0a64 6566  index..    ..def
-0001b410: 2067 6574 5f73 706f 745f 6461 7461 7365   get_spot_datase
-0001b420: 7428 7370 6f74 5f64 6174 6173 6574 2c20  t(spot_dataset, 
-0001b430: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001b440: 706f 745f 6b65 7973 2c20 7863 616c 6962  pot_keys, xcalib
-0001b450: 7261 7469 6f6e 2c20 7963 616c 6962 7261  ration, ycalibra
-0001b460: 7469 6f6e 2c20 7a63 616c 6962 7261 7469  tion, zcalibrati
-0001b470: 6f6e 2c20 4174 7472 6962 7574 6542 6f78  on, AttributeBox
-0001b480: 6e61 6d65 2c20 6465 7465 6374 696f 6e63  name, detectionc
-0001b490: 6861 6e6e 656c 293a 0d0a 2020 2020 2020  hannel):..      
-0001b4a0: 2020 416c 6c56 616c 7565 7320 3d20 7b7d    AllValues = {}
-0001b4b0: 0d0a 2020 2020 2020 2020 706f 7369 7820  ..        posix 
-0001b4c0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001b4d0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-0001b4e0: 7822 5d0d 0a20 2020 2020 2020 2070 6f73  x"]..        pos
-0001b4f0: 6979 203d 2074 7261 636b 5f61 6e61 6c79  iy = track_analy
-0001b500: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-0001b510: 6f73 6979 225d 0d0a 2020 2020 2020 2020  osiy"]..        
-0001b520: 706f 7369 7a20 3d20 7472 6163 6b5f 616e  posiz = track_an
-0001b530: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001b540: 5b22 706f 7369 7a22 5d0d 0a20 2020 2020  ["posiz"]..     
-0001b550: 2020 2066 7261 6d65 203d 2074 7261 636b     frame = track
-0001b560: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001b570: 6579 735b 2266 7261 6d65 225d 0d0a 2020  eys["frame"]..  
-0001b580: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001b590: 4c6f 6361 7469 6f6e 5820 3d20 280d 0a20  LocationX = (.. 
-0001b5a0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001b5b0: 6461 7461 7365 745b 706f 7369 785d 2e61  dataset[posix].a
-0001b5c0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001b5d0: 2078 6361 6c69 6272 6174 696f 6e0d 0a20   xcalibration.. 
-0001b5e0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001b5f0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001b600: 4c6f 6361 7469 6f6e 5920 3d20 280d 0a20  LocationY = (.. 
-0001b610: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001b620: 6461 7461 7365 745b 706f 7369 795d 2e61  dataset[posiy].a
-0001b630: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001b640: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
-0001b650: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001b660: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001b670: 4c6f 6361 7469 6f6e 5a20 3d20 280d 0a20  LocationZ = (.. 
-0001b680: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001b690: 6461 7461 7365 745b 706f 7369 7a5d 2e61  dataset[posiz].a
-0001b6a0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001b6b0: 207a 6361 6c69 6272 6174 696f 6e0d 0a20   zcalibration.. 
-0001b6c0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001b6d0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001b6e0: 4c6f 6361 7469 6f6e 5420 3d20 2873 706f  LocationT = (spo
-0001b6f0: 745f 6461 7461 7365 745b 6672 616d 655d  t_dataset[frame]
-0001b700: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001b710: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001b720: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
-0001b730: 2020 2020 2069 676e 6f72 655f 7661 6c75       ignore_valu
-0001b740: 6573 203d 205b 7472 6163 6b5f 616e 616c  es = [track_anal
-0001b750: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001b760: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-0001b770: 2c74 7261 636b 5f61 6e61 6c79 7369 735f  ,track_analysis_
-0001b780: 7370 6f74 5f6b 6579 735b 2274 6f74 616c  spot_keys["total
-0001b790: 5f69 6e74 656e 7369 7479 225d 5d0d 0a20  _intensity"]].. 
-0001b7a0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-0001b7b0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001b7c0: 6973 5f73 706f 745f 6b65 7973 2e69 7465  is_spot_keys.ite
-0001b7d0: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
-0001b7e0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
-0001b7f0: 6374 696f 6e63 6861 6e6e 656c 203d 3d20  ctionchannel == 
-0001b800: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-0001b810: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
-0001b820: 2022 6d65 616e 5f69 6e74 656e 7369 7479   "mean_intensity
-0001b830: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
-0001b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b850: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
-0001b860: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001b870: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
-0001b880: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
-0001b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8a0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
-0001b8b0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
-0001b8c0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001b8d0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
-0001b8e0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
-0001b8f0: 3d3d 2022 746f 7461 6c5f 696e 7465 6e73  == "total_intens
-0001b900: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
-0001b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b920: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
-0001b930: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001b940: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
-0001b950: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
-0001b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b970: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001b980: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
-0001b990: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-0001b9a0: 2266 6c6f 6174 2229 2020 2020 2020 200d  "float")       .
-0001b9b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001b9c0: 2020 2069 6620 7620 6e6f 7420 696e 2069     if v not in i
-0001b9d0: 676e 6f72 655f 7661 6c75 6573 3a0d 0a20  gnore_values:.. 
-0001b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001ba00: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0001ba10: 6c6c 5661 6c75 6573 5b76 5d20 3d20 7370  llValues[v] = sp
-0001ba20: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
-0001ba30: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba50: 2020 0d0a 0d0a 2020 2020 2020 2020 416c    ....        Al
-0001ba60: 6c56 616c 7565 735b 706f 7369 785d 203d  lValues[posix] =
-0001ba70: 2072 6f75 6e64 284c 6f63 6174 696f 6e58   round(LocationX
-0001ba80: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
-0001ba90: 5661 6c75 6573 5b70 6f73 6979 5d20 3d20  Values[posiy] = 
-0001baa0: 726f 756e 6428 4c6f 6361 7469 6f6e 592c  round(LocationY,
-0001bab0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
-0001bac0: 616c 7565 735b 706f 7369 7a5d 203d 2072  alues[posiz] = r
-0001bad0: 6f75 6e64 284c 6f63 6174 696f 6e5a 2c33  ound(LocationZ,3
-0001bae0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
-0001baf0: 6c75 6573 5b66 7261 6d65 5d20 3d20 726f  lues[frame] = ro
-0001bb00: 756e 6428 4c6f 6361 7469 6f6e 542c 3329  und(LocationT,3)
-0001bb10: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-0001bb20: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
-0001bb30: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001bb40: 732e 6170 7065 6e64 2841 7474 7269 6275  s.append(Attribu
-0001bb50: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
-0001bb60: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
-0001bb70: 656e 616d 6520 696e 2041 6c6c 5661 6c75  ename in AllValu
-0001bb80: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
-0001bb90: 2020 2020 2020 2020 2020 4174 7472 6962            Attrib
-0001bba0: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
-0001bbb0: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
-0001bbc0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001bbd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001bbe0: 2020 7265 7475 726e 2041 7474 7269 6275    return Attribu
-0001bbf0: 7465 6964 732c 2041 6c6c 5661 6c75 6573  teids, AllValues
-0001bc00: 2020 2020 200d 0a20 2020 200d 0a0d 0a64       ..    ....d
-0001bc10: 6566 2067 6574 5f74 7261 636b 5f64 6174  ef get_track_dat
-0001bc20: 6173 6574 2874 7261 636b 5f64 6174 6173  aset(track_datas
-0001bc30: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
-0001bc40: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
-0001bc50: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
-0001bc60: 636b 5f6b 6579 732c 2054 7261 636b 4174  ck_keys, TrackAt
-0001bc70: 7472 6962 7574 6542 6f78 6e61 6d65 293a  tributeBoxname):
-0001bc80: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
-0001bc90: 7261 636b 5661 6c75 6573 203d 207b 7d0d  rackValues = {}.
-0001bca0: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
-0001bcb0: 6420 3d20 7472 6163 6b5f 616e 616c 7973  d = track_analys
-0001bcc0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
-0001bcd0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
-0001bce0: 2020 5469 6420 3d20 7472 6163 6b5f 6461    Tid = track_da
-0001bcf0: 7461 7365 745b 7472 6163 6b5f 6964 5d2e  taset[track_id].
-0001bd00: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001bd10: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-0001bd20: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
-0001bd30: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
-0001bd40: 0d0a 2020 2020 2020 0d0a 2020 2020 2020  ..      ..      
-0001bd50: 2020 666f 7220 286b 2c20 7629 2069 6e20    for (k, v) in 
-0001bd60: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-0001bd70: 7261 636b 5f6b 6579 732e 6974 656d 7328  rack_keys.items(
-0001bd80: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0001bd90: 2020 2020 2020 7820 3d20 7472 6163 6b5f        x = track_
-0001bda0: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
-0001bdb0: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
-0001bdc0: 2020 2020 2020 2020 2020 2020 6d69 6e76              minv
-0001bdd0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
-0001bde0: 2020 2020 2020 2020 2020 2020 206d 6178               max
-0001bdf0: 7661 6c20 3d20 6d61 7828 7829 0d0a 0d0a  val = max(x)....
-0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be10: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
-0001be20: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
-0001be30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001be40: 2020 2020 2020 7820 3d20 7820 2b20 310d        x = x + 1.
-0001be50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001be60: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001be70: 735b 6b5d 203d 2072 6f75 6e64 2878 2c20  s[k] = round(x, 
-0001be80: 3329 0d0a 0d0a 2020 2020 2020 2020 5472  3)....        Tr
-0001be90: 6163 6b41 7474 7269 6275 7465 6964 7320  ackAttributeids 
-0001bea0: 3d20 5b5d 0d0a 2020 2020 2020 2020 5472  = []..        Tr
-0001beb0: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
-0001bec0: 6170 7065 6e64 2854 7261 636b 4174 7472  append(TrackAttr
-0001bed0: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-0001bee0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
-0001bef0: 6275 7465 6e61 6d65 2069 6e20 7472 6163  butename in trac
-0001bf00: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
-0001bf10: 5f6b 6579 732e 6b65 7973 2829 3a0d 0a20  _keys.keys():.. 
-0001bf20: 2020 2020 2020 2020 2020 2054 7261 636b             Track
-0001bf30: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001bf40: 656e 6428 6174 7472 6962 7574 656e 616d  end(attributenam
-0001bf50: 6529 2020 2020 0d0a 2020 2020 0d0a 2020  e)    ..    ..  
-0001bf60: 2020 2020 2020 7265 7475 726e 2054 7261        return Tra
-0001bf70: 636b 4174 7472 6962 7574 6569 6473 2c20  ckAttributeids, 
-0001bf80: 416c 6c54 7261 636b 5661 6c75 6573 0d0a  AllTrackValues..
-0001bf90: 2020 2020 0d0a 6465 6620 6765 745f 6564      ..def get_ed
-0001bfa0: 6765 735f 6461 7461 7365 7428 6564 6765  ges_dataset(edge
-0001bfb0: 735f 6461 7461 7365 742c 2065 6467 6573  s_dataset, edges
-0001bfc0: 5f64 6174 6173 6574 5f69 6e64 6578 2c20  _dataset_index, 
-0001bfd0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001bfe0: 706f 745f 6b65 7973 2c20 7472 6163 6b5f  pot_keys, track_
-0001bff0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-0001c000: 6579 7329 3a0d 0a0d 0a20 2020 2020 2020  eys):....       
-0001c010: 2041 6c6c 4564 6765 7356 616c 7565 7320   AllEdgesValues 
-0001c020: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
-0001c030: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
-0001c040: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001c050: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
-0001c060: 2020 2020 2020 2054 6964 203d 2065 6467         Tid = edg
-0001c070: 6573 5f64 6174 6173 6574 5b74 7261 636b  es_dataset[track
-0001c080: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
-0001c090: 6174 2229 0d0a 2020 2020 2020 2020 696e  at")..        in
-0001c0a0: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
-0001c0b0: 2854 6964 203d 3d20 3029 0d0a 2020 2020  (Tid == 0)..    
-0001c0c0: 2020 2020 6d61 7874 7261 636b 5f69 6420      maxtrack_id 
-0001c0d0: 3d20 6d61 7828 5469 6429 0d0a 2020 2020  = max(Tid)..    
-0001c0e0: 2020 2020 636f 6e64 6974 696f 6e5f 696e      condition_in
-0001c0f0: 6469 6365 7320 3d20 6564 6765 735f 6461  dices = edges_da
-0001c100: 7461 7365 745f 696e 6465 785b 696e 6469  taset_index[indi
-0001c110: 6365 735d 0d0a 2020 2020 2020 2020 5469  ces]..        Ti
-0001c120: 645b 636f 6e64 6974 696f 6e5f 696e 6469  d[condition_indi
-0001c130: 6365 735d 203d 206d 6178 7472 6163 6b5f  ces] = maxtrack_
-0001c140: 6964 202b 2031 0d0a 2020 2020 2020 2020  id + 1..        
-0001c150: 416c 6c45 6467 6573 5661 6c75 6573 5b74  AllEdgesValues[t
-0001c160: 7261 636b 5f69 645d 203d 2054 6964 0d0a  rack_id] = Tid..
-0001c170: 0d0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
-0001c180: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001c190: 735f 6564 6765 735f 6b65 7973 2e76 616c  s_edges_keys.val
-0001c1a0: 7565 7328 293a 0d0a 0d0a 2020 2020 2020  ues():....      
-0001c1b0: 2020 2020 2020 6966 206b 2021 3d20 7472        if k != tr
-0001c1c0: 6163 6b5f 6964 3a0d 0a20 2020 2020 2020  ack_id:..       
-0001c1d0: 2020 2020 2020 2020 2078 203d 2065 6467           x = edg
-0001c1e0: 6573 5f64 6174 6173 6574 5b6b 5d2e 6173  es_dataset[k].as
-0001c1f0: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
-0001c200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c210: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
-0001c220: 6b5d 203d 2078 2020 200d 0a20 2020 2020  k] = x   ..     
-0001c230: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-0001c240: 7475 726e 2041 6c6c 4564 6765 7356 616c  turn AllEdgesVal
-0001c250: 7565 7320 2020 0d0a 2020 2020 0d0a 2020  ues   ..    ..  
-0001c260: 2020 2020 200d 0a20 2020 200d 0a64 6566       ..    ..def
-0001c270: 2073 6361 6c65 5f76 616c 7565 2878 2c20   scale_value(x, 
-0001c280: 7363 616c 6520 3d20 3235 3520 2a20 3235  scale = 255 * 25
-0001c290: 3529 3a0d 0a0d 0a0d 0a20 2020 2020 7265  5):......     re
-0001c2a0: 7475 726e 2078 202a 2073 6361 6c65 2020  turn x * scale  
-0001c2b0: 200d 0a20 2020 200d 0a0d 0a0d 0a64 6566   ..    ......def
-0001c2c0: 2070 726f 625f 7369 676d 6f69 6428 7829   prob_sigmoid(x)
-0001c2d0: 3a0d 0a20 2020 2072 6574 7572 6e20 3120  :..    return 1 
-0001c2e0: 2d20 6d61 7468 2e65 7870 282d 7829 0d0a  - math.exp(-x)..
-0001c2f0: 0d0a 0d0a 6465 6620 616e 6775 6c61 725f  ....def angular_
-0001c300: 6368 616e 6765 2876 6563 5f30 2c20 7665  change(vec_0, ve
-0001c310: 635f 3129 3a0d 0a20 2020 2020 2020 200d  c_1):..        .
-0001c320: 0a20 2020 2020 2020 2076 6563 5f30 203d  .        vec_0 =
-0001c330: 2076 6563 5f30 202f 206e 702e 6c69 6e61   vec_0 / np.lina
-0001c340: 6c67 2e6e 6f72 6d28 7665 635f 3029 0d0a  lg.norm(vec_0)..
-0001c350: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
-0001c360: 7665 635f 3120 2f20 6e70 2e6c 696e 616c  vec_1 / np.linal
-0001c370: 672e 6e6f 726d 2876 6563 5f31 290d 0a20  g.norm(vec_1).. 
-0001c380: 2020 2020 2020 2061 6e67 6c65 203d 206e         angle = n
-0001c390: 702e 6172 6363 6f73 286e 702e 636c 6970  p.arccos(np.clip
-0001c3a0: 286e 702e 646f 7428 7665 635f 302c 2076  (np.dot(vec_0, v
-0001c3b0: 6563 5f31 292c 202d 312e 302c 2031 2e30  ec_1), -1.0, 1.0
-0001c3c0: 2929 0d0a 2020 2020 2020 2020 616e 676c  ))..        angl
-0001c3d0: 6520 3d20 616e 676c 6520 2a20 3138 3020  e = angle * 180 
-0001c3e0: 2f20 6e70 2e70 690d 0a20 2020 2020 2020  / np.pi..       
-0001c3f0: 2072 6574 7572 6e20 616e 676c 650d 0a20   return angle.. 
-0001c400: 2020 2020 0d0a 0d0a 6465 6620 6576 616c      ....def eval
-0001c410: 5f62 6f6f 6c28 7661 6c75 6529 3a0d 0a20  _bool(value):.. 
-0001c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c430: 200d 0a20 2020 2020 2020 2069 6620 7661   ..        if va
-0001c440: 6c75 6520 203d 3d20 2754 7275 6527 3a20  lue  == 'True': 
-0001c450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c460: 2020 6469 765f 6b65 7920 3d20 5472 7565    div_key = True
-0001c470: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001c480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c490: 2064 6976 5f6b 6579 203d 2046 616c 7365   div_key = False
-0001c4a0: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
-0001c4b0: 7572 6e20 6469 765f 6b65 7920 2020 2020  urn div_key     
-0001c4c0: 2020 2020 2020 2020 2020 200d 0a0d 0a64             ....d
-0001c4d0: 6566 2063 6865 636b 5f61 6e64 5f75 7064  ef check_and_upd
-0001c4e0: 6174 655f 6d61 736b 286d 6173 6b2c 696d  ate_mask(mask,im
-0001c4f0: 6167 6529 3a0d 0a20 2020 2020 2020 0d0a  age):..       ..
-0001c500: 2020 2020 2020 2020 6966 206c 656e 286d          if len(m
-0001c510: 6173 6b2e 7368 6170 6529 203c 206c 656e  ask.shape) < len
-0001c520: 2869 6d61 6765 2e73 6861 7065 293a 0d0a  (image.shape):..
-0001c530: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-0001c540: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
-0001c550: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
-0001c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c570: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c590: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
-0001c5a0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-0001c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5c0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001c5d0: 5b31 5d2c 0d0a 2020 2020 2020 2020 2020  [1],..          
-0001c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5f0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001c600: 655b 325d 2c0d 0a20 2020 2020 2020 2020  e[2],..         
-0001c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c620: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001c630: 7065 5b33 5d2c 0d0a 2020 2020 2020 2020  pe[3],..        
-0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c650: 2020 2020 5d2c 2064 7479 7065 3d22 7569      ], dtype="ui
-0001c660: 6e74 3822 0d0a 2020 2020 2020 2020 2020  nt8"..          
-0001c670: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0001c680: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0001c690: 2069 2069 6e20 7261 6e67 6528 302c 2075   i in range(0, u
-0001c6a0: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
-0001c6b0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
-0001c6c0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0001c6d0: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
-0001c6e0: 6d61 736b 2e73 6861 7065 5b31 5d29 3a0d  mask.shape[1]):.
-0001c6f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001c700: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001c710: 736b 5b69 2c20 6a2c 203a 2c20 3a5d 203d  sk[i, j, :, :] =
-0001c720: 206d 6173 6b5b 692c 203a 2c20 3a5d 0d0a   mask[i, :, :]..
-0001c730: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0001c740: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001c750: 7064 6174 655f 6d61 736b 203d 206d 6173  pdate_mask = mas
-0001c760: 6b0d 0a0d 0a20 2020 2020 2020 2072 6574  k....        ret
-0001c770: 7572 6e20 7570 6461 7465 5f6d 6173 6b20  urn update_mask 
-0001c780: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001c790: 0d0a                                     ..
+0001ac90: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+0001aca0: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
+0001acb0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+0001acc0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+0001acd0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001ace0: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+0001acf0: 5f76 616c 7565 7320 3d20 5b76 616c 2066  _values = [val f
+0001ad00: 6f72 2076 616c 2069 6e20 6e6f 6e5f 6d69  or val in non_mi
+0001ad10: 746f 7469 635f 7261 6469 7573 2069 6620  totic_radius if 
+0001ad20: 7661 6c20 6973 206e 6f74 204e 6f6e 655d  val is not None]
+0001ad30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ad40: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+0001ad50: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+0001ad60: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
+0001ad70: 6e28 6669 6c74 6572 6564 5f76 616c 7565  n(filtered_value
+0001ad80: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
+0001ad90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001ada0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001adb0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+0001adc0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
+0001add0: 6428 6e70 2e73 7464 2866 696c 7465 7265  d(np.std(filtere
+0001ade0: 645f 7661 6c75 6573 2929 0d0a 0d0a 2020  d_values))....  
+0001adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae00: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+0001ae10: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
+0001ae20: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+0001ae30: 5f6d 6974 6f74 6963 5f73 7065 6564 2929  _mitotic_speed))
+0001ae40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ae50: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+0001ae60: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
+0001ae70: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+0001ae80: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
+0001ae90: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+0001aea0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001aeb0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+0001aec0: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
+0001aed0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f61  an(non_mitotic_a
+0001aee0: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
+0001aef0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001af00: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
+0001af10: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
+0001af20: 286e 6f6e 5f6d 6974 6f74 6963 5f61 6363  (non_mitotic_acc
+0001af30: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+0001af40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0001af50: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+0001af60: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+0001af70: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
+0001af80: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+0001af90: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+0001afa0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001afb0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+0001afc0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6972  _mitotic_var_dir
+0001afd0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+0001afe0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+0001aff0: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+0001b000: 696f 6e61 6c5f 6368 616e 6765 2929 200d  ional_change)) .
+0001b010: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b020: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+0001b030: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+0001b040: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+0001b050: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+0001b060: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+0001b070: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+0001b080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b090: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+0001b0a0: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
+0001b0b0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+0001b0c0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+0001b0d0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+0001b0e0: 6365 6c6c 5f6d 6173 6b29 290d 0a0d 0a0d  cell_mask)).....
+0001b0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b100: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+0001b110: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
+0001b120: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+0001b130: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
+0001b140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001b150: 616c 6c5f 7661 725f 6469 7370 5f7a 2e61  all_var_disp_z.a
+0001b160: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
+0001b170: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
+0001b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b190: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+0001b1a0: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
+0001b1b0: 6d65 616e 2861 6c6c 5f64 6973 705f 7929  mean(all_disp_y)
+0001b1c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b1d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0001b1e0: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
+0001b1f0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+0001b200: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
+0001b210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001b220: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+0001b230: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
+0001b240: 2861 6c6c 5f64 6973 705f 7829 290d 0a20  (all_disp_x)).. 
+0001b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b260: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+0001b270: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
+0001b280: 2e73 7464 2861 6c6c 5f64 6973 705f 7829  .std(all_disp_x)
+0001b290: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001b2a0: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
+0001b2b0: 645f 7661 6c75 6573 203d 205b 7661 6c20  d_values = [val 
+0001b2c0: 666f 7220 7661 6c20 696e 2061 6c6c 5f72  for val in all_r
+0001b2d0: 6164 6975 7320 6966 2076 616c 2069 7320  adius if val is 
+0001b2e0: 6e6f 7420 4e6f 6e65 5d0d 0a20 2020 2020  not None]..     
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001b300: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
+0001b310: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
+0001b320: 616e 2866 696c 7465 7265 645f 7661 6c75  an(filtered_valu
+0001b330: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
+0001b340: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b360: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
+0001b370: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
+0001b380: 6428 6669 6c74 6572 6564 5f76 616c 7565  d(filtered_value
+0001b390: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
+0001b3a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001b3b0: 616c 6c5f 6d65 616e 5f73 7065 6564 2e61  all_mean_speed.a
+0001b3c0: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+0001b3d0: 6c5f 7370 6565 6429 290d 0a20 2020 2020  l_speed))..     
+0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001b3f0: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
+0001b400: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
+0001b410: 616c 6c5f 7370 6565 6429 290d 0a0d 0a20  all_speed)).... 
+0001b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b430: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+0001b440: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+0001b450: 6561 6e28 616c 6c5f 6163 6329 290d 0a20  ean(all_acc)).. 
+0001b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b470: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+0001b480: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
+0001b490: 6428 616c 6c5f 6163 6329 290d 0a0d 0a0d  d(all_acc)).....
+0001b4a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b4b0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0001b4c0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+0001b4d0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+0001b4e0: 702e 6d65 616e 2861 6c6c 5f64 6972 6563  p.mean(all_direc
+0001b4f0: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+0001b500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b510: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+0001b520: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+0001b530: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+0001b540: 7464 2861 6c6c 5f64 6972 6563 7469 6f6e  td(all_direction
+0001b550: 616c 5f63 6861 6e67 6529 290d 0a0d 0a20  al_change)).... 
+0001b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b570: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+0001b580: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+0001b590: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
+0001b5a0: 616e 2861 6c6c 5f64 6973 7461 6e63 655f  an(all_distance_
+0001b5b0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+0001b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5d0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+0001b5e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0001b5f0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+0001b600: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+0001b610: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+0001b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b630: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+0001b640: 0a64 6566 2062 6f75 6e64 6172 795f 706f  .def boundary_po
+0001b650: 696e 7473 286d 6173 6b2c 2078 6361 6c69  ints(mask, xcali
+0001b660: 6272 6174 696f 6e2c 2079 6361 6c69 6272  bration, ycalibr
+0001b670: 6174 696f 6e2c 207a 6361 6c69 6272 6174  ation, zcalibrat
+0001b680: 696f 6e29 3a0d 0a0d 0a20 2020 206e 6469  ion):....    ndi
+0001b690: 6d20 3d20 6c65 6e28 6d61 736b 2e73 6861  m = len(mask.sha
+0001b6a0: 7065 290d 0a20 2020 2074 696d 6564 5f6d  pe)..    timed_m
+0001b6b0: 6173 6b20 3d20 7b7d 0d0a 2020 2020 6d61  ask = {}..    ma
+0001b6c0: 736b 203d 206d 6173 6b20 3e20 300d 0a20  sk = mask > 0.. 
+0001b6d0: 2020 206d 6173 6b20 3d20 6d61 736b 2e61     mask = mask.a
+0001b6e0: 7374 7970 6528 2775 696e 7438 2729 0d0a  stype('uint8')..
+0001b6f0: 2020 2020 2320 5958 2073 6861 7065 6420      # YX shaped 
+0001b700: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+0001b710: 6469 6d20 3d3d 2032 3a0d 0a20 2020 2020  dim == 2:..     
+0001b720: 2020 200d 0a20 2020 2020 2020 2062 6f75     ..        bou
+0001b730: 6e64 6172 7920 3d20 6669 6e64 5f62 6f75  ndary = find_bou
+0001b740: 6e64 6172 6965 7328 6d61 736b 290d 0a20  ndaries(mask).. 
+0001b750: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
+0001b760: 7472 6f69 6420 3d20 2830 2c29 202b 2063  troid = (0,) + c
+0001b770: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+0001b780: 626f 756e 6461 7279 2920 0d0a 2020 2020  boundary) ..    
+0001b790: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+0001b7a0: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
+0001b7b0: 3e20 3029 0d0a 2020 2020 2020 2020 7265  > 0)..        re
+0001b7c0: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
+0001b7d0: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
+0001b7e0: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
+0001b7f0: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
+0001b800: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+0001b810: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+0001b820: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
+0001b830: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
+0001b840: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+0001b850: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
+0001b860: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+0001b870: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+0001b880: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001b890: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
+0001b8a0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001b8b0: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
+0001b8c0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 7472  on....        tr
+0001b8d0: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+0001b8e0: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
+0001b8f0: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+0001b900: 6973 206f 626a 6563 7420 636f 6e74 6169  is object contai
+0001b910: 6e73 206c 6973 7420 6f66 2061 6c6c 2074  ns list of all t
+0001b920: 6865 2070 6f69 6e74 7320 666f 7220 616c  he points for al
+0001b930: 6c20 7468 6520 6c61 6265 6c73 2069 6e20  l the labels in 
+0001b940: 7468 6520 4d61 736b 2069 6d61 6765 2077  the Mask image w
+0001b950: 6974 6820 7468 6520 6c61 6265 6c20 6964  ith the label id
+0001b960: 2061 6e64 2076 6f6c 756d 6520 6f66 2065   and volume of e
+0001b970: 6163 6820 6c61 6265 6c0d 0a20 2020 2020  ach label..     
+0001b980: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
+0001b990: 7228 3029 5d20 3d20 5b74 7265 652c 2069  r(0)] = [tree, i
+0001b9a0: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
+0001b9b0: 6e74 726f 6964 5d0d 0a0d 0a20 2020 2023  ntroid]....    #
+0001b9c0: 2054 5958 2073 6861 7065 6420 6f62 6a65   TYX shaped obje
+0001b9d0: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+0001b9e0: 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020 2020  == 3:......     
+0001b9f0: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
+0001ba00: 2872 616e 6765 2830 2c20 6d61 736b 2e73  (range(0, mask.s
+0001ba10: 6861 7065 5b30 5d29 293a 0d0a 2020 2020  hape[0])):..    
+0001ba20: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001ba30: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0001ba40: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
+0001ba50: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
+0001ba60: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
+0001ba70: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+0001ba80: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
+0001ba90: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
+0001baa0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
+0001bab0: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+0001bac0: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+0001bad0: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+0001bae0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001baf0: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
+0001bb00: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
+0001bb10: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
+0001bb20: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
+0001bb30: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
+0001bb40: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0001bb50: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+0001bb60: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+0001bb70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bb80: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+0001bb90: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
+0001bba0: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
+0001bbb0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbd0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+0001bbe0: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+0001bbf0: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
+0001bc00: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+0001bc10: 2020 2020 2020 2020 2020 2020 7472 6565              tree
+0001bc20: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+0001bc30: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
+0001bc40: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001bc50: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
+0001bc60: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
+0001bc70: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
+0001bc80: 656e 7472 6f69 645d 0d0a 2020 2020 2020  entroid]..      
+0001bc90: 2020 2020 2020 0d0a 2020 2020 2320 545a        ..    # TZ
+0001bca0: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
+0001bcb0: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
+0001bcc0: 2034 3a0d 0a20 2020 2020 2020 2070 7269   4:..        pri
+0001bcd0: 6e74 2827 4d61 6b69 6e67 206d 6173 6b20  nt('Making mask 
+0001bce0: 696e 2034 4427 290d 0a20 2020 2020 2020  in 4D')..       
+0001bcf0: 2062 6f75 6e64 6172 7920 3d20 6e70 2e7a   boundary = np.z
+0001bd00: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001bd10: 2020 205b 6d61 736b 2e73 6861 7065 5b30     [mask.shape[0
+0001bd20: 5d2c 206d 6173 6b2e 7368 6170 655b 315d  ], mask.shape[1]
+0001bd30: 2c20 6d61 736b 2e73 6861 7065 5b32 5d2c  , mask.shape[2],
+0001bd40: 206d 6173 6b2e 7368 6170 655b 335d 5d2c   mask.shape[3]],
+0001bd50: 2064 7479 7065 3d6e 702e 7569 6e74 380d   dtype=np.uint8.
+0001bd60: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+0001bd70: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0001bd80: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
+0001bd90: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+0001bda0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001bdb0: 2062 6f75 6e64 6172 795b 692c 3a5d 203d   boundary[i,:] =
+0001bdc0: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
+0001bdd0: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
+0001bde0: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
+0001bdf0: 656e 7472 6f69 6420 3d20 636f 6d70 7574  entroid = comput
+0001be00: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
+0001be10: 6172 795b 692c 3a5d 2920 0d0a 2020 2020  ary[i,:]) ..    
+0001be20: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+0001be30: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
+0001be40: 6172 795b 692c 3a5d 203e 2030 290d 0a20  ary[i,:] > 0).. 
+0001be50: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+0001be60: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
+0001be70: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
+0001be80: 7928 696e 6469 6365 732c 2064 7479 7065  y(indices, dtype
+0001be90: 3d6e 702e 666c 6f61 7433 3229 292e 636f  =np.float32)).co
+0001bea0: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+0001beb0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0001bec0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+0001bed0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+0001bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bef0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001bf00: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+0001bf10: 6573 5b6a 5d5b 305d 202a 207a 6361 6c69  es[j][0] * zcali
+0001bf20: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+0001bf30: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0001bf40: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+0001bf50: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+0001bf60: 5d5b 315d 202a 2079 6361 6c69 6272 6174  ][1] * ycalibrat
+0001bf70: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+0001bf80: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+0001bf90: 6469 6365 735b 6a5d 5b32 5d20 3d20 7265  dices[j][2] = re
+0001bfa0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+0001bfb0: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+0001bfc0: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+0001bfd0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+0001bfe0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+0001bff0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+0001c000: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
+0001c010: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
+0001c020: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
+0001c030: 726f 6964 5d0d 0a20 2020 2070 7269 6e74  roid]..    print
+0001c040: 2827 436f 6d70 7574 6564 2074 6865 2062  ('Computed the b
+0001c050: 6f75 6e64 6172 7920 706f 696e 7473 2729  oundary points')
+0001c060: 0d0a 0d0a 2020 2020 7265 7475 726e 2074  ....    return t
+0001c070: 696d 6564 5f6d 6173 6b2c 2062 6f75 6e64  imed_mask, bound
+0001c080: 6172 7920 2020 2020 2020 200d 0a0d 0a64  ary        ....d
+0001c090: 6566 2063 6f6d 7075 7465 5f63 656e 7472  ef compute_centr
+0001c0a0: 6f69 6428 6269 6e61 7279 5f69 6d61 6765  oid(binary_image
+0001c0b0: 293a 0d0a 2020 2020 2320 456e 7375 7265  ):..    # Ensure
+0001c0c0: 2062 696e 6172 7920 696d 6167 6520 6973   binary image is
+0001c0d0: 2061 204e 756d 5079 2061 7272 6179 0d0a   a NumPy array..
+0001c0e0: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
+0001c0f0: 203d 206e 702e 6172 7261 7928 6269 6e61   = np.array(bina
+0001c100: 7279 5f69 6d61 6765 290d 0a0d 0a20 2020  ry_image)....   
+0001c110: 2077 6869 7465 5f70 6978 656c 7320 3d20   white_pixels = 
+0001c120: 6e70 2e77 6865 7265 2862 696e 6172 795f  np.where(binary_
+0001c130: 696d 6167 6520 3d3d 2031 290d 0a20 2020  image == 1)..   
+0001c140: 206e 756d 5f70 6978 656c 7320 3d20 6c65   num_pixels = le
+0001c150: 6e28 7768 6974 655f 7069 7865 6c73 5b30  n(white_pixels[0
+0001c160: 5d29 0d0a 0d0a 2020 2020 2320 436f 6d70  ])....    # Comp
+0001c170: 7574 6520 7468 6520 6365 6e74 726f 6964  ute the centroid
+0001c180: 206f 6620 7468 6520 7768 6974 6520 7069   of the white pi
+0001c190: 7865 6c73 2069 6e20 7468 6520 626f 756e  xels in the boun
+0001c1a0: 6461 7279 2069 6d61 6765 0d0a 2020 2020  dary image..    
+0001c1b0: 6365 6e74 726f 6964 203d 206e 702e 7a65  centroid = np.ze
+0001c1c0: 726f 7328 6269 6e61 7279 5f69 6d61 6765  ros(binary_image
+0001c1d0: 2e6e 6469 6d29 0d0a 2020 2020 666f 7220  .ndim)..    for 
+0001c1e0: 6469 6d20 696e 2072 616e 6765 2862 696e  dim in range(bin
+0001c1f0: 6172 795f 696d 6167 652e 6e64 696d 293a  ary_image.ndim):
+0001c200: 0d0a 2020 2020 2020 2020 6365 6e74 726f  ..        centro
+0001c210: 6964 5b64 696d 5d20 3d20 7768 6974 655f  id[dim] = white_
+0001c220: 7069 7865 6c73 5b64 696d 5d2e 7375 6d28  pixels[dim].sum(
+0001c230: 2920 2f20 6e75 6d5f 7069 7865 6c73 0d0a  ) / num_pixels..
+0001c240: 0d0a 2020 2020 7265 7475 726e 2063 656e  ..    return cen
+0001c250: 7472 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a  troid........ ..
+0001c260: 0d0a 6465 6620 6765 745f 6373 765f 6461  ..def get_csv_da
+0001c270: 7461 2863 7376 293a 0d0a 0d0a 2020 2020  ta(csv):....    
+0001c280: 2020 2020 6461 7461 7365 7420 3d20 7064      dataset = pd
+0001c290: 2e72 6561 645f 6373 7628 0d0a 2020 2020  .read_csv(..    
+0001c2a0: 2020 2020 2020 2020 6373 762c 2064 656c          csv, del
+0001c2b0: 696d 6974 6572 3d22 2c22 2c20 656e 636f  imiter=",", enco
+0001c2c0: 6469 6e67 3d22 756e 6963 6f64 655f 6573  ding="unicode_es
+0001c2d0: 6361 7065 222c 206c 6f77 5f6d 656d 6f72  cape", low_memor
+0001c2e0: 793d 4661 6c73 650d 0a20 2020 2020 2020  y=False..       
+0001c2f0: 2029 5b33 3a5d 0d0a 2020 2020 2020 2020   )[3:]..        
+0001c300: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
+0001c310: 6461 7461 7365 742e 696e 6465 780d 0a20  dataset.index.. 
+0001c320: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+0001c330: 7461 7365 742c 2064 6174 6173 6574 5f69  taset, dataset_i
+0001c340: 6e64 6578 0d0a 2020 2020 0d0a 6465 6620  ndex..    ..def 
+0001c350: 6765 745f 7370 6f74 5f64 6174 6173 6574  get_spot_dataset
+0001c360: 2873 706f 745f 6461 7461 7365 742c 2074  (spot_dataset, t
+0001c370: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001c380: 6f74 5f6b 6579 732c 2078 6361 6c69 6272  ot_keys, xcalibr
+0001c390: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
+0001c3a0: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
+0001c3b0: 6e2c 2041 7474 7269 6275 7465 426f 786e  n, AttributeBoxn
+0001c3c0: 616d 652c 2064 6574 6563 7469 6f6e 6368  ame, detectionch
+0001c3d0: 616e 6e65 6c29 3a0d 0a20 2020 2020 2020  annel):..       
+0001c3e0: 2041 6c6c 5661 6c75 6573 203d 207b 7d0d   AllValues = {}.
+0001c3f0: 0a20 2020 2020 2020 2070 6f73 6978 203d  .        posix =
+0001c400: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001c410: 7370 6f74 5f6b 6579 735b 2270 6f73 6978  spot_keys["posix
+0001c420: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
+0001c430: 7920 3d20 7472 6163 6b5f 616e 616c 7973  y = track_analys
+0001c440: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+0001c450: 7369 7922 5d0d 0a20 2020 2020 2020 2070  siy"]..        p
+0001c460: 6f73 697a 203d 2074 7261 636b 5f61 6e61  osiz = track_ana
+0001c470: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001c480: 2270 6f73 697a 225d 0d0a 2020 2020 2020  "posiz"]..      
+0001c490: 2020 6672 616d 6520 3d20 7472 6163 6b5f    frame = track_
+0001c4a0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001c4b0: 7973 5b22 6672 616d 6522 5d0d 0a20 2020  ys["frame"]..   
+0001c4c0: 2020 2020 200d 0a20 2020 2020 2020 204c       ..        L
+0001c4d0: 6f63 6174 696f 6e58 203d 2028 0d0a 2020  ocationX = (..  
+0001c4e0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001c4f0: 6174 6173 6574 5b70 6f73 6978 5d2e 6173  ataset[posix].as
+0001c500: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001c510: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+0001c520: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001c530: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001c540: 6f63 6174 696f 6e59 203d 2028 0d0a 2020  ocationY = (..  
+0001c550: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001c560: 6174 6173 6574 5b70 6f73 6979 5d2e 6173  ataset[posiy].as
+0001c570: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001c580: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+0001c590: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001c5a0: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001c5b0: 6f63 6174 696f 6e5a 203d 2028 0d0a 2020  ocationZ = (..  
+0001c5c0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001c5d0: 6174 6173 6574 5b70 6f73 697a 5d2e 6173  ataset[posiz].as
+0001c5e0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001c5f0: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+0001c600: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001c610: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001c620: 6f63 6174 696f 6e54 203d 2028 7370 6f74  ocationT = (spot
+0001c630: 5f64 6174 6173 6574 5b66 7261 6d65 5d2e  _dataset[frame].
+0001c640: 6173 7479 7065 2822 666c 6f61 7422 2929  astype("float"))
+0001c650: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+0001c660: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0001c670: 2020 2020 6967 6e6f 7265 5f76 616c 7565      ignore_value
+0001c680: 7320 3d20 5b74 7261 636b 5f61 6e61 6c79  s = [track_analy
+0001c690: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+0001c6a0: 6561 6e5f 696e 7465 6e73 6974 7922 5d2c  ean_intensity"],
+0001c6b0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001c6c0: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
+0001c6d0: 696e 7465 6e73 6974 7922 5d5d 0d0a 2020  intensity"]]..  
+0001c6e0: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+0001c6f0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001c700: 735f 7370 6f74 5f6b 6579 732e 6974 656d  s_spot_keys.item
+0001c710: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001c720: 2020 2020 2020 2020 6966 2064 6574 6563          if detec
+0001c730: 7469 6f6e 6368 616e 6e65 6c20 3d3d 2031  tionchannel == 1
+0001c740: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001c750: 2020 2020 2020 2020 6966 206b 203d 3d20          if k == 
+0001c760: 226d 6561 6e5f 696e 7465 6e73 6974 795f  "mean_intensity_
+0001c770: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
+0001c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c790: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
+0001c7a0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001c7b0: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
+0001c7c0: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
+0001c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c7e0: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
+0001c7f0: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001c800: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001c810: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0001c820: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
+0001c830: 3d20 2274 6f74 616c 5f69 6e74 656e 7369  = "total_intensi
+0001c840: 7479 5f63 6832 223a 0d0a 2020 2020 2020  ty_ch2":..      
+0001c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c860: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
+0001c870: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001c880: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
+0001c890: 656e 7369 7479 225d 0d0a 2020 2020 2020  ensity"]..      
+0001c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c8b0: 2020 2020 2041 6c6c 5661 6c75 6573 5b76       AllValues[v
+0001c8c0: 616c 7565 5d20 3d20 7370 6f74 5f64 6174  alue] = spot_dat
+0001c8d0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001c8e0: 666c 6f61 7422 2920 2020 2020 2020 0d0a  float")       ..
+0001c8f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c900: 2020 6966 2076 206e 6f74 2069 6e20 6967    if v not in ig
+0001c910: 6e6f 7265 5f76 616c 7565 733a 0d0a 2020  nore_values:..  
+0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c930: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0001c940: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001c950: 6c56 616c 7565 735b 765d 203d 2073 706f  lValues[v] = spo
+0001c960: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
+0001c970: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c990: 200d 0a0d 0a20 2020 2020 2020 2041 6c6c   ....        All
+0001c9a0: 5661 6c75 6573 5b70 6f73 6978 5d20 3d20  Values[posix] = 
+0001c9b0: 726f 756e 6428 4c6f 6361 7469 6f6e 582c  round(LocationX,
+0001c9c0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+0001c9d0: 616c 7565 735b 706f 7369 795d 203d 2072  alues[posiy] = r
+0001c9e0: 6f75 6e64 284c 6f63 6174 696f 6e59 2c33  ound(LocationY,3
+0001c9f0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
+0001ca00: 6c75 6573 5b70 6f73 697a 5d20 3d20 726f  lues[posiz] = ro
+0001ca10: 756e 6428 4c6f 6361 7469 6f6e 5a2c 3329  und(LocationZ,3)
+0001ca20: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
+0001ca30: 7565 735b 6672 616d 655d 203d 2072 6f75  ues[frame] = rou
+0001ca40: 6e64 284c 6f63 6174 696f 6e54 2c33 290d  nd(LocationT,3).
+0001ca50: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+0001ca60: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
+0001ca70: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
+0001ca80: 2e61 7070 656e 6428 4174 7472 6962 7574  .append(Attribut
+0001ca90: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
+0001caa0: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
+0001cab0: 6e61 6d65 2069 6e20 416c 6c56 616c 7565  name in AllValue
+0001cac0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+0001cad0: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
+0001cae0: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001caf0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001cb00: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0001cb10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001cb20: 2072 6574 7572 6e20 4174 7472 6962 7574   return Attribut
+0001cb30: 6569 6473 2c20 416c 6c56 616c 7565 7320  eids, AllValues 
+0001cb40: 2020 2020 0d0a 2020 2020 0d0a 0d0a 6465      ..    ....de
+0001cb50: 6620 6765 745f 7472 6163 6b5f 6461 7461  f get_track_data
+0001cb60: 7365 7428 7472 6163 6b5f 6461 7461 7365  set(track_datase
+0001cb70: 742c 2074 7261 636b 5f61 6e61 6c79 7369  t, track_analysi
+0001cb80: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
+0001cb90: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
+0001cba0: 6b5f 6b65 7973 2c20 5472 6163 6b41 7474  k_keys, TrackAtt
+0001cbb0: 7269 6275 7465 426f 786e 616d 6529 3a0d  ributeBoxname):.
+0001cbc0: 0a0d 0a20 2020 2020 2020 2041 6c6c 5472  ...        AllTr
+0001cbd0: 6163 6b56 616c 7565 7320 3d20 7b7d 0d0a  ackValues = {}..
+0001cbe0: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+0001cbf0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+0001cc00: 735f 7370 6f74 5f6b 6579 735b 2274 7261  s_spot_keys["tra
+0001cc10: 636b 5f69 6422 5d0d 0a20 2020 2020 2020  ck_id"]..       
+0001cc20: 2054 6964 203d 2074 7261 636b 5f64 6174   Tid = track_dat
+0001cc30: 6173 6574 5b74 7261 636b 5f69 645d 2e61  aset[track_id].a
+0001cc40: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
+0001cc50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001cc60: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
+0001cc70: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
+0001cc80: 0a20 2020 2020 200d 0a20 2020 2020 2020  .      ..       
+0001cc90: 2066 6f72 2028 6b2c 2076 2920 696e 2074   for (k, v) in t
+0001cca0: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
+0001ccb0: 6163 6b5f 6b65 7973 2e69 7465 6d73 2829  ack_keys.items()
+0001ccc0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001ccd0: 2020 2020 2078 203d 2074 7261 636b 5f64       x = track_d
+0001cce0: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+0001ccf0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+0001cd00: 2020 2020 2020 2020 2020 206d 696e 7661             minva
+0001cd10: 6c20 3d20 6d69 6e28 7829 0d0a 2020 2020  l = min(x)..    
+0001cd20: 2020 2020 2020 2020 2020 2020 6d61 7876              maxv
+0001cd30: 616c 203d 206d 6178 2878 290d 0a0d 0a20  al = max(x).... 
+0001cd40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001cd50: 6620 6d69 6e76 616c 203e 2030 2061 6e64  f minval > 0 and
+0001cd60: 206d 6178 7661 6c20 3c3d 2031 3a0d 0a0d   maxval <= 1:...
+0001cd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cd80: 2020 2020 2078 203d 2078 202b 2031 0d0a       x = x + 1..
+0001cd90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001cda0: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+0001cdb0: 5b6b 5d20 3d20 726f 756e 6428 782c 2033  [k] = round(x, 3
+0001cdc0: 290d 0a0d 0a20 2020 2020 2020 2054 7261  )....        Tra
+0001cdd0: 636b 4174 7472 6962 7574 6569 6473 203d  ckAttributeids =
+0001cde0: 205b 5d0d 0a20 2020 2020 2020 2054 7261   []..        Tra
+0001cdf0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
+0001ce00: 7070 656e 6428 5472 6163 6b41 7474 7269  ppend(TrackAttri
+0001ce10: 6275 7465 426f 786e 616d 6529 0d0a 2020  buteBoxname)..  
+0001ce20: 2020 2020 2020 666f 7220 6174 7472 6962        for attrib
+0001ce30: 7574 656e 616d 6520 696e 2074 7261 636b  utename in track
+0001ce40: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001ce50: 6b65 7973 2e6b 6579 7328 293a 0d0a 2020  keys.keys():..  
+0001ce60: 2020 2020 2020 2020 2020 5472 6163 6b41            TrackA
+0001ce70: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
+0001ce80: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
+0001ce90: 2920 2020 200d 0a20 2020 200d 0a20 2020  )    ..    ..   
+0001cea0: 2020 2020 2072 6574 7572 6e20 5472 6163       return Trac
+0001ceb0: 6b41 7474 7269 6275 7465 6964 732c 2041  kAttributeids, A
+0001cec0: 6c6c 5472 6163 6b56 616c 7565 730d 0a20  llTrackValues.. 
+0001ced0: 2020 200d 0a64 6566 2067 6574 5f65 6467     ..def get_edg
+0001cee0: 6573 5f64 6174 6173 6574 2865 6467 6573  es_dataset(edges
+0001cef0: 5f64 6174 6173 6574 2c20 6564 6765 735f  _dataset, edges_
+0001cf00: 6461 7461 7365 745f 696e 6465 782c 2074  dataset_index, t
+0001cf10: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001cf20: 6f74 5f6b 6579 732c 2074 7261 636b 5f61  ot_keys, track_a
+0001cf30: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
+0001cf40: 7973 293a 0d0a 0d0a 2020 2020 2020 2020  ys):....        
+0001cf50: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
+0001cf60: 207b 7d0d 0a20 2020 2020 2020 2074 7261   {}..        tra
+0001cf70: 636b 5f69 6420 3d20 7472 6163 6b5f 616e  ck_id = track_an
+0001cf80: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001cf90: 5b22 7472 6163 6b5f 6964 225d 0d0a 2020  ["track_id"]..  
+0001cfa0: 2020 2020 2020 5469 6420 3d20 6564 6765        Tid = edge
+0001cfb0: 735f 6461 7461 7365 745b 7472 6163 6b5f  s_dataset[track_
+0001cfc0: 6964 5d2e 6173 7479 7065 2822 666c 6f61  id].astype("floa
+0001cfd0: 7422 290d 0a20 2020 2020 2020 2069 6e64  t")..        ind
+0001cfe0: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
+0001cff0: 5469 6420 3d3d 2030 290d 0a20 2020 2020  Tid == 0)..     
+0001d000: 2020 206d 6178 7472 6163 6b5f 6964 203d     maxtrack_id =
+0001d010: 206d 6178 2854 6964 290d 0a20 2020 2020   max(Tid)..     
+0001d020: 2020 2063 6f6e 6469 7469 6f6e 5f69 6e64     condition_ind
+0001d030: 6963 6573 203d 2065 6467 6573 5f64 6174  ices = edges_dat
+0001d040: 6173 6574 5f69 6e64 6578 5b69 6e64 6963  aset_index[indic
+0001d050: 6573 5d0d 0a20 2020 2020 2020 2054 6964  es]..        Tid
+0001d060: 5b63 6f6e 6469 7469 6f6e 5f69 6e64 6963  [condition_indic
+0001d070: 6573 5d20 3d20 6d61 7874 7261 636b 5f69  es] = maxtrack_i
+0001d080: 6420 2b20 310d 0a20 2020 2020 2020 2041  d + 1..        A
+0001d090: 6c6c 4564 6765 7356 616c 7565 735b 7472  llEdgesValues[tr
+0001d0a0: 6163 6b5f 6964 5d20 3d20 5469 640d 0a0d  ack_id] = Tid...
+0001d0b0: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
+0001d0c0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001d0d0: 5f65 6467 6573 5f6b 6579 732e 7661 6c75  _edges_keys.valu
+0001d0e0: 6573 2829 3a0d 0a0d 0a20 2020 2020 2020  es():....       
+0001d0f0: 2020 2020 2069 6620 6b20 213d 2074 7261       if k != tra
+0001d100: 636b 5f69 643a 0d0a 2020 2020 2020 2020  ck_id:..        
+0001d110: 2020 2020 2020 2020 7820 3d20 6564 6765          x = edge
+0001d120: 735f 6461 7461 7365 745b 6b5d 2e61 7374  s_dataset[k].ast
+0001d130: 7970 6528 2266 6c6f 6174 2229 0d0a 0d0a  ype("float")....
+0001d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d150: 416c 6c45 6467 6573 5661 6c75 6573 5b6b  AllEdgesValues[k
+0001d160: 5d20 3d20 7820 2020 0d0a 2020 2020 2020  ] = x   ..      
+0001d170: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001d180: 7572 6e20 416c 6c45 6467 6573 5661 6c75  urn AllEdgesValu
+0001d190: 6573 2020 200d 0a20 2020 200d 0a20 2020  es   ..    ..   
+0001d1a0: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
+0001d1b0: 7363 616c 655f 7661 6c75 6528 782c 2073  scale_value(x, s
+0001d1c0: 6361 6c65 203d 2032 3535 202a 2032 3535  cale = 255 * 255
+0001d1d0: 293a 0d0a 0d0a 0d0a 2020 2020 2072 6574  ):......     ret
+0001d1e0: 7572 6e20 7820 2a20 7363 616c 6520 2020  urn x * scale   
+0001d1f0: 0d0a 2020 2020 0d0a 0d0a 0d0a 6465 6620  ..    ......def 
+0001d200: 7072 6f62 5f73 6967 6d6f 6964 2878 293a  prob_sigmoid(x):
+0001d210: 0d0a 2020 2020 7265 7475 726e 2031 202d  ..    return 1 -
+0001d220: 206d 6174 682e 6578 7028 2d78 290d 0a0d   math.exp(-x)...
+0001d230: 0a0d 0a64 6566 2061 6e67 756c 6172 5f63  ...def angular_c
+0001d240: 6861 6e67 6528 7665 635f 302c 2076 6563  hange(vec_0, vec
+0001d250: 5f31 293a 0d0a 2020 2020 2020 2020 0d0a  _1):..        ..
+0001d260: 2020 2020 2020 2020 7665 635f 3020 3d20          vec_0 = 
+0001d270: 7665 635f 3020 2f20 6e70 2e6c 696e 616c  vec_0 / np.linal
+0001d280: 672e 6e6f 726d 2876 6563 5f30 290d 0a20  g.norm(vec_0).. 
+0001d290: 2020 2020 2020 2076 6563 5f31 203d 2076         vec_1 = v
+0001d2a0: 6563 5f31 202f 206e 702e 6c69 6e61 6c67  ec_1 / np.linalg
+0001d2b0: 2e6e 6f72 6d28 7665 635f 3129 0d0a 2020  .norm(vec_1)..  
+0001d2c0: 2020 2020 2020 616e 676c 6520 3d20 6e70        angle = np
+0001d2d0: 2e61 7263 636f 7328 6e70 2e63 6c69 7028  .arccos(np.clip(
+0001d2e0: 6e70 2e64 6f74 2876 6563 5f30 2c20 7665  np.dot(vec_0, ve
+0001d2f0: 635f 3129 2c20 2d31 2e30 2c20 312e 3029  c_1), -1.0, 1.0)
+0001d300: 290d 0a20 2020 2020 2020 2061 6e67 6c65  )..        angle
+0001d310: 203d 2061 6e67 6c65 202a 2031 3830 202f   = angle * 180 /
+0001d320: 206e 702e 7069 0d0a 2020 2020 2020 2020   np.pi..        
+0001d330: 7265 7475 726e 2061 6e67 6c65 0d0a 2020  return angle..  
+0001d340: 2020 200d 0a0d 0a64 6566 2065 7661 6c5f     ....def eval_
+0001d350: 626f 6f6c 2876 616c 7565 293a 0d0a 2020  bool(value):..  
+0001d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d370: 0d0a 2020 2020 2020 2020 6966 2076 616c  ..        if val
+0001d380: 7565 2020 3d3d 2027 5472 7565 273a 200d  ue  == 'True': .
+0001d390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d3a0: 2064 6976 5f6b 6579 203d 2054 7275 650d   div_key = True.
+0001d3b0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+0001d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3d0: 6469 765f 6b65 7920 3d20 4661 6c73 6520  div_key = False 
+0001d3e0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+0001d3f0: 726e 2064 6976 5f6b 6579 2020 2020 2020  rn div_key      
+0001d400: 2020 2020 2020 2020 2020 0d0a 0d0a 6465            ....de
+0001d410: 6620 6368 6563 6b5f 616e 645f 7570 6461  f check_and_upda
+0001d420: 7465 5f6d 6173 6b28 6d61 736b 2c69 6d61  te_mask(mask,ima
+0001d430: 6765 293a 0d0a 2020 2020 2020 200d 0a20  ge):..       .. 
+0001d440: 2020 2020 2020 2069 6620 6c65 6e28 6d61         if len(ma
+0001d450: 736b 2e73 6861 7065 2920 3c20 6c65 6e28  sk.shape) < len(
+0001d460: 696d 6167 652e 7368 6170 6529 3a0d 0a20  image.shape):.. 
+0001d470: 2020 2020 2020 2020 2020 2075 7064 6174             updat
+0001d480: 655f 6d61 736b 203d 206e 702e 7a65 726f  e_mask = np.zero
+0001d490: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4b0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4d0: 2020 2069 6d61 6765 2e73 6861 7065 5b30     image.shape[0
+0001d4e0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d500: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001d510: 315d 2c0d 0a20 2020 2020 2020 2020 2020  1],..           
+0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d530: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001d540: 5b32 5d2c 0d0a 2020 2020 2020 2020 2020  [2],..          
+0001d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d560: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001d570: 655b 335d 2c0d 0a20 2020 2020 2020 2020  e[3],..         
+0001d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d590: 2020 205d 2c20 6474 7970 653d 2275 696e     ], dtype="uin
+0001d5a0: 7438 220d 0a20 2020 2020 2020 2020 2020  t8"..           
+0001d5b0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001d5c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001d5d0: 6920 696e 2072 616e 6765 2830 2c20 7570  i in range(0, up
+0001d5e0: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
+0001d5f0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+0001d600: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+0001d610: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
+0001d620: 6173 6b2e 7368 6170 655b 315d 293a 0d0a  ask.shape[1]):..
+0001d630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d640: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
+0001d650: 6b5b 692c 206a 2c20 3a2c 203a 5d20 3d20  k[i, j, :, :] = 
+0001d660: 6d61 736b 5b69 2c20 3a2c 203a 5d0d 0a20  mask[i, :, :].. 
+0001d670: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001d680: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0001d690: 6461 7465 5f6d 6173 6b20 3d20 6d61 736b  date_mask = mask
+0001d6a0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
+0001d6b0: 726e 2075 7064 6174 655f 6d61 736b 2020  rn update_mask  
+0001d6c0: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
+0001d6d0: 0a                                       .
```

### Comparing `napatrackmater-4.0.0/napatrackmater/Trackvector.py` & `napatrackmater-4.0.1/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/__init__.py` & `napatrackmater-4.0.1/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/clustering.py` & `napatrackmater-4.0.1/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/fast_radius_regression.py` & `napatrackmater-4.0.1/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/fate_mapping.py` & `napatrackmater-4.0.1/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater/pretrained.py` & `napatrackmater-4.0.1/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-4.0.1/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 4.0.0
+Version: 4.0.1
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-4.0.0/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-4.0.1/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-4.0.0/setup.py` & `napatrackmater-4.0.1/setup.py`

 * *Files identical despite different names*

