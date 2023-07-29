# Comparing `tmp/napatrackmater-3.9.5.tar.gz` & `tmp/napatrackmater-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.9.5.tar", last modified: Sat Jul 29 16:29:02 2023, max compression
+gzip compressed data, was "napatrackmater-3.9.6.tar", last modified: Sat Jul 29 16:36:26 2023, max compression
```

## Comparing `napatrackmater-3.9.5.tar` & `napatrackmater-3.9.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:29:02.952074 napatrackmater-3.9.5/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:29:02.951971 napatrackmater-3.9.5/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:29:02.950982 napatrackmater-3.9.5/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   114117 2023-07-29 16:28:30.000000 napatrackmater-3.9.5/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 16:28:33.000000 napatrackmater-3.9.5/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:29:02.951803 napatrackmater-3.9.5/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 16:29:02.000000 napatrackmater-3.9.5/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 16:29:02.952109 napatrackmater-3.9.5/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.5/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:36:26.228767 napatrackmater-3.9.6/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:36:26.228668 napatrackmater-3.9.6/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:36:26.227867 napatrackmater-3.9.6/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   114144 2023-07-29 16:35:11.000000 napatrackmater-3.9.6/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 16:35:52.000000 napatrackmater-3.9.6/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:36:26.228523 napatrackmater-3.9.6/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 16:36:26.000000 napatrackmater-3.9.6/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 16:36:26.228798 napatrackmater-3.9.6/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.6/setup.py
```

### Comparing `napatrackmater-3.9.5/LICENSE` & `napatrackmater-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/PKG-INFO` & `napatrackmater-3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.5
+Version: 3.9.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.5/README.md` & `napatrackmater-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.9.6/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.9.6/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/Trackmate.py` & `napatrackmater-3.9.6/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,6329 +805,6330 @@
 00003240: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
 00003250: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
 00003260: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
 00003270: 626f 7865 730d 0a20 2020 2020 2020 2020  boxes..         
 00003280: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
 00003290: 745f 6174 7472 6962 7574 6573 2873 656c  t_attributes(sel
 000032a0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-000032b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000032c0: 7365 6c66 2e41 7474 7269 6275 7465 6964  self.Attributeid
-000032d0: 732c 2073 656c 662e 416c 6c56 616c 7565  s, self.AllValue
-000032e0: 7320 3d20 2067 6574 5f73 706f 745f 6461  s =  get_spot_da
-000032f0: 7461 7365 7428 7365 6c66 2e73 706f 745f  taset(self.spot_
-00003300: 6461 7461 7365 742c 2073 656c 662e 7472  dataset, self.tr
-00003310: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00003320: 745f 6b65 7973 2c20 7365 6c66 2e78 6361  t_keys, self.xca
-00003330: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
-00003340: 7963 616c 6962 7261 7469 6f6e 2c20 7365  ycalibration, se
-00003350: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-00003360: 2073 656c 662e 4174 7472 6962 7574 6542   self.AttributeB
-00003370: 6f78 6e61 6d65 2c20 7365 6c66 2e64 6574  oxname, self.det
-00003380: 6563 746f 7263 6861 6e6e 656c 290d 0a20  ectorchannel).. 
-00003390: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000033a0: 7428 276f 6274 6961 6e65 6420 7370 6f74  t('obtianed spot
-000033b0: 2061 7474 7269 6275 7465 7327 290d 0a20   attributes').. 
-000033c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000033d0: 2e54 7261 636b 4174 7472 6962 7574 6569  .TrackAttributei
-000033e0: 6473 2c20 7365 6c66 2e41 6c6c 5472 6163  ds, self.AllTrac
-000033f0: 6b56 616c 7565 7320 3d20 6765 745f 7472  kValues = get_tr
-00003400: 6163 6b5f 6461 7461 7365 7428 7365 6c66  ack_dataset(self
-00003410: 2e74 7261 636b 5f64 6174 6173 6574 2c20  .track_dataset, 
-00003420: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00003430: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-00003440: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-00003450: 7369 735f 7472 6163 6b5f 6b65 7973 2c20  sis_track_keys, 
-00003460: 7365 6c66 2e54 7261 636b 4174 7472 6962  self.TrackAttrib
-00003470: 7574 6542 6f78 6e61 6d65 290d 0a20 2020  uteBoxname)..   
-00003480: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003490: 276f 6274 6169 6e65 6420 7472 6163 6b20  'obtained track 
-000034a0: 6174 7472 6962 7574 6573 2729 0d0a 2020  attributes')..  
-000034b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000034c0: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
-000034d0: 2067 6574 5f65 6467 6573 5f64 6174 6173   get_edges_datas
-000034e0: 6574 2873 656c 662e 6564 6765 735f 6461  et(self.edges_da
-000034f0: 7461 7365 742c 2073 656c 662e 6564 6765  taset, self.edge
-00003500: 735f 6461 7461 7365 745f 696e 6465 782c  s_dataset_index,
-00003510: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
-00003520: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
-00003530: 7365 6c66 2e74 7261 636b 5f61 6e61 6c79  self.track_analy
-00003540: 7369 735f 6564 6765 735f 6b65 7973 290d  sis_edges_keys).
-00003550: 0a20 2020 2020 2020 2020 2020 2020 7072  .             pr
-00003560: 696e 7428 276f 6274 6169 6e65 6420 6564  int('obtained ed
-00003570: 6765 2061 7474 7269 6275 7465 7327 290d  ge attributes').
-00003580: 0a0d 0a20 2020 200d 0a20 2020 2020 2020  ...    ..       
-00003590: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000035a0: 2020 2064 6566 205f 6765 745f 626f 756e     def _get_boun
-000035b0: 6461 7279 5f70 6f69 6e74 7328 7365 6c66  dary_points(self
-000035c0: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-000035d0: 2020 2020 2020 2070 7269 6e74 2827 436f         print('Co
-000035e0: 6d70 7574 696e 6720 626f 756e 6461 7279  mputing boundary
-000035f0: 2070 6f69 6e74 7327 2920 0d0a 2020 2020   points') ..    
-00003600: 2020 2020 6966 2020 7365 6c66 2e6d 6173      if  self.mas
-00003610: 6b20 6973 206e 6f74 204e 6f6e 653a 0d0a  k is not None:..
-00003620: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00003630: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-00003640: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-00003650: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00003660: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003680: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
-00003690: 203d 2063 6865 636b 5f61 6e64 5f75 7064   = check_and_upd
-000036a0: 6174 655f 6d61 736b 2873 656c 662e 6d61  ate_mask(self.ma
-000036b0: 736b 2c20 7365 6c66 2e63 6861 6e6e 656c  sk, self.channel
-000036c0: 5f73 6567 5f69 6d61 6765 290d 0a0d 0a20  _seg_image).... 
-000036d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000036e0: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
-000036f0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00003700: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00003710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003720: 2020 2020 2020 2020 2073 656c 662e 7570           self.up
-00003730: 6461 7465 5f6d 6173 6b20 3d20 6368 6563  date_mask = chec
-00003740: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
-00003750: 6b28 7365 6c66 2e6d 6173 6b2c 2073 656c  k(self.mask, sel
-00003760: 662e 7365 675f 696d 6167 6529 0d0a 2020  f.seg_image)..  
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00003790: 2020 6966 2073 656c 662e 7365 675f 696d    if self.seg_im
-000037a0: 6167 6520 6973 204e 6f6e 6520 616e 6420  age is None and 
-000037b0: 7365 6c66 2e69 6d61 6765 2069 7320 6e6f  self.image is no
-000037c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000037f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003800: 7570 6461 7465 5f6d 6173 6b20 3d20 6368  update_mask = ch
-00003810: 6563 6b5f 616e 645f 7570 6461 7465 5f6d  eck_and_update_m
-00003820: 6173 6b28 7365 6c66 2e6d 6173 6b2c 2073  ask(self.mask, s
-00003830: 656c 662e 696d 6167 6529 2020 2020 0d0a  elf.image)    ..
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00003860: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00003870: 736b 203d 2073 656c 662e 7570 6461 7465  sk = self.update
-00003880: 5f6d 6173 6b0d 0a20 2020 2020 2020 2020  _mask..         
-00003890: 2020 2073 656c 662e 7469 6d65 645f 6d61     self.timed_ma
-000038a0: 736b 2c20 7365 6c66 2e62 6f75 6e64 6172  sk, self.boundar
-000038b0: 7920 3d20 626f 756e 6461 7279 5f70 6f69  y = boundary_poi
-000038c0: 6e74 7328 7365 6c66 2e6d 6173 6b2c 2073  nts(self.mask, s
-000038d0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-000038e0: 2c20 7365 6c66 2e79 6361 6c69 6272 6174  , self.ycalibrat
-000038f0: 696f 6e2c 2073 656c 662e 7a63 616c 6962  ion, self.zcalib
-00003900: 7261 7469 6f6e 290d 0a20 2020 2020 2020  ration)..       
-00003910: 2065 6c69 6620 7365 6c66 2e6d 6173 6b20   elif self.mask 
-00003920: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-00003930: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-00003940: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-00003950: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00003960: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
-00003990: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
-000039a0: 2e73 6567 5f69 6d61 6765 2e73 6861 7065  .seg_image.shape
-000039b0: 2c20 6474 7970 653d 6e70 2e75 696e 7438  , dtype=np.uint8
-000039c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000039d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000039e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000039f0: 2e73 6567 5f69 6d61 6765 2069 7320 4e6f  .seg_image is No
-00003a00: 6e65 2061 6e64 2073 656c 662e 696d 6167  ne and self.imag
-00003a10: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-00003a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003a30: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
-00003a40: 655f 6d61 736b 203d 206e 702e 7a65 726f  e_mask = np.zero
-00003a50: 7328 7365 6c66 2e69 6d61 6765 2e73 6861  s(self.image.sha
-00003a60: 7065 2c20 6474 7970 653d 6e70 2e75 696e  pe, dtype=np.uin
-00003a70: 7438 2920 0d0a 2020 2020 2020 2020 2020  t8) ..          
-00003a80: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00003a90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003aa0: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
-00003ab0: 6e70 2e7a 6572 6f73 2873 656c 662e 696d  np.zeros(self.im
-00003ac0: 6167 6573 697a 652c 2064 7479 7065 3d6e  agesize, dtype=n
-00003ad0: 702e 7569 6e74 3829 2020 2020 2020 200d  p.uint8)       .
-00003ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003af0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00003b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003b10: 6d61 736b 203d 2073 656c 662e 7570 6461  mask = self.upda
-00003b20: 7465 5f6d 6173 6b0d 0a20 2020 2020 2020  te_mask..       
-00003b30: 2020 2020 2073 656c 662e 6d61 736b 5b3a       self.mask[:
-00003b40: 2c3a 2c31 3a2d 312c 313a 2d31 5d20 3d20  ,:,1:-1,1:-1] = 
-00003b50: 310d 0a20 2020 2020 2020 2020 2020 2073  1..            s
-00003b60: 656c 662e 7469 6d65 645f 6d61 736b 2c20  elf.timed_mask, 
-00003b70: 7365 6c66 2e62 6f75 6e64 6172 7920 3d20  self.boundary = 
-00003b80: 626f 756e 6461 7279 5f70 6f69 6e74 7328  boundary_points(
-00003b90: 7365 6c66 2e6d 6173 6b2c 2073 656c 662e  self.mask, self.
-00003ba0: 7863 616c 6962 7261 7469 6f6e 2c20 7365  xcalibration, se
-00003bb0: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-00003bc0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00003bd0: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
-00003be0: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
-00003bf0: 6765 6e65 7261 7465 5f67 656e 6572 6174  generate_generat
-00003c00: 696f 6e73 2873 656c 662c 2074 7261 636b  ions(self, track
-00003c10: 293a 0d0a 2020 2020 2020 2020 200d 0a20  ):..         .. 
-00003c20: 2020 2020 2020 2061 6c6c 5f73 6f75 7263         all_sourc
-00003c30: 655f 6964 7320 3d20 5b5d 0d0a 2020 2020  e_ids = []..    
-00003c40: 2020 2020 616c 6c5f 7461 7267 6574 5f69      all_target_i
-00003c50: 6473 203d 205b 5d20 0d0a 0d0a 0d0a 2020  ds = [] ......  
-00003c60: 2020 2020 2020 666f 7220 6564 6765 2069        for edge i
-00003c70: 6e20 7472 6163 6b2e 6669 6e64 616c 6c28  n track.findall(
-00003c80: 2745 6467 6527 293a 0d0a 0d0a 2020 2020  'Edge'):....    
-00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ca0: 2020 2020 2020 2020 736f 7572 6365 5f69          source_i
-00003cb0: 6420 3d20 696e 7428 6564 6765 2e67 6574  d = int(edge.get
-00003cc0: 2873 656c 662e 7370 6f74 5f73 6f75 7263  (self.spot_sourc
-00003cd0: 655f 6964 5f6b 6579 2929 0d0a 2020 2020  e_id_key))..    
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2020 2020 2020 7461 7267 6574 5f69          target_i
-00003d00: 6420 3d20 696e 7428 6564 6765 2e67 6574  d = int(edge.get
-00003d10: 2873 656c 662e 7370 6f74 5f74 6172 6765  (self.spot_targe
-00003d20: 745f 6964 5f6b 6579 2929 0d0a 2020 2020  t_id_key))..    
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2020 2020 616c 6c5f 736f 7572          all_sour
-00003d50: 6365 5f69 6473 2e61 7070 656e 6428 736f  ce_ids.append(so
-00003d60: 7572 6365 5f69 6429 0d0a 2020 2020 2020  urce_id)..      
-00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2020 2020 2020 616c 6c5f 7461 7267 6574        all_target
-00003d90: 5f69 6473 2e61 7070 656e 6428 7461 7267  _ids.append(targ
-00003da0: 6574 5f69 6429 0d0a 2020 2020 2020 2020  et_id)..        
-00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003dc0: 2020 2020 6966 2073 6f75 7263 655f 6964      if source_id
-00003dd0: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
-00003de0: 7267 6574 5f6c 6f6f 6b75 702e 6b65 7973  rget_lookup.keys
-00003df0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 2020 7365 6c66 2e65 6467 655f 7461      self.edge_ta
-00003e20: 7267 6574 5f6c 6f6f 6b75 705b 736f 7572  rget_lookup[sour
-00003e30: 6365 5f69 645d 2e61 7070 656e 6428 7461  ce_id].append(ta
-00003e40: 7267 6574 5f69 6429 0d0a 2020 2020 2020  rget_id)..      
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e60: 2020 2020 2020 656c 7365 3a20 2020 2020        else:     
-00003e70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 7365 6c66 2e65 6467 655f 7461 7267    self.edge_targ
-00003ea0: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00003eb0: 5f69 645d 203d 205b 7461 7267 6574 5f69  _id] = [target_i
-00003ec0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-00003ef0: 5f6c 6f6f 6b75 705b 7461 7267 6574 5f69  _lookup[target_i
-00003f00: 645d 203d 2073 6f75 7263 655f 6964 200d  d] = source_id .
-00003f10: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00003f20: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
-00003f30: 2c20 616c 6c5f 7461 7267 6574 5f69 6473  , all_target_ids
-00003f40: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
-00003f50: 6372 6561 7465 5f67 656e 6572 6174 696f  create_generatio
-00003f60: 6e73 2873 656c 662c 2061 6c6c 5f73 6f75  ns(self, all_sou
-00003f70: 7263 655f 6964 733a 206c 6973 7429 3a0d  rce_ids: list):.
-00003f80: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-00003f90: 2020 2020 726f 6f74 5f6c 6561 6620 3d20      root_leaf = 
-00003fa0: 5b5d 0d0a 2020 2020 2020 2020 726f 6f74  []..        root
-00003fb0: 5f72 6f6f 7420 3d20 5b5d 0d0a 2020 2020  _root = []..    
-00003fc0: 2020 2020 726f 6f74 5f73 706c 6974 7320      root_splits 
-00003fd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2347  = []..        #G
-00003fe0: 6574 2074 6865 2072 6f6f 7420 6964 0d0a  et the root id..
-00003ff0: 2020 2020 2020 2020 666f 7220 736f 7572          for sour
-00004000: 6365 5f69 6420 696e 2061 6c6c 5f73 6f75  ce_id in all_sou
-00004010: 7263 655f 6964 733a 0d0a 2020 2020 2020  rce_ids:..      
-00004020: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
-00004030: 655f 6964 2069 6e20 7365 6c66 2e65 6467  e_id in self.edg
-00004040: 655f 736f 7572 6365 5f6c 6f6f 6b75 703a  e_source_lookup:
-00004050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004060: 2020 736f 7572 6365 5f74 6172 6765 745f    source_target_
-00004070: 6964 203d 2073 656c 662e 6564 6765 5f73  id = self.edge_s
-00004080: 6f75 7263 655f 6c6f 6f6b 7570 5b73 6f75  ource_lookup[sou
-00004090: 7263 655f 6964 5d0d 0a20 2020 2020 2020  rce_id]..       
-000040a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000040b0: 2020 2020 2020 2020 2020 2020 2020 736f                so
-000040c0: 7572 6365 5f74 6172 6765 745f 6964 203d  urce_target_id =
-000040d0: 204e 6f6e 6520 2020 2020 2020 2020 200d   None          .
-000040e0: 0a20 2020 2020 2020 2020 2020 2020 2074  .              t
-000040f0: 6172 6765 745f 7461 7267 6574 5f69 6420  arget_target_id 
-00004100: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
-00004110: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00004120: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00004130: 2020 2020 6966 2073 6f75 7263 655f 7461      if source_ta
-00004140: 7267 6574 5f69 6420 6973 204e 6f6e 653a  rget_id is None:
-00004150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004160: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00004170: 6420 6e6f 7420 696e 2072 6f6f 745f 726f  d not in root_ro
-00004180: 6f74 3a0d 0a20 2020 2020 2020 2020 2020  ot:..           
-00004190: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-000041a0: 726f 6f74 2e61 7070 656e 6428 736f 7572  root.append(sour
-000041b0: 6365 5f69 6429 200d 0a20 2020 2020 2020  ce_id) ..       
-000041c0: 2020 2020 2020 2069 6620 6c65 6e28 7461         if len(ta
-000041d0: 7267 6574 5f74 6172 6765 745f 6964 2920  rget_target_id) 
-000041e0: 3e20 313a 0d0a 2020 2020 2020 2020 2020  > 1:..          
-000041f0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
-00004200: 6365 5f69 6420 6e6f 7420 696e 2072 6f6f  ce_id not in roo
-00004210: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2072 6f6f 745f 7370 6c69 7473 2e61 7070   root_splits.app
-00004240: 656e 6428 736f 7572 6365 5f69 6429 0d0a  end(source_id)..
-00004250: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004260: 2074 6172 6765 745f 7461 7267 6574 5f69   target_target_i
-00004270: 645b 305d 206e 6f74 2069 6e20 7365 6c66  d[0] not in self
-00004280: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00004290: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-000042a0: 2020 2020 2020 2020 2072 6f6f 745f 6c65           root_le
-000042b0: 6166 2e61 7070 656e 6428 7461 7267 6574  af.append(target
-000042c0: 5f74 6172 6765 745f 6964 5b30 5d29 2020  _target_id[0])  
-000042d0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000042e0: 2020 2020 7265 7475 726e 2072 6f6f 745f      return root_
-000042f0: 726f 6f74 2c20 726f 6f74 5f73 706c 6974  root, root_split
-00004300: 732c 2072 6f6f 745f 6c65 6166 0d0a 0d0a  s, root_leaf....
-00004310: 2020 2020 6465 6620 5f73 6f72 745f 6469      def _sort_di
-00004320: 7669 6469 6e67 5f63 656c 6c73 2873 656c  viding_cells(sel
-00004330: 662c 2072 6f6f 745f 7370 6c69 7473 293a  f, root_splits):
-00004340: 0d0a 2020 2020 2020 2020 2020 2063 656c  ..           cel
-00004350: 6c5f 6964 5f74 696d 6573 203d 205b 5d0d  l_id_times = [].
-00004360: 0a20 2020 2020 2020 2020 2020 6365 6c6c  .           cell
-00004370: 5f69 6473 203d 205b 5d0d 0a20 2020 2020  _ids = []..     
-00004380: 2020 2020 2020 666f 7220 726f 6f74 5f73        for root_s
-00004390: 706c 6974 2069 6e20 726f 6f74 5f73 706c  plit in root_spl
-000043a0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-000043b0: 2020 2020 2020 2020 7370 6c69 745f 6365          split_ce
-000043c0: 6c6c 5f69 645f 7469 6d65 203d 2073 656c  ll_id_time = sel
-000043d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000043e0: 6f70 6572 7469 6573 5b72 6f6f 745f 7370  operties[root_sp
-000043f0: 6c69 745d 5b73 656c 662e 6672 616d 6569  lit][self.framei
-00004400: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-00004410: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-00004420: 645f 7469 6d65 732e 6170 7065 6e64 2873  d_times.append(s
-00004430: 706c 6974 5f63 656c 6c5f 6964 5f74 696d  plit_cell_id_tim
-00004440: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00004450: 2020 2020 2020 6365 6c6c 5f69 6473 2e61        cell_ids.a
-00004460: 7070 656e 6428 726f 6f74 5f73 706c 6974  ppend(root_split
-00004470: 290d 0a20 2020 2020 2020 2020 2020 736f  )..           so
-00004480: 7274 6564 5f69 6e64 6963 6573 203d 2073  rted_indices = s
-00004490: 6f72 7465 6428 7261 6e67 6528 6c65 6e28  orted(range(len(
-000044a0: 6365 6c6c 5f69 645f 7469 6d65 7329 292c  cell_id_times)),
-000044b0: 206b 6579 3d6c 616d 6264 6120 6b3a 2063   key=lambda k: c
-000044c0: 656c 6c5f 6964 5f74 696d 6573 5b6b 5d29  ell_id_times[k])
-000044d0: 0d0a 2020 2020 2020 2020 2020 2073 6f72  ..           sor
-000044e0: 7465 645f 6365 6c6c 5f69 6473 203d 205b  ted_cell_ids = [
-000044f0: 6365 6c6c 5f69 6473 5b69 5d20 666f 7220  cell_ids[i] for 
-00004500: 6920 696e 2073 6f72 7465 645f 696e 6469  i in sorted_indi
-00004510: 6365 735d 0d0a 0d0a 2020 2020 2020 2020  ces]....        
-00004520: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00004530: 5f63 656c 6c5f 6964 7320 2020 2020 2020  _cell_ids       
-00004540: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00004550: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00004560: 2020 6465 6620 5f69 7465 7261 7465 5f64    def _iterate_d
-00004570: 6976 6964 696e 675f 7265 6375 7273 6976  ividing_recursiv
-00004580: 6528 7365 6c66 2c20 726f 6f74 5f6c 6561  e(self, root_lea
-00004590: 662c 2074 6172 6765 745f 6365 6c6c 2c20  f, target_cell, 
-000045a0: 736f 7274 6564 5f72 6f6f 745f 7370 6c69  sorted_root_spli
-000045b0: 7473 2c20 6765 6e5f 636f 756e 742c 2074  ts, gen_count, t
-000045c0: 7261 636b 6c65 745f 636f 756e 742c 2074  racklet_count, t
-000045d0: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-000045e0: 6b65 6e29 3a0d 0a20 2020 2020 2020 2020  ken):..         
-000045f0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-00004600: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00004610: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00004620: 6e65 7261 7469 6f6e 5f64 6963 745b 7461  neration_dict[ta
-00004630: 7267 6574 5f63 656c 6c5d 203d 2067 656e  rget_cell] = gen
-00004640: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-00004650: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00004660: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
-00004670: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
-00004680: 6574 5f63 6f75 6e74 0d0a 0d0a 2020 2020  et_count....    
-00004690: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000046a0: 6172 6765 745f 6365 6c6c 203d 3d20 726f  arget_cell == ro
-000046b0: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
-000046c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000046d0: 7475 726e 0d0a 2020 2020 2020 2020 2020  turn..          
-000046e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000046f0: 2020 2020 2020 2020 6e65 7874 5f74 6172          next_tar
-00004700: 6765 745f 6365 6c6c 203d 204e 6f6e 650d  get_cell = None.
-00004710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004720: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004730: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-00004740: 6c20 696e 2073 6f72 7465 645f 726f 6f74  l in sorted_root
-00004750: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2020 206e 6578 745f 6765 6e5f 636f       next_gen_co
-00004780: 756e 7420 3d20 6765 6e5f 636f 756e 7420  unt = gen_count 
-00004790: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
-000047c0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-000047d0: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047f0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00004800: 6574 5f63 656c 6c73 203d 2073 656c 662e  et_cells = self.
-00004810: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00004820: 7570 5b74 6172 6765 745f 6365 6c6c 5d0d  up[target_cell].
-00004830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2066 6f72 206b 2069 6e20 7261 6e67 6528   for k in range(
-00004860: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
-00004870: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 2020 2020 2064 6175 6768 7465           daughte
-000048a0: 725f 7461 7267 6574 5f63 656c 6c20 3d20  r_target_cell = 
-000048b0: 7461 7267 6574 5f63 656c 6c73 5b6b 5d0d  target_cells[k].
-000048c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048e0: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
-000048f0: 756e 7420 3d20 7472 6163 6b6c 6574 5f63  unt = tracklet_c
-00004900: 6f75 6e74 202b 2031 202b 206b 0d0a 2020  ount + 1 + k..  
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 7472 6163 6b6c 6574 5f63 6f75 6e74    tracklet_count
-00004940: 203d 2073 656c 662e 5f75 6e69 7175 655f   = self._unique_
-00004950: 7472 6163 6b6c 6574 5f63 6f75 6e74 2874  tracklet_count(t
-00004960: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-00004970: 6b65 6e2c 2074 7261 636b 6c65 745f 636f  ken, tracklet_co
-00004980: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
-000049b0: 6574 5f63 6f75 6e74 5f74 616b 656e 2e61  et_count_taken.a
-000049c0: 7070 656e 6428 7472 6163 6b6c 6574 5f63  ppend(tracklet_c
-000049d0: 6f75 6e74 290d 0a20 2020 2020 2020 2020  ount)..         
-000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004a00: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
-00004a10: 675f 7265 6375 7273 6976 6528 726f 6f74  g_recursive(root
-00004a20: 5f6c 6561 662c 2064 6175 6768 7465 725f  _leaf, daughter_
-00004a30: 7461 7267 6574 5f63 656c 6c2c 2073 6f72  target_cell, sor
-00004a40: 7465 645f 726f 6f74 5f73 706c 6974 732c  ted_root_splits,
-00004a50: 206e 6578 745f 6765 6e5f 636f 756e 742c   next_gen_count,
-00004a60: 2074 7261 636b 6c65 745f 636f 756e 742c   tracklet_count,
-00004a70: 2074 7261 636b 6c65 745f 636f 756e 745f   tracklet_count_
-00004a80: 7461 6b65 6e29 2020 2020 2020 0d0a 0d0a  taken)      ....
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00004ab0: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
-00004ac0: 6365 6c6c 2069 6e20 7365 6c66 2e65 6467  cell in self.edg
-00004ad0: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
-00004ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004af0: 2020 2020 2020 6e65 7874 5f74 6172 6765        next_targe
-00004b00: 745f 6365 6c6c 7320 3d20 7365 6c66 2e65  t_cells = self.e
-00004b10: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004b20: 705b 7461 7267 6574 5f63 656c 6c5d 0d0a  p[target_cell]..
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2020 6e65 7874 5f74 6172 6765 745f      next_target_
-00004b50: 6365 6c6c 203d 206e 6578 745f 7461 7267  cell = next_targ
-00004b60: 6574 5f63 656c 6c73 5b30 5d0d 0a20 2020  et_cells[0]..   
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004bb0: 2020 2020 2020 7768 696c 6520 6e65 7874        while next
-00004bc0: 5f74 6172 6765 745f 6365 6c6c 206e 6f74  _target_cell not
-00004bd0: 2069 6e20 736f 7274 6564 5f72 6f6f 745f   in sorted_root_
-00004be0: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-00004c10: 5f64 6963 745b 6e65 7874 5f74 6172 6765  _dict[next_targe
-00004c20: 745f 6365 6c6c 5d20 3d20 6765 6e5f 636f  t_cell] = gen_co
-00004c30: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00004c40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00004c50: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-00004c60: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
-00004c70: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
-00004c80: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00004c90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00004ca0: 6578 745f 7461 7267 6574 5f63 656c 6c20  ext_target_cell 
-00004cb0: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004ce0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-00004cf0: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-00004d00: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004d30: 2e74 7261 636b 6c65 745f 6469 6374 5b74  .tracklet_dict[t
-00004d40: 6172 6765 745f 6365 6c6c 5d20 3d20 7472  arget_cell] = tr
-00004d50: 6163 6b6c 6574 5f63 6f75 6e74 0d0a 2020  acklet_count..  
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d70: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00004d80: 616b 0d0a 2020 2020 2020 2020 2020 2020  ak..            
-00004d90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00004da0: 6578 745f 7461 7267 6574 5f63 656c 6c20  ext_target_cell 
-00004db0: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
-00004dc0: 6765 745f 6c6f 6f6b 7570 3a0d 0a20 2020  get_lookup:..   
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00004df0: 7267 6574 5f63 656c 6c73 203d 2073 656c  rget_cells = sel
-00004e00: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-00004e10: 6f6b 7570 5b6e 6578 745f 7461 7267 6574  okup[next_target
-00004e20: 5f63 656c 6c5d 0d0a 2020 2020 2020 2020  _cell]..        
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 6e65 7874 5f74 6172 6765 745f      next_target_
-00004e50: 6365 6c6c 203d 206e 6578 745f 7461 7267  cell = next_targ
-00004e60: 6574 5f63 656c 6c73 5b30 5d0d 0a20 2020  et_cells[0]..   
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
-00004e90: 5f74 6172 6765 745f 6365 6c6c 2069 6e20  _target_cell in 
-00004ea0: 726f 6f74 5f6c 6561 663a 0d0a 2020 2020  root_leaf:..    
-00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004ed0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-00004ee0: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
-00004ef0: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00004f20: 6163 6b6c 6574 5f64 6963 745b 7461 7267  acklet_dict[targ
-00004f30: 6574 5f63 656c 6c5d 203d 2074 7261 636b  et_cell] = track
-00004f40: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-00004f70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00004f80: 2020 2069 6620 6e65 7874 5f74 6172 6765     if next_targe
-00004f90: 745f 6365 6c6c 2069 7320 6e6f 7420 4e6f  t_cell is not No
-00004fa0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00004fb0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00004fc0: 6e65 7261 7469 6f6e 5f64 6963 745b 6e65  neration_dict[ne
-00004fd0: 7874 5f74 6172 6765 745f 6365 6c6c 5d20  xt_target_cell] 
-00004fe0: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005000: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
-00005010: 6963 745b 6e65 7874 5f74 6172 6765 745f  ict[next_target_
-00005020: 6365 6c6c 5d20 3d20 7472 6163 6b6c 6574  cell] = tracklet
-00005030: 5f63 6f75 6e74 2020 0d0a 2020 2020 2020  _count  ..      
-00005040: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00005050: 7874 5f67 656e 5f63 6f75 6e74 203d 2067  xt_gen_count = g
-00005060: 656e 5f63 6f75 6e74 202b 2031 0d0a 2020  en_count + 1..  
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00005090: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
-000050a0: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
-000050b0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-000050c0: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
-000050f0: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
-00005100: 7267 6574 5f6c 6f6f 6b75 705b 6e65 7874  rget_lookup[next
-00005110: 5f74 6172 6765 745f 6365 6c6c 5d0d 0a20  _target_cell].. 
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00005140: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
-00005150: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005180: 6172 6765 745f 6365 6c6c 203d 2074 6172  arget_cell = tar
-00005190: 6765 745f 6365 6c6c 735b 6b5d 0d0a 2020  get_cells[k]..  
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000051c0: 6163 6b6c 6574 5f63 6f75 6e74 203d 2074  acklet_count = t
-000051d0: 7261 636b 6c65 745f 636f 756e 7420 2b20  racklet_count + 
-000051e0: 3120 2b20 6b0d 0a20 2020 2020 2020 2020  1 + k..         
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
-00005210: 636f 756e 7420 3d20 7365 6c66 2e5f 756e  count = self._un
-00005220: 6971 7565 5f74 7261 636b 6c65 745f 636f  ique_tracklet_co
-00005230: 756e 7428 7472 6163 6b6c 6574 5f63 6f75  unt(tracklet_cou
-00005240: 6e74 5f74 616b 656e 2c20 7472 6163 6b6c  nt_taken, trackl
-00005250: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00005280: 6c65 745f 636f 756e 745f 7461 6b65 6e2e  let_count_taken.
-00005290: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-000052a0: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-000052d0: 6572 6174 655f 6469 7669 6469 6e67 5f72  erate_dividing_r
-000052e0: 6563 7572 7369 7665 2872 6f6f 745f 6c65  ecursive(root_le
-000052f0: 6166 2c20 7461 7267 6574 5f63 656c 6c2c  af, target_cell,
-00005300: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
-00005310: 6974 732c 206e 6578 745f 6765 6e5f 636f  its, next_gen_co
-00005320: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
-00005330: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
-00005340: 756e 745f 7461 6b65 6e29 2020 2020 2020  unt_taken)      
-00005350: 0d0a 0d0a 0d0a 0d0a 2020 2020 6465 6620  ........    def 
-00005360: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
-00005370: 6728 7365 6c66 2c20 726f 6f74 5f72 6f6f  g(self, root_roo
-00005380: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
-00005390: 6f74 5f73 706c 6974 7329 3a0d 0a20 2020  ot_splits):..   
-000053a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000053b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000053c0: 2020 2020 6765 6e5f 636f 756e 7420 3d20      gen_count = 
-000053d0: 300d 0a20 2020 2020 2020 2020 2020 2074  0..            t
-000053e0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-000053f0: 300d 0a20 2020 2020 2020 2020 2020 2074  0..            t
-00005400: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-00005410: 6b65 6e20 3d20 5b5d 0d0a 2020 2020 2020  ken = []..      
-00005420: 2020 2020 2020 666f 7220 726f 6f74 5f61        for root_a
-00005430: 6c6c 2069 6e20 726f 6f74 5f72 6f6f 743a  ll in root_root:
-00005440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005450: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-00005460: 6174 696f 6e5f 6469 6374 5b72 6f6f 745f  ation_dict[root_
-00005470: 616c 6c5d 203d 2067 656e 5f63 6f75 6e74  all] = gen_count
-00005480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005490: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-000054a0: 6c65 745f 6469 6374 5b72 6f6f 745f 616c  let_dict[root_al
-000054b0: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-000054c0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000054d0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-000054e0: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
-000054f0: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00005500: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00005510: 2020 2020 2020 2020 2020 6966 2072 6f6f            if roo
-00005520: 745f 616c 6c20 696e 2073 656c 662e 6564  t_all in self.ed
-00005530: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00005540: 2061 6e64 2072 6f6f 745f 616c 6c20 6e6f   and root_all no
-00005550: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
-00005560: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005570: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00005580: 6574 5f63 656c 6c20 3d20 7365 6c66 2e65  et_cell = self.e
-00005590: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-000055a0: 705b 726f 6f74 5f61 6c6c 5d5b 305d 0d0a  p[root_all][0]..
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 2020 2020 2077 6869 6c65 2074           while t
-000055d0: 6172 6765 745f 6365 6c6c 206e 6f74 2069  arget_cell not i
-000055e0: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005610: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
-00005620: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
-00005630: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005660: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
-00005670: 6469 6374 5b74 6172 6765 745f 6365 6c6c  dict[target_cell
-00005680: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
-00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-000056c0: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
-000056d0: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-000056e0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-00005710: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
-00005720: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00005730: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005760: 5f63 656c 6c20 3d20 7365 6c66 2e65 6467  _cell = self.edg
-00005770: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
-00005780: 7461 7267 6574 5f63 656c 6c5d 5b30 5d0d  target_cell][0].
-00005790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000032b0: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+000032c0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+000032d0: 2020 2020 7365 6c66 2e41 7474 7269 6275      self.Attribu
+000032e0: 7465 6964 732c 2073 656c 662e 416c 6c56  teids, self.AllV
+000032f0: 616c 7565 7320 3d20 2067 6574 5f73 706f  alues =  get_spo
+00003300: 745f 6461 7461 7365 7428 7365 6c66 2e73  t_dataset(self.s
+00003310: 706f 745f 6461 7461 7365 742c 2073 656c  pot_dataset, sel
+00003320: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
+00003330: 5f73 706f 745f 6b65 7973 2c20 7365 6c66  _spot_keys, self
+00003340: 2e78 6361 6c69 6272 6174 696f 6e2c 2073  .xcalibration, s
+00003350: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00003360: 2c20 7365 6c66 2e7a 6361 6c69 6272 6174  , self.zcalibrat
+00003370: 696f 6e2c 2073 656c 662e 4174 7472 6962  ion, self.Attrib
+00003380: 7574 6542 6f78 6e61 6d65 2c20 7365 6c66  uteBoxname, self
+00003390: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
+000033a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000033b0: 7072 696e 7428 276f 6274 6961 6e65 6420  print('obtianed 
+000033c0: 7370 6f74 2061 7474 7269 6275 7465 7327  spot attributes'
+000033d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000033e0: 7365 6c66 2e54 7261 636b 4174 7472 6962  self.TrackAttrib
+000033f0: 7574 6569 6473 2c20 7365 6c66 2e41 6c6c  uteids, self.All
+00003400: 5472 6163 6b56 616c 7565 7320 3d20 6765  TrackValues = ge
+00003410: 745f 7472 6163 6b5f 6461 7461 7365 7428  t_track_dataset(
+00003420: 2041 6c6c 5472 6163 6b56 616c 7565 732c   AllTrackValues,
+00003430: 2073 656c 662e 7472 6163 6b5f 6461 7461   self.track_data
+00003440: 7365 742c 2020 7365 6c66 2e74 7261 636b  set,  self.track
+00003450: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00003460: 6579 732c 2073 656c 662e 7472 6163 6b5f  eys, self.track_
+00003470: 616e 616c 7973 6973 5f74 7261 636b 5f6b  analysis_track_k
+00003480: 6579 732c 2073 656c 662e 5472 6163 6b41  eys, self.TrackA
+00003490: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
+000034a0: 0d0a 2020 2020 2020 2020 2020 2020 2070  ..             p
+000034b0: 7269 6e74 2827 6f62 7461 696e 6564 2074  rint('obtained t
+000034c0: 7261 636b 2061 7474 7269 6275 7465 7327  rack attributes'
+000034d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000034e0: 7365 6c66 2e41 6c6c 4564 6765 7356 616c  self.AllEdgesVal
+000034f0: 7565 7320 3d20 6765 745f 6564 6765 735f  ues = get_edges_
+00003500: 6461 7461 7365 7428 7365 6c66 2e65 6467  dataset(self.edg
+00003510: 6573 5f64 6174 6173 6574 2c20 7365 6c66  es_dataset, self
+00003520: 2e65 6467 6573 5f64 6174 6173 6574 5f69  .edges_dataset_i
+00003530: 6e64 6578 2c20 7365 6c66 2e74 7261 636b  ndex, self.track
+00003540: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+00003550: 6579 732c 2073 656c 662e 7472 6163 6b5f  eys, self.track_
+00003560: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
+00003570: 6579 7329 0d0a 2020 2020 2020 2020 2020  eys)..          
+00003580: 2020 2070 7269 6e74 2827 6f62 7461 696e     print('obtain
+00003590: 6564 2065 6467 6520 6174 7472 6962 7574  ed edge attribut
+000035a0: 6573 2729 0d0a 0d0a 2020 2020 0d0a 2020  es')....    ..  
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035c0: 2020 0d0a 2020 2020 6465 6620 5f67 6574    ..    def _get
+000035d0: 5f62 6f75 6e64 6172 795f 706f 696e 7473  _boundary_points
+000035e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000035f0: 2020 0d0a 2020 2020 2020 2020 7072 696e    ..        prin
+00003600: 7428 2743 6f6d 7075 7469 6e67 2062 6f75  t('Computing bou
+00003610: 6e64 6172 7920 706f 696e 7473 2729 200d  ndary points') .
+00003620: 0a20 2020 2020 2020 2069 6620 2073 656c  .        if  sel
+00003630: 662e 6d61 736b 2069 7320 6e6f 7420 4e6f  f.mask is not No
+00003640: 6e65 3a0d 0a0d 0a20 2020 2020 2020 2020  ne:....         
+00003650: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+00003660: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+00003670: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00003680: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000036a0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+000036b0: 5f6d 6173 6b20 3d20 6368 6563 6b5f 616e  _mask = check_an
+000036c0: 645f 7570 6461 7465 5f6d 6173 6b28 7365  d_update_mask(se
+000036d0: 6c66 2e6d 6173 6b2c 2073 656c 662e 6368  lf.mask, self.ch
+000036e0: 616e 6e65 6c5f 7365 675f 696d 6167 6529  annel_seg_image)
+000036f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00003700: 6966 2073 656c 662e 7365 675f 696d 6167  if self.seg_imag
+00003710: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003730: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00003740: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003750: 6c66 2e75 7064 6174 655f 6d61 736b 203d  lf.update_mask =
+00003760: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
+00003770: 655f 6d61 736b 2873 656c 662e 6d61 736b  e_mask(self.mask
+00003780: 2c20 7365 6c66 2e73 6567 5f69 6d61 6765  , self.seg_image
+00003790: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000037a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000037b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000037c0: 6567 5f69 6d61 6765 2069 7320 4e6f 6e65  eg_image is None
+000037d0: 2061 6e64 2073 656c 662e 696d 6167 6520   and self.image 
+000037e0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
+00003830: 203d 2063 6865 636b 5f61 6e64 5f75 7064   = check_and_upd
+00003840: 6174 655f 6d61 736b 2873 656c 662e 6d61  ate_mask(self.ma
+00003850: 736b 2c20 7365 6c66 2e69 6d61 6765 2920  sk, self.image) 
+00003860: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003890: 6c66 2e6d 6173 6b20 3d20 7365 6c66 2e75  lf.mask = self.u
+000038a0: 7064 6174 655f 6d61 736b 0d0a 2020 2020  pdate_mask..    
+000038b0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000038c0: 6564 5f6d 6173 6b2c 2073 656c 662e 626f  ed_mask, self.bo
+000038d0: 756e 6461 7279 203d 2062 6f75 6e64 6172  undary = boundar
+000038e0: 795f 706f 696e 7473 2873 656c 662e 6d61  y_points(self.ma
+000038f0: 736b 2c20 7365 6c66 2e78 6361 6c69 6272  sk, self.xcalibr
+00003900: 6174 696f 6e2c 2073 656c 662e 7963 616c  ation, self.ycal
+00003910: 6962 7261 7469 6f6e 2c20 7365 6c66 2e7a  ibration, self.z
+00003920: 6361 6c69 6272 6174 696f 6e29 0d0a 2020  calibration)..  
+00003930: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00003940: 6d61 736b 2069 7320 4e6f 6e65 3a0d 0a20  mask is None:.. 
+00003950: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00003960: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
+00003970: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00003980: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00003990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039a0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+000039b0: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+000039c0: 2873 656c 662e 7365 675f 696d 6167 652e  (self.seg_image.
+000039d0: 7368 6170 652c 2064 7479 7065 3d6e 702e  shape, dtype=np.
+000039e0: 7569 6e74 3829 0d0a 2020 2020 2020 2020  uint8)..        
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00003a10: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
+00003a20: 6973 204e 6f6e 6520 616e 6420 7365 6c66  is None and self
+00003a30: 2e69 6d61 6765 2069 7320 6e6f 7420 4e6f  .image is not No
+00003a40: 6e65 3a0d 0a0d 0a20 2020 2020 2020 2020  ne:....         
+00003a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003a60: 7570 6461 7465 5f6d 6173 6b20 3d20 6e70  update_mask = np
+00003a70: 2e7a 6572 6f73 2873 656c 662e 696d 6167  .zeros(self.imag
+00003a80: 652e 7368 6170 652c 2064 7479 7065 3d6e  e.shape, dtype=n
+00003a90: 702e 7569 6e74 3829 200d 0a20 2020 2020  p.uint8) ..     
+00003aa0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2020 7365 6c66 2e75 7064 6174 655f 6d61    self.update_ma
+00003ad0: 736b 203d 206e 702e 7a65 726f 7328 7365  sk = np.zeros(se
+00003ae0: 6c66 2e69 6d61 6765 7369 7a65 2c20 6474  lf.imagesize, dt
+00003af0: 7970 653d 6e70 2e75 696e 7438 2920 2020  ype=np.uint8)   
+00003b00: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00003b30: 7365 6c66 2e6d 6173 6b20 3d20 7365 6c66  self.mask = self
+00003b40: 2e75 7064 6174 655f 6d61 736b 0d0a 2020  .update_mask..  
+00003b50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00003b60: 6173 6b5b 3a2c 3a2c 313a 2d31 2c31 3a2d  ask[:,:,1:-1,1:-
+00003b70: 315d 203d 2031 0d0a 2020 2020 2020 2020  1] = 1..        
+00003b80: 2020 2020 7365 6c66 2e74 696d 6564 5f6d      self.timed_m
+00003b90: 6173 6b2c 2073 656c 662e 626f 756e 6461  ask, self.bounda
+00003ba0: 7279 203d 2062 6f75 6e64 6172 795f 706f  ry = boundary_po
+00003bb0: 696e 7473 2873 656c 662e 6d61 736b 2c20  ints(self.mask, 
+00003bc0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00003bd0: 6e2c 2073 656c 662e 7963 616c 6962 7261  n, self.ycalibra
+00003be0: 7469 6f6e 2c20 7365 6c66 2e7a 6361 6c69  tion, self.zcali
+00003bf0: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+00003c00: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
+00003c10: 6465 6620 5f67 656e 6572 6174 655f 6765  def _generate_ge
+00003c20: 6e65 7261 7469 6f6e 7328 7365 6c66 2c20  nerations(self, 
+00003c30: 7472 6163 6b29 3a0d 0a20 2020 2020 2020  track):..       
+00003c40: 2020 0d0a 2020 2020 2020 2020 616c 6c5f    ..        all_
+00003c50: 736f 7572 6365 5f69 6473 203d 205b 5d0d  source_ids = [].
+00003c60: 0a20 2020 2020 2020 2061 6c6c 5f74 6172  .        all_tar
+00003c70: 6765 745f 6964 7320 3d20 5b5d 200d 0a0d  get_ids = [] ...
+00003c80: 0a0d 0a20 2020 2020 2020 2066 6f72 2065  ...        for e
+00003c90: 6467 6520 696e 2074 7261 636b 2e66 696e  dge in track.fin
+00003ca0: 6461 6c6c 2827 4564 6765 2729 3a0d 0a0d  dall('Edge'):...
+00003cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cc0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+00003cd0: 7263 655f 6964 203d 2069 6e74 2865 6467  rce_id = int(edg
+00003ce0: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
+00003cf0: 736f 7572 6365 5f69 645f 6b65 7929 290d  source_id_key)).
+00003d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d10: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00003d20: 6765 745f 6964 203d 2069 6e74 2865 6467  get_id = int(edg
+00003d30: 652e 6765 7428 7365 6c66 2e73 706f 745f  e.get(self.spot_
+00003d40: 7461 7267 6574 5f69 645f 6b65 7929 290d  target_id_key)).
+00003d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00003d70: 5f73 6f75 7263 655f 6964 732e 6170 7065  _source_ids.appe
+00003d80: 6e64 2873 6f75 7263 655f 6964 290d 0a20  nd(source_id).. 
+00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003da0: 2020 2020 2020 2020 2020 2061 6c6c 5f74             all_t
+00003db0: 6172 6765 745f 6964 732e 6170 7065 6e64  arget_ids.append
+00003dc0: 2874 6172 6765 745f 6964 290d 0a20 2020  (target_id)..   
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00003df0: 6365 5f69 6420 696e 2073 656c 662e 6564  ce_id in self.ed
+00003e00: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00003e10: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e30: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+00003e40: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00003e50: 5b73 6f75 7263 655f 6964 5d2e 6170 7065  [source_id].appe
+00003e60: 6e64 2874 6172 6765 745f 6964 290d 0a20  nd(target_id).. 
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003e90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
+00003ec0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+00003ed0: 6f75 7263 655f 6964 5d20 3d20 5b74 6172  ource_id] = [tar
+00003ee0: 6765 745f 6964 5d0d 0a20 2020 2020 2020  get_id]..       
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2020 2073 656c 662e 6564 6765 5f73       self.edge_s
+00003f10: 6f75 7263 655f 6c6f 6f6b 7570 5b74 6172  ource_lookup[tar
+00003f20: 6765 745f 6964 5d20 3d20 736f 7572 6365  get_id] = source
+00003f30: 5f69 6420 0d0a 0d0a 2020 2020 2020 2020  _id ....        
+00003f40: 7265 7475 726e 2061 6c6c 5f73 6f75 7263  return all_sourc
+00003f50: 655f 6964 732c 2061 6c6c 5f74 6172 6765  e_ids, all_targe
+00003f60: 745f 6964 7320 0d0a 0d0a 0d0a 2020 2020  t_ids ......    
+00003f70: 6465 6620 5f63 7265 6174 655f 6765 6e65  def _create_gene
+00003f80: 7261 7469 6f6e 7328 7365 6c66 2c20 616c  rations(self, al
+00003f90: 6c5f 736f 7572 6365 5f69 6473 3a20 6c69  l_source_ids: li
+00003fa0: 7374 293a 0d0a 2020 2020 2020 2020 200d  st):..         .
+00003fb0: 0a20 2020 2020 2020 2072 6f6f 745f 6c65  .        root_le
+00003fc0: 6166 203d 205b 5d0d 0a20 2020 2020 2020  af = []..       
+00003fd0: 2072 6f6f 745f 726f 6f74 203d 205b 5d0d   root_root = [].
+00003fe0: 0a20 2020 2020 2020 2072 6f6f 745f 7370  .        root_sp
+00003ff0: 6c69 7473 203d 205b 5d0d 0a20 2020 2020  lits = []..     
+00004000: 2020 2023 4765 7420 7468 6520 726f 6f74     #Get the root
+00004010: 2069 640d 0a20 2020 2020 2020 2066 6f72   id..        for
+00004020: 2073 6f75 7263 655f 6964 2069 6e20 616c   source_id in al
+00004030: 6c5f 736f 7572 6365 5f69 6473 3a0d 0a20  l_source_ids:.. 
+00004040: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004050: 736f 7572 6365 5f69 6420 696e 2073 656c  source_id in sel
+00004060: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
+00004070: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
+00004080: 2020 2020 2020 2073 6f75 7263 655f 7461         source_ta
+00004090: 7267 6574 5f69 6420 3d20 7365 6c66 2e65  rget_id = self.e
+000040a0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+000040b0: 705b 736f 7572 6365 5f69 645d 0d0a 2020  p[source_id]..  
+000040c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000040d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000040e0: 2020 2073 6f75 7263 655f 7461 7267 6574     source_target
+000040f0: 5f69 6420 3d20 4e6f 6e65 2020 2020 2020  _id = None      
+00004100: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00004110: 2020 2020 7461 7267 6574 5f74 6172 6765      target_targe
+00004120: 745f 6964 203d 2073 656c 662e 6564 6765  t_id = self.edge
+00004130: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+00004140: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00004150: 2020 2020 2020 2020 2069 6620 736f 7572           if sour
+00004160: 6365 5f74 6172 6765 745f 6964 2069 7320  ce_target_id is 
+00004170: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00004180: 2020 2020 2020 2020 2020 6966 2073 6f75            if sou
+00004190: 7263 655f 6964 206e 6f74 2069 6e20 726f  rce_id not in ro
+000041a0: 6f74 5f72 6f6f 743a 0d0a 2020 2020 2020  ot_root:..      
+000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041c0: 726f 6f74 5f72 6f6f 742e 6170 7065 6e64  root_root.append
+000041d0: 2873 6f75 7263 655f 6964 2920 0d0a 2020  (source_id) ..  
+000041e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000041f0: 656e 2874 6172 6765 745f 7461 7267 6574  en(target_target
+00004200: 5f69 6429 203e 2031 3a0d 0a20 2020 2020  _id) > 1:..     
+00004210: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004220: 2073 6f75 7263 655f 6964 206e 6f74 2069   source_id not i
+00004230: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 2020 2020 726f 6f74 5f73 706c 6974        root_split
+00004260: 732e 6170 7065 6e64 2873 6f75 7263 655f  s.append(source_
+00004270: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+00004280: 2020 2069 6620 7461 7267 6574 5f74 6172     if target_tar
+00004290: 6765 745f 6964 5b30 5d20 6e6f 7420 696e  get_id[0] not in
+000042a0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
+000042b0: 745f 6c6f 6f6b 7570 3a0d 0a20 2020 2020  t_lookup:..     
+000042c0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+000042d0: 6f74 5f6c 6561 662e 6170 7065 6e64 2874  ot_leaf.append(t
+000042e0: 6172 6765 745f 7461 7267 6574 5f69 645b  arget_target_id[
+000042f0: 305d 2920 2020 2020 2020 2020 200d 0a0d  0])          ...
+00004300: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004310: 726f 6f74 5f72 6f6f 742c 2072 6f6f 745f  root_root, root_
+00004320: 7370 6c69 7473 2c20 726f 6f74 5f6c 6561  splits, root_lea
+00004330: 660d 0a0d 0a20 2020 2064 6566 205f 736f  f....    def _so
+00004340: 7274 5f64 6976 6964 696e 675f 6365 6c6c  rt_dividing_cell
+00004350: 7328 7365 6c66 2c20 726f 6f74 5f73 706c  s(self, root_spl
+00004360: 6974 7329 3a0d 0a20 2020 2020 2020 2020  its):..         
+00004370: 2020 6365 6c6c 5f69 645f 7469 6d65 7320    cell_id_times 
+00004380: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00004390: 2063 656c 6c5f 6964 7320 3d20 5b5d 0d0a   cell_ids = []..
+000043a0: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+000043b0: 6f6f 745f 7370 6c69 7420 696e 2072 6f6f  oot_split in roo
+000043c0: 745f 7370 6c69 7473 3a0d 0a20 2020 2020  t_splits:..     
+000043d0: 2020 2020 2020 2020 2020 2020 2073 706c               spl
+000043e0: 6974 5f63 656c 6c5f 6964 5f74 696d 6520  it_cell_id_time 
+000043f0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00004400: 6f74 5f70 726f 7065 7274 6965 735b 726f  ot_properties[ro
+00004410: 6f74 5f73 706c 6974 5d5b 7365 6c66 2e66  ot_split][self.f
+00004420: 7261 6d65 6964 5f6b 6579 5d0d 0a20 2020  rameid_key]..   
+00004430: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00004440: 656c 6c5f 6964 5f74 696d 6573 2e61 7070  ell_id_times.app
+00004450: 656e 6428 7370 6c69 745f 6365 6c6c 5f69  end(split_cell_i
+00004460: 645f 7469 6d65 290d 0a20 2020 2020 2020  d_time)..       
+00004470: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00004480: 6964 732e 6170 7065 6e64 2872 6f6f 745f  ids.append(root_
+00004490: 7370 6c69 7429 0d0a 2020 2020 2020 2020  split)..        
+000044a0: 2020 2073 6f72 7465 645f 696e 6469 6365     sorted_indice
+000044b0: 7320 3d20 736f 7274 6564 2872 616e 6765  s = sorted(range
+000044c0: 286c 656e 2863 656c 6c5f 6964 5f74 696d  (len(cell_id_tim
+000044d0: 6573 2929 2c20 6b65 793d 6c61 6d62 6461  es)), key=lambda
+000044e0: 206b 3a20 6365 6c6c 5f69 645f 7469 6d65   k: cell_id_time
+000044f0: 735b 6b5d 290d 0a20 2020 2020 2020 2020  s[k])..         
+00004500: 2020 736f 7274 6564 5f63 656c 6c5f 6964    sorted_cell_id
+00004510: 7320 3d20 5b63 656c 6c5f 6964 735b 695d  s = [cell_ids[i]
+00004520: 2066 6f72 2069 2069 6e20 736f 7274 6564   for i in sorted
+00004530: 5f69 6e64 6963 6573 5d0d 0a0d 0a20 2020  _indices]....   
+00004540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00004550: 6f72 7465 645f 6365 6c6c 5f69 6473 2020  orted_cell_ids  
+00004560: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00004570: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004580: 0a0d 0a20 2020 2064 6566 205f 6974 6572  ...    def _iter
+00004590: 6174 655f 6469 7669 6469 6e67 5f72 6563  ate_dividing_rec
+000045a0: 7572 7369 7665 2873 656c 662c 2072 6f6f  ursive(self, roo
+000045b0: 745f 6c65 6166 2c20 7461 7267 6574 5f63  t_leaf, target_c
+000045c0: 656c 6c2c 2073 6f72 7465 645f 726f 6f74  ell, sorted_root
+000045d0: 5f73 706c 6974 732c 2067 656e 5f63 6f75  _splits, gen_cou
+000045e0: 6e74 2c20 7472 6163 6b6c 6574 5f63 6f75  nt, tracklet_cou
+000045f0: 6e74 2c20 7472 6163 6b6c 6574 5f63 6f75  nt, tracklet_cou
+00004600: 6e74 5f74 616b 656e 293a 0d0a 2020 2020  nt_taken):..    
+00004610: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00004620: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00004630: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004640: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00004650: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
+00004660: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
+00004670: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00004680: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+00004690: 7461 7267 6574 5f63 656c 6c5d 203d 2074  target_cell] = t
+000046a0: 7261 636b 6c65 745f 636f 756e 740d 0a0d  racklet_count...
+000046b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000046c0: 2069 6620 7461 7267 6574 5f63 656c 6c20   if target_cell 
+000046d0: 3d3d 2072 6f6f 745f 6c65 6166 3a0d 0a20  == root_leaf:.. 
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046f0: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00004700: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004710: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00004720: 745f 7461 7267 6574 5f63 656c 6c20 3d20  t_target_cell = 
+00004730: 4e6f 6e65 0d0a 2020 2020 2020 2020 2020  None..          
+00004740: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00004750: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004760: 745f 6365 6c6c 2069 6e20 736f 7274 6564  t_cell in sorted
+00004770: 5f72 6f6f 745f 7370 6c69 7473 3a0d 0a20  _root_splits:.. 
+00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004790: 2020 2020 2020 2020 2020 6e65 7874 5f67            next_g
+000047a0: 656e 5f63 6f75 6e74 203d 2067 656e 5f63  en_count = gen_c
+000047b0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
+000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047d0: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
+000047e0: 656c 6c20 696e 2073 656c 662e 6564 6765  ell in self.edge
+000047f0: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00004800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004820: 2074 6172 6765 745f 6365 6c6c 7320 3d20   target_cells = 
+00004830: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
+00004840: 5f6c 6f6f 6b75 705b 7461 7267 6574 5f63  _lookup[target_c
+00004850: 656c 6c5d 0d0a 2020 2020 2020 2020 2020  ell]..          
+00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004870: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
+00004880: 616e 6765 286c 656e 2874 6172 6765 745f  ange(len(target_
+00004890: 6365 6c6c 7329 293a 0d0a 2020 2020 2020  cells)):..      
+000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000048c0: 7567 6874 6572 5f74 6172 6765 745f 6365  ughter_target_ce
+000048d0: 6c6c 203d 2074 6172 6765 745f 6365 6c6c  ll = target_cell
+000048e0: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
+000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
+00004910: 6574 5f63 6f75 6e74 203d 2074 7261 636b  et_count = track
+00004920: 6c65 745f 636f 756e 7420 2b20 3120 2b20  let_count + 1 + 
+00004930: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
+00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004950: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+00004960: 636f 756e 7420 3d20 7365 6c66 2e5f 756e  count = self._un
+00004970: 6971 7565 5f74 7261 636b 6c65 745f 636f  ique_tracklet_co
+00004980: 756e 7428 7472 6163 6b6c 6574 5f63 6f75  unt(tracklet_cou
+00004990: 6e74 5f74 616b 656e 2c20 7472 6163 6b6c  nt_taken, trackl
+000049a0: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000049d0: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
+000049e0: 6b65 6e2e 6170 7065 6e64 2874 7261 636b  ken.append(track
+000049f0: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a20: 7365 6c66 2e5f 6974 6572 6174 655f 6469  self._iterate_di
+00004a30: 7669 6469 6e67 5f72 6563 7572 7369 7665  viding_recursive
+00004a40: 2872 6f6f 745f 6c65 6166 2c20 6461 7567  (root_leaf, daug
+00004a50: 6874 6572 5f74 6172 6765 745f 6365 6c6c  hter_target_cell
+00004a60: 2c20 736f 7274 6564 5f72 6f6f 745f 7370  , sorted_root_sp
+00004a70: 6c69 7473 2c20 6e65 7874 5f67 656e 5f63  lits, next_gen_c
+00004a80: 6f75 6e74 2c20 7472 6163 6b6c 6574 5f63  ount, tracklet_c
+00004a90: 6f75 6e74 2c20 7472 6163 6b6c 6574 5f63  ount, tracklet_c
+00004aa0: 6f75 6e74 5f74 616b 656e 2920 2020 2020  ount_taken)     
+00004ab0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00004ac0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00004ad0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00004ae0: 7267 6574 5f63 656c 6c20 696e 2073 656c  rget_cell in sel
+00004af0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00004b00: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
+00004b10: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00004b20: 7461 7267 6574 5f63 656c 6c73 203d 2073  target_cells = s
+00004b30: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+00004b40: 6c6f 6f6b 7570 5b74 6172 6765 745f 6365  lookup[target_ce
+00004b50: 6c6c 5d0d 0a20 2020 2020 2020 2020 2020  ll]..           
+00004b60: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00004b70: 7267 6574 5f63 656c 6c20 3d20 6e65 7874  rget_cell = next
+00004b80: 5f74 6172 6765 745f 6365 6c6c 735b 305d  _target_cells[0]
+00004b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ba0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00004bd0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+00004be0: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004bf0: 6c20 6e6f 7420 696e 2073 6f72 7465 645f  l not in sorted_
+00004c00: 726f 6f74 5f73 706c 6974 733a 0d0a 2020  root_splits:..  
+00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c20: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
+00004c30: 6174 696f 6e5f 6469 6374 5b6e 6578 745f  ation_dict[next_
+00004c40: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
+00004c50: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
+00004c80: 6469 6374 5b6e 6578 745f 7461 7267 6574  dict[next_target
+00004c90: 5f63 656c 6c5d 203d 2074 7261 636b 6c65  _cell] = trackle
+00004ca0: 745f 636f 756e 740d 0a20 2020 2020 2020  t_count..       
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2069 6620 6e65 7874 5f74 6172 6765 745f   if next_target_
+00004cd0: 6365 6c6c 2069 6e20 726f 6f74 5f6c 6561  cell in root_lea
+00004ce0: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004d10: 6f6e 5f64 6963 745b 7461 7267 6574 5f63  on_dict[target_c
+00004d20: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
+00004d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
+00004d60: 6963 745b 7461 7267 6574 5f63 656c 6c5d  ict[target_cell]
+00004d70: 203d 2074 7261 636b 6c65 745f 636f 756e   = tracklet_coun
+00004d80: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004da0: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2069 6620 6e65 7874 5f74 6172 6765 745f   if next_target_
+00004dd0: 6365 6c6c 2069 6e20 7365 6c66 2e65 6467  cell in self.edg
+00004de0: 655f 7461 7267 6574 5f6c 6f6f 6b75 703a  e_target_lookup:
+00004df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e00: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00004e10: 7874 5f74 6172 6765 745f 6365 6c6c 7320  xt_target_cells 
+00004e20: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
+00004e30: 6574 5f6c 6f6f 6b75 705b 6e65 7874 5f74  et_lookup[next_t
+00004e40: 6172 6765 745f 6365 6c6c 5d0d 0a20 2020  arget_cell]..   
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00004e70: 7267 6574 5f63 656c 6c20 3d20 6e65 7874  rget_cell = next
+00004e80: 5f74 6172 6765 745f 6365 6c6c 735b 305d  _target_cells[0]
+00004e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004eb0: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004ec0: 6c20 696e 2072 6f6f 745f 6c65 6166 3a0d  l in root_leaf:.
+00004ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ef0: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
+00004f00: 6469 6374 5b74 6172 6765 745f 6365 6c6c  dict[target_cell
+00004f10: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004f40: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
+00004f50: 5b74 6172 6765 745f 6365 6c6c 5d20 3d20  [target_cell] = 
+00004f60: 7472 6163 6b6c 6574 5f63 6f75 6e74 0d0a  tracklet_count..
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00004f90: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
+00004fa0: 2020 2020 2020 2020 6966 206e 6578 745f          if next_
+00004fb0: 7461 7267 6574 5f63 656c 6c20 6973 206e  target_cell is n
+00004fc0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00004fd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004fe0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
+00004ff0: 6374 5b6e 6578 745f 7461 7267 6574 5f63  ct[next_target_c
+00005000: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
+00005010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005020: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00005030: 6c65 745f 6469 6374 5b6e 6578 745f 7461  let_dict[next_ta
+00005040: 7267 6574 5f63 656c 6c5d 203d 2074 7261  rget_cell] = tra
+00005050: 636b 6c65 745f 636f 756e 7420 200d 0a20  cklet_count  .. 
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 206e 6578 745f 6765 6e5f 636f 756e     next_gen_coun
+00005080: 7420 3d20 6765 6e5f 636f 756e 7420 2b20  t = gen_count + 
+00005090: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+000050a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000050b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000050c0: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+000050d0: 2069 6e20 7365 6c66 2e65 6467 655f 7461   in self.edge_ta
+000050e0: 7267 6574 5f6c 6f6f 6b75 703a 0d0a 2020  rget_lookup:..  
+000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005100: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00005110: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
+00005120: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+00005130: 5b6e 6578 745f 7461 7267 6574 5f63 656c  [next_target_cel
+00005140: 6c5d 0d0a 2020 2020 2020 2020 2020 2020  l]..            
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 666f 7220 6b20 696e 2072 616e 6765 286c  for k in range(l
+00005170: 656e 2874 6172 6765 745f 6365 6c6c 7329  en(target_cells)
+00005180: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051a0: 2020 2020 7461 7267 6574 5f63 656c 6c20      target_cell 
+000051b0: 3d20 7461 7267 6574 5f63 656c 6c73 5b6b  = target_cells[k
+000051c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
+000051f0: 7420 3d20 7472 6163 6b6c 6574 5f63 6f75  t = tracklet_cou
+00005200: 6e74 202b 2031 202b 206b 0d0a 2020 2020  nt + 1 + k..    
+00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00005230: 6b6c 6574 5f63 6f75 6e74 203d 2073 656c  klet_count = sel
+00005240: 662e 5f75 6e69 7175 655f 7472 6163 6b6c  f._unique_trackl
+00005250: 6574 5f63 6f75 6e74 2874 7261 636b 6c65  et_count(trackle
+00005260: 745f 636f 756e 745f 7461 6b65 6e2c 2074  t_count_taken, t
+00005270: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052a0: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
+000052b0: 616b 656e 2e61 7070 656e 6428 7472 6163  aken.append(trac
+000052c0: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000052f0: 662e 5f69 7465 7261 7465 5f64 6976 6964  f._iterate_divid
+00005300: 696e 675f 7265 6375 7273 6976 6528 726f  ing_recursive(ro
+00005310: 6f74 5f6c 6561 662c 2074 6172 6765 745f  ot_leaf, target_
+00005320: 6365 6c6c 2c20 736f 7274 6564 5f72 6f6f  cell, sorted_roo
+00005330: 745f 7370 6c69 7473 2c20 6e65 7874 5f67  t_splits, next_g
+00005340: 656e 5f63 6f75 6e74 2c20 7472 6163 6b6c  en_count, trackl
+00005350: 6574 5f63 6f75 6e74 2c20 7472 6163 6b6c  et_count, trackl
+00005360: 6574 5f63 6f75 6e74 5f74 616b 656e 2920  et_count_taken) 
+00005370: 2020 2020 200d 0a0d 0a0d 0a0d 0a20 2020       ........   
+00005380: 2064 6566 205f 6974 6572 6174 655f 6469   def _iterate_di
+00005390: 7669 6469 6e67 2873 656c 662c 2072 6f6f  viding(self, roo
+000053a0: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
+000053b0: 662c 2072 6f6f 745f 7370 6c69 7473 293a  f, root_splits):
+000053c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+000053d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000053e0: 2020 2020 2020 2020 2067 656e 5f63 6f75           gen_cou
+000053f0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+00005400: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00005410: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+00005420: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00005430: 6e74 5f74 616b 656e 203d 205b 5d0d 0a20  nt_taken = [].. 
+00005440: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+00005450: 6f6f 745f 616c 6c20 696e 2072 6f6f 745f  oot_all in root_
+00005460: 726f 6f74 3a0d 0a20 2020 2020 2020 2020  root:..         
+00005470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005480: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
+00005490: 726f 6f74 5f61 6c6c 5d20 3d20 6765 6e5f  root_all] = gen_
+000054a0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+000054b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000054c0: 7472 6163 6b6c 6574 5f64 6963 745b 726f  tracklet_dict[ro
+000054d0: 6f74 5f61 6c6c 5d20 3d20 7472 6163 6b6c  ot_all] = trackl
+000054e0: 6574 5f63 6f75 6e74 0d0a 2020 2020 2020  et_count..      
+000054f0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00005500: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
+00005510: 656e 2e61 7070 656e 6428 7472 6163 6b6c  en.append(trackl
+00005520: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00005530: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005540: 6620 726f 6f74 5f61 6c6c 2069 6e20 7365  f root_all in se
+00005550: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00005560: 6f6f 6b75 7020 616e 6420 726f 6f74 5f61  ookup and root_a
+00005570: 6c6c 206e 6f74 2069 6e20 726f 6f74 5f73  ll not in root_s
+00005580: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
+00005590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055a0: 2074 6172 6765 745f 6365 6c6c 203d 2073   target_cell = s
+000055b0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
+000055c0: 6c6f 6f6b 7570 5b72 6f6f 745f 616c 6c5d  lookup[root_all]
+000055d0: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
+000055e0: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+000055f0: 696c 6520 7461 7267 6574 5f63 656c 6c20  ile target_cell 
+00005600: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
+00005610: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005630: 2020 2020 2069 6620 7461 7267 6574 5f63       if target_c
+00005640: 656c 6c20 696e 2073 656c 662e 6564 6765  ell in self.edge
+00005650: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00005660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+00005690: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
+000056a0: 5f63 656c 6c5d 203d 2067 656e 5f63 6f75  _cell] = gen_cou
+000056b0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056d0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+000056e0: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
+000056f0: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
+00005700: 6574 5f63 6f75 6e74 0d0a 2020 2020 2020  et_count..      
+00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005720: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00005730: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
+00005740: 656e 2e61 7070 656e 6428 7472 6163 6b6c  en.append(trackl
+00005750: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00005780: 6172 6765 745f 6365 6c6c 203d 2073 656c  arget_cell = sel
+00005790: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+000057a0: 6f6b 7570 5b74 6172 6765 745f 6365 6c6c  okup[target_cell
+000057b0: 5d5b 305d 0d0a 2020 2020 2020 2020 2020  ][0]..          
 000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000057e0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-000057f0: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-00005800: 3d20 6765 6e5f 636f 756e 740d 0a20 2020  = gen_count..   
-00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-00005840: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
-00005850: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-00005860: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00005890: 6c65 745f 636f 756e 745f 7461 6b65 6e2e  let_count_taken.
-000058a0: 6170 7065 6e64 2874 7261 636b 6c65 745f  append(tracklet_
-000058b0: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-000058e0: 6561 6b20 0d0a 2020 2020 2020 2020 2020  eak ..          
-000058f0: 2020 2020 2020 2020 2020 2353 7461 7274            #Start
-00005900: 206f 6620 7472 6163 6b20 6973 2061 2064   of track is a d
-00005910: 6976 6964 696e 6720 6365 6c6c 2020 2020  ividing cell    
-00005920: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005940: 6620 726f 6f74 5f61 6c6c 2069 6e20 7365  f root_all in se
-00005950: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00005960: 6f6f 6b75 7020 616e 6420 726f 6f74 5f61  ookup and root_a
-00005970: 6c6c 2069 6e20 726f 6f74 5f73 706c 6974  ll in root_split
-00005980: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00005990: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-000059a0: 6765 745f 6365 6c6c 7320 3d20 7365 6c66  get_cells = self
-000059b0: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-000059c0: 6b75 705b 726f 6f74 5f61 6c6c 5d0d 0a20  kup[root_all].. 
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2020 2020 2020 6765 6e5f 636f 756e          gen_coun
-000059f0: 7420 3d20 6765 6e5f 636f 756e 7420 2b20  t = gen_count + 
-00005a00: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-00005a10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005a20: 6a20 696e 2072 616e 6765 286c 656e 2874  j in range(len(t
-00005a30: 6172 6765 745f 6365 6c6c 7329 293a 0d0a  arget_cells)):..
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a60: 7461 7267 6574 5f63 656c 6c20 3d20 7461  target_cell = ta
-00005a70: 7267 6574 5f63 656c 6c73 5b6a 5d0d 0a20  rget_cells[j].. 
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005aa0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-00005ab0: 7472 6163 6b6c 6574 5f63 6f75 6e74 202b  tracklet_count +
-00005ac0: 2031 202b 206a 0d0a 2020 2020 2020 2020   1 + j..        
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00005af0: 5f63 6f75 6e74 203d 2073 656c 662e 5f75  _count = self._u
-00005b00: 6e69 7175 655f 7472 6163 6b6c 6574 5f63  nique_tracklet_c
-00005b10: 6f75 6e74 2874 7261 636b 6c65 745f 636f  ount(tracklet_co
-00005b20: 756e 745f 7461 6b65 6e2c 2074 7261 636b  unt_taken, track
-00005b30: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00005b60: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
-00005b70: 2e61 7070 656e 6428 7472 6163 6b6c 6574  .append(tracklet
-00005b80: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
-00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 2020 2073 656c 662e 5f69           self._i
-00005bb0: 7465 7261 7465 5f64 6976 6964 696e 675f  terate_dividing_
-00005bc0: 7265 6375 7273 6976 6528 726f 6f74 5f6c  recursive(root_l
-00005bd0: 6561 662c 2074 6172 6765 745f 6365 6c6c  eaf, target_cell
-00005be0: 2c20 726f 6f74 5f73 706c 6974 732c 2067  , root_splits, g
-00005bf0: 656e 5f63 6f75 6e74 2c20 7472 6163 6b6c  en_count, trackl
-00005c00: 6574 5f63 6f75 6e74 2c20 7472 6163 6b6c  et_count, trackl
-00005c10: 6574 5f63 6f75 6e74 5f74 616b 656e 290d  et_count_taken).
-00005c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000057d0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00005810: 6f6e 5f64 6963 745b 7461 7267 6574 5f63  on_dict[target_c
+00005820: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
+00005830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005850: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00005860: 636b 6c65 745f 6469 6374 5b74 6172 6765  cklet_dict[targe
+00005870: 745f 6365 6c6c 5d20 3d20 7472 6163 6b6c  t_cell] = trackl
+00005880: 6574 5f63 6f75 6e74 0d0a 2020 2020 2020  et_count..      
+00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058b0: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
+000058c0: 616b 656e 2e61 7070 656e 6428 7472 6163  aken.append(trac
+000058d0: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
+000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2062 7265 616b 200d 0a20 2020 2020     break ..     
+00005910: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005920: 5374 6172 7420 6f66 2074 7261 636b 2069  Start of track i
+00005930: 7320 6120 6469 7669 6469 6e67 2063 656c  s a dividing cel
+00005940: 6c20 2020 2020 2020 2020 2020 2020 0d0a  l             ..
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 6966 2072 6f6f 745f 616c 6c20      if root_all 
+00005970: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
+00005980: 6765 745f 6c6f 6f6b 7570 2061 6e64 2072  get_lookup and r
+00005990: 6f6f 745f 616c 6c20 696e 2072 6f6f 745f  oot_all in root_
+000059a0: 7370 6c69 7473 3a0d 0a20 2020 2020 2020  splits:..       
+000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059c0: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
+000059d0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
+000059e0: 745f 6c6f 6f6b 7570 5b72 6f6f 745f 616c  t_lookup[root_al
+000059f0: 6c5d 0d0a 2020 2020 2020 2020 2020 2020  l]..            
+00005a00: 2020 2020 2020 2020 2020 2020 2067 656e               gen
+00005a10: 5f63 6f75 6e74 203d 2067 656e 5f63 6f75  _count = gen_cou
+00005a20: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+00005a50: 6c65 6e28 7461 7267 6574 5f63 656c 6c73  len(target_cells
+00005a60: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a80: 2020 2020 2074 6172 6765 745f 6365 6c6c       target_cell
+00005a90: 203d 2074 6172 6765 745f 6365 6c6c 735b   = target_cells[
+00005aa0: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00005ad0: 6e74 203d 2074 7261 636b 6c65 745f 636f  nt = tracklet_co
+00005ae0: 756e 7420 2b20 3120 2b20 6a0d 0a20 2020  unt + 1 + j..   
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00005b10: 636b 6c65 745f 636f 756e 7420 3d20 7365  cklet_count = se
+00005b20: 6c66 2e5f 756e 6971 7565 5f74 7261 636b  lf._unique_track
+00005b30: 6c65 745f 636f 756e 7428 7472 6163 6b6c  let_count(trackl
+00005b40: 6574 5f63 6f75 6e74 5f74 616b 656e 2c20  et_count_taken, 
+00005b50: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
+00005b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b80: 2074 7261 636b 6c65 745f 636f 756e 745f   tracklet_count_
+00005b90: 7461 6b65 6e2e 6170 7065 6e64 2874 7261  taken.append(tra
+00005ba0: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005bd0: 6c66 2e5f 6974 6572 6174 655f 6469 7669  lf._iterate_divi
+00005be0: 6469 6e67 5f72 6563 7572 7369 7665 2872  ding_recursive(r
+00005bf0: 6f6f 745f 6c65 6166 2c20 7461 7267 6574  oot_leaf, target
+00005c00: 5f63 656c 6c2c 2072 6f6f 745f 7370 6c69  _cell, root_spli
+00005c10: 7473 2c20 6765 6e5f 636f 756e 742c 2074  ts, gen_count, t
+00005c20: 7261 636b 6c65 745f 636f 756e 742c 2074  racklet_count, t
+00005c30: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
+00005c40: 6b65 6e29 0d0a 2020 2020 2020 2020 2020  ken)..          
 00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00005c70: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00005c80: 2872 6f6f 745f 7370 6c69 7473 2920 3e20  (root_splits) > 
-00005c90: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-00005ca0: 2020 2020 2020 2020 736f 7274 6564 5f72          sorted_r
-00005cb0: 6f6f 745f 7370 6c69 7473 203d 2073 656c  oot_splits = sel
-00005cc0: 662e 5f73 6f72 745f 6469 7669 6469 6e67  f._sort_dividing
-00005cd0: 5f63 656c 6c73 2872 6f6f 745f 7370 6c69  _cells(root_spli
-00005ce0: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-00005cf0: 2020 2020 2020 2020 2066 6972 7374 5f73           first_s
-00005d00: 706c 6974 203d 2073 6f72 7465 645f 726f  plit = sorted_ro
-00005d10: 6f74 5f73 706c 6974 735b 305d 0d0a 2020  ot_splits[0]..  
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
-00005d40: 6e5f 6469 6374 5b66 6972 7374 5f73 706c  n_dict[first_spl
-00005d50: 6974 5d20 3d20 6765 6e5f 636f 756e 740d  it] = gen_count.
-00005d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d70: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-00005d80: 6574 5f64 6963 745b 6669 7273 745f 7370  et_dict[first_sp
-00005d90: 6c69 745d 203d 2074 7261 636b 6c65 745f  lit] = tracklet_
-00005da0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00005db0: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-00005dc0: 7273 745f 7370 6c69 7420 696e 2073 656c  rst_split in sel
-00005dd0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
-00005de0: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005e00: 6172 6765 745f 6365 6c6c 7320 3d20 7365  arget_cells = se
-00005e10: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
-00005e20: 6f6f 6b75 705b 6669 7273 745f 7370 6c69  ookup[first_spli
-00005e30: 745d 0d0a 2020 2020 2020 2020 2020 2020  t]..            
-00005e40: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
-00005e50: 636f 756e 7420 3d20 6765 6e5f 636f 756e  count = gen_coun
-00005e60: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-00005e70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00005e80: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00005e90: 6e28 7461 7267 6574 5f63 656c 6c73 2929  n(target_cells))
-00005ea0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00005ec0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-00005ed0: 7472 6163 6b6c 6574 5f63 6f75 6e74 202b  tracklet_count +
-00005ee0: 2031 202b 2069 0d0a 2020 2020 2020 2020   1 + i..        
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f00: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
-00005f10: 6e74 203d 2073 656c 662e 5f75 6e69 7175  nt = self._uniqu
-00005f20: 655f 7472 6163 6b6c 6574 5f63 6f75 6e74  e_tracklet_count
-00005f30: 2874 7261 636b 6c65 745f 636f 756e 745f  (tracklet_count_
-00005f40: 7461 6b65 6e2c 2074 7261 636b 6c65 745f  taken, tracklet_
-00005f50: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
-00005f80: 6e74 5f74 616b 656e 2e61 7070 656e 6428  nt_taken.append(
-00005f90: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
-00005fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005fb0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00005fc0: 6765 745f 6365 6c6c 203d 2074 6172 6765  get_cell = targe
-00005fd0: 745f 6365 6c6c 735b 695d 0d0a 2020 2020  t_cells[i]..    
-00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00006000: 6572 6174 655f 6469 7669 6469 6e67 5f72  erate_dividing_r
-00006010: 6563 7572 7369 7665 2872 6f6f 745f 6c65  ecursive(root_le
-00006020: 6166 2c20 7461 7267 6574 5f63 656c 6c2c  af, target_cell,
-00006030: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
-00006040: 6974 732c 2067 656e 5f63 6f75 6e74 2c20  its, gen_count, 
-00006050: 7472 6163 6b6c 6574 5f63 6f75 6e74 2c20  tracklet_count, 
-00006060: 7472 6163 6b6c 6574 5f63 6f75 6e74 5f74  tracklet_count_t
-00006070: 616b 656e 290d 0a20 2020 2020 2020 2020  aken)..         
-00006080: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006090: 2064 6566 205f 756e 6971 7565 5f74 7261   def _unique_tra
-000060a0: 636b 6c65 745f 636f 756e 7428 7365 6c66  cklet_count(self
-000060b0: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-000060c0: 5f74 616b 656e 2c20 7472 6163 6b6c 6574  _taken, tracklet
-000060d0: 5f63 6f75 6e74 293a 0d0a 2020 2020 2020  _count):..      
-000060e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000060f0: 2020 7768 696c 6520 7472 6163 6b6c 6574    while tracklet
-00006100: 5f63 6f75 6e74 2069 6e20 7472 6163 6b6c  _count in trackl
-00006110: 6574 5f63 6f75 6e74 5f74 616b 656e 3a0d  et_count_taken:.
-00006120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006130: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
-00006140: 7420 203d 2074 7261 636b 6c65 745f 636f  t  = tracklet_co
-00006150: 756e 7420 2b20 3120 0d0a 2020 2020 2020  unt + 1 ..      
-00006160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006170: 2e5f 756e 6971 7565 5f74 7261 636b 6c65  ._unique_trackle
-00006180: 745f 636f 756e 7428 7472 6163 6b6c 6574  t_count(tracklet
-00006190: 5f63 6f75 6e74 5f74 616b 656e 2c20 7472  _count_taken, tr
-000061a0: 6163 6b6c 6574 5f63 6f75 6e74 290d 0a20  acklet_count).. 
-000061b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000061c0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-000061d0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
-000061e0: 6465 6620 5f69 7465 7261 7465 5f73 706c  def _iterate_spl
-000061f0: 6974 5f64 6f77 6e28 7365 6c66 2c20 726f  it_down(self, ro
-00006200: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-00006210: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-00006220: 3a0d 0a20 2020 2020 2020 2020 0d0a 2020  :..         ..  
-00006230: 2020 2020 2020 7365 6c66 2e5f 6974 6572        self._iter
-00006240: 6174 655f 6469 7669 6469 6e67 2872 6f6f  ate_dividing(roo
-00006250: 745f 726f 6f74 2c20 726f 6f74 5f6c 6561  t_root, root_lea
-00006260: 662c 2072 6f6f 745f 7370 6c69 7473 290d  f, root_splits).
-00006270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006280: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 0d0a 2020 2020 6465 6620 5f67 6574    ..    def _get
-000062b0: 5f62 6f75 6e64 6172 795f 6469 7374 2873  _boundary_dist(s
-000062c0: 656c 662c 2066 7261 6d65 2c20 7465 7374  elf, frame, test
-000062d0: 6c6f 6361 7469 6f6e 293a 0d0a 2020 2020  location):..    
-000062e0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000062f0: 6620 7365 6c66 2e6d 6173 6b20 6973 206e  f self.mask is n
-00006300: 6f74 204e 6f6e 653a 0d0a 0d0a 2020 2020  ot None:....    
-00006310: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-00006320: 2c20 696e 6469 6365 732c 206d 6173 6b63  , indices, maskc
-00006330: 656e 7472 6f69 6420 3d20 7365 6c66 2e74  entroid = self.t
-00006340: 696d 6564 5f6d 6173 6b5b 7374 7228 696e  imed_mask[str(in
-00006350: 7428 666c 6f61 7428 6672 616d 6529 2929  t(float(frame)))
-00006360: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00006370: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006380: 2020 2020 2020 2020 2020 2020 2023 2047               # G
-00006390: 6574 2074 6865 206c 6f63 6174 696f 6e20  et the location 
-000063a0: 616e 6420 6469 7374 616e 6365 2074 6f20  and distance to 
-000063b0: 7468 6520 6e65 6172 6573 7420 626f 756e  the nearest boun
-000063c0: 6461 7279 2070 6f69 6e74 0d0a 2020 2020  dary point..    
-000063d0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-000063e0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
-000063f0: 6c6f 6361 7469 6f6e 696e 6465 7820 3d20  locationindex = 
-00006400: 7472 6565 2e71 7565 7279 2874 6573 746c  tree.query(testl
-00006410: 6f63 6174 696f 6e29 0d0a 2020 2020 2020  ocation)..      
-00006420: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-00006430: 6365 5f63 656c 6c5f 6d61 736b 203d 206d  ce_cell_mask = m
-00006440: 6178 2830 2c20 6469 7374 616e 6365 5f63  ax(0, distance_c
-00006450: 656c 6c5f 6d61 736b 290d 0a20 2020 2020  ell_mask)..     
-00006460: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00006470: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00006480: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00006490: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000064a0: 6b20 3d20 300d 0a20 2020 2020 2020 2020  k = 0..         
-000064b0: 2020 2020 2020 206d 6173 6b63 656e 7472         maskcentr
-000064c0: 6f69 6420 3d20 2831 2c31 2c31 290d 0a0d  oid = (1,1,1)...
-000064d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000064e0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000064f0: 736b 2c20 6d61 736b 6365 6e74 726f 6964  sk, maskcentroid
-00006500: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00006510: 2020 200d 0a20 2020 2064 6566 205f 676c     ..    def _gl
-00006520: 6f62 616c 5f74 7261 636b 5f69 6428 7365  obal_track_id(se
-00006530: 6c66 2c20 7472 6163 6b5f 6964 293a 0d0a  lf, track_id):..
-00006540: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006550: 2020 2020 206e 756d 5f64 6967 6974 7320       num_digits 
-00006560: 3d20 6c65 6e28 7374 7228 7365 6c66 2e6d  = len(str(self.m
-00006570: 6178 5f74 7261 636b 5f64 6967 6974 2929  ax_track_digit))
-00006580: 0d0a 0d0a 2020 2020 2020 2020 7472 6163  ....        trac
-00006590: 6b5f 6964 5f73 7472 203d 2073 7472 2874  k_id_str = str(t
-000065a0: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-000065b0: 2020 6966 206c 656e 2874 7261 636b 5f69    if len(track_i
-000065c0: 645f 7374 7229 203c 206e 756d 5f64 6967  d_str) < num_dig
-000065d0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-000065e0: 2020 2074 7261 636b 5f69 645f 7374 7220     track_id_str 
-000065f0: 3d20 7472 6163 6b5f 6964 5f73 7472 2e7a  = track_id_str.z
-00006600: 6669 6c6c 286e 756d 5f64 6967 6974 7329  fill(num_digits)
-00006610: 0d0a 2020 2020 2020 2020 7472 6163 6b5f  ..        track_
-00006620: 6964 203d 2069 6e74 2874 7261 636b 5f69  id = int(track_i
-00006630: 645f 7374 7229 0d0a 2020 2020 2020 2020  d_str)..        
-00006640: 7265 7475 726e 2074 7261 636b 5f69 640d  return track_id.
-00006650: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
-00006660: 676c 6f62 616c 5f67 656e 6572 6174 696f  global_generatio
-00006670: 6e5f 6964 2873 656c 662c 2067 656e 6572  n_id(self, gener
-00006680: 6174 696f 6e5f 6964 293a 0d0a 2020 2020  ation_id):..    
-00006690: 2020 2020 0d0a 2020 2020 2020 2020 6e75      ..        nu
-000066a0: 6d5f 6469 6769 7473 203d 206c 656e 2873  m_digits = len(s
-000066b0: 7472 2873 656c 662e 6d61 785f 7472 6163  tr(self.max_trac
-000066c0: 6b5f 6469 6769 7429 290d 0a20 2020 2020  k_digit))..     
-000066d0: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
-000066e0: 5f73 7472 203d 2073 7472 2867 656e 6572  _str = str(gener
-000066f0: 6174 696f 6e5f 6964 290d 0a20 2020 2020  ation_id)..     
-00006700: 2020 2069 6620 6c65 6e28 6765 6e65 7261     if len(genera
-00006710: 7469 6f6e 5f69 645f 7374 7229 203c 206e  tion_id_str) < n
-00006720: 756d 5f64 6967 6974 733a 0d0a 2020 2020  um_digits:..    
-00006730: 2020 2020 2020 2020 2020 2020 6765 6e65              gene
-00006740: 7261 7469 6f6e 5f69 645f 7374 7220 3d20  ration_id_str = 
-00006750: 6765 6e65 7261 7469 6f6e 5f69 645f 7374  generation_id_st
-00006760: 722e 7a66 696c 6c28 6e75 6d5f 6469 6769  r.zfill(num_digi
-00006770: 7473 290d 0a20 2020 2020 2020 2067 656e  ts)..        gen
-00006780: 6572 6174 696f 6e5f 6964 203d 2069 6e74  eration_id = int
-00006790: 2867 656e 6572 6174 696f 6e5f 6964 5f73  (generation_id_s
-000067a0: 7472 290d 0a0d 0a20 2020 2020 2020 2072  tr)....        r
-000067b0: 6574 7572 6e20 6765 6e65 7261 7469 6f6e  eturn generation
-000067c0: 5f69 640d 0a0d 0a0d 0a20 2020 2064 6566  _id......    def
-000067d0: 205f 7472 6163 6b5f 636f 6d70 7574 6572   _track_computer
-000067e0: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
-000067f0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
-00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00005c60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
+00005ca0: 6620 6c65 6e28 726f 6f74 5f73 706c 6974  f len(root_split
+00005cb0: 7329 203e 2030 3a0d 0a20 2020 2020 2020  s) > 0:..       
+00005cc0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+00005cd0: 7465 645f 726f 6f74 5f73 706c 6974 7320  ted_root_splits 
+00005ce0: 3d20 7365 6c66 2e5f 736f 7274 5f64 6976  = self._sort_div
+00005cf0: 6964 696e 675f 6365 6c6c 7328 726f 6f74  iding_cells(root
+00005d00: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
+00005d10: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00005d20: 7273 745f 7370 6c69 7420 3d20 736f 7274  rst_split = sort
+00005d30: 6564 5f72 6f6f 745f 7370 6c69 7473 5b30  ed_root_splits[0
+00005d40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00005d50: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
+00005d60: 7261 7469 6f6e 5f64 6963 745b 6669 7273  ration_dict[firs
+00005d70: 745f 7370 6c69 745d 203d 2067 656e 5f63  t_split] = gen_c
+00005d80: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+00005d90: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00005da0: 7261 636b 6c65 745f 6469 6374 5b66 6972  racklet_dict[fir
+00005db0: 7374 5f73 706c 6974 5d20 3d20 7472 6163  st_split] = trac
+00005dc0: 6b6c 6574 5f63 6f75 6e74 0d0a 2020 2020  klet_count..    
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 6966 2066 6972 7374 5f73 706c 6974 2069  if first_split i
+00005df0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
+00005e00: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2020 7461 7267 6574 5f63 656c 6c73      target_cells
+00005e30: 203d 2073 656c 662e 6564 6765 5f74 6172   = self.edge_tar
+00005e40: 6765 745f 6c6f 6f6b 7570 5b66 6972 7374  get_lookup[first
+00005e50: 5f73 706c 6974 5d0d 0a20 2020 2020 2020  _split]..       
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2067 656e 5f63 6f75 6e74 203d 2067 656e   gen_count = gen
+00005e80: 5f63 6f75 6e74 202b 2031 0d0a 2020 2020  _count + 1..    
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00005eb0: 6765 286c 656e 2874 6172 6765 745f 6365  ge(len(target_ce
+00005ec0: 6c6c 7329 293a 0d0a 2020 2020 2020 2020  lls)):..        
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ee0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+00005ef0: 6e74 203d 2074 7261 636b 6c65 745f 636f  nt = tracklet_co
+00005f00: 756e 7420 2b20 3120 2b20 690d 0a20 2020  unt + 1 + i..   
+00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f20: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00005f30: 745f 636f 756e 7420 3d20 7365 6c66 2e5f  t_count = self._
+00005f40: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+00005f50: 636f 756e 7428 7472 6163 6b6c 6574 5f63  count(tracklet_c
+00005f60: 6f75 6e74 5f74 616b 656e 2c20 7472 6163  ount_taken, trac
+00005f70: 6b6c 6574 5f63 6f75 6e74 290d 0a20 2020  klet_count)..   
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00005fa0: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
+00005fb0: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
+00005fc0: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fe0: 2020 7461 7267 6574 5f63 656c 6c20 3d20    target_cell = 
+00005ff0: 7461 7267 6574 5f63 656c 6c73 5b69 5d0d  target_cells[i].
+00006000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006010: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006020: 662e 5f69 7465 7261 7465 5f64 6976 6964  f._iterate_divid
+00006030: 696e 675f 7265 6375 7273 6976 6528 726f  ing_recursive(ro
+00006040: 6f74 5f6c 6561 662c 2074 6172 6765 745f  ot_leaf, target_
+00006050: 6365 6c6c 2c20 736f 7274 6564 5f72 6f6f  cell, sorted_roo
+00006060: 745f 7370 6c69 7473 2c20 6765 6e5f 636f  t_splits, gen_co
+00006070: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
+00006080: 756e 742c 2074 7261 636b 6c65 745f 636f  unt, tracklet_co
+00006090: 756e 745f 7461 6b65 6e29 0d0a 2020 2020  unt_taken)..    
+000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060b0: 0d0a 2020 2020 6465 6620 5f75 6e69 7175  ..    def _uniqu
+000060c0: 655f 7472 6163 6b6c 6574 5f63 6f75 6e74  e_tracklet_count
+000060d0: 2873 656c 662c 2074 7261 636b 6c65 745f  (self, tracklet_
+000060e0: 636f 756e 745f 7461 6b65 6e2c 2074 7261  count_taken, tra
+000060f0: 636b 6c65 745f 636f 756e 7429 3a0d 0a20  cklet_count):.. 
+00006100: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006110: 2020 2020 2020 2077 6869 6c65 2074 7261         while tra
+00006120: 636b 6c65 745f 636f 756e 7420 696e 2074  cklet_count in t
+00006130: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
+00006140: 6b65 6e3a 0d0a 2020 2020 2020 2020 2020  ken:..          
+00006150: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
+00006160: 5f63 6f75 6e74 2020 3d20 7472 6163 6b6c  _count  = trackl
+00006170: 6574 5f63 6f75 6e74 202b 2031 200d 0a20  et_count + 1 .. 
+00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006190: 2073 656c 662e 5f75 6e69 7175 655f 7472   self._unique_tr
+000061a0: 6163 6b6c 6574 5f63 6f75 6e74 2874 7261  acklet_count(tra
+000061b0: 636b 6c65 745f 636f 756e 745f 7461 6b65  cklet_count_take
+000061c0: 6e2c 2074 7261 636b 6c65 745f 636f 756e  n, tracklet_coun
+000061d0: 7429 0d0a 2020 2020 2020 2020 2020 2072  t)..           r
+000061e0: 6574 7572 6e20 7472 6163 6b6c 6574 5f63  eturn tracklet_c
+000061f0: 6f75 6e74 2020 2020 2020 200d 0a0d 0a0d  ount       .....
+00006200: 0a20 2020 2064 6566 205f 6974 6572 6174  .    def _iterat
+00006210: 655f 7370 6c69 745f 646f 776e 2873 656c  e_split_down(sel
+00006220: 662c 2072 6f6f 745f 726f 6f74 2c20 726f  f, root_root, ro
+00006230: 6f74 5f6c 6561 662c 2072 6f6f 745f 7370  ot_leaf, root_sp
+00006240: 6c69 7473 293a 0d0a 2020 2020 2020 2020  lits):..        
+00006250: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00006260: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
+00006270: 6728 726f 6f74 5f72 6f6f 742c 2072 6f6f  g(root_root, roo
+00006280: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
+00006290: 6974 7329 0d0a 2020 2020 2020 2020 2020  its)..          
+000062a0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062c0: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+000062d0: 205f 6765 745f 626f 756e 6461 7279 5f64   _get_boundary_d
+000062e0: 6973 7428 7365 6c66 2c20 6672 616d 652c  ist(self, frame,
+000062f0: 2074 6573 746c 6f63 6174 696f 6e29 3a0d   testlocation):.
+00006300: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
+00006310: 2020 2020 6966 2073 656c 662e 6d61 736b      if self.mask
+00006320: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d   is not None:...
+00006330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006340: 2074 7265 652c 2069 6e64 6963 6573 2c20   tree, indices, 
+00006350: 6d61 736b 6365 6e74 726f 6964 203d 2073  maskcentroid = s
+00006360: 656c 662e 7469 6d65 645f 6d61 736b 5b73  elf.timed_mask[s
+00006370: 7472 2869 6e74 2866 6c6f 6174 2866 7261  tr(int(float(fra
+00006380: 6d65 2929 295d 0d0a 2020 2020 2020 2020  me)))]..        
+00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000063b0: 2020 2320 4765 7420 7468 6520 6c6f 6361    # Get the loca
+000063c0: 7469 6f6e 2061 6e64 2064 6973 7461 6e63  tion and distanc
+000063d0: 6520 746f 2074 6865 206e 6561 7265 7374  e to the nearest
+000063e0: 2062 6f75 6e64 6172 7920 706f 696e 740d   boundary point.
+000063f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006400: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+00006410: 6173 6b2c 206c 6f63 6174 696f 6e69 6e64  ask, locationind
+00006420: 6578 203d 2074 7265 652e 7175 6572 7928  ex = tree.query(
+00006430: 7465 7374 6c6f 6361 7469 6f6e 290d 0a20  testlocation).. 
+00006440: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006450: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00006460: 6b20 3d20 6d61 7828 302c 2064 6973 7461  k = max(0, dista
+00006470: 6e63 655f 6365 6c6c 5f6d 6173 6b29 0d0a  nce_cell_mask)..
+00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006490: 2020 200d 0a20 2020 2020 2020 2065 6c73     ..        els
+000064a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000064b0: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+000064c0: 6c5f 6d61 736b 203d 2030 0d0a 2020 2020  l_mask = 0..    
+000064d0: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+000064e0: 6365 6e74 726f 6964 203d 2028 312c 312c  centroid = (1,1,
+000064f0: 3129 0d0a 0d0a 2020 2020 2020 2020 7265  1)....        re
+00006500: 7475 726e 2064 6973 7461 6e63 655f 6365  turn distance_ce
+00006510: 6c6c 5f6d 6173 6b2c 206d 6173 6b63 656e  ll_mask, maskcen
+00006520: 7472 6f69 6420 2020 2020 2020 200d 0a20  troid        .. 
+00006530: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00006540: 6620 5f67 6c6f 6261 6c5f 7472 6163 6b5f  f _global_track_
+00006550: 6964 2873 656c 662c 2074 7261 636b 5f69  id(self, track_i
+00006560: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
+00006570: 0d0a 2020 2020 2020 2020 6e75 6d5f 6469  ..        num_di
+00006580: 6769 7473 203d 206c 656e 2873 7472 2873  gits = len(str(s
+00006590: 656c 662e 6d61 785f 7472 6163 6b5f 6469  elf.max_track_di
+000065a0: 6769 7429 290d 0a0d 0a20 2020 2020 2020  git))....       
+000065b0: 2074 7261 636b 5f69 645f 7374 7220 3d20   track_id_str = 
+000065c0: 7374 7228 7472 6163 6b5f 6964 290d 0a20  str(track_id).. 
+000065d0: 2020 2020 2020 2069 6620 6c65 6e28 7472         if len(tr
+000065e0: 6163 6b5f 6964 5f73 7472 2920 3c20 6e75  ack_id_str) < nu
+000065f0: 6d5f 6469 6769 7473 3a0d 0a20 2020 2020  m_digits:..     
+00006600: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+00006610: 5f73 7472 203d 2074 7261 636b 5f69 645f  _str = track_id_
+00006620: 7374 722e 7a66 696c 6c28 6e75 6d5f 6469  str.zfill(num_di
+00006630: 6769 7473 290d 0a20 2020 2020 2020 2074  gits)..        t
+00006640: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
+00006650: 6163 6b5f 6964 5f73 7472 290d 0a20 2020  ack_id_str)..   
+00006660: 2020 2020 2072 6574 7572 6e20 7472 6163       return trac
+00006670: 6b5f 6964 0d0a 2020 2020 0d0a 2020 2020  k_id..    ..    
+00006680: 6465 6620 5f67 6c6f 6261 6c5f 6765 6e65  def _global_gene
+00006690: 7261 7469 6f6e 5f69 6428 7365 6c66 2c20  ration_id(self, 
+000066a0: 6765 6e65 7261 7469 6f6e 5f69 6429 3a0d  generation_id):.
+000066b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+000066c0: 2020 206e 756d 5f64 6967 6974 7320 3d20     num_digits = 
+000066d0: 6c65 6e28 7374 7228 7365 6c66 2e6d 6178  len(str(self.max
+000066e0: 5f74 7261 636b 5f64 6967 6974 2929 0d0a  _track_digit))..
+000066f0: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+00006700: 6f6e 5f69 645f 7374 7220 3d20 7374 7228  on_id_str = str(
+00006710: 6765 6e65 7261 7469 6f6e 5f69 6429 0d0a  generation_id)..
+00006720: 2020 2020 2020 2020 6966 206c 656e 2867          if len(g
+00006730: 656e 6572 6174 696f 6e5f 6964 5f73 7472  eneration_id_str
+00006740: 2920 3c20 6e75 6d5f 6469 6769 7473 3a0d  ) < num_digits:.
+00006750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006760: 2067 656e 6572 6174 696f 6e5f 6964 5f73   generation_id_s
+00006770: 7472 203d 2067 656e 6572 6174 696f 6e5f  tr = generation_
+00006780: 6964 5f73 7472 2e7a 6669 6c6c 286e 756d  id_str.zfill(num
+00006790: 5f64 6967 6974 7329 0d0a 2020 2020 2020  _digits)..      
+000067a0: 2020 6765 6e65 7261 7469 6f6e 5f69 6420    generation_id 
+000067b0: 3d20 696e 7428 6765 6e65 7261 7469 6f6e  = int(generation
+000067c0: 5f69 645f 7374 7229 0d0a 0d0a 2020 2020  _id_str)....    
+000067d0: 2020 2020 7265 7475 726e 2067 656e 6572      return gener
+000067e0: 6174 696f 6e5f 6964 0d0a 0d0a 0d0a 2020  ation_id......  
+000067f0: 2020 6465 6620 5f74 7261 636b 5f63 6f6d    def _track_com
+00006800: 7075 7465 7228 7365 6c66 2c20 7472 6163  puter(self, trac
+00006810: 6b2c 2074 7261 636b 5f69 6429 3a0d 0a20  k, track_id):.. 
 00006820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006830: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006830: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00006860: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 756e 6971 7565 5f74 7261        unique_tra
-00006890: 636b 6c65 745f 6964 7320 3d20 5b5d 0d0a  cklet_ids = []..
-000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-000068c0: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-000068d0: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-000068e0: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-000068f0: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-00006900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006910: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00006920: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-00006930: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-00006940: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-00006950: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-00006960: 7572 6365 5f69 6473 2920 0d0a 2020 2020  urce_ids) ..    
-00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006980: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00006990: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
-000069a0: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
-000069b0: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-000069c0: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000069f0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00006a00: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
-00006a10: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
-00006a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006a40: 4465 7465 726d 696e 6520 6966 2061 2074  Determine if a t
-00006a50: 7261 636b 2068 6173 2064 6976 6973 696f  rack has divisio
-00006a60: 6e73 206f 7220 6e6f 6e65 0d0a 2020 2020  ns or none..    
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00006a90: 6f6f 745f 7370 6c69 7473 2920 3e20 303a  oot_splits) > 0:
-00006aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ac0: 2020 7365 6c66 2e75 6e69 7175 655f 7472    self.unique_tr
-00006ad0: 6163 6b5f 6d69 746f 7369 735f 6c61 6265  ack_mitosis_labe
-00006ae0: 6c5b 7472 6163 6b5f 6964 5d20 3d20 5b31  l[track_id] = [1
-00006af0: 2c20 6e75 6d62 6572 5f64 6976 6964 696e  , number_dividin
-00006b00: 675d 0d0a 2020 2020 2020 2020 2020 2020  g]..            
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
-00006b30: 6a65 6374 6f72 7920 3d20 5472 7565 0d0a  jectory = True..
-00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b60: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-00006b70: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
-00006b80: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006bb0: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-00006bc0: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
-00006bd0: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-00006c00: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
-00006c10: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-00006c20: 6b49 6473 3a20 2020 2020 0d0a 2020 2020  kIds:     ..    
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-00006c60: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
-00006c70: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
-00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006850: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00006880: 6365 6c6c 5f69 6473 203d 205b 5d0d 0a20  cell_ids = [].. 
+00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068a0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+000068b0: 655f 7472 6163 6b6c 6574 5f69 6473 203d  e_tracklet_ids =
+000068c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
+000068f0: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
+00006900: 3d20 2073 656c 662e 5f67 656e 6572 6174  =  self._generat
+00006910: 655f 6765 6e65 7261 7469 6f6e 7328 7472  e_generations(tr
+00006920: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 726f 6f74 5f72 6f6f 742c 2072 6f6f    root_root, roo
+00006950: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00006960: 6561 6620 3d20 7365 6c66 2e5f 6372 6561  eaf = self._crea
+00006970: 7465 5f67 656e 6572 6174 696f 6e73 2861  te_generations(a
+00006980: 6c6c 5f73 6f75 7263 655f 6964 7329 200d  ll_source_ids) .
+00006990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000069b0: 662e 5f69 7465 7261 7465 5f73 706c 6974  f._iterate_split
+000069c0: 5f64 6f77 6e28 726f 6f74 5f72 6f6f 742c  _down(root_root,
+000069d0: 2072 6f6f 745f 6c65 6166 2c20 726f 6f74   root_leaf, root
+000069e0: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 206e 756d 6265 725f 6469 7669 6469     number_dividi
+00006a30: 6e67 203d 206c 656e 2872 6f6f 745f 7370  ng = len(root_sp
+00006a40: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2023 2044 6574 6572 6d69 6e65 2069     # Determine i
+00006a70: 6620 6120 7472 6163 6b20 6861 7320 6469  f a track has di
+00006a80: 7669 7369 6f6e 7320 6f72 206e 6f6e 650d  visions or none.
+00006a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006aa0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006ab0: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00006ac0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00006af0: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
+00006b00: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
+00006b10: 203d 205b 312c 206e 756d 6265 725f 6469   = [1, number_di
+00006b20: 7669 6469 6e67 5d0d 0a20 2020 2020 2020  viding]..       
+00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b40: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+00006b50: 675f 7472 616a 6563 746f 7279 203d 2054  g_trajectory = T
+00006b60: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00006b90: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00006ba0: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bd0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00006be0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+00006bf0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00006c20: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00006c30: 2069 6e20 7365 6c66 2e44 6976 6964 696e   in self.Dividin
+00006c40: 6754 7261 636b 4964 733a 2020 2020 200d  gTrackIds:     .
+00006c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c70: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+00006c80: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+00006c90: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+00006ca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00006cc0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006cf0: 6e69 7175 655f 7472 6163 6b5f 6d69 746f  nique_track_mito
-00006d00: 7369 735f 6c61 6265 6c5b 7472 6163 6b5f  sis_label[track_
-00006d10: 6964 5d20 3d20 5b30 2c20 305d 0d0a 2020  id] = [0, 0]..  
-00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d30: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00006d40: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00006d50: 7920 3d20 4661 6c73 650d 0a20 2020 2020  y = False..     
-00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d70: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00006d80: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
-00006d90: 696e 2073 656c 662e 416c 6c54 7261 636b  in self.AllTrack
-00006da0: 4964 733a 0d0a 2020 2020 2020 2020 2020  Ids:..          
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-00006dd0: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-00006de0: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
-00006df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
-00006e20: 6429 206e 6f74 2069 6e20 7365 6c66 2e4e  d) not in self.N
-00006e30: 6f72 6d61 6c54 7261 636b 4964 733a 2020  ormalTrackIds:  
-00006e40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-00006e70: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-00006e80: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-00006e90: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2066 6f72 206c 6561 6620 696e 2072 6f6f   for leaf in roo
-00006ec0: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ee0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-00006ef0: 6365 5f6c 6561 6620 3d20 7365 6c66 2e65  ce_leaf = self.e
-00006f00: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-00006f10: 705b 6c65 6166 5d0d 0a20 2020 2020 2020  p[leaf]..       
-00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00006f40: 656e 745f 6365 6c6c 5f69 6473 2e61 7070  ent_cell_ids.app
-00006f50: 656e 6428 6c65 6166 2920 0d0a 2020 2020  end(leaf) ..    
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006f80: 656c 662e 5f64 6963 745f 7570 6461 7465  elf._dict_update
-00006f90: 2875 6e69 7175 655f 7472 6163 6b6c 6574  (unique_tracklet
-00006fa0: 5f69 6473 2c20 6c65 6166 2c20 7472 6163  _ids, leaf, trac
-00006fb0: 6b5f 6964 2c20 736f 7572 6365 5f6c 6561  k_id, source_lea
-00006fc0: 662c 204e 6f6e 6529 0d0a 2020 2020 2020  f, None)..      
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006ff0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007000: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
-00007010: 7064 6174 6528 7b73 656c 662e 6469 7669  pdate({self.divi
-00007020: 6469 6e67 5f6b 6579 203a 2064 6976 6964  ding_key : divid
-00007030: 696e 675f 7472 616a 6563 746f 7279 7d29  ing_trajectory})
-00007040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00007070: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007080: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
-00007090: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-000070a0: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-000070b0: 5f64 6976 6964 696e 677d 290d 0a0d 0a20  _dividing}).... 
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-000070e0: 6f75 7263 655f 6964 2069 6e20 616c 6c5f  ource_id in all_
-000070f0: 736f 7572 6365 5f69 6473 3a0d 0a20 2020  source_ids:..   
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007120: 2020 2020 2074 6172 6765 745f 6964 7320       target_ids 
-00007130: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
-00007140: 6574 5f6c 6f6f 6b75 705b 736f 7572 6365  et_lookup[source
-00007150: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00007180: 7272 656e 745f 6365 6c6c 5f69 6473 2e61  rrent_cell_ids.a
-00007190: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
-000071a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 2020 2020 2020 2020 2352 6f6f 740d            #Root.
-000071d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007200: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007210: 7469 6573 5b73 6f75 7263 655f 6964 5d2e  ties[source_id].
-00007220: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-00007230: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-00007240: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-00007250: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007280: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00007290: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
-000072a0: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
-000072b0: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
-000072c0: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
-000072d0: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
-000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 6966 2073 6f75 7263 655f 6964 206e 6f74  if source_id not
-00007310: 2069 6e20 616c 6c5f 7461 7267 6574 5f69   in all_target_i
-00007320: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006ce0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006d10: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00006d20: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
+00006d30: 7261 636b 5f69 645d 203d 205b 302c 2030  rack_id] = [0, 0
+00006d40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 2020 2064 6976 6964 696e 675f 7472 616a     dividing_traj
+00006d70: 6563 746f 7279 203d 2046 616c 7365 0d0a  ectory = False..
+00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
+00006db0: 206e 6f74 2069 6e20 7365 6c66 2e41 6c6c   not in self.All
+00006dc0: 5472 6163 6b49 6473 3a0d 0a20 2020 2020  TrackIds:..     
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006df0: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
+00006e00: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00006e10: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e30: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
+00006e40: 6163 6b5f 6964 2920 6e6f 7420 696e 2073  ack_id) not in s
+00006e50: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+00006e60: 6473 3a20 2020 200d 0a20 2020 2020 2020  ds:    ..       
+00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006e90: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+00006ea0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+00006eb0: 6b5f 6964 2929 0d0a 0d0a 2020 2020 2020  k_id))....      
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2020 2020 2020 666f 7220 6c65 6166 2069        for leaf i
+00006ee0: 6e20 726f 6f74 5f6c 6561 663a 0d0a 2020  n root_leaf:..  
+00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2073 6f75 7263 655f 6c65 6166 203d 2073   source_leaf = s
+00006f20: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00006f30: 6c6f 6f6b 7570 5b6c 6561 665d 0d0a 2020  lookup[leaf]..  
+00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
+00006f70: 732e 6170 7065 6e64 286c 6561 6629 200d  s.append(leaf) .
+00006f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 2020 7365 6c66 2e5f 6469 6374 5f75      self._dict_u
+00006fb0: 7064 6174 6528 756e 6971 7565 5f74 7261  pdate(unique_tra
+00006fc0: 636b 6c65 745f 6964 732c 206c 6561 662c  cklet_ids, leaf,
+00006fd0: 2074 7261 636b 5f69 642c 2073 6f75 7263   track_id, sourc
+00006fe0: 655f 6c65 6166 2c20 4e6f 6e65 290d 0a20  e_leaf, None).. 
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00007020: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
+00007030: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
+00007040: 2e64 6976 6964 696e 675f 6b65 7920 3a20  .dividing_key : 
+00007050: 6469 7669 6469 6e67 5f74 7261 6a65 6374  dividing_traject
+00007060: 6f72 797d 290d 0a20 2020 2020 2020 2020  ory})..         
+00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007080: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007090: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000070a0: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
+000070b0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
+000070c0: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
+000070d0: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
+000070e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 666f 7220 736f 7572 6365 5f69 6420 696e  for source_id in
+00007110: 2061 6c6c 5f73 6f75 7263 655f 6964 733a   all_source_ids:
+00007120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00007150: 5f69 6473 203d 2073 656c 662e 6564 6765  _ids = self.edge
+00007160: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b73  _target_lookup[s
+00007170: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071a0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+000071b0: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
+000071c0: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
+000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000071f0: 526f 6f74 0d0a 2020 2020 2020 2020 2020  Root..          
+00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007210: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007220: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00007230: 726f 7065 7274 6965 735b 736f 7572 6365  roperties[source
+00007240: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+00007250: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+00007260: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+00007270: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
+00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000072b0: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
+000072c0: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
+000072d0: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+000072e0: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
+000072f0: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
+00007330: 6420 6e6f 7420 696e 2061 6c6c 5f74 6172  d not in all_tar
+00007340: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 2066 6f72 2074 6172 6765         for targe
-00007390: 745f 6964 2069 6e20 7461 7267 6574 5f69  t_id in target_i
-000073a0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 2020 2020 2020 2020 7365 6c66 2e5f 6469          self._di
-000073e0: 6374 5f75 7064 6174 6528 756e 6971 7565  ct_update(unique
-000073f0: 5f74 7261 636b 6c65 745f 6964 732c 2073  _tracklet_ids, s
-00007400: 6f75 7263 655f 6964 2c20 7472 6163 6b5f  ource_id, track_
-00007410: 6964 2c20 4e6f 6e65 2c20 7461 7267 6574  id, None, target
-00007420: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
-00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007450: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00007460: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007470: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
-00007480: 7570 6461 7465 287b 7365 6c66 2e64 6976  update({self.div
-00007490: 6964 696e 675f 6b65 7920 3a20 6469 7669  iding_key : divi
-000074a0: 6469 6e67 5f74 7261 6a65 6374 6f72 797d  ding_trajectory}
-000074b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000074f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00007500: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
-00007510: 6174 6528 7b73 656c 662e 6e75 6d62 6572  ate({self.number
-00007520: 5f64 6976 6964 696e 675f 6b65 7920 3a20  _dividing_key : 
-00007530: 6e75 6d62 6572 5f64 6976 6964 696e 677d  number_dividing}
-00007540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00007570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007370: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000073b0: 7461 7267 6574 5f69 6420 696e 2074 6172  target_id in tar
+000073c0: 6765 745f 6964 733a 0d0a 2020 2020 2020  get_ids:..      
+000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007400: 662e 5f64 6963 745f 7570 6461 7465 2875  f._dict_update(u
+00007410: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
+00007420: 6473 2c20 736f 7572 6365 5f69 642c 2074  ds, source_id, t
+00007430: 7261 636b 5f69 642c 204e 6f6e 652c 2074  rack_id, None, t
+00007440: 6172 6765 745f 6964 290d 0a20 2020 2020  arget_id)..     
+00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007470: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007480: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00007490: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
+000074a0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+000074b0: 662e 6469 7669 6469 6e67 5f6b 6579 203a  f.dividing_key :
+000074c0: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
+000074d0: 746f 7279 7d29 0d0a 2020 2020 2020 2020  tory})..        
+000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007510: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00007520: 6572 7469 6573 5b74 6172 6765 745f 6964  erties[target_id
+00007530: 5d2e 7570 6461 7465 287b 7365 6c66 2e6e  ].update({self.n
+00007540: 756d 6265 725f 6469 7669 6469 6e67 5f6b  umber_dividing_k
+00007550: 6579 203a 206e 756d 6265 725f 6469 7669  ey : number_divi
+00007560: 6469 6e67 7d29 0d0a 2020 2020 2020 2020  ding})..        
+00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 234e 6f72 6d61 6c20 2020 2020 2020 200d  #Normal        .
-000075b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000075e0: 6f75 7263 655f 736f 7572 6365 5f69 6420  ource_source_id 
-000075f0: 3d20 7365 6c66 2e65 6467 655f 736f 7572  = self.edge_sour
-00007600: 6365 5f6c 6f6f 6b75 705b 736f 7572 6365  ce_lookup[source
-00007610: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
-00007650: 6420 696e 2074 6172 6765 745f 6964 733a  d in target_ids:
-00007660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 2020 7365 6c66 2e5f 6469 6374        self._dict
-000076a0: 5f75 7064 6174 6528 756e 6971 7565 5f74  _update(unique_t
-000076b0: 7261 636b 6c65 745f 6964 732c 2073 6f75  racklet_ids, sou
-000076c0: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
-000076d0: 2c20 736f 7572 6365 5f73 6f75 7263 655f  , source_source_
-000076e0: 6964 2c20 7461 7267 6574 5f69 6429 200d  id, target_id) .
-000076f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00007730: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00007740: 5b74 6172 6765 745f 6964 5d2e 7570 6461  [target_id].upda
-00007750: 7465 287b 7365 6c66 2e64 6976 6964 696e  te({self.dividin
-00007760: 675f 6b65 7920 3a20 6469 7669 6469 6e67  g_key : dividing
-00007770: 5f74 7261 6a65 6374 6f72 797d 2920 0d0a  _trajectory}) ..
-00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000077c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000077d0: 7461 7267 6574 5f69 645d 2e75 7064 6174  target_id].updat
-000077e0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-000077f0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00007800: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00007810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00007590: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075c0: 2020 2020 2023 4e6f 726d 616c 2020 2020       #Normal    
+000075d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 2020 2020 736f 7572 6365 5f73 6f75 7263      source_sourc
+00007610: 655f 6964 203d 2073 656c 662e 6564 6765  e_id = self.edge
+00007620: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b73  _source_lookup[s
+00007630: 6f75 7263 655f 6964 5d0d 0a20 2020 2020  ource_id]..     
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2020 2020 2020 2066 6f72 2074 6172           for tar
+00007670: 6765 745f 6964 2069 6e20 7461 7267 6574  get_id in target
+00007680: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000076c0: 5f64 6963 745f 7570 6461 7465 2875 6e69  _dict_update(uni
+000076d0: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
+000076e0: 2c20 736f 7572 6365 5f69 642c 2074 7261  , source_id, tra
+000076f0: 636b 5f69 642c 2073 6f75 7263 655f 736f  ck_id, source_so
+00007700: 7572 6365 5f69 642c 2074 6172 6765 745f  urce_id, target_
+00007710: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007740: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00007750: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00007760: 7274 6965 735b 7461 7267 6574 5f69 645d  rties[target_id]
+00007770: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
+00007780: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
+00007790: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
+000077a0: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000077e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000077f0: 7469 6573 5b74 6172 6765 745f 6964 5d2e  ties[target_id].
+00007800: 7570 6461 7465 287b 7365 6c66 2e6e 756d  update({self.num
+00007810: 6265 725f 6469 7669 6469 6e67 5f6b 6579  ber_dividing_key
+00007820: 203a 206e 756d 6265 725f 6469 7669 6469   : number_dividi
+00007830: 6e67 7d29 0d0a 2020 2020 2020 2020 2020  ng})..          
 00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007860: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00007850: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00007860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007880: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007880: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
-000078b0: 726f 6f74 2069 6e20 726f 6f74 5f72 6f6f  root in root_roo
-000078c0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-000078f0: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
-00007900: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
-00007910: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00007920: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
-00007930: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
-00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007950: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 2020 2020 7365 6c66 2e61 6c6c 5f63        self.all_c
-00007980: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
-00007990: 696e 7428 7472 6163 6b5f 6964 295d 203d  int(track_id)] =
-000079a0: 2063 7572 7265 6e74 5f63 656c 6c5f 6964   current_cell_id
-000079b0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000079d0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-000079e0: 6e28 6375 7272 656e 745f 6365 6c6c 5f69  n(current_cell_i
-000079f0: 6473 2929 3a0d 0a20 2020 2020 2020 2020  ds)):..         
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a10: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000078a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2066 6f72 2063 7572           for cur
+000078d0: 7265 6e74 5f72 6f6f 7420 696e 2072 6f6f  rent_root in roo
+000078e0: 745f 726f 6f74 3a0d 0a20 2020 2020 2020  t_root:..       
+000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007910: 2e72 6f6f 745f 7370 6f74 735b 696e 7428  .root_spots[int(
+00007920: 6375 7272 656e 745f 726f 6f74 295d 203d  current_root)] =
+00007930: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00007940: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00007950: 2863 7572 7265 6e74 5f72 6f6f 7429 5d0d  (current_root)].
+00007960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007970: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000079a0: 616c 6c5f 6375 7272 656e 745f 6365 6c6c  all_current_cell
+000079b0: 5f69 6473 5b69 6e74 2874 7261 636b 5f69  _ids[int(track_i
+000079c0: 6429 5d20 3d20 6375 7272 656e 745f 6365  d)] = current_ce
+000079d0: 6c6c 5f69 6473 0d0a 2020 2020 2020 2020  ll_ids..        
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079f0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00007a00: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
+00007a10: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a40: 2020 2020 206b 203d 2069 6e74 2863 7572       k = int(cur
-00007a50: 7265 6e74 5f63 656c 6c5f 6964 735b 695d  rent_cell_ids[i]
-00007a60: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00007a90: 6963 745f 7661 6c75 6573 203d 2073 656c  ict_values = sel
-00007aa0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00007ab0: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+00007a70: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
+00007a80: 6473 5b69 5d29 2020 2020 0d0a 2020 2020  ds[i])    ..    
+00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ab0: 616c 6c5f 6469 6374 5f76 616c 7565 7320  all_dict_values 
+00007ac0: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00007ad0: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
 00007ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
-00007b10: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00007b20: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-00007b30: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00007b60: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00007b70: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
-00007b80: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
-00007bb0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00007bc0: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
-00007bd0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00007c00: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-00007c10: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
-00007c20: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00007b00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b20: 2020 2020 2020 2020 2020 2074 203d 2069             t = i
+00007b30: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
+00007b40: 745f 7661 6c75 6573 5b73 656c 662e 6672  t_values[self.fr
+00007b50: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b80: 2020 7a20 3d20 666c 6f61 7428 616c 6c5f    z = float(all_
+00007b90: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00007ba0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 2079 203d 2066 6c6f 6174 2861 6c6c     y = float(all
+00007be0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00007bf0: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2020 2020 7820 3d20 666c 6f61 7428 616c      x = float(al
+00007c30: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00007c40: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+00007c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-00007c80: 745f 6365 6e74 726f 6964 203d 2028 726f  t_centroid = (ro
-00007c90: 756e 6428 7a29 2f73 656c 662e 7a63 616c  und(z)/self.zcal
-00007ca0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
-00007cb0: 7929 2f73 656c 662e 7963 616c 6962 7261  y)/self.ycalibra
-00007cc0: 7469 6f6e 2c20 726f 756e 6428 7829 2f73  tion, round(x)/s
-00007cd0: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-00007ce0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
-00007d10: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
-00007d20: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
-00007d30: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
-00007d40: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
-00007d50: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
-00007d60: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
-00007d70: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007da0: 756e 6971 7565 5f73 706f 745f 6365 6e74  unique_spot_cent
-00007db0: 726f 6964 5b66 7261 6d65 5f73 706f 745f  roid[frame_spot_
-00007dc0: 6365 6e74 726f 6964 5d20 3d20 6b0d 0a20  centroid] = k.. 
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00007e00: 7261 636b 5f63 656e 7472 6f69 645b 6672  rack_centroid[fr
-00007e10: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00007e20: 645d 203d 2074 7261 636b 5f69 640d 0a0d  d] = track_id...
-00007e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e50: 2020 2020 2069 6620 7374 7228 7429 2069       if str(t) i
-00007e60: 6e20 7365 6c66 2e5f 7469 6d65 645f 6365  n self._timed_ce
-00007e70: 6e74 726f 6964 3a0d 0a20 2020 2020 2020  ntroid:..       
-00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 7472 6565 2c20 7370 6f74 5f63      tree, spot_c
-00007eb0: 656e 7472 6f69 6473 203d 2073 656c 662e  entroids = self.
-00007ec0: 5f74 696d 6564 5f63 656e 7472 6f69 645b  _timed_centroid[
-00007ed0: 7374 7228 7429 5d0d 0a20 2020 2020 2020  str(t)]..       
-00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00007f10: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
-00007f20: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
-00007f60: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
-00007f70: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
-00007fb0: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
-00007fc0: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
-00007fd0: 745f 6365 6e74 726f 6964 7320 0d0a 2020  t_centroids ..  
-00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008000: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00007c70: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 7370 6f74 5f63 656e 7472 6f69 6420    spot_centroid 
+00007cb0: 3d20 2872 6f75 6e64 287a 292f 7365 6c66  = (round(z)/self
+00007cc0: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
+00007cd0: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
+00007ce0: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
+00007cf0: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
+00007d00: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+00007d30: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+00007d40: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
+00007d50: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00007d60: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+00007d70: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+00007d80: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+00007d90: 6272 6174 696f 6e29 0d0a 0d0a 2020 2020  bration)....    
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dc0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00007dd0: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+00007de0: 7370 6f74 5f63 656e 7472 6f69 645d 203d  spot_centroid] =
+00007df0: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
+00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e10: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00007e20: 7175 655f 7472 6163 6b5f 6365 6e74 726f  que_track_centro
+00007e30: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
+00007e40: 6e74 726f 6964 5d20 3d20 7472 6163 6b5f  ntroid] = track_
+00007e50: 6964 0d0a 0d0a 2020 2020 2020 2020 2020  id....          
+00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e70: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00007e80: 2874 2920 696e 2073 656c 662e 5f74 696d  (t) in self._tim
+00007e90: 6564 5f63 656e 7472 6f69 643a 0d0a 2020  ed_centroid:..  
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ec0: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
+00007ed0: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
+00007ee0: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+00007ef0: 726f 6964 5b73 7472 2874 295d 0d0a 2020  roid[str(t)]..  
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f20: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+00007f30: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
+00007f40: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
+00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f70: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+00007f80: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00007f90: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
+00007fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007fd0: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00007fe0: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
+00007ff0: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
+00008000: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00008040: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008070: 2020 2020 7370 6f74 5f63 656e 7472 6f69      spot_centroi
-00008080: 6473 2e61 7070 656e 6428 7370 6f74 5f63  ds.append(spot_c
-00008090: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
-000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080c0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
-000080d0: 6961 6c2e 634b 4454 7265 6528 7370 6f74  ial.cKDTree(spot
-000080e0: 5f63 656e 7472 6f69 6473 290d 0a20 2020  _centroids)..   
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008110: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
-00008120: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
-00008130: 2874 295d 203d 2074 7265 652c 2073 706f  (t)] = tree, spo
-00008140: 745f 6365 6e74 726f 6964 730d 0a20 2020  t_centroids..   
-00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00008170: 2064 6566 205f 6d61 7374 6572 5f74 7261   def _master_tra
-00008180: 636b 5f63 6f6d 7075 7465 7228 7365 6c66  ck_computer(self
-00008190: 2c20 7472 6163 6b2c 2074 7261 636b 5f69  , track, track_i
-000081a0: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008020: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008050: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+00008060: 6e74 726f 6964 7320 3d20 5b5d 0d0a 2020  ntroids = []..  
+00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2073 706f 745f 6365           spot_ce
+000080a0: 6e74 726f 6964 732e 6170 7065 6e64 2873  ntroids.append(s
+000080b0: 706f 745f 6365 6e74 726f 6964 290d 0a20  pot_centroid).. 
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
+000080f0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+00008100: 2873 706f 745f 6365 6e74 726f 6964 7329  (spot_centroids)
+00008110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008140: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
+00008150: 645b 7374 7228 7429 5d20 3d20 7472 6565  d[str(t)] = tree
+00008160: 2c20 7370 6f74 5f63 656e 7472 6f69 6473  , spot_centroids
+00008170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008180: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00008190: 0d0a 2020 2020 6465 6620 5f6d 6173 7465  ..    def _maste
+000081a0: 725f 7472 6163 6b5f 636f 6d70 7574 6572  r_track_computer
+000081b0: 2873 656c 662c 2074 7261 636b 2c20 7472  (self, track, tr
+000081c0: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000081f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00008200: 7272 656e 745f 6365 6c6c 5f69 6473 203d  rrent_cell_ids =
-00008210: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008240: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008260: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00008270: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
-00008280: 7461 7267 6574 5f69 6473 203d 2020 7365  target_ids =  se
-00008290: 6c66 2e5f 6765 6e65 7261 7465 5f67 656e  lf._generate_gen
-000082a0: 6572 6174 696f 6e73 2874 7261 636b 290d  erations(track).
-000082b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000082c0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-000082d0: 745f 726f 6f74 2c20 726f 6f74 5f73 706c  t_root, root_spl
-000082e0: 6974 732c 2072 6f6f 745f 6c65 6166 203d  its, root_leaf =
-000082f0: 2073 656c 662e 5f63 7265 6174 655f 6765   self._create_ge
-00008300: 6e65 7261 7469 6f6e 7328 616c 6c5f 736f  nerations(all_so
-00008310: 7572 6365 5f69 6473 2920 0d0a 2020 2020  urce_ids) ..    
-00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-00008340: 6572 6174 655f 7370 6c69 745f 646f 776e  erate_split_down
-00008350: 2872 6f6f 745f 726f 6f74 2c20 726f 6f74  (root_root, root
-00008360: 5f6c 6561 662c 2072 6f6f 745f 7370 6c69  _leaf, root_spli
-00008370: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000083b0: 2044 6574 6572 6d69 6e65 2069 6620 6120   Determine if a 
-000083c0: 7472 6163 6b20 6861 7320 6469 7669 7369  track has divisi
-000083d0: 6f6e 7320 6f72 206e 6f6e 650d 0a20 2020  ons or none..   
-000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083f0: 2020 2020 2020 2020 206e 756d 6265 725f           number_
-00008400: 6469 7669 6469 6e67 203d 206c 656e 2872  dividing = len(r
-00008410: 6f6f 745f 7370 6c69 7473 290d 0a20 2020  oot_splits)..   
-00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00008440: 726f 6f74 5f73 706c 6974 7329 203e 2030  root_splits) > 0
-00008450: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00008480: 7261 636b 5f6d 6974 6f73 6973 5f6c 6162  rack_mitosis_lab
-00008490: 656c 5b74 7261 636b 5f69 645d 203d 205b  el[track_id] = [
-000084a0: 312c 206e 756d 6265 725f 6469 7669 6469  1, number_dividi
-000084b0: 6e67 5d0d 0a20 2020 2020 2020 2020 2020  ng]..           
-000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 2064 6976 6964 696e 675f 7472       dividing_tr
-000084e0: 616a 6563 746f 7279 203d 2054 7275 650d  ajectory = True.
-000084f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
-00008520: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
-00008530: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008560: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00008570: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
-00008580: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-000085b0: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-000085c0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-000085d0: 636b 4964 733a 2020 2020 200d 0a20 2020  ckIds:     ..   
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-00008610: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
-00008620: 7428 7472 6163 6b5f 6964 2929 0d0a 2020  t(track_id))..  
-00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000081e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008200: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
+00008230: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008290: 2061 6c6c 5f73 6f75 7263 655f 6964 732c   all_source_ids,
+000082a0: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
+000082b0: 3d20 2073 656c 662e 5f67 656e 6572 6174  =  self._generat
+000082c0: 655f 6765 6e65 7261 7469 6f6e 7328 7472  e_generations(tr
+000082d0: 6163 6b29 0d0a 2020 2020 2020 2020 2020  ack)..          
+000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082f0: 2020 726f 6f74 5f72 6f6f 742c 2072 6f6f    root_root, roo
+00008300: 745f 7370 6c69 7473 2c20 726f 6f74 5f6c  t_splits, root_l
+00008310: 6561 6620 3d20 7365 6c66 2e5f 6372 6561  eaf = self._crea
+00008320: 7465 5f67 656e 6572 6174 696f 6e73 2861  te_generations(a
+00008330: 6c6c 5f73 6f75 7263 655f 6964 7329 200d  ll_source_ids) .
+00008340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008350: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008360: 662e 5f69 7465 7261 7465 5f73 706c 6974  f._iterate_split
+00008370: 5f64 6f77 6e28 726f 6f74 5f72 6f6f 742c  _down(root_root,
+00008380: 2072 6f6f 745f 6c65 6166 2c20 726f 6f74   root_leaf, root
+00008390: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083d0: 2020 2020 2320 4465 7465 726d 696e 6520      # Determine 
+000083e0: 6966 2061 2074 7261 636b 2068 6173 2064  if a track has d
+000083f0: 6976 6973 696f 6e73 206f 7220 6e6f 6e65  ivisions or none
+00008400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008410: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00008420: 6d62 6572 5f64 6976 6964 696e 6720 3d20  mber_dividing = 
+00008430: 6c65 6e28 726f 6f74 5f73 706c 6974 7329  len(root_splits)
+00008440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008450: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00008460: 206c 656e 2872 6f6f 745f 7370 6c69 7473   len(root_splits
+00008470: 2920 3e20 303a 0d0a 2020 2020 2020 2020  ) > 0:..        
+00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008490: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000084a0: 7175 655f 7472 6163 6b5f 6d69 746f 7369  que_track_mitosi
+000084b0: 735f 6c61 6265 6c5b 7472 6163 6b5f 6964  s_label[track_id
+000084c0: 5d20 3d20 5b31 2c20 6e75 6d62 6572 5f64  ] = [1, number_d
+000084d0: 6976 6964 696e 675d 0d0a 2020 2020 2020  ividing]..      
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 2020 2020 6469 7669 6469            dividi
+00008500: 6e67 5f74 7261 6a65 6374 6f72 7920 3d20  ng_trajectory = 
+00008510: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
+00008540: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
+00008550: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
+00008560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+00008590: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+000085a0: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000085d0: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
+000085e0: 7420 696e 2073 656c 662e 4469 7669 6469  t in self.Dividi
+000085f0: 6e67 5472 6163 6b49 6473 3a20 2020 2020  ngTrackIds:     
+00008600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+00008630: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+00008640: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
+00008650: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008670: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00008670: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000086a0: 756e 6971 7565 5f74 7261 636b 5f6d 6974  unique_track_mit
-000086b0: 6f73 6973 5f6c 6162 656c 5b74 7261 636b  osis_label[track
-000086c0: 5f69 645d 203d 205b 302c 2030 5d0d 0a20  _id] = [0, 0].. 
-000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000086f0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
-00008700: 7279 203d 2046 616c 7365 0d0a 2020 2020  ry = False..    
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00008730: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
-00008740: 2069 6e20 7365 6c66 2e41 6c6c 5472 6163   in self.AllTrac
-00008750: 6b49 6473 3a0d 0a20 2020 2020 2020 2020  kIds:..         
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008780: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
-00008790: 6e64 2869 6e74 2874 7261 636b 5f69 6429  nd(int(track_id)
-000087a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2020 2069 6620 696e 7428 7472 6163 6b5f     if int(track_
-000087d0: 6964 2920 6e6f 7420 696e 2073 656c 662e  id) not in self.
-000087e0: 4e6f 726d 616c 5472 6163 6b49 6473 3a20  NormalTrackIds: 
-000087f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
-00008820: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
-00008830: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00008840: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008860: 2020 666f 7220 6c65 6166 2069 6e20 726f    for leaf in ro
-00008870: 6f74 5f6c 6561 663a 0d0a 2020 2020 2020  ot_leaf:..      
-00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000088a0: 662e 5f73 6563 6f6e 645f 6368 616e 6e65  f._second_channe
-000088b0: 6c5f 7570 6461 7465 286c 6561 662c 2074  l_update(leaf, t
-000088c0: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000088f0: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
-00008900: 7065 6e64 286c 6561 6629 200d 0a20 2020  pend(leaf) ..   
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008940: 5f70 726f 7065 7274 6965 735b 6c65 6166  _properties[leaf
-00008950: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
-00008960: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
-00008970: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
-00008980: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000089b0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000089c0: 6965 735b 6c65 6166 5d2e 7570 6461 7465  ies[leaf].update
-000089d0: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
-000089e0: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
-000089f0: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008a20: 736f 7572 6365 5f69 6420 696e 2061 6c6c  source_id in all
-00008a30: 5f73 6f75 7263 655f 6964 733a 0d0a 2020  _source_ids:..  
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a60: 2073 656c 662e 5f73 6563 6f6e 645f 6368   self._second_ch
-00008a70: 616e 6e65 6c5f 7570 6461 7465 2873 6f75  annel_update(sou
-00008a80: 7263 655f 6964 2c20 7472 6163 6b5f 6964  rce_id, track_id
-00008a90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00008ac0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00008ad0: 735b 736f 7572 6365 5f69 645d 2e75 7064  s[source_id].upd
-00008ae0: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00008af0: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00008b00: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
-00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00008b40: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
-00008b50: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
-00008b60: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
-00008b70: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
-00008b80: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bb0: 2020 2063 7572 7265 6e74 5f63 656c 6c5f     current_cell_
-00008bc0: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
-00008bd0: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
-00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00008690: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
+000086d0: 6b5f 6d69 746f 7369 735f 6c61 6265 6c5b  k_mitosis_label[
+000086e0: 7472 6163 6b5f 6964 5d20 3d20 5b30 2c20  track_id] = [0, 
+000086f0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2020 6469 7669 6469 6e67 5f74 7261      dividing_tra
+00008720: 6a65 6374 6f72 7920 3d20 4661 6c73 650d  jectory = False.
+00008730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
+00008760: 2920 6e6f 7420 696e 2073 656c 662e 416c  ) not in self.Al
+00008770: 6c54 7261 636b 4964 733a 0d0a 2020 2020  lTrackIds:..    
+00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087a0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
+000087b0: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+000087c0: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087e0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
+000087f0: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
+00008800: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+00008810: 4964 733a 2020 2020 0d0a 2020 2020 2020  Ids:    ..      
+00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008830: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008840: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+00008850: 732e 6170 7065 6e64 2869 6e74 2874 7261  s.append(int(tra
+00008860: 636b 5f69 6429 290d 0a0d 0a20 2020 2020  ck_id))....     
+00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008880: 2020 2020 2020 2066 6f72 206c 6561 6620         for leaf 
+00008890: 696e 2072 6f6f 745f 6c65 6166 3a0d 0a20  in root_leaf:.. 
+000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088c0: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
+000088d0: 6861 6e6e 656c 5f75 7064 6174 6528 6c65  hannel_update(le
+000088e0: 6166 2c20 7472 6163 6b5f 6964 290d 0a20  af, track_id).. 
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+00008920: 6473 2e61 7070 656e 6428 6c65 6166 2920  ds.append(leaf) 
+00008930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008950: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00008960: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00008970: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
+00008980: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+00008990: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
+000089a0: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000089d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000089e0: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
+000089f0: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+00008a00: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+00008a10: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00008a20: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2066 6f72 2073 6f75 7263 655f 6964 2069   for source_id i
+00008a50: 6e20 616c 6c5f 736f 7572 6365 5f69 6473  n all_source_ids
+00008a60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a80: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
+00008a90: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
+00008aa0: 6528 736f 7572 6365 5f69 642c 2074 7261  e(source_id, tra
+00008ab0: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008ae0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00008af0: 6572 7469 6573 5b73 6f75 7263 655f 6964  erties[source_id
+00008b00: 5d2e 7570 6461 7465 287b 7365 6c66 2e64  ].update({self.d
+00008b10: 6976 6964 696e 675f 6b65 7920 3a20 6469  ividing_key : di
+00008b20: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00008b30: 797d 290d 0a20 2020 2020 2020 2020 2020  y})..           
+00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00008b60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00008b70: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
+00008b80: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
+00008b90: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
+00008ba0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
+00008bb0: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
+00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00008be0: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
+00008bf0: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
+00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c20: 2020 2020 2020 2066 6f72 2063 7572 7265         for curre
-00008c30: 6e74 5f72 6f6f 7420 696e 2072 6f6f 745f  nt_root in root_
-00008c40: 726f 6f74 3a0d 0a20 2020 2020 2020 2020  root:..         
-00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c60: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008c70: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
-00008c80: 7064 6174 6528 6375 7272 656e 745f 726f  pdate(current_ro
-00008c90: 6f74 2c20 7472 6163 6b5f 6964 290d 0a20  ot, track_id).. 
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cc0: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
-00008cd0: 735b 696e 7428 6375 7272 656e 745f 726f  s[int(current_ro
-00008ce0: 6f74 295d 203d 2073 656c 662e 756e 6971  ot)] = self.uniq
-00008cf0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00008d00: 6573 5b69 6e74 2863 7572 7265 6e74 5f72  es[int(current_r
-00008d10: 6f6f 7429 5d0d 0a20 2020 2020 2020 2020  oot)]..         
-00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d30: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00008d40: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00008d50: 7274 6965 735b 736f 7572 6365 5f69 645d  rties[source_id]
-00008d60: 2e75 7064 6174 6528 7b73 656c 662e 6469  .update({self.di
-00008d70: 7669 6469 6e67 5f6b 6579 203a 2064 6976  viding_key : div
-00008d80: 6964 696e 675f 7472 616a 6563 746f 7279  iding_trajectory
-00008d90: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008db0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00008dc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00008dd0: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
-00008de0: 6461 7465 287b 7365 6c66 2e6e 756d 6265  date({self.numbe
-00008df0: 725f 6469 7669 6469 6e67 5f6b 6579 203a  r_dividing_key :
-00008e00: 206e 756d 6265 725f 6469 7669 6469 6e67   number_dividing
-00008e10: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008e40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008e50: 6c66 2e61 6c6c 5f63 7572 7265 6e74 5f63  lf.all_current_c
-00008e60: 656c 6c5f 6964 735b 696e 7428 7472 6163  ell_ids[int(trac
-00008e70: 6b5f 6964 295d 203d 2063 7572 7265 6e74  k_id)] = current
-00008e80: 5f63 656c 6c5f 6964 730d 0a20 2020 2020  _cell_ids..     
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ea0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008c20: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008c50: 6375 7272 656e 745f 726f 6f74 2069 6e20  current_root in 
+00008c60: 726f 6f74 5f72 6f6f 743a 0d0a 2020 2020  root_root:..    
+00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008c90: 656c 662e 5f73 6563 6f6e 645f 6368 616e  elf._second_chan
+00008ca0: 6e65 6c5f 7570 6461 7465 2863 7572 7265  nel_update(curre
+00008cb0: 6e74 5f72 6f6f 742c 2074 7261 636b 5f69  nt_root, track_i
+00008cc0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ce0: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
+00008cf0: 5f73 706f 7473 5b69 6e74 2863 7572 7265  _spots[int(curre
+00008d00: 6e74 5f72 6f6f 7429 5d20 3d20 7365 6c66  nt_root)] = self
+00008d10: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008d20: 7065 7274 6965 735b 696e 7428 6375 7272  perties[int(curr
+00008d30: 656e 745f 726f 6f74 295d 0d0a 2020 2020  ent_root)]..    
+00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008d60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00008d70: 7072 6f70 6572 7469 6573 5b73 6f75 7263  properties[sourc
+00008d80: 655f 6964 5d2e 7570 6461 7465 287b 7365  e_id].update({se
+00008d90: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+00008da0: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00008db0: 6374 6f72 797d 290d 0a20 2020 2020 2020  ctory})..       
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008de0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008df0: 7065 7274 6965 735b 736f 7572 6365 5f69  perties[source_i
+00008e00: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
+00008e10: 6e75 6d62 6572 5f64 6976 6964 696e 675f  number_dividing_
+00008e20: 6b65 7920 3a20 6e75 6d62 6572 5f64 6976  key : number_div
+00008e30: 6964 696e 677d 290d 0a20 2020 2020 2020  iding})..       
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e70: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
+00008e80: 656e 745f 6365 6c6c 5f69 6473 5b69 6e74  ent_cell_ids[int
+00008e90: 2874 7261 636b 5f69 6429 5d20 3d20 6375  (track_id)] = cu
+00008ea0: 7272 656e 745f 6365 6c6c 5f69 6473 0d0a  rrent_cell_ids..
 00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ec0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00008ed0: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
-00008ee0: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008ec0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00008ef0: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
+00008f00: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
+00008f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f30: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-00008f40: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
-00008f50: 6473 5b69 5d29 2020 200d 0a20 2020 2020  ds[i])   ..     
-00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00008f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008f30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f50: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00008f60: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
+00008f70: 656c 6c5f 6964 735b 695d 2920 2020 0d0a  ell_ids[i])   ..
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fa0: 2020 2020 2061 6c6c 5f64 6963 745f 7661       all_dict_va
-00008fb0: 6c75 6573 203d 2073 656c 662e 756e 6971  lues = self.uniq
-00008fc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00008fd0: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ff0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008fa0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fc0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00008fd0: 6374 5f76 616c 7565 7320 3d20 7365 6c66  ct_values = self
+00008fe0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00008ff0: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
 00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2020 2020 2074 203d 2069 6e74 2866 6c6f       t = int(flo
-00009050: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009060: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
-00009070: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2020 2020 2020 2020 2020 7a20 3d20              z = 
-000090a0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-000090b0: 616c 7565 735b 7365 6c66 2e7a 706f 7369  alues[self.zposi
-000090c0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090e0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
-000090f0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00009100: 7661 6c75 6573 5b73 656c 662e 7970 6f73  values[self.ypos
-00009110: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009130: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-00009140: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00009150: 5f76 616c 7565 735b 7365 6c66 2e78 706f  _values[self.xpo
-00009160: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009190: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00009040: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2020 2020 2020 2020 2020 7420 3d20 696e            t = in
+00009070: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
+00009080: 5f76 616c 7565 735b 7365 6c66 2e66 7261  _values[self.fra
+00009090: 6d65 6964 5f6b 6579 5d29 290d 0a20 2020  meid_key]))..   
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 207a 203d 2066 6c6f 6174 2861 6c6c 5f64   z = float(all_d
+000090d0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+000090e0: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
+000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009110: 2020 7920 3d20 666c 6f61 7428 616c 6c5f    y = float(all_
+00009120: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00009130: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 2020 2078 203d 2066 6c6f 6174 2861 6c6c     x = float(all
+00009170: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009180: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091b0: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
-000091c0: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
-000091d0: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
-000091e0: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
-000091f0: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
-00009200: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
-00009210: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
-00009220: 6f6e 2920 0d0a 0d0a 2020 2020 2020 2020  on) ....        
-00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009250: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-00009260: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-00009270: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
-00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000092b0: 7472 6163 6b5f 6365 6e74 726f 6964 5b66  track_centroid[f
-000092c0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
-000092d0: 6964 5d20 3d20 7472 6163 6b5f 6964 0d0a  id] = track_id..
-000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009300: 2020 200d 0a20 2020 2064 6566 205f 7365     ..    def _se
-00009310: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
-00009320: 6174 6528 7365 6c66 2c20 6365 6c6c 5f69  ate(self, cell_i
-00009330: 642c 2074 7261 636b 5f69 6429 3a0d 0a20  d, track_id):.. 
-00009340: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00009350: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00009360: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-00009370: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00009380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009390: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000093a0: 2020 2066 7261 6d65 203d 2073 656c 662e     frame = self.
-000093b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000093c0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000093d0: 6964 295d 5b73 656c 662e 6672 616d 6569  id)][self.framei
-000093e0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-000093f0: 2020 2020 2020 2020 7a20 3d20 7365 6c66          z = self
-00009400: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00009410: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00009420: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
-00009430: 645f 6b65 795d 2f73 656c 662e 7a63 616c  d_key]/self.zcal
-00009440: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00009450: 2020 2020 2020 2020 2020 7920 3d20 7365            y = se
-00009460: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00009470: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00009480: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00009490: 7369 645f 6b65 795d 2f73 656c 662e 7963  sid_key]/self.yc
-000094a0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-000094b0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-000094c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000094d0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000094e0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-000094f0: 706f 7369 645f 6b65 795d 2f73 656c 662e  posid_key]/self.
-00009500: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
-00009510: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009520: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
-00009530: 656c 5f73 706f 7473 2866 7261 6d65 2c20  el_spots(frame, 
-00009540: 7a2c 2079 2c20 782c 2063 656c 6c5f 6964  z, y, x, cell_id
-00009550: 2c20 7472 6163 6b5f 6964 290d 0a20 2020  , track_id)..   
-00009560: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00009570: 6669 6e61 6c5f 7472 6163 6b73 2873 656c  final_tracks(sel
-00009580: 662c 2074 7261 636b 5f69 6429 3a0d 0a0d  f, track_id):...
-00009590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000095a0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000095b0: 7265 6e74 5f63 656c 6c5f 6964 7320 3d20  rent_cell_ids = 
-000095c0: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
-000095d0: 5f63 656c 6c5f 6964 735b 696e 7428 7472  _cell_ids[int(tr
-000095e0: 6163 6b5f 6964 295d 0d0a 2020 2020 2020  ack_id)]..      
-000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
-00009610: 6163 6b6c 6574 7320 3d20 7b7d 0d0a 2020  acklets = {}..  
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00009640: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-00009650: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
-00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009670: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009690: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000096a0: 7261 6e67 6528 6c65 6e28 6375 7272 656e  range(len(curren
-000096b0: 745f 6365 6c6c 5f69 6473 2929 3a0d 0a20  t_cell_ids)):.. 
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000091b0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091d0: 2020 2020 2020 2020 2020 2020 6672 616d              fram
+000091e0: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
+000091f0: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
+00009200: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00009210: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
+00009220: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
+00009230: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
+00009240: 6272 6174 696f 6e29 200d 0a0d 0a20 2020  bration) ....   
+00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009270: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00009280: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
+00009290: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
+000092a0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
+000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092c0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+000092d0: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
+000092e0: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
+000092f0: 656e 7472 6f69 645d 203d 2074 7261 636b  entroid] = track
+00009300: 5f69 640d 0a20 2020 2020 2020 2020 2020  _id..           
+00009310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009320: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+00009330: 6620 5f73 6563 6f6e 645f 6368 616e 6e65  f _second_channe
+00009340: 6c5f 7570 6461 7465 2873 656c 662c 2063  l_update(self, c
+00009350: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
+00009360: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00009370: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009380: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+00009390: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+000093a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000093b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000093c0: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
+000093d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000093e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000093f0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e66  cell_id)][self.f
+00009400: 7261 6d65 6964 5f6b 6579 5d0d 0a20 2020  rameid_key]..   
+00009410: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+00009420: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00009430: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00009440: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00009450: 7a70 6f73 6964 5f6b 6579 5d2f 7365 6c66  zposid_key]/self
+00009460: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
+00009470: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00009480: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+00009490: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000094a0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+000094b0: 662e 7970 6f73 6964 5f6b 6579 5d2f 7365  f.yposid_key]/se
+000094c0: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
+000094d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094e0: 2078 203d 2073 656c 662e 756e 6971 7565   x = self.unique
+000094f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00009500: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00009510: 656c 662e 7870 6f73 6964 5f6b 6579 5d2f  elf.xposid_key]/
+00009520: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+00009530: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00009540: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+00009550: 6368 616e 6e65 6c5f 7370 6f74 7328 6672  channel_spots(fr
+00009560: 616d 652c 207a 2c20 792c 2078 2c20 6365  ame, z, y, x, ce
+00009570: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
+00009580: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00009590: 6465 6620 5f66 696e 616c 5f74 7261 636b  def _final_track
+000095a0: 7328 7365 6c66 2c20 7472 6163 6b5f 6964  s(self, track_id
+000095b0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095d0: 2020 6375 7272 656e 745f 6365 6c6c 5f69    current_cell_i
+000095e0: 6473 203d 2073 656c 662e 616c 6c5f 6375  ds = self.all_cu
+000095f0: 7272 656e 745f 6365 6c6c 5f69 6473 5b69  rrent_cell_ids[i
+00009600: 6e74 2874 7261 636b 5f69 6429 5d0d 0a20  nt(track_id)].. 
+00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009620: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00009630: 6e74 5f74 7261 636b 6c65 7473 203d 207b  nt_tracklets = {
+00009640: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00009650: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009660: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009670: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
+00009680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009690: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000096c0: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
+000096d0: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
+000096e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
 000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009700: 2020 2020 2020 2020 2020 2020 206b 203d               k =
-00009710: 2069 6e74 2863 7572 7265 6e74 5f63 656c   int(current_cel
-00009720: 6c5f 6964 735b 695d 2920 2020 200d 0a20  l_ids[i])    .. 
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2061 6c6c 5f64 6963 745f 7661 6c75     all_dict_valu
-00009760: 6573 203d 2073 656c 662e 756e 6971 7565  es = self.unique
-00009770: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00009780: 5b6b 5d0d 0a20 2020 2020 2020 2020 2020  [k]..           
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097a0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-000097b0: 6964 203d 2073 7472 2861 6c6c 5f64 6963  id = str(all_dic
-000097c0: 745f 7661 6c75 6573 5b73 656c 662e 756e  t_values[self.un
-000097d0: 6971 7565 6964 5f6b 6579 5d29 0d0a 2020  iqueid_key])..  
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
-00009810: 6964 203d 2073 7472 2861 6c6c 5f64 6963  id = str(all_dic
-00009820: 745f 7661 6c75 6573 5b73 656c 662e 7472  t_values[self.tr
-00009830: 6163 6b69 645f 6b65 795d 290d 0a20 2020  ackid_key])..   
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2074 203d 2069 6e74 2866 6c6f 6174 2861   t = int(float(a
-00009870: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009880: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
-00009890: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098b0: 2020 2020 2020 2020 7a20 3d20 666c 6f61          z = floa
-000098c0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-000098d0: 735b 7365 6c66 2e7a 706f 7369 645f 6b65  s[self.zposid_ke
-000098e0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2020 2020 2079 203d 2066 6c6f           y = flo
-00009910: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009920: 6573 5b73 656c 662e 7970 6f73 6964 5f6b  es[self.yposid_k
-00009930: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 2020 2020 2020 7820 3d20 666c            x = fl
-00009960: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00009970: 7565 735b 7365 6c66 2e78 706f 7369 645f  ues[self.xposid_
-00009980: 6b65 795d 290d 0a0d 0a20 2020 2020 2020  key])....       
-00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000099b0: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
-000099c0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-000099d0: 735f 7072 6f70 6572 7469 6573 203d 2073  s_properties = s
-000099e0: 656c 662e 5f74 7261 636b 6c65 745f 616e  elf._tracklet_an
-000099f0: 645f 7072 6f70 6572 7469 6573 2869 6e74  d_properties(int
-00009a00: 2874 7261 636b 5f69 6429 2c20 616c 6c5f  (track_id), all_
-00009a10: 6469 6374 5f76 616c 7565 732c 2074 2c20  dict_values, t, 
-00009a20: 7a2c 2079 2c20 782c 206b 2c20 6375 7272  z, y, x, k, curr
-00009a30: 656e 745f 7472 6163 6b5f 6964 2c20 756e  ent_track_id, un
-00009a40: 6971 7565 5f69 642c 2063 7572 7265 6e74  ique_id, current
-00009a50: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
-00009a60: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-00009a70: 6f70 6572 7469 6573 290d 0a20 2020 2020  operties)..     
-00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00009aa0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00009ab0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009ac0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009ad0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00009ae0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
-00009af0: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
-00009b00: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00009b10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00009b30: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009b40: 5f70 726f 7065 7274 6965 7320 3d20 6e70  _properties = np
-00009b50: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00009b60: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-00009b70: 7274 6965 735b 7374 7228 7472 6163 6b5f  rties[str(track_
-00009b80: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
-00009b90: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009700: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009730: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
+00009740: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
+00009750: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009770: 2020 2020 2020 2020 616c 6c5f 6469 6374          all_dict
+00009780: 5f76 616c 7565 7320 3d20 7365 6c66 2e75  _values = self.u
+00009790: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000097a0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
+000097b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097c0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000097d0: 6971 7565 5f69 6420 3d20 7374 7228 616c  ique_id = str(al
+000097e0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+000097f0: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
+00009800: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00009830: 7261 636b 5f69 6420 3d20 7374 7228 616c  rack_id = str(al
+00009840: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009850: 6c66 2e74 7261 636b 6964 5f6b 6579 5d29  lf.trackid_key])
+00009860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 2020 2020 2020 7420 3d20 696e 7428 666c        t = int(fl
+00009890: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+000098a0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
+000098b0: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098d0: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+000098e0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+000098f0: 7661 6c75 6573 5b73 656c 662e 7a70 6f73  values[self.zpos
+00009900: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00009910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009920: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+00009930: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00009940: 5f76 616c 7565 735b 7365 6c66 2e79 706f  _values[self.ypo
+00009950: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+00009980: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00009990: 745f 7661 6c75 6573 5b73 656c 662e 7870  t_values[self.xp
+000099a0: 6f73 6964 5f6b 6579 5d29 0d0a 0d0a 2020  osid_key])....  
+000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+000099e0: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
+000099f0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+00009a00: 7320 3d20 7365 6c66 2e5f 7472 6163 6b6c  s = self._trackl
+00009a10: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
+00009a20: 7328 696e 7428 7472 6163 6b5f 6964 292c  s(int(track_id),
+00009a30: 2061 6c6c 5f64 6963 745f 7661 6c75 6573   all_dict_values
+00009a40: 2c20 742c 207a 2c20 792c 2078 2c20 6b2c  , t, z, y, x, k,
+00009a50: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
+00009a60: 642c 2075 6e69 7175 655f 6964 2c20 6375  d, unique_id, cu
+00009a70: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
+00009a80: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+00009a90: 7473 5f70 726f 7065 7274 6965 7329 0d0a  ts_properties)..
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ac0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009af0: 6b6c 6574 7320 3d20 6e70 2e61 7361 7272  klets = np.asarr
+00009b00: 6179 2863 7572 7265 6e74 5f74 7261 636b  ay(current_track
+00009b10: 6c65 7473 5b73 7472 2874 7261 636b 5f69  lets[str(track_i
+00009b20: 6429 5d2c 2064 7479 7065 3d6e 702e 666c  d)], dtype=np.fl
+00009b30: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009b60: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009b70: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00009b80: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
+00009b90: 7072 6f70 6572 7469 6573 5b73 7472 2874  properties[str(t
+00009ba0: 7261 636b 5f69 6429 5d2c 2064 7479 7065  rack_id)], dtype
+00009bb0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
 00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
-00009be0: 7261 636b 735b 7472 6163 6b5f 6964 5d20  racks[track_id] 
-00009bf0: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
-00009c00: 6574 7320 2020 2020 0d0a 2020 2020 2020  ets     ..      
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00009c30: 655f 7472 6163 6b5f 7072 6f70 6572 7469  e_track_properti
-00009c40: 6573 5b74 7261 636b 5f69 645d 203d 2063  es[track_id] = c
-00009c50: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009c60: 5f70 726f 7065 7274 6965 7320 2020 200d  _properties    .
-00009c70: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
-00009c80: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
-00009c90: 6965 7328 7365 6c66 2c20 7472 6163 6b5f  ies(self, track_
-00009ca0: 6964 2c20 616c 6c5f 6469 6374 5f76 616c  id, all_dict_val
-00009cb0: 7565 732c 2074 2c20 7a2c 2079 2c20 782c  ues, t, z, y, x,
-00009cc0: 206b 2c20 6375 7272 656e 745f 7472 6163   k, current_trac
-00009cd0: 6b5f 6964 2c20 756e 6971 7565 5f69 642c  k_id, unique_id,
-00009ce0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-00009cf0: 7473 2c20 6375 7272 656e 745f 7472 6163  ts, current_trac
-00009d00: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-00009d10: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
-00009d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d40: 2020 2020 2067 656e 5f69 6420 3d20 696e       gen_id = in
-00009d50: 7428 666c 6f61 7428 616c 6c5f 6469 6374  t(float(all_dict
-00009d60: 5f76 616c 7565 735b 7365 6c66 2e67 656e  _values[self.gen
-00009d70: 6572 6174 696f 6e69 645f 6b65 795d 2929  erationid_key]))
-00009d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 2020 7370 6565 6420 3d20 666c        speed = fl
-00009db0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00009dc0: 7565 735b 7365 6c66 2e73 7065 6564 5f6b  ues[self.speed_k
-00009dd0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2020 2020 2020 2020 2020 6163 6365 6c65            accele
-00009e00: 7261 7469 6f6e 203d 2066 6c6f 6174 2861  ration = float(a
-00009e10: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009e20: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00009e30: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
-00009e60: 6f6e 5f61 6e67 6c65 203d 2066 6c6f 6174  on_angle = float
-00009e70: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00009e80: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-00009e90: 6c65 5f6b 6579 5d29 0d0a 2020 2020 2020  le_key])..      
-00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009eb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00009ec0: 6469 616c 5f61 6e67 6c65 203d 2066 6c6f  dial_angle = flo
-00009ed0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009ee0: 6573 5b73 656c 662e 7261 6469 616c 5f61  es[self.radial_a
-00009ef0: 6e67 6c65 5f6b 6579 5d29 0d0a 2020 2020  ngle_key])..    
-00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 7261 6469 7573 203d 2066 6c6f 6174 2861  radius = float(a
-00009f30: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009f40: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00009f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 2020 2020 766f 6c75 6d65 5f70 6978        volume_pix
-00009f80: 656c 7320 3d20 696e 7428 666c 6f61 7428  els = int(float(
-00009f90: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009fa0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-00009fb0: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fd0: 2020 2020 2020 2020 2074 6f74 616c 5f69           total_i
-00009fe0: 6e74 656e 7369 7479 203d 2020 666c 6f61  ntensity =  floa
-00009ff0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-0000a000: 735b 7365 6c66 2e74 6f74 616c 5f69 6e74  s[self.total_int
-0000a010: 656e 7369 7479 5f6b 6579 5d29 0d0a 2020  ensity_key])..  
-0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00009bd0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bf0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00009c00: 7175 655f 7472 6163 6b73 5b74 7261 636b  que_tracks[track
+00009c10: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+00009c20: 7261 636b 6c65 7473 2020 2020 200d 0a20  racklets     .. 
+00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009c50: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
+00009c60: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00009c70: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
+00009c80: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009c90: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+00009ca0: 5f74 7261 636b 6c65 745f 616e 645f 7072  _tracklet_and_pr
+00009cb0: 6f70 6572 7469 6573 2873 656c 662c 2074  operties(self, t
+00009cc0: 7261 636b 5f69 642c 2061 6c6c 5f64 6963  rack_id, all_dic
+00009cd0: 745f 7661 6c75 6573 2c20 742c 207a 2c20  t_values, t, z, 
+00009ce0: 792c 2078 2c20 6b2c 2063 7572 7265 6e74  y, x, k, current
+00009cf0: 5f74 7261 636b 5f69 642c 2075 6e69 7175  _track_id, uniqu
+00009d00: 655f 6964 2c20 6375 7272 656e 745f 7472  e_id, current_tr
+00009d10: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
+00009d20: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+00009d30: 7274 6965 7329 3a0d 0a20 2020 2020 2020  rties):..       
+00009d40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d60: 2020 2020 2020 2020 2020 6765 6e5f 6964            gen_id
+00009d70: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
+00009d80: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009d90: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
+00009da0: 6579 5d29 290d 0a20 2020 2020 2020 2020  ey]))..         
+00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009dc0: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+00009dd0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+00009de0: 745f 7661 6c75 6573 5b73 656c 662e 7370  t_values[self.sp
+00009df0: 6565 645f 6b65 795d 290d 0a20 2020 2020  eed_key])..     
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e10: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00009e20: 6363 656c 6572 6174 696f 6e20 3d20 666c  cceleration = fl
+00009e30: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00009e40: 7565 735b 7365 6c66 2e61 6363 656c 6572  ues[self.acceler
+00009e50: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e80: 206d 6f74 696f 6e5f 616e 676c 6520 3d20   motion_angle = 
+00009e90: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+00009ea0: 616c 7565 735b 7365 6c66 2e6d 6f74 696f  alues[self.motio
+00009eb0: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ee0: 2020 2072 6164 6961 6c5f 616e 676c 6520     radial_angle 
+00009ef0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
+00009f00: 5f76 616c 7565 735b 7365 6c66 2e72 6164  _values[self.rad
+00009f10: 6961 6c5f 616e 676c 655f 6b65 795d 290d  ial_angle_key]).
+00009f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f40: 2020 2020 2072 6164 6975 7320 3d20 666c       radius = fl
+00009f50: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00009f60: 7565 735b 7365 6c66 2e72 6164 6975 735f  ues[self.radius_
+00009f70: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
+00009fa0: 655f 7069 7865 6c73 203d 2069 6e74 2866  e_pixels = int(f
+00009fb0: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00009fc0: 6c75 6573 5b73 656c 662e 7175 616c 6974  lues[self.qualit
+00009fd0: 795f 6b65 795d 2929 0d0a 2020 2020 2020  y_key]))..      
+00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000a000: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
+0000a010: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+0000a020: 7661 6c75 6573 5b73 656c 662e 746f 7461  values[self.tota
+0000a030: 6c5f 696e 7465 6e73 6974 795f 6b65 795d  l_intensity_key]
+0000a040: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-0000a070: 6365 6c6c 5f6d 6173 6b20 3d20 666c 6f61  cell_mask = floa
-0000a080: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-0000a090: 735b 7365 6c66 2e64 6973 7461 6e63 655f  s[self.distance_
-0000a0a0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 290d  cell_mask_key]).
-0000a0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000a060: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+0000a090: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+0000a0a0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+0000a0b0: 7661 6c75 6573 5b73 656c 662e 6469 7374  values[self.dist
+0000a0c0: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+0000a0d0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-0000a100: 5f64 6973 706c 6163 656d 656e 7420 3d20  _displacement = 
-0000a110: 666c 6f61 7428 7365 6c66 2e41 6c6c 5472  float(self.AllTr
-0000a120: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
-0000a130: 6964 5d5b 7365 6c66 2e64 6973 706c 6163  id][self.displac
-0000a140: 656d 656e 745f 6b65 795d 290d 0a20 2020  ement_key])..   
-0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a170: 2074 6f74 616c 5f74 7261 636b 5f64 6973   total_track_dis
-0000a180: 7461 6e63 6520 3d20 666c 6f61 7428 7365  tance = float(se
-0000a190: 6c66 2e41 6c6c 5472 6163 6b56 616c 7565  lf.AllTrackValue
-0000a1a0: 735b 7472 6163 6b5f 6964 5d5b 7365 6c66  s[track_id][self
-0000a1b0: 2e74 6f74 616c 5f74 7261 636b 5f64 6973  .total_track_dis
-0000a1c0: 7461 6e63 655f 6b65 795d 290d 0a20 2020  tance_key])..   
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
-0000a200: 6e63 6520 3d20 666c 6f61 7428 7365 6c66  nce = float(self
-0000a210: 2e41 6c6c 5472 6163 6b56 616c 7565 735b  .AllTrackValues[
-0000a220: 7472 6163 6b5f 6964 5d5b 7365 6c66 2e6d  track_id][self.m
-0000a230: 6178 5f64 6973 7461 6e63 655f 7472 6176  ax_distance_trav
-0000a240: 656c 6564 5f6b 6579 5d29 0d0a 2020 2020  eled_key])..    
-0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a270: 7472 6163 6b5f 6475 7261 7469 6f6e 203d  track_duration =
-0000a280: 2066 6c6f 6174 2873 656c 662e 416c 6c54   float(self.AllT
-0000a290: 7261 636b 5661 6c75 6573 5b74 7261 636b  rackValues[track
-0000a2a0: 5f69 645d 5b73 656c 662e 7472 6163 6b5f  _id][self.track_
-0000a2b0: 6475 7261 7469 6f6e 5f6b 6579 5d29 0d0a  duration_key])..
-0000a2c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000a0f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a120: 7472 6163 6b5f 6469 7370 6c61 6365 6d65  track_displaceme
+0000a130: 6e74 203d 2066 6c6f 6174 2873 656c 662e  nt = float(self.
+0000a140: 416c 6c54 7261 636b 5661 6c75 6573 5b74  AllTrackValues[t
+0000a150: 7261 636b 5f69 645d 5b73 656c 662e 6469  rack_id][self.di
+0000a160: 7370 6c61 6365 6d65 6e74 5f6b 6579 5d29  splacement_key])
+0000a170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a190: 2020 2020 2020 746f 7461 6c5f 7472 6163        total_trac
+0000a1a0: 6b5f 6469 7374 616e 6365 203d 2066 6c6f  k_distance = flo
+0000a1b0: 6174 2873 656c 662e 416c 6c54 7261 636b  at(self.AllTrack
+0000a1c0: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
+0000a1d0: 5b73 656c 662e 746f 7461 6c5f 7472 6163  [self.total_trac
+0000a1e0: 6b5f 6469 7374 616e 6365 5f6b 6579 5d29  k_distance_key])
+0000a1f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2020 2020 6d61 785f 7472 6163 6b5f        max_track_
+0000a220: 6469 7374 616e 6365 203d 2066 6c6f 6174  distance = float
+0000a230: 2873 656c 662e 416c 6c54 7261 636b 5661  (self.AllTrackVa
+0000a240: 6c75 6573 5b74 7261 636b 5f69 645d 5b73  lues[track_id][s
+0000a250: 656c 662e 6d61 785f 6469 7374 616e 6365  elf.max_distance
+0000a260: 5f74 7261 7665 6c65 645f 6b65 795d 290d  _traveled_key]).
+0000a270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 2020 2020 2074 7261 636b 5f64 7572 6174       track_durat
+0000a2a0: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
+0000a2b0: 2e41 6c6c 5472 6163 6b56 616c 7565 735b  .AllTrackValues[
+0000a2c0: 7472 6163 6b5f 6964 5d5b 7365 6c66 2e74  track_id][self.t
+0000a2d0: 7261 636b 5f64 7572 6174 696f 6e5f 6b65  rack_duration_ke
+0000a2e0: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
 0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a310: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
-0000a320: 6561 5f6b 6579 2069 6e20 616c 6c5f 6469  ea_key in all_di
-0000a330: 6374 5f76 616c 7565 732e 6b65 7973 2829  ct_values.keys()
-0000a340: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000a300: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a330: 2020 2069 6620 7365 6c66 2e73 7572 6661     if self.surfa
+0000a340: 6365 5f61 7265 615f 6b65 7920 696e 2061  ce_area_key in a
+0000a350: 6c6c 5f64 6963 745f 7661 6c75 6573 2e6b  ll_dict_values.k
+0000a360: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
 0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a390: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
-0000a3a0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-0000a3b0: 7374 203d 2066 6c6f 6174 2861 6c6c 5f64  st = float(all_d
-0000a3c0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-0000a3d0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000a3e0: 705f 6669 7273 746b 6579 5d29 0d0a 2020  p_firstkey])..  
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a410: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-0000a420: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000a430: 6420 3d20 666c 6f61 7428 616c 6c5f 6469  d = float(all_di
-0000a440: 6374 5f76 616c 7565 735b 7365 6c66 2e65  ct_values[self.e
-0000a450: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000a460: 5f73 6563 6f6e 646b 6579 5d29 0d0a 2020  _secondkey])..  
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a490: 2020 2020 2020 2020 2073 7572 6661 6365           surface
-0000a4a0: 5f61 7265 6120 3d20 666c 6f61 7428 616c  _area = float(al
-0000a4b0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-0000a4c0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000a4d0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-0000a510: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-0000a520: 745f 7661 6c75 6573 5b73 656c 662e 6365  t_values[self.ce
-0000a530: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 795d  llaxis_mask_key]
-0000a540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000a390: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000a3d0: 705f 6669 7273 7420 3d20 666c 6f61 7428  p_first = float(
+0000a3e0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+0000a3f0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+0000a400: 795f 636f 6d70 5f66 6972 7374 6b65 795d  y_comp_firstkey]
+0000a410: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a430: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+0000a440: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000a450: 7365 636f 6e64 203d 2066 6c6f 6174 2861  second = float(a
+0000a460: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000a470: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+0000a480: 5f63 6f6d 705f 7365 636f 6e64 6b65 795d  _comp_secondkey]
+0000a490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+0000a4c0: 7266 6163 655f 6172 6561 203d 2066 6c6f  rface_area = flo
+0000a4d0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000a4e0: 6573 5b73 656c 662e 7375 7266 6163 655f  es[self.surface_
+0000a4f0: 6172 6561 5f6b 6579 5d29 0d0a 2020 2020  area_key])..    
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+0000a530: 5f6d 6173 6b20 3d20 666c 6f61 7428 616c  _mask = float(al
+0000a540: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000a550: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+0000a560: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000a5a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a590: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000a5c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-0000a600: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-0000a610: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
-0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-0000a650: 6f6d 705f 7365 636f 6e64 203d 202d 310d  omp_second = -1.
-0000a660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-0000a690: 6661 6365 5f61 7265 6120 3d20 2d31 0d0a  face_area = -1..
+0000a5e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0000a5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+0000a620: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+0000a630: 6972 7374 203d 202d 310d 0a20 2020 2020  irst = -1..     
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
+0000a670: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
+0000a680: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000a6d0: 5f61 7869 735f 6d61 736b 203d 202d 3120  _axis_mask = -1 
-0000a6e0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a700: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-0000a710: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-0000a720: 3d20 2874 2c72 6f75 6e64 287a 292f 7365  = (t,round(z)/se
-0000a730: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
-0000a740: 2072 6f75 6e64 2879 292f 7365 6c66 2e79   round(y)/self.y
-0000a750: 6361 6c69 6272 6174 696f 6e2c 2072 6f75  calibration, rou
-0000a760: 6e64 2878 292f 7365 6c66 2e78 6361 6c69  nd(x)/self.xcali
-0000a770: 6272 6174 696f 6e29 200d 0a20 2020 2020  bration) ..     
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a7a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-0000a7b0: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
-0000a7c0: 706f 745f 6365 6e74 726f 6964 5d20 3d20  pot_centroid] = 
-0000a7d0: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
-0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
-0000a800: 656e 745f 7472 6163 6b5f 6964 2069 6e20  ent_track_id in 
-0000a810: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-0000a820: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-0000a850: 6b6c 6574 5f61 7272 6179 203d 2063 7572  klet_array = cur
-0000a860: 7265 6e74 5f74 7261 636b 6c65 7473 5b63  rent_tracklets[c
-0000a870: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
-0000a880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-0000a8b0: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
-0000a8c0: 203d 206e 702e 6172 7261 7928 5b69 6e74   = np.array([int
-0000a8d0: 2866 6c6f 6174 2875 6e69 7175 655f 6964  (float(unique_id
-0000a8e0: 2929 2c20 742c 207a 2f73 656c 662e 7a63  )), t, z/self.zc
-0000a8f0: 616c 6962 7261 7469 6f6e 2c20 792f 7365  alibration, y/se
-0000a900: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
-0000a910: 2078 2f73 656c 662e 7863 616c 6962 7261   x/self.xcalibra
-0000a920: 7469 6f6e 5d29 0d0a 2020 2020 2020 2020  tion])..        
-0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a950: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-0000a960: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
-0000a970: 6964 5d20 3d20 6e70 2e76 7374 6163 6b28  id] = np.vstack(
-0000a980: 2874 7261 636b 6c65 745f 6172 7261 792c  (tracklet_array,
-0000a990: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000a9a0: 745f 6172 7261 7929 290d 0a0d 0a20 2020  t_array))....   
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9d0: 2020 2020 2076 616c 7565 5f61 7272 6179       value_array
-0000a9e0: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
-0000a9f0: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
-0000aa00: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-0000aa10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa30: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0000aa40: 6e74 5f76 616c 7565 5f61 7272 6179 203d  nt_value_array =
-0000aa50: 206e 702e 6172 7261 7928 5b74 2c20 696e   np.array([t, in
-0000aa60: 7428 666c 6f61 7428 756e 6971 7565 5f69  t(float(unique_i
-0000aa70: 6429 292c 2067 656e 5f69 642c 2072 6164  d)), gen_id, rad
-0000aa80: 6975 732c 2076 6f6c 756d 655f 7069 7865  ius, volume_pixe
-0000aa90: 6c73 2c20 6563 6365 6e74 7269 6369 7479  ls, eccentricity
-0000aaa0: 5f63 6f6d 705f 6669 7273 742c 2065 6363  _comp_first, ecc
-0000aab0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-0000aac0: 6563 6f6e 642c 2073 7572 6661 6365 5f61  econd, surface_a
-0000aad0: 7265 612c 2074 6f74 616c 5f69 6e74 656e  rea, total_inten
-0000aae0: 7369 7479 2c20 7370 6565 642c 206d 6f74  sity, speed, mot
-0000aaf0: 696f 6e5f 616e 676c 652c 2061 6363 656c  ion_angle, accel
-0000ab00: 6572 6174 696f 6e2c 2064 6973 7461 6e63  eration, distanc
-0000ab10: 655f 6365 6c6c 5f6d 6173 6b2c 2072 6164  e_cell_mask, rad
-0000ab20: 6961 6c5f 616e 676c 652c 2063 656c 6c5f  ial_angle, cell_
-0000ab30: 6178 6973 5f6d 6173 6b2c 7472 6163 6b5f  axis_mask,track_
-0000ab40: 6469 7370 6c61 6365 6d65 6e74 2c20 746f  displacement, to
-0000ab50: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
-0000ab60: 6365 2c20 6d61 785f 7472 6163 6b5f 6469  ce, max_track_di
-0000ab70: 7374 616e 6365 2c20 7472 6163 6b5f 6475  stance, track_du
-0000ab80: 7261 7469 6f6e 205d 290d 0a20 2020 2020  ration ])..     
-0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a6b0: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
+0000a6c0: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6f0: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
+0000a700: 3d20 2d31 2020 2020 200d 0a0d 0a20 2020  = -1     ....   
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a730: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
+0000a740: 726f 6964 203d 2028 742c 726f 756e 6428  roid = (t,round(
+0000a750: 7a29 2f73 656c 662e 7a63 616c 6962 7261  z)/self.zcalibra
+0000a760: 7469 6f6e 2c20 726f 756e 6428 7929 2f73  tion, round(y)/s
+0000a770: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+0000a780: 2c20 726f 756e 6428 7829 2f73 656c 662e  , round(x)/self.
+0000a790: 7863 616c 6962 7261 7469 6f6e 2920 0d0a  xcalibration) ..
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000a7d0: 7370 6f74 5f63 656e 7472 6f69 645b 6672  spot_centroid[fr
+0000a7e0: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+0000a7f0: 645d 203d 206b 0d0a 0d0a 2020 2020 2020  d] = k....      
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a820: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
+0000a830: 6420 696e 2063 7572 7265 6e74 5f74 7261  d in current_tra
+0000a840: 636b 6c65 7473 3a0d 0a20 2020 2020 2020  cklets:..       
+0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a870: 2074 7261 636b 6c65 745f 6172 7261 7920   tracklet_array 
+0000a880: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
+0000a890: 6574 735b 6375 7272 656e 745f 7472 6163  ets[current_trac
+0000a8a0: 6b5f 6964 5d0d 0a20 2020 2020 2020 2020  k_id]..         
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000a8d0: 7572 7265 6e74 5f74 7261 636b 6c65 745f  urrent_tracklet_
+0000a8e0: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
+0000a8f0: 285b 696e 7428 666c 6f61 7428 756e 6971  ([int(float(uniq
+0000a900: 7565 5f69 6429 292c 2074 2c20 7a2f 7365  ue_id)), t, z/se
+0000a910: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+0000a920: 2079 2f73 656c 662e 7963 616c 6962 7261   y/self.ycalibra
+0000a930: 7469 6f6e 2c20 782f 7365 6c66 2e78 6361  tion, x/self.xca
+0000a940: 6c69 6272 6174 696f 6e5d 290d 0a20 2020  libration])..   
+0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a970: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+0000a980: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
+0000a990: 7261 636b 5f69 645d 203d 206e 702e 7673  rack_id] = np.vs
+0000a9a0: 7461 636b 2828 7472 6163 6b6c 6574 5f61  tack((tracklet_a
+0000a9b0: 7272 6179 2c20 6375 7272 656e 745f 7472  rray, current_tr
+0000a9c0: 6163 6b6c 6574 5f61 7272 6179 2929 0d0a  acklet_array))..
+0000a9d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9f0: 2020 2020 2020 2020 2020 7661 6c75 655f            value_
+0000aa00: 6172 7261 7920 3d20 6375 7272 656e 745f  array = current_
+0000aa10: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+0000aa20: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
+0000aa30: 636b 5f69 645d 0d0a 2020 2020 2020 2020  ck_id]..        
+0000aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa60: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
+0000aa70: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
+0000aa80: 742c 2069 6e74 2866 6c6f 6174 2875 6e69  t, int(float(uni
+0000aa90: 7175 655f 6964 2929 2c20 6765 6e5f 6964  que_id)), gen_id
+0000aaa0: 2c20 7261 6469 7573 2c20 766f 6c75 6d65  , radius, volume
+0000aab0: 5f70 6978 656c 732c 2065 6363 656e 7472  _pixels, eccentr
+0000aac0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+0000aad0: 2c20 6563 6365 6e74 7269 6369 7479 5f63  , eccentricity_c
+0000aae0: 6f6d 705f 7365 636f 6e64 2c20 7375 7266  omp_second, surf
+0000aaf0: 6163 655f 6172 6561 2c20 746f 7461 6c5f  ace_area, total_
+0000ab00: 696e 7465 6e73 6974 792c 2073 7065 6564  intensity, speed
+0000ab10: 2c20 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  , motion_angle, 
+0000ab20: 6163 6365 6c65 7261 7469 6f6e 2c20 6469  acceleration, di
+0000ab30: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000ab40: 2c20 7261 6469 616c 5f61 6e67 6c65 2c20  , radial_angle, 
+0000ab50: 6365 6c6c 5f61 7869 735f 6d61 736b 2c74  cell_axis_mask,t
+0000ab60: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+0000ab70: 742c 2074 6f74 616c 5f74 7261 636b 5f64  t, total_track_d
+0000ab80: 6973 7461 6e63 652c 206d 6178 5f74 7261  istance, max_tra
+0000ab90: 636b 5f64 6973 7461 6e63 652c 2074 7261  ck_distance, tra
+0000aba0: 636b 5f64 7572 6174 696f 6e20 5d29 0d0a  ck_duration ])..
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abd0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0000abe0: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-0000abf0: 726f 7065 7274 6965 735b 6375 7272 656e  roperties[curren
-0000ac00: 745f 7472 6163 6b5f 6964 5d20 3d20 6e70  t_track_id] = np
-0000ac10: 2e76 7374 6163 6b28 2876 616c 7565 5f61  .vstack((value_a
-0000ac20: 7272 6179 2c20 6375 7272 656e 745f 7661  rray, current_va
-0000ac30: 6c75 655f 6172 7261 7929 290d 0a0d 0a20  lue_array)).... 
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac60: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000abd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+0000ac10: 6574 735f 7072 6f70 6572 7469 6573 5b63  ets_properties[c
+0000ac20: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+0000ac30: 203d 206e 702e 7673 7461 636b 2828 7661   = np.vstack((va
+0000ac40: 6c75 655f 6172 7261 792c 2063 7572 7265  lue_array, curre
+0000ac50: 6e74 5f76 616c 7565 5f61 7272 6179 2929  nt_value_array))
+0000ac60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac90: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-0000aca0: 6574 5f61 7272 6179 203d 206e 702e 6172  et_array = np.ar
-0000acb0: 7261 7928 5b69 6e74 2866 6c6f 6174 2875  ray([int(float(u
-0000acc0: 6e69 7175 655f 6964 2929 2c20 742c 207a  nique_id)), t, z
-0000acd0: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
-0000ace0: 6f6e 2c20 792f 7365 6c66 2e79 6361 6c69  on, y/self.ycali
-0000acf0: 6272 6174 696f 6e2c 2078 2f73 656c 662e  bration, x/self.
-0000ad00: 7863 616c 6962 7261 7469 6f6e 5d29 0d0a  xcalibration])..
-0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad30: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0000ad40: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
-0000ad50: 745f 7472 6163 6b5f 6964 5d20 3d20 6375  t_track_id] = cu
-0000ad60: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
-0000ad70: 7272 6179 200d 0a0d 0a20 2020 2020 2020  rray ....       
-0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ada0: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
-0000adb0: 7272 6179 203d 206e 702e 6172 7261 7928  rray = np.array(
-0000adc0: 5b74 2c20 696e 7428 666c 6f61 7428 756e  [t, int(float(un
-0000add0: 6971 7565 5f69 6429 292c 2067 656e 5f69  ique_id)), gen_i
-0000ade0: 642c 2072 6164 6975 732c 2076 6f6c 756d  d, radius, volum
-0000adf0: 655f 7069 7865 6c73 2c20 2065 6363 656e  e_pixels,  eccen
-0000ae00: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-0000ae10: 7374 2c20 6563 6365 6e74 7269 6369 7479  st, eccentricity
-0000ae20: 5f63 6f6d 705f 7365 636f 6e64 2c20 7375  _comp_second, su
-0000ae30: 7266 6163 655f 6172 6561 2c20 2074 6f74  rface_area,  tot
-0000ae40: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
-0000ae50: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
-0000ae60: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
-0000ae70: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
-0000ae80: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
-0000ae90: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
-0000aea0: 6b2c 7472 6163 6b5f 6469 7370 6c61 6365  k,track_displace
-0000aeb0: 6d65 6e74 2c20 746f 7461 6c5f 7472 6163  ment, total_trac
-0000aec0: 6b5f 6469 7374 616e 6365 2c20 6d61 785f  k_distance, max_
-0000aed0: 7472 6163 6b5f 6469 7374 616e 6365 2c20  track_distance, 
-0000aee0: 7472 6163 6b5f 6475 7261 7469 6f6e 205d  track_duration ]
-0000aef0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0000af20: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-0000af30: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
-0000af40: 7472 6163 6b5f 6964 5d20 3d20 6375 7272  track_id] = curr
-0000af50: 656e 745f 7661 6c75 655f 6172 7261 790d  ent_value_array.
-0000af60: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 2020 2020 2020 2072 6574 7572 6e20 6375         return cu
-0000af90: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
-0000afa0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000afb0: 7473 5f70 726f 7065 7274 6965 7320 2020  ts_properties   
-0000afc0: 2020 0d0a 0d0a 2020 2020 6465 6620 5f6d    ....    def _m
-0000afd0: 6173 7465 725f 7370 6f74 5f63 6f6d 7075  aster_spot_compu
-0000afe0: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
-0000aff0: 3a0d 0a20 2020 2020 2020 2020 200d 0a20  :..          .. 
-0000b000: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
-0000b010: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
-0000b020: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
-0000b030: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b040: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
-0000b070: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b080: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
-0000b090: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000b0a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0c0: 2020 2020 6966 2073 656c 662e 756e 6971      if self.uniq
-0000b0d0: 7565 6964 5f6b 6579 2069 6e20 5370 6f74  ueid_key in Spot
-0000b0e0: 6f62 6a65 6374 2e6b 6579 7328 293a 0d0a  object.keys():..
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b120: 2020 2020 2020 2020 2020 7261 6469 7573            radius
-0000b130: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000b140: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
-0000b150: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
-0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2020 2020 2020 2020 2020 2071 7561 6c69             quali
-0000b180: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
-0000b190: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000b1a0: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000b1d0: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
-0000b1e0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000b1f0: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
-0000b200: 696e 7465 6e73 6974 795f 6b65 7929 290d  intensity_key)).
-0000b210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 206d 6561 6e5f 696e 7465 6e73 6974 7920   mean_intensity 
-0000b240: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
-0000b250: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
-0000b260: 5f69 6e74 656e 7369 7479 5f6b 6579 2929  _intensity_key))
-0000b270: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000b2a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000b2b0: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
-0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
-0000b2f0: 793a 2069 6e74 2866 6c6f 6174 2853 706f  y: int(float(Spo
-0000b300: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b310: 2e73 706f 7469 645f 6b65 7929 2929 2c20  .spotid_key))), 
-0000b320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
-0000b350: 6964 5f6b 6579 203a 2069 6e74 2866 6c6f  id_key : int(flo
-0000b360: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b370: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
-0000b380: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
-0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b3b0: 2e7a 706f 7369 645f 6b65 7920 3a20 666c  .zposid_key : fl
-0000b3c0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b3d0: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
-0000b3e0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b410: 7970 6f73 6964 5f6b 6579 203a 2066 6c6f  yposid_key : flo
-0000b420: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b430: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
-0000b440: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b460: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000b470: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000b480: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b490: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000b4a0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4c0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
-0000b4d0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000b4e0: 7920 3a20 746f 7461 6c5f 696e 7465 6e73  y : total_intens
-0000b4f0: 6974 792c 0d0a 2020 2020 2020 2020 2020  ity,..          
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000b520: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
-0000b530: 7920 3a20 6d65 616e 5f69 6e74 656e 7369  y : mean_intensi
-0000b540: 7479 2c0d 0a20 2020 2020 2020 2020 2020  ty,..           
-0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-0000b570: 6469 7573 5f6b 6579 203a 2072 6164 6975  dius_key : radiu
-0000b580: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5a0: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
-0000b5b0: 6c69 7479 5f6b 6579 203a 2071 7561 6c69  lity_key : quali
-0000b5c0: 7479 2c0d 0a20 2020 2020 2020 2020 2020  ty,..           
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
-0000b5f0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000b600: 5f6b 6579 3a20 2866 6c6f 6174 2853 706f  _key: (float(Spo
-0000b610: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b620: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-0000b630: 6173 6b5f 6b65 7929 2929 2c0d 0a20 2020  ask_key))),..   
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2073 656c 662e 756e 6971 7565 6964 5f6b   self.uniqueid_k
-0000b670: 6579 203a 2073 7472 2853 706f 746f 626a  ey : str(Spotobj
-0000b680: 6563 742e 6765 7428 7365 6c66 2e75 6e69  ect.get(self.uni
-0000b690: 7175 6569 645f 6b65 7929 292c 0d0a 2020  queid_key)),..  
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6c0: 2020 7365 6c66 2e74 7261 636b 6c65 7469    self.trackleti
-0000b6d0: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
-0000b6e0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b6f0: 7472 6163 6b6c 6574 6964 5f6b 6579 2929  trackletid_key))
-0000b700: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b720: 2020 2020 2020 2073 656c 662e 6765 6e65         self.gene
-0000b730: 7261 7469 6f6e 6964 5f6b 6579 203a 2073  rationid_key : s
-0000b740: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
-0000b750: 7428 7365 6c66 2e67 656e 6572 6174 696f  t(self.generatio
-0000b760: 6e69 645f 6b65 7929 292c 0d0a 2020 2020  nid_key)),..    
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000b7a0: 203a 2073 7472 2853 706f 746f 626a 6563   : str(Spotobjec
-0000b7b0: 742e 6765 7428 7365 6c66 2e74 7261 636b  t.get(self.track
-0000b7c0: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b7f0: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-0000b800: 5f6b 6579 203a 2028 666c 6f61 7428 5370  _key : (float(Sp
-0000b810: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b820: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-0000b830: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
-0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b860: 2e73 7065 6564 5f6b 6579 203a 2028 666c  .speed_key : (fl
-0000b870: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b880: 6574 2873 656c 662e 7370 6565 645f 6b65  et(self.speed_ke
-0000b890: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b8c0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-0000b8d0: 203a 2028 666c 6f61 7428 5370 6f74 6f62   : (float(Spotob
-0000b8e0: 6a65 6374 2e67 6574 2873 656c 662e 6163  ject.get(self.ac
-0000b8f0: 6365 6c65 7261 7469 6f6e 5f6b 6579 2929  celeration_key))
-0000b900: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b920: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000b930: 6961 6c5f 616e 676c 655f 6b65 793a 2066  ial_angle_key: f
-0000b940: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b950: 6765 7428 7365 6c66 2e72 6164 6961 6c5f  get(self.radial_
-0000b960: 616e 676c 655f 6b65 7929 292c 0d0a 2020  angle_key)),..  
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-0000b990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+0000acc0: 7261 636b 6c65 745f 6172 7261 7920 3d20  racklet_array = 
+0000acd0: 6e70 2e61 7272 6179 285b 696e 7428 666c  np.array([int(fl
+0000ace0: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
+0000acf0: 2074 2c20 7a2f 7365 6c66 2e7a 6361 6c69   t, z/self.zcali
+0000ad00: 6272 6174 696f 6e2c 2079 2f73 656c 662e  bration, y/self.
+0000ad10: 7963 616c 6962 7261 7469 6f6e 2c20 782f  ycalibration, x/
+0000ad20: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000ad30: 6e5d 290d 0a20 2020 2020 2020 2020 2020  n])..           
+0000ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad50: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0000ad60: 7265 6e74 5f74 7261 636b 6c65 7473 5b63  rent_tracklets[c
+0000ad70: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
+0000ad80: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
+0000ad90: 6c65 745f 6172 7261 7920 0d0a 0d0a 2020  let_array ....  
+0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adc0: 2020 2020 2020 6375 7272 656e 745f 7661        current_va
+0000add0: 6c75 655f 6172 7261 7920 3d20 6e70 2e61  lue_array = np.a
+0000ade0: 7272 6179 285b 742c 2069 6e74 2866 6c6f  rray([t, int(flo
+0000adf0: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
+0000ae00: 6765 6e5f 6964 2c20 7261 6469 7573 2c20  gen_id, radius, 
+0000ae10: 766f 6c75 6d65 5f70 6978 656c 732c 2020  volume_pixels,  
+0000ae20: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000ae30: 705f 6669 7273 742c 2065 6363 656e 7472  p_first, eccentr
+0000ae40: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+0000ae50: 642c 2073 7572 6661 6365 5f61 7265 612c  d, surface_area,
+0000ae60: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+0000ae70: 792c 2073 7065 6564 2c20 6d6f 7469 6f6e  y, speed, motion
+0000ae80: 5f61 6e67 6c65 2c20 6163 6365 6c65 7261  _angle, accelera
+0000ae90: 7469 6f6e 2c20 6469 7374 616e 6365 5f63  tion, distance_c
+0000aea0: 656c 6c5f 6d61 736b 2c20 7261 6469 616c  ell_mask, radial
+0000aeb0: 5f61 6e67 6c65 2c20 6365 6c6c 5f61 7869  _angle, cell_axi
+0000aec0: 735f 6d61 736b 2c74 7261 636b 5f64 6973  s_mask,track_dis
+0000aed0: 706c 6163 656d 656e 742c 2074 6f74 616c  placement, total
+0000aee0: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
+0000aef0: 206d 6178 5f74 7261 636b 5f64 6973 7461   max_track_dista
+0000af00: 6e63 652c 2074 7261 636b 5f64 7572 6174  nce, track_durat
+0000af10: 696f 6e20 5d29 0d0a 2020 2020 2020 2020  ion ])..        
+0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af40: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+0000af50: 735f 7072 6f70 6572 7469 6573 5b63 7572  s_properties[cur
+0000af60: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
+0000af70: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
+0000af80: 7272 6179 0d0a 0d0a 2020 2020 2020 2020  rray....        
+0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afa0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000afb0: 726e 2063 7572 7265 6e74 5f74 7261 636b  rn current_track
+0000afc0: 6c65 7473 2c20 6375 7272 656e 745f 7472  lets, current_tr
+0000afd0: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+0000afe0: 6573 2020 2020 200d 0a0d 0a20 2020 2064  es     ....    d
+0000aff0: 6566 205f 6d61 7374 6572 5f73 706f 745f  ef _master_spot_
+0000b000: 636f 6d70 7574 6572 2873 656c 662c 2066  computer(self, f
+0000b010: 7261 6d65 293a 0d0a 2020 2020 2020 2020  rame):..        
+0000b020: 2020 0d0a 2020 2020 2020 2020 2020 666f    ..          fo
+0000b030: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
+0000b040: 6672 616d 652e 6669 6e64 616c 6c28 2753  frame.findall('S
+0000b050: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+0000b060: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000b070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b080: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000b090: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000b0a0: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000b0b0: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000b0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b0e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000b0f0: 2e75 6e69 7175 6569 645f 6b65 7920 696e  .uniqueid_key in
+0000b100: 2053 706f 746f 626a 6563 742e 6b65 7973   Spotobject.keys
+0000b110: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0000b120: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b150: 6164 6975 7320 3d20 666c 6f61 7428 5370  adius = float(Sp
+0000b160: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b170: 662e 7261 6469 7573 5f6b 6579 2929 0d0a  f.radius_key))..
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 7175 616c 6974 7920 3d20 666c 6f61 7428  quality = float(
+0000b1b0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b1c0: 656c 662e 7175 616c 6974 795f 6b65 7929  elf.quality_key)
+0000b1d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1f0: 2020 2074 6f74 616c 5f69 6e74 656e 7369     total_intensi
+0000b200: 7479 203d 2066 6c6f 6174 2853 706f 746f  ty = float(Spoto
+0000b210: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000b220: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000b230: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b250: 2020 2020 2020 6d65 616e 5f69 6e74 656e        mean_inten
+0000b260: 7369 7479 203d 2066 6c6f 6174 2853 706f  sity = float(Spo
+0000b270: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b280: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+0000b290: 6b65 7929 290d 0a0d 0a20 2020 2020 2020  key))....       
+0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2b0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000b2c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000b2d0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+0000b2e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+0000b310: 6964 5f6b 6579 3a20 696e 7428 666c 6f61  id_key: int(floa
+0000b320: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000b330: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000b340: 2929 292c 200d 0a20 2020 2020 2020 2020  ))), ..         
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b370: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+0000b380: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000b390: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
+0000b3a0: 6569 645f 6b65 7929 2929 2c0d 0a20 2020  eid_key))),..   
+0000b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3d0: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000b3e0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000b3f0: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000b400: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 7365 6c66 2e79 706f 7369 645f 6b65 7920  self.yposid_key 
+0000b440: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000b450: 6374 2e67 6574 2873 656c 662e 7970 6f73  ct.get(self.ypos
+0000b460: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b490: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000b4a0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000b4b0: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000b4c0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b4f0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000b500: 7479 5f6b 6579 203a 2074 6f74 616c 5f69  ty_key : total_i
+0000b510: 6e74 656e 7369 7479 2c0d 0a20 2020 2020  ntensity,..     
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b540: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000b550: 7479 5f6b 6579 203a 206d 6561 6e5f 696e  ty_key : mean_in
+0000b560: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b590: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
+0000b5a0: 7261 6469 7573 2c0d 0a20 2020 2020 2020  radius,..       
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b5d0: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000b5e0: 7175 616c 6974 792c 0d0a 2020 2020 2020  quality,..      
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b610: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+0000b620: 5f6d 6173 6b5f 6b65 793a 2028 666c 6f61  _mask_key: (floa
+0000b630: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000b640: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
+0000b650: 656c 6c5f 6d61 736b 5f6b 6579 2929 292c  ell_mask_key))),
+0000b660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000b690: 6569 645f 6b65 7920 3a20 7374 7228 5370  eid_key : str(Sp
+0000b6a0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b6b0: 662e 756e 6971 7565 6964 5f6b 6579 2929  f.uniqueid_key))
+0000b6c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+0000b6f0: 6b6c 6574 6964 5f6b 6579 203a 2073 7472  kletid_key : str
+0000b700: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b710: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
+0000b720: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b750: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
+0000b760: 7920 3a20 7374 7228 5370 6f74 6f62 6a65  y : str(Spotobje
+0000b770: 6374 2e67 6574 2873 656c 662e 6765 6e65  ct.get(self.gene
+0000b780: 7261 7469 6f6e 6964 5f6b 6579 2929 2c0d  rationid_key)),.
+0000b790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7b0: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+0000b7c0: 645f 6b65 7920 3a20 7374 7228 5370 6f74  d_key : str(Spot
+0000b7d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b7e0: 7472 6163 6b69 645f 6b65 7929 292c 0d0a  trackid_key)),..
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2020 7365 6c66 2e6d 6f74 696f 6e5f      self.motion_
+0000b820: 616e 676c 655f 6b65 7920 3a20 2866 6c6f  angle_key : (flo
+0000b830: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000b840: 7428 7365 6c66 2e6d 6f74 696f 6e5f 616e  t(self.motion_an
+0000b850: 676c 655f 6b65 7929 2929 2c0d 0a20 2020  gle_key))),..   
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b880: 2073 656c 662e 7370 6565 645f 6b65 7920   self.speed_key 
+0000b890: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
+0000b8a0: 6563 742e 6765 7428 7365 6c66 2e73 7065  ect.get(self.spe
+0000b8b0: 6564 5f6b 6579 2929 292c 0d0a 2020 2020  ed_key))),..    
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+0000b8f0: 6e5f 6b65 7920 3a20 2866 6c6f 6174 2853  n_key : (float(S
+0000b900: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b910: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+0000b920: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b950: 662e 7261 6469 616c 5f61 6e67 6c65 5f6b  f.radial_angle_k
+0000b960: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
+0000b970: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000b980: 6469 616c 5f61 6e67 6c65 5f6b 6579 2929  dial_angle_key))
+0000b990: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2069 6620 7365 6c66 2e73 7572 6661 6365   if self.surface
-0000b9c0: 5f61 7265 615f 6b65 7920 696e 2053 706f  _area_key in Spo
-0000b9d0: 746f 626a 6563 742e 6b65 7973 2829 3a0d  tobject.keys():.
-0000b9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba00: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000ba10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000ba20: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-0000ba30: 7064 6174 6528 7b0d 0a20 2020 2020 2020  pdate({..       
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9b0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9d0: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000b9e0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000b9f0: 6e20 5370 6f74 6f62 6a65 6374 2e6b 6579  n Spotobject.key
+0000ba00: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba20: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000ba30: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000ba40: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+0000ba50: 6429 5d2e 7570 6461 7465 287b 0d0a 2020  d)].update({..  
 0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 2073 656c 662e 6563 6365 6e74 7269 6369   self.eccentrici
-0000baa0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-0000bab0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000bac0: 6563 742e 6765 7428 7365 6c66 2e65 6363  ect.get(self.ecc
-0000bad0: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-0000bae0: 6972 7374 6b65 7929 292c 0d0a 2020 2020  irstkey)),..    
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
+0000bac0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+0000bad0: 7374 6b65 7920 3a20 666c 6f61 7428 5370  stkey : float(Sp
+0000bae0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000baf0: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+0000bb00: 6f6d 705f 6669 7273 746b 6579 2929 2c0d  omp_firstkey)),.
+0000bb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 2020 2020 7365 6c66 2e65 6363 656e 7472      self.eccentr
-0000bb50: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000bb60: 646b 6579 203a 2066 6c6f 6174 2853 706f  dkey : float(Spo
-0000bb70: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bb80: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
-0000bb90: 6d70 5f73 6563 6f6e 646b 6579 2929 2c0d  mp_secondkey)),.
-0000bba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb60: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
+0000bb70: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000bb80: 7365 636f 6e64 6b65 7920 3a20 666c 6f61  secondkey : floa
+0000bb90: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bba0: 2873 656c 662e 6563 6365 6e74 7269 6369  (self.eccentrici
+0000bbb0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+0000bbc0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
 0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbf0: 2020 2020 2020 2020 2073 656c 662e 7375           self.su
-0000bc00: 7266 6163 655f 6172 6561 5f6b 6579 203a  rface_area_key :
-0000bc10: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000bc20: 742e 6765 7428 7365 6c66 2e73 7572 6661  t.get(self.surfa
-0000bc30: 6365 5f61 7265 615f 6b65 7929 292c 0d0a  ce_area_key)),..
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000bc20: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+0000bc30: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000bc40: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bc50: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+0000bc60: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc90: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000bca0: 6c61 7869 735f 6d61 736b 5f6b 6579 3a20  laxis_mask_key: 
-0000bcb0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000bcc0: 2e67 6574 2873 656c 662e 6365 6c6c 6178  .get(self.cellax
-0000bcd0: 6973 5f6d 6173 6b5f 6b65 7929 290d 0a20  is_mask_key)).. 
-0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bcc0: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+0000bcd0: 6b65 793a 2066 6c6f 6174 2853 706f 746f  key: float(Spoto
+0000bce0: 626a 6563 742e 6765 7428 7365 6c66 2e63  bject.get(self.c
+0000bcf0: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
+0000bd00: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 2020 2020 207d 290d 0a20             }).. 
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000bd60: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
 0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000bd90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bdb0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-0000bde0: 662e 756e 6971 7565 6964 5f6b 6579 206e  f.uniqueid_key n
-0000bdf0: 6f74 2069 6e20 5370 6f74 6f62 6a65 6374  ot in Spotobject
-0000be00: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000bdf0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000be00: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
+0000be10: 6b65 7920 6e6f 7420 696e 2053 706f 746f  key not in Spoto
+0000be20: 626a 6563 742e 6b65 7973 2829 3a0d 0a20  bject.keys():.. 
 0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be70: 2020 6966 2073 656c 662e 6465 7465 6374    if self.detect
-0000be80: 6f72 6368 616e 6e65 6c20 3d3d 2031 3a0d  orchannel == 1:.
-0000be90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000bed0: 5349 5459 203d 2053 706f 746f 626a 6563  SITY = Spotobjec
-0000bee0: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000bef0: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
-0000bf00: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
-0000bf40: 5445 4e53 4954 5920 3d20 5370 6f74 6f62  TENSITY = Spotob
-0000bf50: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
-0000bf60: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-0000bf70: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2065 6c73 653a 2020 2020 2020 2020     else:        
-0000bfb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
-0000bff0: 4e53 4954 5920 3d20 5370 6f74 6f62 6a65  NSITY = Spotobje
-0000c000: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
-0000c010: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
-0000c020: 6b65 7929 0d0a 2020 2020 2020 2020 2020  key)..          
-0000c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
-0000c060: 4e54 454e 5349 5459 203d 2053 706f 746f  NTENSITY = Spoto
-0000c070: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
-0000c080: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
-0000c090: 315f 6b65 7929 0d0a 2020 2020 2020 2020  1_key)..        
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 5241 4449 5553 203d 2066 6c6f      RADIUS = flo
-0000c0d0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000c0e0: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
-0000c0f0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 2051 5541 4c49 5459 203d 2066 6c6f 6174   QUALITY = float
-0000c130: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000c140: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-0000c150: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000c190: 5349 5459 203d 2066 6c6f 6174 2854 4f54  SITY = float(TOT
-0000c1a0: 414c 5f49 4e54 454e 5349 5459 290d 0a20  AL_INTENSITY).. 
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
-0000c1e0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
-0000c1f0: 7428 4d45 414e 5f49 4e54 454e 5349 5459  t(MEAN_INTENSITY
-0000c200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c230: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-0000c240: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000c250: 6964 5d20 3d20 7b0d 0a20 2020 2020 2020  id] = {..       
-0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c280: 2020 2020 2073 656c 662e 6365 6c6c 6964       self.cellid
-0000c290: 5f6b 6579 3a20 696e 7428 6365 6c6c 5f69  _key: int(cell_i
-0000c2a0: 6429 2c20 0d0a 2020 2020 2020 2020 2020  d), ..          
-0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 7365 6c66 2e66 7261 6d65 6964 5f6b    self.frameid_k
-0000c2e0: 6579 203a 2069 6e74 2866 6c6f 6174 2853  ey : int(float(S
-0000c2f0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c300: 6c66 2e66 7261 6d65 6964 5f6b 6579 2929  lf.frameid_key))
-0000c310: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 7365 6c66 2e7a 706f 7369 645f 6b65 7920  self.zposid_key 
-0000c350: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000c360: 6374 2e67 6574 2873 656c 662e 7a70 6f73  ct.get(self.zpos
-0000c370: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
-0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2073 656c 662e 7970 6f73         self.ypos
-0000c3b0: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
-0000c3c0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c3d0: 6c66 2e79 706f 7369 645f 6b65 7929 292c  lf.yposid_key)),
-0000c3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c400: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c410: 6c66 2e78 706f 7369 645f 6b65 7920 3a20  lf.xposid_key : 
-0000c420: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000c430: 2e67 6574 2873 656c 662e 7870 6f73 6964  .get(self.xposid
-0000c440: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-0000c480: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
-0000c490: 544f 5441 4c5f 494e 5445 4e53 4954 592c  TOTAL_INTENSITY,
-0000c4a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c4d0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000c4e0: 795f 6b65 7920 3a20 4d45 414e 5f49 4e54  y_key : MEAN_INT
-0000c4f0: 454e 5349 5459 2c0d 0a20 2020 2020 2020  ENSITY,..       
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 2020 2073 656c 662e 7261 6469 7573       self.radius
-0000c530: 5f6b 6579 203a 2052 4144 4955 532c 0d0a  _key : RADIUS,..
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c570: 2e71 7561 6c69 7479 5f6b 6579 203a 2051  .quality_key : Q
-0000c580: 5541 4c49 5459 0d0a 2020 2020 2020 2020  UALITY..        
-0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 7d0d 0a20 2020 2020 2020 0d0a 2020 2020  }..       ..    
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c5d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c5e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000c5f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c600: 0a0d 0a20 2020 2064 6566 205f 7370 6f74  ...    def _spot
-0000c610: 5f63 6f6d 7075 7465 7228 7365 6c66 2c20  _computer(self, 
-0000c620: 6672 616d 6529 3a0d 0a0d 0a20 2020 2020  frame):....     
-0000c630: 2020 2020 2066 6f72 2053 706f 746f 626a       for Spotobj
-0000c640: 6563 7420 696e 2066 7261 6d65 2e66 696e  ect in frame.fin
-0000c650: 6461 6c6c 2827 5370 6f74 2729 3a0d 0a20  dall('Spot'):.. 
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c670: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0000c680: 6f62 6a65 6374 2077 6974 6820 756e 6971  object with uniq
-0000c690: 7565 2063 656c 6c20 4944 0d0a 2020 2020  ue cell ID..    
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6b0: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
-0000c6c0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000c6d0: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
-0000c6e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000c6f0: 2020 2020 2020 2020 2020 2020 2320 4765              # Ge
-0000c700: 7420 7468 6520 545a 5958 206c 6f63 6174  t the TZYX locat
-0000c710: 696f 6e20 6f66 2074 6865 2063 656c 6c73  ion of the cells
-0000c720: 2069 6e20 7468 6174 2066 7261 6d65 0d0a   in that frame..
-0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c740: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c750: 6465 7465 6374 6f72 6368 616e 6e65 6c20  detectorchannel 
-0000c760: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c780: 2020 2020 2020 2069 6620 5370 6f74 6f62         if Spotob
-0000c790: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
-0000c7a0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0000c7b0: 325f 6b65 7929 2069 7320 6e6f 7420 4e6f  2_key) is not No
-0000c7c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000c7f0: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
-0000c800: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000c810: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
-0000c820: 6e74 656e 7369 7479 5f63 6832 5f6b 6579  ntensity_ch2_key
-0000c830: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c850: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
-0000c860: 5f49 4e54 454e 5349 5459 203d 2066 6c6f  _INTENSITY = flo
-0000c870: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000c880: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
-0000c890: 6e73 6974 795f 6368 325f 6b65 7929 290d  nsity_ch2_key)).
-0000c8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000be60: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be90: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0000bea0: 6574 6563 746f 7263 6861 6e6e 656c 203d  etectorchannel =
+0000beb0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000bef0: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
+0000bf00: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bf10: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000bf20: 6368 325f 6b65 7929 0d0a 2020 2020 2020  ch2_key)..      
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf50: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000bf60: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
+0000bf70: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000bf80: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000bf90: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
+0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+0000bfd0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c000: 2020 2020 2020 2020 2020 2054 4f54 414c             TOTAL
+0000c010: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
+0000c020: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000c030: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000c040: 5f63 6831 5f6b 6579 290d 0a20 2020 2020  _ch1_key)..     
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c070: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000c080: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000c090: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c0a0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000c0b0: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0e0: 2020 2020 2020 2020 2052 4144 4955 5320           RADIUS 
+0000c0f0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000c100: 6374 2e67 6574 2873 656c 662e 7261 6469  ct.get(self.radi
+0000c110: 7573 5f6b 6579 2929 0d0a 2020 2020 2020  us_key))..      
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c140: 2020 2020 2020 5155 414c 4954 5920 3d20        QUALITY = 
+0000c150: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000c160: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
+0000c170: 795f 6b65 7929 2920 2020 2020 0d0a 2020  y_key))     ..  
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1a0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000c1b0: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000c1c0: 7428 544f 5441 4c5f 494e 5445 4e53 4954  t(TOTAL_INTENSIT
+0000c1d0: 5929 0d0a 2020 2020 2020 2020 2020 2020  Y)..            
+0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000c210: 2066 6c6f 6174 284d 4541 4e5f 494e 5445   float(MEAN_INTE
+0000c220: 4e53 4954 5929 0d0a 2020 2020 2020 2020  NSITY)..        
+0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c250: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000c260: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000c270: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
+0000c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000c2b0: 656c 6c69 645f 6b65 793a 2069 6e74 2863  ellid_key: int(c
+0000c2c0: 656c 6c5f 6964 292c 200d 0a20 2020 2020  ell_id), ..     
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 2020 2020 2073 656c 662e 6672 616d         self.fram
+0000c300: 6569 645f 6b65 7920 3a20 696e 7428 666c  eid_key : int(fl
+0000c310: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000c320: 6574 2873 656c 662e 6672 616d 6569 645f  et(self.frameid_
+0000c330: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
+0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 2020 2073 656c 662e 7a70 6f73 6964       self.zposid
+0000c370: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000c380: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000c390: 2e7a 706f 7369 645f 6b65 7929 292c 0d0a  .zposid_key)),..
+0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c3d0: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
+0000c3e0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000c3f0: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000c400: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c430: 2020 2073 656c 662e 7870 6f73 6964 5f6b     self.xposid_k
+0000c440: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000c450: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
+0000c460: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c490: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000c4a0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
+0000c4b0: 6579 203a 2054 4f54 414c 5f49 4e54 454e  ey : TOTAL_INTEN
+0000c4c0: 5349 5459 2c0d 0a20 2020 2020 2020 2020  SITY,..         
+0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4f0: 2020 2073 656c 662e 6d65 616e 5f69 6e74     self.mean_int
+0000c500: 656e 7369 7479 5f6b 6579 203a 204d 4541  ensity_key : MEA
+0000c510: 4e5f 494e 5445 4e53 4954 592c 0d0a 2020  N_INTENSITY,..  
+0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c540: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000c550: 6164 6975 735f 6b65 7920 3a20 5241 4449  adius_key : RADI
+0000c560: 5553 2c0d 0a20 2020 2020 2020 2020 2020  US,..           
+0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c590: 2073 656c 662e 7175 616c 6974 795f 6b65   self.quality_ke
+0000c5a0: 7920 3a20 5155 414c 4954 590d 0a20 2020  y : QUALITY..   
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2020 2020 207d 0d0a 2020 2020 2020 200d       }..       .
+0000c5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c5f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000c600: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+0000c630: 5f73 706f 745f 636f 6d70 7574 6572 2873  _spot_computer(s
+0000c640: 656c 662c 2066 7261 6d65 293a 0d0a 0d0a  elf, frame):....
+0000c650: 2020 2020 2020 2020 2020 666f 7220 5370            for Sp
+0000c660: 6f74 6f62 6a65 6374 2069 6e20 6672 616d  otobject in fram
+0000c670: 652e 6669 6e64 616c 6c28 2753 706f 7427  e.findall('Spot'
+0000c680: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000c690: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+0000c6a0: 6561 7465 206f 626a 6563 7420 7769 7468  eate object with
+0000c6b0: 2075 6e69 7175 6520 6365 6c6c 2049 440d   unique cell ID.
+0000c6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c6d0: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+0000c6e0: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+0000c6f0: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+0000c700: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000c710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c720: 2023 2047 6574 2074 6865 2054 5a59 5820   # Get the TZYX 
+0000c730: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
+0000c740: 6365 6c6c 7320 696e 2074 6861 7420 6672  cells in that fr
+0000c750: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+0000c760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000c770: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000c780: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
+0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7a0: 2020 2020 2020 2020 2020 2020 6966 2053              if S
+0000c7b0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000c7c0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000c7d0: 7479 5f63 6832 5f6b 6579 2920 6973 206e  ty_ch2_key) is n
+0000c7e0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c810: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
+0000c820: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
+0000c830: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
+0000c840: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0000c850: 325f 6b65 7929 290d 0a20 2020 2020 2020  2_key))..       
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c880: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000c890: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000c8a0: 6374 2e67 6574 2873 656c 662e 6d65 616e  ct.get(self.mean
+0000c8b0: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
+0000c8c0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000c8f0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000c900: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
-0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c920: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
-0000c930: 5f49 4e54 454e 5349 5459 203d 202d 3120  _INTENSITY = -1 
-0000c940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c960: 656c 7365 3a20 2020 2020 2020 200d 0a20  else:        .. 
+0000c8e0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c910: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
+0000c920: 4954 5920 3d20 2d31 0d0a 2020 2020 2020  ITY = -1..      
+0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c950: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000c960: 3d20 2d31 2020 2020 2020 200d 0a20 2020  = -1       ..   
 0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000c990: 6620 5370 6f74 6f62 6a65 6374 2e67 6574  f Spotobject.get
-0000c9a0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000c9b0: 6e73 6974 795f 6368 315f 6b65 7929 2069  nsity_ch1_key) i
-0000c9c0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9f0: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
-0000ca00: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000ca10: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000ca20: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000ca30: 5f63 6831 5f6b 6579 2929 0d0a 2020 2020  _ch1_key))..    
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
-0000ca70: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000ca80: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
-0000ca90: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
-0000caa0: 315f 6b65 7929 290d 0a20 2020 2020 2020  1_key))..       
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000c980: 2020 2020 2065 6c73 653a 2020 2020 2020       else:      
+0000c990: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 2020 6966 2053 706f 746f 626a 6563      if Spotobjec
+0000c9c0: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
+0000c9d0: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
+0000c9e0: 6579 2920 6973 206e 6f74 204e 6f6e 653a  ey) is not None:
+0000c9f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca10: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000ca20: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
+0000ca30: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ca40: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
+0000ca50: 6e73 6974 795f 6368 315f 6b65 7929 290d  nsity_ch1_key)).
+0000ca60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca80: 2020 2020 2020 2020 204d 4541 4e5f 494e           MEAN_IN
+0000ca90: 5445 4e53 4954 5920 3d20 666c 6f61 7428  TENSITY = float(
+0000caa0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000cab0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000cac0: 7479 5f63 6831 5f6b 6579 2929 0d0a 2020  ty_ch1_key))..  
 0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2020 2020 2020 544f 5441 4c5f 494e          TOTAL_IN
-0000cb00: 5445 4e53 4954 5920 3d20 2d31 0d0a 2020  TENSITY = -1..  
-0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb30: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000cb40: 5349 5459 203d 202d 3120 2020 2020 2020  SITY = -1       
-0000cb50: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000cae0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000caf0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000cb20: 414c 5f49 4e54 454e 5349 5459 203d 202d  AL_INTENSITY = -
+0000cb30: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb50: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
+0000cb60: 494e 5445 4e53 4954 5920 3d20 2d31 2020  INTENSITY = -1  
+0000cb70: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
 0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb90: 5241 4449 5553 203d 2066 6c6f 6174 2853  RADIUS = float(S
-0000cba0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000cbb0: 6c66 2e72 6164 6975 735f 6b65 7929 290d  lf.radius_key)).
-0000cbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cbd0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
-0000cbe0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000cbf0: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
-0000cc00: 6c69 7479 5f6b 6579 2929 0d0a 2020 2020  lity_key))..    
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 7465 7374 6c6f 6361 7469 6f6e      testlocation
-0000cc30: 203d 2028 666c 6f61 7428 5370 6f74 6f62   = (float(Spotob
-0000cc40: 6a65 6374 2e67 6574 2873 656c 662e 7a70  ject.get(self.zp
-0000cc50: 6f73 6964 5f6b 6579 2929 2c20 666c 6f61  osid_key)), floa
-0000cc60: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000cc70: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
-0000cc80: 2929 2c20 2066 6c6f 6174 2853 706f 746f  )),  float(Spoto
-0000cc90: 626a 6563 742e 6765 7428 7365 6c66 2e78  bject.get(self.x
-0000cca0: 706f 7369 645f 6b65 7929 2929 0d0a 2020  posid_key)))..  
-0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 2020 2020 2020 6672 616d 6520 3d20 5370        frame = Sp
-0000ccd0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000cce0: 662e 6672 616d 6569 645f 6b65 7929 0d0a  f.frameid_key)..
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-0000cd10: 5f63 656c 6c5f 6d61 736b 2c20 6d61 736b  _cell_mask, mask
-0000cd20: 6365 6e74 726f 6964 203d 2073 656c 662e  centroid = self.
-0000cd30: 5f67 6574 5f62 6f75 6e64 6172 795f 6469  _get_boundary_di
-0000cd40: 7374 2866 7261 6d65 2c20 7465 7374 6c6f  st(frame, testlo
-0000cd50: 6361 7469 6f6e 290d 0a20 2020 2020 2020  cation)..       
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000cd80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cd90: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000cda0: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
-0000cdb0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2073 656c 662e 6365 6c6c 6964 5f6b 6579   self.cellid_key
-0000cde0: 3a20 696e 7428 6365 6c6c 5f69 6429 2c20  : int(cell_id), 
-0000cdf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ce10: 6c66 2e66 7261 6d65 6964 5f6b 6579 203a  lf.frameid_key :
-0000ce20: 2069 6e74 2866 6c6f 6174 2853 706f 746f   int(float(Spoto
-0000ce30: 626a 6563 742e 6765 7428 7365 6c66 2e66  bject.get(self.f
-0000ce40: 7261 6d65 6964 5f6b 6579 2929 292c 0d0a  rameid_key))),..
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ce70: 2e7a 706f 7369 645f 6b65 7920 3a20 666c  .zposid_key : fl
-0000ce80: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000ce90: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
-0000cea0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2073 656c 662e 7970 6f73 6964 5f6b     self.yposid_k
-0000ced0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000cee0: 626a 6563 742e 6765 7428 7365 6c66 2e79  bject.get(self.y
-0000cef0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000cf20: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000cf30: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000cf40: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000cf50: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf70: 2073 656c 662e 746f 7461 6c5f 696e 7465   self.total_inte
-0000cf80: 6e73 6974 795f 6b65 7920 3a20 544f 5441  nsity_key : TOTA
-0000cf90: 4c5f 494e 5445 4e53 4954 592c 0d0a 2020  L_INTENSITY,..  
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000cfc0: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
-0000cfd0: 7920 3a20 4d45 414e 5f49 4e54 454e 5349  y : MEAN_INTENSI
-0000cfe0: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d000: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
-0000d010: 203a 2052 4144 4955 532c 0d0a 2020 2020   : RADIUS,..    
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
-0000d040: 6c69 7479 5f6b 6579 203a 2051 5541 4c49  lity_key : QUALI
-0000d050: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
-0000d080: 656c 6c5f 6d61 736b 5f6b 6579 3a20 666c  ell_mask_key: fl
-0000d090: 6f61 7428 6469 7374 616e 6365 5f63 656c  oat(distance_cel
-0000d0a0: 6c5f 6d61 736b 292c 0d0a 2020 2020 2020  l_mask),..      
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-0000d0d0: 656e 7472 6f69 645f 7a5f 6b65 793a 2066  entroid_z_key: f
-0000d0e0: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-0000d0f0: 645b 305d 292c 0d0a 2020 2020 2020 2020  d[0]),..        
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-0000d120: 7472 6f69 645f 795f 6b65 793a 2066 6c6f  troid_y_key: flo
-0000d130: 6174 286d 6173 6b63 656e 7472 6f69 645b  at(maskcentroid[
-0000d140: 315d 292c 0d0a 2020 2020 2020 2020 2020  1]),..          
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-0000d170: 6f69 645f 785f 6b65 793a 2066 6c6f 6174  oid_x_key: float
-0000d180: 286d 6173 6b63 656e 7472 6f69 645b 325d  (maskcentroid[2]
-0000d190: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-0000d1a0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-0000d1b0: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-0000d1c0: 5f67 6574 5f6d 6173 7465 725f 786d 6c5f  _get_master_xml_
-0000d1d0: 6461 7461 2873 656c 6629 3a0d 0a20 2020  data(self):..   
-0000d1e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000d1f0: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-0000d200: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-0000d210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d220: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-0000d230: 6e65 6c5f 786d 6c5f 636f 6e74 656e 7420  nel_xml_content 
-0000d240: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000d250: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-0000d260: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
-0000d270: 6d6c 5f74 7265 6520 3d20 6574 2e70 6172  ml_tree = et.par
-0000d280: 7365 2873 656c 662e 786d 6c5f 7061 7468  se(self.xml_path
-0000d290: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000d2a0: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
-0000d2b0: 6c5f 726f 6f74 203d 2073 656c 662e 786d  l_root = self.xm
-0000d2c0: 6c5f 7472 6565 2e67 6574 726f 6f74 2829  l_tree.getroot()
-0000d2d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d2e0: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-0000d2f0: 6e6e 656c 5f78 6d6c 5f6e 616d 6520 3d20  nnel_xml_name = 
-0000d300: 2773 6563 6f6e 645f 6368 616e 6e65 6c5f  'second_channel_
-0000d310: 2720 2b20 6f73 2e70 6174 682e 7370 6c69  ' + os.path.spli
-0000d320: 7465 7874 286f 732e 7061 7468 2e62 6173  text(os.path.bas
-0000d330: 656e 616d 6528 7365 6c66 2e78 6d6c 5f70  ename(self.xml_p
-0000d340: 6174 6829 295b 305d 202b 2027 2e78 6d6c  ath))[0] + '.xml
-0000d350: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-0000d360: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000d370: 616e 6e65 6c5f 786d 6c5f 7061 7468 203d  annel_xml_path =
-0000d380: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
-0000d390: 2873 656c 662e 786d 6c5f 7061 7468 290d  (self.xml_path).
-0000d3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d3b0: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-0000d3c0: 6174 655f 6368 616e 6e65 6c5f 7472 6565  ate_channel_tree
-0000d3d0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-0000d3e0: 2020 7365 6c66 2e75 6e69 7175 655f 6f62    self.unique_ob
-0000d3f0: 6a65 6374 7320 3d20 7b7d 0d0a 2020 2020  jects = {}..    
-0000d400: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000d410: 7175 655f 7072 6f70 6572 7469 6573 203d  que_properties =
-0000d420: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-0000d430: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000d440: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000d450: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
-0000d460: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
-0000d470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d480: 2e4e 6f72 6d61 6c54 7261 636b 4964 7320  .NormalTrackIds 
-0000d490: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000d4a0: 2020 7365 6c66 2e61 6c6c 5f74 7261 636b    self.all_track
-0000d4b0: 5f70 726f 7065 7274 6965 7320 3d20 5b5d  _properties = []
-0000d4c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d4d0: 6c66 2e73 706c 6974 5f70 6f69 6e74 735f  lf.split_points_
-0000d4e0: 7469 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  times = []....  
-0000d4f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d500: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000d510: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
-0000d520: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000d530: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000d540: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000d550: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000d560: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000d570: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
-0000d580: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000d590: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000d5a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d5b0: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-0000d5c0: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
-0000d5d0: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
-0000d5e0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000d5f0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000d600: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000d610: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d620: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000d630: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000d640: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000d650: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d660: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000d670: 2020 2073 656c 662e 5370 6f74 6f62 6a65     self.Spotobje
-0000d680: 6374 7320 3d20 7365 6c66 2e78 6d6c 5f63  cts = self.xml_c
-0000d690: 6f6e 7465 6e74 2e66 696e 6428 274d 6f64  ontent.find('Mod
-0000d6a0: 656c 2729 2e66 696e 6428 2741 6c6c 5370  el').find('AllSp
-0000d6b0: 6f74 7327 290d 0a20 2020 2020 2020 2020  ots')..         
-0000d6c0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-0000d6d0: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
-0000d6e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d6f0: 6c66 2e74 7261 636b 7320 3d20 7365 6c66  lf.tracks = self
-0000d700: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000d710: 6428 224d 6f64 656c 2229 2e66 696e 6428  d("Model").find(
-0000d720: 2241 6c6c 5472 6163 6b73 2229 0d0a 2020  "AllTracks")..  
-0000d730: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000d740: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
-0000d750: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000d760: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
-0000d770: 2822 496d 6167 6544 6174 6122 290d 0a20  ("ImageData").. 
-0000d780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d790: 7863 616c 6962 7261 7469 6f6e 203d 2066  xcalibration = f
-0000d7a0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000d7b0: 6773 2e67 6574 2822 7069 7865 6c77 6964  gs.get("pixelwid
-0000d7c0: 7468 2229 290d 0a20 2020 2020 2020 2020  th"))..         
-0000d7d0: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
-0000d7e0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000d7f0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000d800: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
-0000d810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d820: 2e7a 6361 6c69 6272 6174 696f 6e20 3d20  .zcalibration = 
-0000d830: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000d840: 6e67 732e 6765 7428 2276 6f78 656c 6465  ngs.get("voxelde
-0000d850: 7074 6822 2929 0d0a 2020 2020 2020 2020  pth"))..        
-0000d860: 2020 2020 7365 6c66 2e74 6361 6c69 6272      self.tcalibr
-0000d870: 6174 696f 6e20 3d20 696e 7428 666c 6f61  ation = int(floa
-0000d880: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000d890: 6765 7428 2274 696d 6569 6e74 6572 7661  get("timeinterva
-0000d8a0: 6c22 2929 290d 0a20 2020 2020 2020 2020  l")))..         
-0000d8b0: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000d8c0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
-0000d8d0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
-0000d8e0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
-0000d8f0: 6428 2244 6574 6563 746f 7253 6574 7469  d("DetectorSetti
-0000d900: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-0000d910: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
-0000d920: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
-0000d930: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
-0000d940: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
-0000d950: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
-0000d960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d970: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000d980: 6c20 3d20 696e 7428 666c 6f61 7428 7365  l = int(float(se
-0000d990: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000d9a0: 6e67 732e 6765 7428 2254 4152 4745 545f  ngs.get("TARGET_
-0000d9b0: 4348 414e 4e45 4c22 2929 290d 0a20 2020  CHANNEL")))..   
-0000d9c0: 2020 2020 2020 2020 2073 656c 662e 7473           self.ts
-0000d9d0: 7461 7274 203d 2069 6e74 2866 6c6f 6174  tart = int(float
-0000d9e0: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
-0000d9f0: 6e67 732e 6765 7428 2274 7374 6172 7422  ngs.get("tstart"
-0000da00: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000da10: 2073 656c 662e 7465 6e64 203d 2069 6e74   self.tend = int
-0000da20: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-0000da30: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-0000da40: 656e 6422 2929 2920 2020 2020 200d 0a0d  end")))      ...
-0000da50: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000da60: 6e74 2827 4974 6572 6174 696e 6720 6f76  nt('Iterating ov
-0000da70: 6572 2073 706f 7473 2069 6e20 6672 616d  er spots in fram
-0000da80: 6527 290d 0a20 2020 2020 2020 2020 2020  e')..           
-0000da90: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
-0000daa0: 0a20 2020 2020 2020 2020 2020 2066 7574  .            fut
-0000dab0: 7572 6573 203d 205b 5d0d 0a0d 0a20 2020  ures = []....   
-0000dac0: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000dad0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000dae0: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-0000daf0: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-0000db00: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000db10: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
-0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000db40: 2020 666f 7220 6672 616d 6520 696e 2073    for frame in s
-0000db50: 656c 662e 5370 6f74 6f62 6a65 6374 732e  elf.Spotobjects.
-0000db60: 6669 6e64 616c 6c28 2753 706f 7473 496e  findall('SpotsIn
-0000db70: 4672 616d 6527 293a 0d0a 2020 2020 2020  Frame'):..      
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
-0000dba0: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
-0000dbb0: 626d 6974 2873 656c 662e 5f6d 6173 7465  bmit(self._maste
-0000dbc0: 725f 7370 6f74 5f63 6f6d 7075 7465 722c  r_spot_computer,
-0000dbd0: 2066 7261 6d65 2929 0d0a 2020 2020 2020   frame))..      
-0000dbe0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000dbf0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-0000dc00: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dc50: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000dc60: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-0000dc70: 7469 6e67 2053 706f 7473 220d 0a20 2020  ting Spots"..   
-0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000dca0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000dcb0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-0000dce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cb90: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2020 2020 2052 4144 4955 5320 3d20 666c       RADIUS = fl
+0000cbc0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000cbd0: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000cbe0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 5155                QU
+0000cc00: 414c 4954 5920 3d20 666c 6f61 7428 5370  ALITY = float(Sp
+0000cc10: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000cc20: 662e 7175 616c 6974 795f 6b65 7929 290d  f.quality_key)).
+0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc40: 2020 2020 2020 2020 2074 6573 746c 6f63           testloc
+0000cc50: 6174 696f 6e20 3d20 2866 6c6f 6174 2853  ation = (float(S
+0000cc60: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000cc70: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000cc80: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000cc90: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000cca0: 645f 6b65 7929 292c 2020 666c 6f61 7428  d_key)),  float(
+0000ccb0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ccc0: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
+0000ccd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000cce0: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+0000ccf0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000cd00: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
+0000cd10: 6579 290d 0a20 2020 2020 2020 2020 2020  ey)..           
+0000cd20: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+0000cd30: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+0000cd40: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
+0000cd50: 7365 6c66 2e5f 6765 745f 626f 756e 6461  self._get_bounda
+0000cd60: 7279 5f64 6973 7428 6672 616d 652c 2074  ry_dist(frame, t
+0000cd70: 6573 746c 6f63 6174 696f 6e29 0d0a 2020  estlocation)..  
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000cdc0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000cdd0: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
+0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdf0: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+0000ce00: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
+0000ce10: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 2020 2073 656c 662e 6672 616d 6569 645f     self.frameid_
+0000ce40: 6b65 7920 3a20 696e 7428 666c 6f61 7428  key : int(float(
+0000ce50: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000ce60: 656c 662e 6672 616d 6569 645f 6b65 7929  elf.frameid_key)
+0000ce70: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2073 656c 662e 7a70 6f73 6964 5f6b 6579   self.zposid_key
+0000cea0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
+0000ceb0: 6563 742e 6765 7428 7365 6c66 2e7a 706f  ect.get(self.zpo
+0000cec0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 2020 2020 2020 2020 7365 6c66 2e79 706f          self.ypo
+0000cef0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000cf00: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000cf10: 656c 662e 7970 6f73 6964 5f6b 6579 2929  elf.yposid_key))
+0000cf20: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cf40: 656c 662e 7870 6f73 6964 5f6b 6579 203a  elf.xposid_key :
+0000cf50: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000cf60: 742e 6765 7428 7365 6c66 2e78 706f 7369  t.get(self.xposi
+0000cf70: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+0000cfa0: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
+0000cfb0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000cfc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cfe0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000cff0: 7479 5f6b 6579 203a 204d 4541 4e5f 494e  ty_key : MEAN_IN
+0000d000: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
+0000d030: 735f 6b65 7920 3a20 5241 4449 5553 2c0d  s_key : RADIUS,.
+0000d040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d050: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d060: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+0000d070: 5155 414c 4954 592c 0d0a 2020 2020 2020  QUALITY,..      
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
+0000d0a0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+0000d0b0: 793a 2066 6c6f 6174 2864 6973 7461 6e63  y: float(distanc
+0000d0c0: 655f 6365 6c6c 5f6d 6173 6b29 2c0d 0a20  e_cell_mask),.. 
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d0f0: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
+0000d100: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+0000d110: 6e74 726f 6964 5b30 5d29 2c0d 0a20 2020  ntroid[0]),..   
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
+0000d140: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
+0000d150: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
+0000d160: 726f 6964 5b31 5d29 2c0d 0a20 2020 2020  roid[1]),..     
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+0000d190: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
+0000d1a0: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+0000d1b0: 6964 5b32 5d29 200d 0a20 2020 2020 2020  id[2]) ..       
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 207d 0d0a 2020 2020 2020 200d 0a20 2020   }..       ..   
+0000d1e0: 2064 6566 205f 6765 745f 6d61 7374 6572   def _get_master
+0000d1f0: 5f78 6d6c 5f64 6174 6128 7365 6c66 293a  _xml_data(self):
+0000d200: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000d210: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000d220: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000d230: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000d240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d250: 2e63 6861 6e6e 656c 5f78 6d6c 5f63 6f6e  .channel_xml_con
+0000d260: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
+0000d270: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d290: 656c 662e 786d 6c5f 7472 6565 203d 2065  elf.xml_tree = e
+0000d2a0: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000d2b0: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d2d0: 6c66 2e78 6d6c 5f72 6f6f 7420 3d20 7365  lf.xml_root = se
+0000d2e0: 6c66 2e78 6d6c 5f74 7265 652e 6765 7472  lf.xml_tree.getr
+0000d2f0: 6f6f 7428 290d 0a20 2020 2020 2020 2020  oot()..         
+0000d300: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d310: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
+0000d320: 6d65 203d 2027 7365 636f 6e64 5f63 6861  me = 'second_cha
+0000d330: 6e6e 656c 5f27 202b 206f 732e 7061 7468  nnel_' + os.path
+0000d340: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
+0000d350: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
+0000d360: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
+0000d370: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
+0000d380: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d390: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000d3a0: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
+0000d3b0: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
+0000d3c0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000d3d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d3e0: 2e5f 6372 6561 7465 5f63 6861 6e6e 656c  ._create_channel
+0000d3f0: 5f74 7265 6528 290d 0a0d 0a20 2020 2020  _tree()....     
+0000d400: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000d410: 7565 5f6f 626a 6563 7473 203d 207b 7d0d  ue_objects = {}.
+0000d420: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d430: 662e 756e 6971 7565 5f70 726f 7065 7274  f.unique_propert
+0000d440: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+0000d450: 2020 2020 2020 7365 6c66 2e41 6c6c 5472        self.AllTr
+0000d460: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000d470: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000d480: 7669 6469 6e67 5472 6163 6b49 6473 203d  vidingTrackIds =
+0000d490: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+0000d4a0: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000d4b0: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000d4c0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0000d4d0: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
+0000d4e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000d4f0: 2020 2073 656c 662e 7370 6c69 745f 706f     self.split_po
+0000d500: 696e 7473 5f74 696d 6573 203d 205b 5d0d  ints_times = [].
+0000d510: 0a0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
+0000d520: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000d530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d540: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000d550: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000d560: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000d570: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000d580: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000d590: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000d5a0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000d5b0: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000d5c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000d5d0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000d5e0: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000d5f0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000d600: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000d610: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
+0000d620: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
+0000d630: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
+0000d640: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+0000d650: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
+0000d660: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
+0000d670: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d680: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d690: 2020 2020 2020 2020 7365 6c66 2e53 706f          self.Spo
+0000d6a0: 746f 626a 6563 7473 203d 2073 656c 662e  tobjects = self.
+0000d6b0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
+0000d6c0: 2827 4d6f 6465 6c27 292e 6669 6e64 2827  ('Model').find('
+0000d6d0: 416c 6c53 706f 7473 2729 0d0a 2020 2020  AllSpots')..    
+0000d6e0: 2020 2020 2020 2020 2320 4578 7472 6163          # Extrac
+0000d6f0: 7420 7468 6520 7472 6163 6b73 2066 726f  t the tracks fro
+0000d700: 6d20 786d 6c0d 0a20 2020 2020 2020 2020  m xml..         
+0000d710: 2020 2073 656c 662e 7472 6163 6b73 203d     self.tracks =
+0000d720: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000d730: 742e 6669 6e64 2822 4d6f 6465 6c22 292e  t.find("Model").
+0000d740: 6669 6e64 2822 416c 6c54 7261 636b 7322  find("AllTracks"
+0000d750: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000d760: 656c 662e 7365 7474 696e 6773 203d 2073  elf.settings = s
+0000d770: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000d780: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000d790: 2e66 696e 6428 2249 6d61 6765 4461 7461  .find("ImageData
+0000d7a0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000d7b0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
+0000d7c0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000d7d0: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000d7e0: 656c 7769 6474 6822 2929 0d0a 2020 2020  elwidth"))..    
+0000d7f0: 2020 2020 2020 2020 7365 6c66 2e79 6361          self.yca
+0000d800: 6c69 6272 6174 696f 6e20 3d20 666c 6f61  libration = floa
+0000d810: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000d820: 6765 7428 2270 6978 656c 6865 6967 6874  get("pixelheight
+0000d830: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
+0000d840: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+0000d850: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
+0000d860: 7365 7474 696e 6773 2e67 6574 2822 766f  settings.get("vo
+0000d870: 7865 6c64 6570 7468 2229 290d 0a20 2020  xeldepth"))..   
+0000d880: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0000d890: 616c 6962 7261 7469 6f6e 203d 2069 6e74  alibration = int
+0000d8a0: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
+0000d8b0: 696e 6773 2e67 6574 2822 7469 6d65 696e  ings.get("timein
+0000d8c0: 7465 7276 616c 2229 2929 0d0a 2020 2020  terval")))..    
+0000d8d0: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000d8e0: 6563 746f 7273 6574 7469 6e67 7320 3d20  ectorsettings = 
+0000d8f0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000d900: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000d910: 292e 6669 6e64 2822 4465 7465 6374 6f72  ).find("Detector
+0000d920: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
+0000d930: 2020 2020 2020 2020 7365 6c66 2e62 6173          self.bas
+0000d940: 6963 7365 7474 696e 6773 203d 2073 656c  icsettings = sel
+0000d950: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000d960: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000d970: 696e 6428 2242 6173 6963 5365 7474 696e  ind("BasicSettin
+0000d980: 6773 2229 0d0a 2020 2020 2020 2020 2020  gs")..          
+0000d990: 2020 7365 6c66 2e64 6574 6563 746f 7263    self.detectorc
+0000d9a0: 6861 6e6e 656c 203d 2069 6e74 2866 6c6f  hannel = int(flo
+0000d9b0: 6174 2873 656c 662e 6465 7465 6374 6f72  at(self.detector
+0000d9c0: 7365 7474 696e 6773 2e67 6574 2822 5441  settings.get("TA
+0000d9d0: 5247 4554 5f43 4841 4e4e 454c 2229 2929  RGET_CHANNEL")))
+0000d9e0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d9f0: 6c66 2e74 7374 6172 7420 3d20 696e 7428  lf.tstart = int(
+0000da00: 666c 6f61 7428 7365 6c66 2e62 6173 6963  float(self.basic
+0000da10: 7365 7474 696e 6773 2e67 6574 2822 7473  settings.get("ts
+0000da20: 7461 7274 2229 2929 0d0a 2020 2020 2020  tart")))..      
+0000da30: 2020 2020 2020 7365 6c66 2e74 656e 6420        self.tend 
+0000da40: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000da50: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
+0000da60: 6574 2822 7465 6e64 2229 2929 2020 2020  et("tend")))    
+0000da70: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000da80: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
+0000da90: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
+0000daa0: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
+0000dab0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+0000dac0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
+0000dad0: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
+0000dae0: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0000daf0: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+0000db00: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+0000db10: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+0000db20: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+0000db30: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+0000db40: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+0000db50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000db60: 2020 2020 2020 2066 6f72 2066 7261 6d65         for frame
+0000db70: 2069 6e20 7365 6c66 2e53 706f 746f 626a   in self.Spotobj
+0000db80: 6563 7473 2e66 696e 6461 6c6c 2827 5370  ects.findall('Sp
+0000db90: 6f74 7349 6e46 7261 6d65 2729 3a0d 0a20  otsInFrame'):.. 
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbb0: 2020 2020 2020 2020 2020 2066 7574 7572             futur
+0000dbc0: 6573 2e61 7070 656e 6428 6578 6563 7574  es.append(execut
+0000dbd0: 6f72 2e73 7562 6d69 7428 7365 6c66 2e5f  or.submit(self._
+0000dbe0: 6d61 7374 6572 5f73 706f 745f 636f 6d70  master_spot_comp
+0000dbf0: 7574 6572 2c20 6672 616d 6529 290d 0a20  uter, frame)).. 
+0000dc00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000dc10: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+0000dc20: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+0000dc30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000dc80: 735f 6261 722e 6c61 6265 6c20 3d20 2243  s_bar.label = "C
+0000dc90: 6f6c 6c65 6374 696e 6720 5370 6f74 7322  ollecting Spots"
+0000dca0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000dcd0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd00: 2020 2020 2020 6c65 6e28 6675 7475 7265        len(future
-0000dd10: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd30: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0000dd00: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+0000dd30: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
 0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000dd60: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-0000dd70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000dd80: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
-0000dd90: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-0000dda0: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-0000ddb0: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dde0: 2e63 6f75 6e74 203d 2073 656c 662e 636f  .count = self.co
-0000ddf0: 756e 7420 2b20 310d 0a20 2020 2020 2020  unt + 1..       
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000de20: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000de30: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000de70: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-0000de80: 3d20 2073 656c 662e 636f 756e 740d 0a20  =  self.count.. 
-0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000deb0: 2020 2072 2e72 6573 756c 7428 2920 2020     r.result()   
-0000dec0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000ded0: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
-0000dee0: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
-0000def0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-0000df00: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
-0000df10: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000df20: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000df30: 2020 2020 2020 2020 2020 2066 7574 7572             futur
-0000df40: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000df50: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000df60: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000df70: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000df80: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-0000df90: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
-0000dfa0: 3d20 2243 6f6c 6c65 6374 696e 6720 5472  = "Collecting Tr
-0000dfb0: 6163 6b73 220d 0a20 2020 2020 2020 2020  acks"..         
-0000dfc0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000dfd0: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-0000dfe0: 2028 302c 206c 656e 2873 656c 662e 6669   (0, len(self.fi
-0000dff0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000e000: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000e010: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e020: 735f 6261 722e 7368 6f77 2829 0d0a 0d0a  s_bar.show()....
-0000e030: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e040: 7472 6163 6b20 696e 2073 656c 662e 7472  track in self.tr
-0000e050: 6163 6b73 2e66 696e 6461 6c6c 2827 5472  acks.findall('Tr
-0000e060: 6163 6b27 293a 0d0a 2020 2020 2020 2020  ack'):..        
-0000e070: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0000e080: 203d 2069 6e74 2874 7261 636b 2e67 6574   = int(track.get
-0000e090: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
-0000e0a0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000e0b0: 2020 2020 2069 6620 7472 6163 6b5f 6964       if track_id
-0000e0c0: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
-0000e0d0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
-0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0f0: 2020 7365 6c66 2e5f 6d61 7374 6572 5f74    self._master_t
-0000e100: 7261 636b 5f63 6f6d 7075 7465 7228 7472  rack_computer(tr
-0000e110: 6163 6b2c 2074 7261 636b 5f69 6429 0d0a  ack, track_id)..
-0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e130: 2020 2020 7365 6c66 2e63 6f75 6e74 202b      self.count +
-0000e140: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
-0000e150: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000e160: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-0000e170: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e190: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e1a0: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
-0000e1b0: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
-0000e1c0: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-0000e1d0: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-0000e1e0: 6973 206e 6f74 204e 6f6e 653a 2020 0d0a  is not None:  ..
-0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e200: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e220: 7365 6c66 2e5f 6372 6561 7465 5f73 6563  self._create_sec
-0000e230: 6f6e 645f 6368 616e 6e65 6c5f 786d 6c28  ond_channel_xml(
-0000e240: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e250: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0000e260: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000e270: 2028 6b2c 7629 2069 6e20 7365 6c66 2e67   (k,v) in self.g
-0000e280: 7261 7068 5f73 706c 6974 2e69 7465 6d73  raph_split.items
-0000e290: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e2c0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000e2d0: 7567 6874 6572 5f74 7261 636b 5f69 6420  ughter_track_id 
-0000e2e0: 3d20 2069 6e74 2866 6c6f 6174 2873 7472  =  int(float(str
-0000e2f0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-0000e300: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-0000e310: 2866 6c6f 6174 286b 2929 5d5b 7365 6c66  (float(k))][self
-0000e320: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
-0000e330: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e340: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000e350: 6172 656e 745f 7472 6163 6b5f 6964 203d  arent_track_id =
-0000e360: 2069 6e74 2866 6c6f 6174 2873 7472 2873   int(float(str(s
-0000e370: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-0000e380: 7072 6f70 6572 7469 6573 5b69 6e74 2866  properties[int(f
-0000e390: 6c6f 6174 2876 2929 5d5b 7365 6c66 2e75  loat(v))][self.u
-0000e3a0: 6e69 7175 6569 645f 6b65 795d 2929 290d  niqueid_key]))).
-0000e3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e3c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e3d0: 662e 6772 6170 685f 7472 6163 6b73 5b64  f.graph_tracks[d
-0000e3e0: 6175 6768 7465 725f 7472 6163 6b5f 6964  aughter_track_id
-0000e3f0: 5d20 3d20 7061 7265 6e74 5f74 7261 636b  ] = parent_track
-0000e400: 5f69 640d 0a0d 0a20 2020 2020 2020 2020  _id....         
-0000e410: 2020 2070 7269 6e74 2827 6765 7474 696e     print('gettin
-0000e420: 6720 6174 7472 6962 7574 6573 2729 2020  g attributes')  
-0000e430: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000e440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e450: 2e5f 6765 745f 6174 7472 6962 7574 6573  ._get_attributes
-0000e460: 2829 0d0a 2020 2020 2020 2020 2020 200d  ()..           .
-0000e470: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e480: 662e 636f 756e 7420 3d20 300d 0a20 2020  f.count = 0..   
-0000e490: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
-0000e4a0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
-0000e4b0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000e4c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4e0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000e4f0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000e500: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e530: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000e540: 6261 722e 6c61 6265 6c20 3d20 224a 7573  bar.label = "Jus
-0000e550: 7420 6f6e 6520 6d6f 7265 2074 6869 6e67  t one more thing
-0000e560: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e590: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
-0000e5a0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5d0: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+0000dd50: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000dd80: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000dd90: 686f 7728 290d 0a0d 0a20 2020 2020 2020  how()....       
+0000dda0: 2020 2020 2020 2020 2066 6f72 2072 2069           for r i
+0000ddb0: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+0000ddc0: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+0000ddd0: 6428 6675 7475 7265 7329 3a0d 0a20 2020  d(futures):..   
+0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de00: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
+0000de10: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de40: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000de50: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000de60: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000de90: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000dea0: 616c 7565 203d 2020 7365 6c66 2e63 6f75  alue =  self.cou
+0000deb0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ded0: 2020 2020 2020 2020 722e 7265 7375 6c74          r.result
+0000dee0: 2829 2020 2020 0d0a 0d0a 2020 2020 2020  ()    ....      
+0000def0: 2020 2020 2020 7072 696e 7428 6627 4974        print(f'It
+0000df00: 6572 6174 696e 6720 6f76 6572 2074 7261  erating over tra
+0000df10: 636b 7320 7b6c 656e 2873 656c 662e 6669  cks {len(self.fi
+0000df20: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000df30: 297d 2729 2020 0d0a 2020 2020 2020 2020  )}')  ..        
+0000df40: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000df50: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+0000df60: 6675 7475 7265 7320 3d20 5b5d 0d0a 2020  futures = []..  
+0000df70: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000df80: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+0000df90: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000dfa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000dfb0: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+0000dfc0: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
+0000dfd0: 6e67 2054 7261 636b 7322 0d0a 2020 2020  ng Tracks"..    
+0000dfe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dff0: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
+0000e000: 6e67 6520 3d20 2830 2c20 6c65 6e28 7365  nge = (0, len(se
+0000e010: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+0000e020: 6b5f 6964 7329 290d 0a20 2020 2020 2020  k_ids))..       
+0000e030: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000e040: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+0000e050: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000e060: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
+0000e070: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
+0000e080: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
+0000e090: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000e0a0: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
+0000e0b0: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
+0000e0c0: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
+0000e0d0: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+0000e0e0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+0000e0f0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+0000e100: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e110: 2020 2020 2020 2073 656c 662e 5f6d 6173         self._mas
+0000e120: 7465 725f 7472 6163 6b5f 636f 6d70 7574  ter_track_comput
+0000e130: 6572 2874 7261 636b 2c20 7472 6163 6b5f  er(track, track_
+0000e140: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+0000e150: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000e160: 756e 7420 2b3d 2031 0d0a 2020 2020 2020  unt += 1..      
+0000e170: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e180: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000e190: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000e1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1b0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000e1c0: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+0000e1d0: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+0000e1e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e1f0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+0000e200: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+0000e210: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+0000e220: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e240: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+0000e250: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
+0000e260: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000e290: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+0000e2a0: 656c 662e 6772 6170 685f 7370 6c69 742e  elf.graph_split.
+0000e2b0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2f0: 2020 2064 6175 6768 7465 725f 7472 6163     daughter_trac
+0000e300: 6b5f 6964 203d 2020 696e 7428 666c 6f61  k_id =  int(floa
+0000e310: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
+0000e320: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e330: 735b 696e 7428 666c 6f61 7428 6b29 295d  s[int(float(k))]
+0000e340: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
+0000e350: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 2020 2020 7061 7265 6e74 5f74 7261 636b      parent_track
+0000e380: 5f69 6420 3d20 696e 7428 666c 6f61 7428  _id = int(float(
+0000e390: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+0000e3a0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000e3b0: 696e 7428 666c 6f61 7428 7629 295d 5b73  int(float(v))][s
+0000e3c0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000e3d0: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3f0: 2020 7365 6c66 2e67 7261 7068 5f74 7261    self.graph_tra
+0000e400: 636b 735b 6461 7567 6874 6572 5f74 7261  cks[daughter_tra
+0000e410: 636b 5f69 645d 203d 2070 6172 656e 745f  ck_id] = parent_
+0000e420: 7472 6163 6b5f 6964 0d0a 0d0a 2020 2020  track_id....    
+0000e430: 2020 2020 2020 2020 7072 696e 7428 2767          print('g
+0000e440: 6574 7469 6e67 2061 7474 7269 6275 7465  etting attribute
+0000e450: 7327 2920 2020 2020 2020 2020 2020 2020  s')             
+0000e460: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e470: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
+0000e480: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
+0000e490: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000e4a0: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
+0000e4b0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000e4c0: 7220 7472 6163 6b5f 6964 2069 6e20 7365  r track_id in se
+0000e4d0: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+0000e4e0: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e510: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000e520: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000e560: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+0000e570: 2022 4a75 7374 206f 6e65 206d 6f72 6520   "Just one more 
+0000e580: 7468 696e 6722 0d0a 2020 2020 2020 2020  thing"..        
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5b0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000e5c0: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
-0000e610: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000e620: 6163 6b5f 6964 7329 2c0d 0a20 2020 2020  ack_ids),..     
-0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000e5f0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
+0000e600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 206c 656e 2873 656c 662e 6669 6c74 6572   len(self.filter
+0000e640: 6564 5f74 7261 636b 5f69 6473 292c 0d0a  ed_track_ids),..
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e680: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000e690: 6261 722e 7368 6f77 2829 0d0a 2020 2020  bar.show()..    
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6c0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000e6d0: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
-0000e6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e700: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000e710: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-0000e720: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
-0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e750: 2020 2073 656c 662e 5f66 696e 616c 5f74     self._final_t
-0000e760: 7261 636b 7328 7472 6163 6b5f 6964 2920  racks(track_id) 
-0000e770: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000e780: 6966 2073 656c 662e 666f 7572 6965 723a  if self.fourier:
-0000e790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e7a0: 2020 2020 2070 7269 6e74 2827 636f 6d70       print('comp
-0000e7b0: 7574 696e 6720 466f 7572 6965 7227 290d  uting Fourier').
-0000e7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e7d0: 2020 2020 7365 6c66 2e5f 636f 6d70 7574      self._comput
-0000e7e0: 655f 7068 656e 6f74 7970 6573 2829 2020  e_phenotypes()  
-0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e810: 2020 2020 7365 6c66 2e5f 7465 6d70 6f72      self._tempor
-0000e820: 616c 5f70 6c6f 7473 5f74 7261 636b 6d61  al_plots_trackma
-0000e830: 7465 2829 2020 2020 2020 2020 0d0a 0d0a  te()        ....
-0000e840: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
-0000e850: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
-0000e860: 5f78 6d6c 2873 656c 6629 3a0d 0a20 2020  _xml(self):..   
-0000e870: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e880: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000e890: 696e 7428 2754 7261 6e73 6665 7272 696e  int('Transferrin
-0000e8a0: 6720 584d 4c27 2920 2020 0d0a 2020 2020  g XML')   ..    
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 6368 616e 6e65 6c5f 6669 6c74 6572 6564  channel_filtered
-0000e8d0: 5f74 7261 636b 7320 3d20 5b5d 2020 2020  _tracks = []    
-0000e8e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000e900: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
-0000e910: 7365 6c66 2e78 6d6c 5f72 6f6f 742e 6974  self.xml_root.it
-0000e920: 6572 2827 5370 6f74 2729 3a0d 0a20 2020  er('Spot'):..   
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e940: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
-0000e950: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
-0000e960: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
-0000e970: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
-0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e990: 2020 2020 2069 6620 6365 6c6c 5f69 6420       if cell_id 
-0000e9a0: 696e 2073 656c 662e 6368 616e 6e65 6c5f  in self.channel_
-0000e9b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000e9c0: 6572 7469 6573 2e6b 6579 7328 293a 2020  erties.keys():  
-0000e9d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000e670: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000e6b0: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
+0000e6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000e6f0: 756e 7420 3d20 7365 6c66 2e63 6f75 6e74  unt = self.count
+0000e700: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e720: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e730: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+0000e740: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
+0000e750: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 2020 7365 6c66 2e5f 6669          self._fi
+0000e780: 6e61 6c5f 7472 6163 6b73 2874 7261 636b  nal_tracks(track
+0000e790: 5f69 6429 200d 0a0d 0a20 2020 2020 2020  _id) ....       
+0000e7a0: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
+0000e7b0: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
+0000e7c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000e7d0: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
+0000e7e0: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
+0000e7f0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+0000e800: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
+0000e810: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
+0000e820: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000e830: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+0000e840: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
+0000e850: 6163 6b6d 6174 6528 2920 2020 2020 2020  ackmate()       
+0000e860: 200d 0a0d 0a0d 0a20 2020 2064 6566 205f   ......    def _
+0000e870: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
+0000e880: 616e 6e65 6c5f 786d 6c28 7365 6c66 293a  annel_xml(self):
+0000e890: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8b0: 2020 2070 7269 6e74 2827 5472 616e 7366     print('Transf
+0000e8c0: 6572 7269 6e67 2058 4d4c 2729 2020 200d  erring XML')   .
+0000e8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e8e0: 2020 2020 2063 6861 6e6e 656c 5f66 696c       channel_fil
+0000e8f0: 7465 7265 645f 7472 6163 6b73 203d 205b  tered_tracks = [
+0000e900: 5d20 2020 2020 2020 2020 2020 200d 0a20  ]            .. 
+0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e920: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
+0000e930: 7420 696e 2073 656c 662e 786d 6c5f 726f  t in self.xml_ro
+0000e940: 6f74 2e69 7465 7228 2753 706f 7427 293a  ot.iter('Spot'):
+0000e950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e960: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+0000e970: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
+0000e980: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000e990: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 2020 2020 6966 2063 656c            if cel
+0000e9c0: 6c5f 6964 2069 6e20 7365 6c66 2e63 6861  l_id in self.cha
+0000e9d0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000e9e0: 5f70 726f 7065 7274 6965 732e 6b65 7973  _properties.keys
+0000e9f0: 2829 3a20 2020 2020 2020 200d 0a20 2020  ():        ..   
 0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 2020 2020 2020 2020 2020 6e65 775f 706f            new_po
-0000ea20: 7369 7469 6f6e 7820 3d20 2073 656c 662e  sitionx =  self.
-0000ea30: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000ea40: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000ea50: 656c 6c5f 6964 5d5b 7365 6c66 2e78 706f  ell_id][self.xpo
-0000ea60: 7369 645f 6b65 795d 0d0a 2020 2020 2020  sid_key]..      
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000ea90: 775f 706f 7369 7469 6f6e 7920 3d20 2073  w_positiony =  s
-0000eaa0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000eab0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000eac0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
-0000ead0: 2e79 706f 7369 645f 6b65 795d 0d0a 2020  .yposid_key]..  
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb00: 2020 6e65 775f 706f 7369 7469 6f6e 7a20    new_positionz 
-0000eb10: 3d20 2073 656c 662e 6368 616e 6e65 6c5f  =  self.channel_
-0000eb20: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000eb30: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000eb40: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-0000eb50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2020 2020 2020 2020 6e65 775f 746f 7461          new_tota
-0000eb80: 6c5f 696e 7465 6e73 6974 7920 3d20 7365  l_intensity = se
-0000eb90: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-0000eba0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000ebb0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
-0000ebc0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000ebd0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebf0: 2020 2020 2020 2020 2020 6e65 775f 6d65            new_me
-0000ec00: 616e 5f69 6e74 656e 7369 7479 203d 2073  an_intensity = s
-0000ec10: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-0000ec20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000ec30: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
-0000ec40: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000ec50: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000ec80: 7261 6469 7573 203d 2073 656c 662e 6368  radius = self.ch
-0000ec90: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000eca0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000ecb0: 6c5f 6964 5d5b 7365 6c66 2e72 6164 6975  l_id][self.radiu
-0000ecc0: 735f 6b65 795d 0d0a 2020 2020 2020 2020  s_key]..        
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000ecf0: 7175 616c 6974 7920 3d20 7365 6c66 2e63  quality = self.c
-0000ed00: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
-0000ed10: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000ed20: 6c6c 5f69 645d 5b73 656c 662e 7175 616c  ll_id][self.qual
-0000ed30: 6974 795f 6b65 795d 0d0a 2020 2020 2020  ity_key]..      
-0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed50: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000ed60: 775f 6469 7374 616e 6365 5f63 656c 6c5f  w_distance_cell_
-0000ed70: 6d61 736b 203d 2073 656c 662e 6368 616e  mask = self.chan
-0000ed80: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000ed90: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000eda0: 6964 5d5b 7365 6c66 2e64 6973 7461 6e63  id][self.distanc
-0000edb0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 795d  e_cell_mask_key]
-0000edc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ede0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000edf0: 6374 2e73 6574 2873 656c 662e 7870 6f73  ct.set(self.xpos
-0000ee00: 6964 5f6b 6579 2c20 7374 7228 6e65 775f  id_key, str(new_
-0000ee10: 706f 7369 7469 6f6e 7829 2920 2020 2020  positionx))     
-0000ee20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ee30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee40: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
-0000ee50: 2e73 6574 2873 656c 662e 7970 6f73 6964  .set(self.yposid
-0000ee60: 5f6b 6579 2c20 7374 7228 6e65 775f 706f  _key, str(new_po
-0000ee70: 7369 7469 6f6e 7929 290d 0a20 2020 2020  sitiony))..     
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000eea0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000eeb0: 6c66 2e7a 706f 7369 645f 6b65 792c 2073  lf.zposid_key, s
-0000eec0: 7472 286e 6577 5f70 6f73 6974 696f 6e7a  tr(new_positionz
-0000eed0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eef0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000ef00: 6a65 6374 2e73 6574 2873 656c 662e 746f  ject.set(self.to
-0000ef10: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000ef20: 792c 2073 7472 286e 6577 5f74 6f74 616c  y, str(new_total
-0000ef30: 5f69 6e74 656e 7369 7479 2929 2020 2020  _intensity))    
-0000ef40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef60: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000ef70: 742e 7365 7428 7365 6c66 2e6d 6561 6e5f  t.set(self.mean_
-0000ef80: 696e 7465 6e73 6974 795f 6b65 792c 2073  intensity_key, s
-0000ef90: 7472 286e 6577 5f6d 6561 6e5f 696e 7465  tr(new_mean_inte
-0000efa0: 6e73 6974 7929 290d 0a20 2020 2020 2020  nsity))..       
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000efd0: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000efe0: 2e72 6164 6975 735f 6b65 792c 2073 7472  .radius_key, str
-0000eff0: 286e 6577 5f72 6164 6975 7329 2920 2020  (new_radius))   
-0000f000: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000f030: 6374 2e73 6574 2873 656c 662e 7175 616c  ct.set(self.qual
-0000f040: 6974 795f 6b65 792c 2073 7472 286e 6577  ity_key, str(new
-0000f050: 5f71 7561 6c69 7479 2929 0d0a 2020 2020  _quality))..    
-0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000f090: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
-0000f0a0: 6c5f 6d61 736b 5f6b 6579 2c20 7374 7228  l_mask_key, str(
-0000f0b0: 6e65 775f 6469 7374 616e 6365 5f63 656c  new_distance_cel
-0000f0c0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000f0f0: 6163 6b5f 6964 203d 2073 656c 662e 6368  ack_id = self.ch
-0000f100: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000f110: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-0000f120: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-0000f130: 7472 6163 6b69 645f 6b65 795d 0d0a 2020  trackid_key]..  
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f160: 2020 6368 616e 6e65 6c5f 6669 6c74 6572    channel_filter
-0000f170: 6564 5f74 7261 636b 732e 6170 7065 6e64  ed_tracks.append
-0000f180: 2874 7261 636b 5f69 6429 0d0a 2020 2020  (track_id)..    
-0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f1c0: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
-0000f1d0: 7265 652e 7772 6974 6528 6f73 2e70 6174  ree.write(os.pat
-0000f1e0: 682e 6a6f 696e 2873 656c 662e 6368 616e  h.join(self.chan
-0000f1f0: 6e65 6c5f 786d 6c5f 7061 7468 2c20 7365  nel_xml_path, se
-0000f200: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f6e  lf.channel_xml_n
-0000f210: 616d 6529 2920 0d0a 0d0a 2020 2020 6465  ame)) ....    de
-0000f220: 6620 5f67 6574 5f78 6d6c 5f64 6174 6128  f _get_xml_data(
-0000f230: 7365 6c66 293a 0d0a 0d0a 2020 2020 2020  self):....      
-0000f240: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-0000f250: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000f260: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-0000f270: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-0000f280: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000f290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f2a0: 2e63 6861 6e6e 656c 5f78 6d6c 5f63 6f6e  .channel_xml_con
-0000f2b0: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
-0000f2c0: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
-0000f2d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f2e0: 656c 662e 786d 6c5f 7472 6565 203d 2065  elf.xml_tree = e
-0000f2f0: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
-0000f300: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f310: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f320: 6c66 2e78 6d6c 5f72 6f6f 7420 3d20 7365  lf.xml_root = se
-0000f330: 6c66 2e78 6d6c 5f74 7265 652e 6765 7472  lf.xml_tree.getr
-0000f340: 6f6f 7428 290d 0a20 2020 2020 2020 2020  oot()..         
-0000f350: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f360: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
-0000f370: 6d65 203d 2027 7365 636f 6e64 5f63 6861  me = 'second_cha
-0000f380: 6e6e 656c 5f27 202b 206f 732e 7061 7468  nnel_' + os.path
-0000f390: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
-0000f3a0: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
-0000f3b0: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
-0000f3c0: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f3e0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
-0000f3f0: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
-0000f400: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
-0000f410: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-0000f420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f430: 2e5f 6372 6561 7465 5f63 6861 6e6e 656c  ._create_channel
-0000f440: 5f74 7265 6528 290d 0a20 2020 2020 2020  _tree()..       
-0000f450: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000f460: 2e61 7574 6f65 6e63 6f64 6572 5f6d 6f64  .autoencoder_mod
-0000f470: 656c 2069 7320 6e6f 7420 4e6f 6e65 2061  el is not None a
-0000f480: 6e64 2073 656c 662e 7365 675f 696d 6167  nd self.seg_imag
-0000f490: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4b0: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-0000f4c0: 6572 5f78 6d6c 5f63 6f6e 7465 6e74 203d  er_xml_content =
-0000f4d0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000f4e0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-0000f4f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-0000f500: 6173 7465 725f 786d 6c5f 7472 6565 203d  aster_xml_tree =
-0000f510: 2065 742e 7061 7273 6528 7365 6c66 2e78   et.parse(self.x
-0000f520: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
-0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f540: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-0000f550: 5f72 6f6f 7420 3d20 7365 6c66 2e6d 6173  _root = self.mas
-0000f560: 7465 725f 786d 6c5f 7472 6565 2e67 6574  ter_xml_tree.get
-0000f570: 726f 6f74 2829 0d0a 2020 2020 2020 2020  root()..        
-0000f580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f590: 656c 662e 6d61 7374 6572 5f78 6d6c 5f6e  elf.master_xml_n
-0000f5a0: 616d 6520 3d20 276d 6173 7465 725f 2720  ame = 'master_' 
-0000f5b0: 2b20 7365 6c66 2e6d 6173 7465 725f 6578  + self.master_ex
-0000f5c0: 7472 615f 6e61 6d65 2020 2b20 6f73 2e70  tra_name  + os.p
-0000f5d0: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
-0000f5e0: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
-0000f5f0: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
-0000f600: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f620: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
-0000f630: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
-0000f640: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
-0000f650: 6c5f 7061 7468 2920 2020 2020 200d 0a20  l_path)      .. 
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f670: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000f680: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000f690: 7175 655f 6f62 6a65 6374 7320 3d20 7b7d  que_objects = {}
-0000f6a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f6b0: 2020 7365 6c66 2e75 6e69 7175 655f 7072    self.unique_pr
-0000f6c0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f6e0: 656c 662e 416c 6c54 7261 636b 4964 7320  elf.AllTrackIds 
-0000f6f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000f700: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-0000f710: 696e 6754 7261 636b 4964 7320 3d20 5b5d  ingTrackIds = []
-0000f720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f730: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
-0000f740: 636b 4964 7320 3d20 5b5d 0d0a 2020 2020  ckIds = []..    
-0000f750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f760: 2e61 6c6c 5f74 7261 636b 5f70 726f 7065  .all_track_prope
-0000f770: 7274 6965 7320 3d20 5b5d 0d0a 2020 2020  rties = []..    
-0000f780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f790: 2e73 706c 6974 5f70 6f69 6e74 735f 7469  .split_points_ti
-0000f7a0: 6d65 7320 3d20 5b5d 0d0a 0d0a 2020 2020  mes = []....    
-0000f7b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000f7c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7e0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-0000f7f0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
-0000f800: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f810: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
-0000f820: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
-0000f830: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f840: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000f850: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000f860: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000f870: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000f880: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-0000f890: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
-0000f8a0: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
-0000f8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f8c0: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000f8d0: 6163 6b49 6473 2e61 7070 656e 6428 7365  ackIds.append(se
-0000f8e0: 6c66 2e54 7261 636b 6964 426f 7829 0d0a  lf.TrackidBox)..
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000f910: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000f920: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000f930: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000f940: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f960: 2073 656c 662e 5370 6f74 6f62 6a65 6374   self.Spotobject
-0000f970: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000f980: 7465 6e74 2e66 696e 6428 274d 6f64 656c  tent.find('Model
-0000f990: 2729 2e66 696e 6428 2741 6c6c 5370 6f74  ').find('AllSpot
-0000f9a0: 7327 290d 0a20 2020 2020 2020 2020 2020  s')..           
-0000f9b0: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
-0000f9c0: 6865 2074 7261 636b 7320 6672 6f6d 2078  he tracks from x
-0000f9d0: 6d6c 0d0a 2020 2020 2020 2020 2020 2020  ml..            
-0000f9e0: 2020 2020 7365 6c66 2e74 7261 636b 7320      self.tracks 
-0000f9f0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000fa00: 6e74 2e66 696e 6428 224d 6f64 656c 2229  nt.find("Model")
-0000fa10: 2e66 696e 6428 2241 6c6c 5472 6163 6b73  .find("AllTracks
-0000fa20: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0000fa30: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000fa40: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000fa50: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
-0000fa60: 6e67 7322 292e 6669 6e64 2822 496d 6167  ngs").find("Imag
-0000fa70: 6544 6174 6122 290d 0a20 2020 2020 2020  eData")..       
-0000fa80: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-0000fa90: 6167 6573 697a 6520 3d20 2869 6e74 2866  agesize = (int(f
-0000faa0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000fab0: 6773 2e67 6574 2822 6e66 7261 6d65 7322  gs.get("nframes"
-0000fac0: 2929 292c 696e 7428 666c 6f61 7428 7365  ))),int(float(se
-0000fad0: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000fae0: 226e 736c 6963 6573 2229 2929 2c69 6e74  "nslices"))),int
-0000faf0: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
-0000fb00: 696e 6773 2e67 6574 2822 6865 6967 6874  ings.get("height
-0000fb10: 2229 2929 2c20 2069 6e74 2866 6c6f 6174  "))),  int(float
-0000fb20: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000fb30: 6574 2822 7769 6474 6822 2929 2929 0d0a  et("width"))))..
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 7072 696e 7428 6627 584d 4c20 6669 6c65  print(f'XML file
-0000fb60: 206d 6164 6520 7573 696e 6720 696d 6167   made using imag
-0000fb70: 6520 6f66 207b 7365 6c66 2e69 6d61 6765  e of {self.image
-0000fb80: 7369 7a65 7d27 290d 0a20 2020 2020 2020  size}')..       
-0000fb90: 2020 2020 2020 2020 2073 656c 662e 7863           self.xc
-0000fba0: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
-0000fbb0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000fbc0: 2e67 6574 2822 7069 7865 6c77 6964 7468  .get("pixelwidth
-0000fbd0: 2229 290d 0a20 2020 2020 2020 2020 2020  "))..           
-0000fbe0: 2020 2020 2073 656c 662e 7963 616c 6962       self.ycalib
-0000fbf0: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000fc00: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000fc10: 2822 7069 7865 6c68 6569 6768 7422 2929  ("pixelheight"))
-0000fc20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fc30: 2020 7365 6c66 2e7a 6361 6c69 6272 6174    self.zcalibrat
-0000fc40: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
-0000fc50: 2e73 6574 7469 6e67 732e 6765 7428 2276  .settings.get("v
-0000fc60: 6f78 656c 6465 7074 6822 2929 0d0a 2020  oxeldepth"))..  
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fc80: 6c66 2e74 6361 6c69 6272 6174 696f 6e20  lf.tcalibration 
-0000fc90: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
-0000fca0: 2e73 6574 7469 6e67 732e 6765 7428 2274  .settings.get("t
-0000fcb0: 696d 6569 6e74 6572 7661 6c22 2929 290d  imeinterval"))).
-0000fcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fcd0: 2073 656c 662e 6465 7465 6374 6f72 7365   self.detectorse
-0000fce0: 7474 696e 6773 203d 2073 656c 662e 786d  ttings = self.xm
-0000fcf0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
-0000fd00: 5365 7474 696e 6773 2229 2e66 696e 6428  Settings").find(
-0000fd10: 2244 6574 6563 746f 7253 6574 7469 6e67  "DetectorSetting
-0000fd20: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000fd30: 2020 2020 2073 656c 662e 6261 7369 6373       self.basics
-0000fd40: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
-0000fd50: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000fd60: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
-0000fd70: 2822 4261 7369 6353 6574 7469 6e67 7322  ("BasicSettings"
-0000fd80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fd90: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000fda0: 6368 616e 6e65 6c20 3d20 696e 7428 666c  channel = int(fl
-0000fdb0: 6f61 7428 7365 6c66 2e64 6574 6563 746f  oat(self.detecto
-0000fdc0: 7273 6574 7469 6e67 732e 6765 7428 2254  rsettings.get("T
-0000fdd0: 4152 4745 545f 4348 414e 4e45 4c22 2929  ARGET_CHANNEL"))
-0000fde0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fdf0: 2020 2073 656c 662e 7473 7461 7274 203d     self.tstart =
-0000fe00: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
-0000fe10: 6261 7369 6373 6574 7469 6e67 732e 6765  basicsettings.ge
-0000fe20: 7428 2274 7374 6172 7422 2929 290d 0a20  t("tstart"))).. 
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fe40: 656c 662e 7465 6e64 203d 2069 6e74 2866  elf.tend = int(f
-0000fe50: 6c6f 6174 2873 656c 662e 6261 7369 6373  loat(self.basics
-0000fe60: 6574 7469 6e67 732e 6765 7428 2274 656e  ettings.get("ten
-0000fe70: 6422 2929 290d 0a20 2020 2020 2020 2020  d")))..         
-0000fe80: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-0000fe90: 5f62 6f75 6e64 6172 795f 706f 696e 7473  _boundary_points
-0000fea0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000feb0: 2020 2020 7072 696e 7428 2749 7465 7261      print('Itera
-0000fec0: 7469 6e67 206f 7665 7220 7370 6f74 7320  ting over spots 
-0000fed0: 696e 2066 7261 6d65 2729 0d0a 2020 2020  in frame')..    
-0000fee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fef0: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
-0000ff00: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000ff10: 7265 7320 3d20 5b5d 0d0a 0d0a 2020 2020  res = []....    
-0000ff20: 2020 2020 2020 2020 2020 2020 7769 7468              with
-0000ff30: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-0000ff40: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
-0000ff50: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
-0000ff60: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
-0000ff70: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
-0000ff80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ff90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000ffa0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000ffb0: 2066 7261 6d65 2069 6e20 7365 6c66 2e53   frame in self.S
-0000ffc0: 706f 746f 626a 6563 7473 2e66 696e 6461  potobjects.finda
-0000ffd0: 6c6c 2827 5370 6f74 7349 6e46 7261 6d65  ll('SpotsInFrame
-0000ffe0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010000: 2020 6675 7475 7265 732e 6170 7065 6e64    futures.append
-00010010: 2865 7865 6375 746f 722e 7375 626d 6974  (executor.submit
-00010020: 2873 656c 662e 5f73 706f 745f 636f 6d70  (self._spot_comp
-00010030: 7574 6572 2c20 6672 616d 6529 290d 0a20  uter, frame)).. 
-00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010050: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-00010060: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-00010070: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000ea10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000ea40: 6577 5f70 6f73 6974 696f 6e78 203d 2020  ew_positionx =  
+0000ea50: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+0000ea60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000ea70: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
+0000ea80: 662e 7870 6f73 6964 5f6b 6579 5d0d 0a20  f.xposid_key].. 
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eab0: 2020 206e 6577 5f70 6f73 6974 696f 6e79     new_positiony
+0000eac0: 203d 2020 7365 6c66 2e63 6861 6e6e 656c   =  self.channel
+0000ead0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000eae0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000eaf0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+0000eb00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb20: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
+0000eb30: 696f 6e7a 203d 2020 7365 6c66 2e63 6861  ionz =  self.cha
+0000eb40: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000eb50: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000eb60: 5f69 645d 5b73 656c 662e 7a70 6f73 6964  _id][self.zposid
+0000eb70: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb90: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000eba0: 5f74 6f74 616c 5f69 6e74 656e 7369 7479  _total_intensity
+0000ebb0: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000ebc0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000ebd0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000ebe0: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000ebf0: 7369 7479 5f6b 6579 5d0d 0a20 2020 2020  sity_key]..     
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000ec20: 6577 5f6d 6561 6e5f 696e 7465 6e73 6974  ew_mean_intensit
+0000ec30: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
+0000ec40: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000ec50: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000ec60: 5b73 656c 662e 6d65 616e 5f69 6e74 656e  [self.mean_inten
+0000ec70: 7369 7479 5f6b 6579 5d0d 0a0d 0a20 2020  sity_key]....   
+0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eca0: 206e 6577 5f72 6164 6975 7320 3d20 7365   new_radius = se
+0000ecb0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000ecc0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000ecd0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000ece0: 7261 6469 7573 5f6b 6579 5d0d 0a20 2020  radius_key]..   
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed10: 206e 6577 5f71 7561 6c69 7479 203d 2073   new_quality = s
+0000ed20: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000ed30: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000ed40: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000ed50: 2e71 7561 6c69 7479 5f6b 6579 5d0d 0a20  .quality_key].. 
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed80: 2020 206e 6577 5f64 6973 7461 6e63 655f     new_distance_
+0000ed90: 6365 6c6c 5f6d 6173 6b20 3d20 7365 6c66  cell_mask = self
+0000eda0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000edb0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000edc0: 6365 6c6c 5f69 645d 5b73 656c 662e 6469  cell_id][self.di
+0000edd0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000ede0: 5f6b 6579 5d0d 0a0d 0a20 2020 2020 2020  _key]....       
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000ee10: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000ee20: 2e78 706f 7369 645f 6b65 792c 2073 7472  .xposid_key, str
+0000ee30: 286e 6577 5f70 6f73 6974 696f 6e78 2929  (new_positionx))
+0000ee40: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee60: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000ee70: 626a 6563 742e 7365 7428 7365 6c66 2e79  bject.set(self.y
+0000ee80: 706f 7369 645f 6b65 792c 2073 7472 286e  posid_key, str(n
+0000ee90: 6577 5f70 6f73 6974 696f 6e79 2929 0d0a  ew_positiony))..
+0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eec0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000eed0: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
+0000eee0: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
+0000eef0: 7469 6f6e 7a29 290d 0a0d 0a20 2020 2020  tionz))....     
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef10: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000ef20: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
+0000ef30: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000ef40: 7479 5f6b 6579 2c20 7374 7228 6e65 775f  ty_key, str(new_
+0000ef50: 746f 7461 6c5f 696e 7465 6e73 6974 7929  total_intensity)
+0000ef60: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
+0000ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef80: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000ef90: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000efa0: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
+0000efb0: 6579 2c20 7374 7228 6e65 775f 6d65 616e  ey, str(new_mean
+0000efc0: 5f69 6e74 656e 7369 7479 2929 0d0a 2020  _intensity))..  
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eff0: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000f000: 2873 656c 662e 7261 6469 7573 5f6b 6579  (self.radius_key
+0000f010: 2c20 7374 7228 6e65 775f 7261 6469 7573  , str(new_radius
+0000f020: 2929 2020 2020 200d 0a20 2020 2020 2020  ))     ..       
+0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f040: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000f050: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000f060: 2e71 7561 6c69 7479 5f6b 6579 2c20 7374  .quality_key, st
+0000f070: 7228 6e65 775f 7175 616c 6974 7929 290d  r(new_quality)).
+0000f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0a0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000f0b0: 7365 7428 7365 6c66 2e64 6973 7461 6e63  set(self.distanc
+0000f0c0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 792c  e_cell_mask_key,
+0000f0d0: 2073 7472 286e 6577 5f64 6973 7461 6e63   str(new_distanc
+0000f0e0: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f110: 2020 2074 7261 636b 5f69 6420 3d20 7365     track_id = se
+0000f120: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000f130: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000f140: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+0000f150: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+0000f160: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f180: 2020 2020 2020 2063 6861 6e6e 656c 5f66         channel_f
+0000f190: 696c 7465 7265 645f 7472 6163 6b73 2e61  iltered_tracks.a
+0000f1a0: 7070 656e 6428 7472 6163 6b5f 6964 290d  ppend(track_id).
+0000f1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f1e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f1f0: 786d 6c5f 7472 6565 2e77 7269 7465 286f  xml_tree.write(o
+0000f200: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+0000f210: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000f220: 682c 2073 656c 662e 6368 616e 6e65 6c5f  h, self.channel_
+0000f230: 786d 6c5f 6e61 6d65 2929 200d 0a0d 0a20  xml_name)) .... 
+0000f240: 2020 2064 6566 205f 6765 745f 786d 6c5f     def _get_xml_
+0000f250: 6461 7461 2873 656c 6629 3a0d 0a0d 0a20  data(self):.... 
+0000f260: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000f270: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000f280: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+0000f290: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+0000f2a0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000f2d0: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
+0000f2e0: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
+0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f300: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
+0000f310: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
+0000f320: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
+0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f340: 2020 2073 656c 662e 786d 6c5f 726f 6f74     self.xml_root
+0000f350: 203d 2073 656c 662e 786d 6c5f 7472 6565   = self.xml_tree
+0000f360: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000f390: 6d6c 5f6e 616d 6520 3d20 2773 6563 6f6e  ml_name = 'secon
+0000f3a0: 645f 6368 616e 6e65 6c5f 2720 2b20 6f73  d_channel_' + os
+0000f3b0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+0000f3c0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0000f3d0: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
+0000f3e0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
+0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f400: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000f410: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
+0000f420: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
+0000f430: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
+0000f460: 616e 6e65 6c5f 7472 6565 2829 0d0a 2020  annel_tree()..  
+0000f470: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f480: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
+0000f490: 725f 6d6f 6465 6c20 6973 206e 6f74 204e  r_model is not N
+0000f4a0: 6f6e 6520 616e 6420 7365 6c66 2e73 6567  one and self.seg
+0000f4b0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+0000f4c0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000f4d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f4e0: 2e6d 6173 7465 725f 786d 6c5f 636f 6e74  .master_xml_cont
+0000f4f0: 656e 7420 3d20 7365 6c66 2e78 6d6c 5f63  ent = self.xml_c
+0000f500: 6f6e 7465 6e74 0d0a 2020 2020 2020 2020  ontent..        
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f520: 656c 662e 6d61 7374 6572 5f78 6d6c 5f74  elf.master_xml_t
+0000f530: 7265 6520 3d20 6574 2e70 6172 7365 2873  ree = et.parse(s
+0000f540: 656c 662e 786d 6c5f 7061 7468 290d 0a20  elf.xml_path).. 
+0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f560: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000f570: 725f 786d 6c5f 726f 6f74 203d 2073 656c  r_xml_root = sel
+0000f580: 662e 6d61 7374 6572 5f78 6d6c 5f74 7265  f.master_xml_tre
+0000f590: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5b0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
+0000f5c0: 786d 6c5f 6e61 6d65 203d 2027 6d61 7374  xml_name = 'mast
+0000f5d0: 6572 5f27 202b 2073 656c 662e 6d61 7374  er_' + self.mast
+0000f5e0: 6572 5f65 7874 7261 5f6e 616d 6520 202b  er_extra_name  +
+0000f5f0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
+0000f600: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+0000f610: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
+0000f620: 2929 5b30 5d20 2b20 272e 786d 6c27 0d0a  ))[0] + '.xml'..
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
+0000f650: 6572 5f78 6d6c 5f70 6174 6820 3d20 6f73  er_xml_path = os
+0000f660: 2e70 6174 682e 6469 726e 616d 6528 7365  .path.dirname(se
+0000f670: 6c66 2e78 6d6c 5f70 6174 6829 2020 2020  lf.xml_path)    
+0000f680: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f690: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f6a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f6b0: 662e 756e 6971 7565 5f6f 626a 6563 7473  f.unique_objects
+0000f6c0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+0000f6d0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000f6e0: 7565 5f70 726f 7065 7274 6965 7320 3d20  ue_properties = 
+0000f6f0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000f700: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000f710: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000f720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f730: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000f740: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000f750: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000f760: 616c 5472 6163 6b49 6473 203d 205b 5d0d  alTrackIds = [].
+0000f770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f780: 2073 656c 662e 616c 6c5f 7472 6163 6b5f   self.all_track_
+0000f790: 7072 6f70 6572 7469 6573 203d 205b 5d0d  properties = [].
+0000f7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7b0: 2073 656c 662e 7370 6c69 745f 706f 696e   self.split_poin
+0000f7c0: 7473 5f74 696d 6573 203d 205b 5d0d 0a0d  ts_times = []...
+0000f7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f7f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f800: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000f810: 636b 4964 732e 6170 7065 6e64 284e 6f6e  ckIds.append(Non
+0000f820: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000f830: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000f840: 6754 7261 636b 4964 732e 6170 7065 6e64  gTrackIds.append
+0000f850: 284e 6f6e 6529 0d0a 2020 2020 2020 2020  (None)..        
+0000f860: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
+0000f870: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
+0000f880: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000f890: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f8a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f8b0: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
+0000f8c0: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
+0000f8d0: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
+0000f8e0: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
+0000f8f0: 696e 6754 7261 636b 4964 732e 6170 7065  ingTrackIds.appe
+0000f900: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000f910: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000f920: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000f930: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000f940: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
+0000f950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f960: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f970: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f980: 2020 2020 2020 7365 6c66 2e53 706f 746f        self.Spoto
+0000f990: 626a 6563 7473 203d 2073 656c 662e 786d  bjects = self.xm
+0000f9a0: 6c5f 636f 6e74 656e 742e 6669 6e64 2827  l_content.find('
+0000f9b0: 4d6f 6465 6c27 292e 6669 6e64 2827 416c  Model').find('Al
+0000f9c0: 6c53 706f 7473 2729 0d0a 2020 2020 2020  lSpots')..      
+0000f9d0: 2020 2020 2020 2020 2020 2320 4578 7472            # Extr
+0000f9e0: 6163 7420 7468 6520 7472 6163 6b73 2066  act the tracks f
+0000f9f0: 726f 6d20 786d 6c0d 0a20 2020 2020 2020  rom xml..       
+0000fa00: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000fa10: 6163 6b73 203d 2073 656c 662e 786d 6c5f  acks = self.xml_
+0000fa20: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
+0000fa30: 6465 6c22 292e 6669 6e64 2822 416c 6c54  del").find("AllT
+0000fa40: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
+0000fa50: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000fa60: 7474 696e 6773 203d 2073 656c 662e 786d  ttings = self.xm
+0000fa70: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+0000fa80: 5365 7474 696e 6773 2229 2e66 696e 6428  Settings").find(
+0000fa90: 2249 6d61 6765 4461 7461 2229 0d0a 2020  "ImageData")..  
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fab0: 6c66 2e69 6d61 6765 7369 7a65 203d 2028  lf.imagesize = (
+0000fac0: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
+0000fad0: 6574 7469 6e67 732e 6765 7428 226e 6672  ettings.get("nfr
+0000fae0: 616d 6573 2229 2929 2c69 6e74 2866 6c6f  ames"))),int(flo
+0000faf0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000fb00: 2e67 6574 2822 6e73 6c69 6365 7322 2929  .get("nslices"))
+0000fb10: 292c 696e 7428 666c 6f61 7428 7365 6c66  ),int(float(self
+0000fb20: 2e73 6574 7469 6e67 732e 6765 7428 2268  .settings.get("h
+0000fb30: 6569 6768 7422 2929 292c 2020 696e 7428  eight"))),  int(
+0000fb40: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000fb50: 6e67 732e 6765 7428 2277 6964 7468 2229  ngs.get("width")
+0000fb60: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000fb70: 2020 2020 2070 7269 6e74 2866 2758 4d4c       print(f'XML
+0000fb80: 2066 696c 6520 6d61 6465 2075 7369 6e67   file made using
+0000fb90: 2069 6d61 6765 206f 6620 7b73 656c 662e   image of {self.
+0000fba0: 696d 6167 6573 697a 657d 2729 0d0a 2020  imagesize}')..  
+0000fbb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fbc0: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+0000fbd0: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000fbe0: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
+0000fbf0: 7769 6474 6822 2929 0d0a 2020 2020 2020  width"))..      
+0000fc00: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
+0000fc10: 6361 6c69 6272 6174 696f 6e20 3d20 666c  calibration = fl
+0000fc20: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
+0000fc30: 732e 6765 7428 2270 6978 656c 6865 6967  s.get("pixelheig
+0000fc40: 6874 2229 290d 0a20 2020 2020 2020 2020  ht"))..         
+0000fc50: 2020 2020 2020 2073 656c 662e 7a63 616c         self.zcal
+0000fc60: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000fc70: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000fc80: 6574 2822 766f 7865 6c64 6570 7468 2229  et("voxeldepth")
+0000fc90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fca0: 2020 2073 656c 662e 7463 616c 6962 7261     self.tcalibra
+0000fcb0: 7469 6f6e 203d 2069 6e74 2866 6c6f 6174  tion = int(float
+0000fcc0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000fcd0: 6574 2822 7469 6d65 696e 7465 7276 616c  et("timeinterval
+0000fce0: 2229 2929 0d0a 2020 2020 2020 2020 2020  ")))..          
+0000fcf0: 2020 2020 2020 7365 6c66 2e64 6574 6563        self.detec
+0000fd00: 746f 7273 6574 7469 6e67 7320 3d20 7365  torsettings = se
+0000fd10: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000fd20: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000fd30: 6669 6e64 2822 4465 7465 6374 6f72 5365  find("DetectorSe
+0000fd40: 7474 696e 6773 2229 0d0a 2020 2020 2020  ttings")..      
+0000fd50: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0000fd60: 6173 6963 7365 7474 696e 6773 203d 2073  asicsettings = s
+0000fd70: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000fd80: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000fd90: 2e66 696e 6428 2242 6173 6963 5365 7474  .find("BasicSett
+0000fda0: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
+0000fdb0: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000fdc0: 6563 746f 7263 6861 6e6e 656c 203d 2069  ectorchannel = i
+0000fdd0: 6e74 2866 6c6f 6174 2873 656c 662e 6465  nt(float(self.de
+0000fde0: 7465 6374 6f72 7365 7474 696e 6773 2e67  tectorsettings.g
+0000fdf0: 6574 2822 5441 5247 4554 5f43 4841 4e4e  et("TARGET_CHANN
+0000fe00: 454c 2229 2929 0d0a 2020 2020 2020 2020  EL")))..        
+0000fe10: 2020 2020 2020 2020 7365 6c66 2e74 7374          self.tst
+0000fe20: 6172 7420 3d20 696e 7428 666c 6f61 7428  art = int(float(
+0000fe30: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000fe40: 6773 2e67 6574 2822 7473 7461 7274 2229  gs.get("tstart")
+0000fe50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000fe60: 2020 2020 7365 6c66 2e74 656e 6420 3d20      self.tend = 
+0000fe70: 696e 7428 666c 6f61 7428 7365 6c66 2e62  int(float(self.b
+0000fe80: 6173 6963 7365 7474 696e 6773 2e67 6574  asicsettings.get
+0000fe90: 2822 7465 6e64 2229 2929 0d0a 2020 2020  ("tend")))..    
+0000fea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000feb0: 2e5f 6765 745f 626f 756e 6461 7279 5f70  ._get_boundary_p
+0000fec0: 6f69 6e74 7328 290d 0a20 2020 2020 2020  oints()..       
+0000fed0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000fee0: 4974 6572 6174 696e 6720 6f76 6572 2073  Iterating over s
+0000fef0: 706f 7473 2069 6e20 6672 616d 6527 290d  pots in frame').
+0000ff00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff10: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
+0000ff20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff30: 2066 7574 7572 6573 203d 205b 5d0d 0a0d   futures = []...
+0000ff40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ff50: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+0000ff60: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+0000ff70: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+0000ff80: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+0000ff90: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+0000ffa0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+0000ffb0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffd0: 2020 666f 7220 6672 616d 6520 696e 2073    for frame in s
+0000ffe0: 656c 662e 5370 6f74 6f62 6a65 6374 732e  elf.Spotobjects.
+0000fff0: 6669 6e64 616c 6c28 2753 706f 7473 496e  findall('SpotsIn
+00010000: 4672 616d 6527 293a 0d0a 2020 2020 2020  Frame'):..      
+00010010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010020: 2020 2020 2020 2066 7574 7572 6573 2e61         futures.a
+00010030: 7070 656e 6428 6578 6563 7574 6f72 2e73  ppend(executor.s
+00010040: 7562 6d69 7428 7365 6c66 2e5f 7370 6f74  ubmit(self._spot
+00010050: 5f63 6f6d 7075 7465 722c 2066 7261 6d65  _computer, frame
+00010060: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00010070: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010080: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00010090: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000100c0: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-000100d0: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
-000100e0: 6e67 2053 706f 7473 220d 0a20 2020 2020  ng Spots"..     
-000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010110: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00010120: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
-00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010150: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+000100b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000100c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100e0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000100f0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+00010100: 6c65 6374 696e 6720 5370 6f74 7322 0d0a  lecting Spots"..
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010130: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010140: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
+00010150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010180: 6c65 6e28 6675 7475 7265 7329 2c0d 0a20  len(futures),.. 
+00010170: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+000101a0: 2020 2020 206c 656e 2866 7574 7572 6573       len(futures
+000101b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000101e0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-000101f0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00010200: 2020 2020 2020 2020 2020 666f 7220 7220            for r 
-00010210: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-00010220: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-00010230: 6564 2866 7574 7572 6573 293a 0d0a 2020  ed(futures):..  
-00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-00010270: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-00010280: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000102b0: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-000102c0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010300: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-00010310: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
-00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010340: 2020 2020 2020 2020 722e 7265 7375 6c74          r.result
-00010350: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00010360: 2020 2020 7072 696e 7428 6627 4974 6572      print(f'Iter
-00010370: 6174 696e 6720 6f76 6572 2074 7261 636b  ating over track
-00010380: 7320 7b6c 656e 2873 656c 662e 6669 6c74  s {len(self.filt
-00010390: 6572 6564 5f74 7261 636b 5f69 6473 297d  ered_track_ids)}
-000103a0: 2729 2020 0d0a 2020 2020 2020 2020 2020  ')  ..          
-000103b0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-000103c0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-000103d0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-000103e0: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
-000103f0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00010400: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010410: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-00010420: 6162 656c 203d 2022 436f 6c6c 6563 7469  abel = "Collecti
-00010430: 6e67 2054 7261 636b 7322 0d0a 2020 2020  ng Tracks"..    
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010450: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010460: 722e 7261 6e67 6520 3d20 2830 2c20 6c65  r.range = (0, le
-00010470: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-00010480: 7472 6163 6b5f 6964 7329 290d 0a20 2020  track_ids))..   
-00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104a0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-000104b0: 6172 2e73 686f 7728 290d 0a0d 0a20 2020  ar.show()....   
-000104c0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000104d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000104e0: 6178 5f6c 656e 6774 6820 3d20 3020 2020  ax_length = 0   
-000104f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010500: 2020 2066 6f72 2074 7261 636b 2069 6e20     for track in 
-00010510: 7365 6c66 2e74 7261 636b 732e 6669 6e64  self.tracks.find
-00010520: 616c 6c28 2754 7261 636b 2729 3a0d 0a20  all('Track'):.. 
-00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010540: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
-00010550: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
-00010560: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
-00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010580: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
-00010590: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-000105a0: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105c0: 2020 2020 2020 2020 2064 6967 6974 5f6c           digit_l
-000105d0: 656e 6774 6820 3d20 6c65 6e28 7374 7228  ength = len(str(
-000105e0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 2020 6966 2064 6967 6974          if digit
-00010610: 5f6c 656e 6774 6820 3e20 6d61 785f 6c65  _length > max_le
-00010620: 6e67 7468 3a0d 0a20 2020 2020 2020 2020  ngth:..         
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 2020 2020 2020 206d 6178 5f6c 656e 6774         max_lengt
-00010650: 6820 3d20 6469 6769 745f 6c65 6e67 7468  h = digit_length
-00010660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010670: 2020 7365 6c66 2e6d 6178 5f74 7261 636b    self.max_track
-00010680: 5f64 6967 6974 203d 206d 6178 5f6c 656e  _digit = max_len
-00010690: 6774 6820 2020 2020 2020 2020 2020 2020  gth             
-000106a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000106b0: 2020 2020 2066 6f72 2074 7261 636b 2069       for track i
-000106c0: 6e20 7365 6c66 2e74 7261 636b 732e 6669  n self.tracks.fi
-000106d0: 6e64 616c 6c28 2754 7261 636b 2729 3a0d  ndall('Track'):.
-000106e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000106f0: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-00010700: 696e 7428 7472 6163 6b2e 6765 7428 7365  int(track.get(se
-00010710: 6c66 2e74 7261 636b 6964 5f6b 6579 2929  lf.trackid_key))
-00010720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010730: 2020 2020 2020 6966 2074 7261 636b 5f69        if track_i
-00010740: 6420 696e 2073 656c 662e 6669 6c74 6572  d in self.filter
-00010750: 6564 5f74 7261 636b 5f69 6473 3a0d 0a20  ed_track_ids:.. 
-00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010770: 2020 2020 2020 2073 656c 662e 5f74 7261         self._tra
-00010780: 636b 5f63 6f6d 7075 7465 7228 7472 6163  ck_computer(trac
-00010790: 6b2c 2074 7261 636b 5f69 6429 0d0a 2020  k, track_id)..  
-000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107b0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-000107c0: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-000107d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000107e0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-000107f0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-00010800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010810: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010820: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-00010830: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
-00010840: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00010850: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
-00010860: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
-00010870: 206e 6f74 204e 6f6e 653a 2020 0d0a 2020   not None:  ..  
-00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010890: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-000108a0: 655f 7365 636f 6e64 5f63 6861 6e6e 656c  e_second_channel
-000108b0: 5f78 6d6c 2829 0d0a 2020 2020 2020 2020  _xml()..        
-000108c0: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000108d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000108e0: 286b 2c76 2920 696e 2073 656c 662e 6772  (k,v) in self.gr
-000108f0: 6170 685f 7370 6c69 742e 6974 656d 7328  aph_split.items(
-00010900: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00010910: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00010920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010930: 2020 2020 2020 2020 2020 2020 2064 6175               dau
-00010940: 6768 7465 725f 7472 6163 6b5f 6964 203d  ghter_track_id =
-00010950: 2020 696e 7428 666c 6f61 7428 7374 7228    int(float(str(
-00010960: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00010970: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00010980: 666c 6f61 7428 6b29 295d 5b73 656c 662e  float(k))][self.
-00010990: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
-000109a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000109b0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000109c0: 7265 6e74 5f74 7261 636b 5f69 6420 3d20  rent_track_id = 
-000109d0: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
-000109e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000109f0: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
-00010a00: 6f61 7428 7629 295d 5b73 656c 662e 756e  oat(v))][self.un
-00010a10: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
-00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010a40: 2e67 7261 7068 5f74 7261 636b 735b 6461  .graph_tracks[da
-00010a50: 7567 6874 6572 5f74 7261 636b 5f69 645d  ughter_track_id]
-00010a60: 203d 2070 6172 656e 745f 7472 6163 6b5f   = parent_track_
-00010a70: 6964 0d0a 2020 2020 2020 2020 2020 2020  id..            
-00010a80: 2020 2020 7365 6c66 2e5f 6765 745f 6174      self._get_at
-00010a90: 7472 6962 7574 6573 2829 0d0a 2020 2020  tributes()..    
-00010aa0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00010ab0: 656c 662e 6175 746f 656e 636f 6465 725f  elf.autoencoder_
-00010ac0: 6d6f 6465 6c20 616e 6420 7365 6c66 2e73  model and self.s
-00010ad0: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
-00010ae0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00010af0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00010b00: 696e 7428 2747 6574 7469 6e67 2061 7574  int('Getting aut
-00010b10: 6f65 6e63 6f64 6572 2063 6c6f 7564 7327  oencoder clouds'
-00010b20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010b30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00010b40: 6173 7369 676e 5f63 6c75 7374 6572 5f63  assign_cluster_c
-00010b50: 6c61 7373 2829 0d0a 2020 2020 2020 2020  lass()..        
-00010b60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00010b70: 7269 6e74 2827 4372 6561 7469 6e67 206d  rint('Creating m
-00010b80: 6173 7465 7220 786d 6c27 290d 0a20 2020  aster xml')..   
-00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ba0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
-00010bb0: 5f6d 6173 7465 725f 786d 6c28 290d 0a20  _master_xml().. 
-00010bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010bd0: 656c 662e 636f 756e 7420 3d20 3020 0d0a  elf.count = 0 ..
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 666f 7220 7472 6163 6b5f 6964 2069 6e20  for track_id in 
-00010c00: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-00010c10: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
-00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010c40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00010c50: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
-00010c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010c90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-00010ca0: 203d 2022 4a75 7374 206f 6e65 206d 6f72   = "Just one mor
-00010cb0: 6520 7468 696e 6722 0d0a 2020 2020 2020  e thing"..      
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ce0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010cf0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
-00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00010d30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000101d0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010200: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00010210: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+00010220: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010230: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
+00010240: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
+00010250: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
+00010260: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010290: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+000102a0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+000102b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102d0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+000102e0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+000102f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010310: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010320: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010330: 7661 6c75 6520 3d20 2073 656c 662e 636f  value =  self.co
+00010340: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2020 2020 2020 2020 2020 2020 2072 2e72               r.r
+00010370: 6573 756c 7428 290d 0a20 2020 2020 2020  esult()..       
+00010380: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00010390: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+000103a0: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
+000103b0: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+000103c0: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
+000103d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000103e0: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
+000103f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010400: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+00010410: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010440: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+00010450: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
+00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010470: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010480: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+00010490: 302c 206c 656e 2873 656c 662e 6669 6c74  0, len(self.filt
+000104a0: 6572 6564 5f74 7261 636b 5f69 6473 2929  ered_track_ids))
+000104b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000104c0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+000104d0: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
+000104e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000104f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00010500: 2020 2020 6d61 785f 6c65 6e67 7468 203d      max_length =
+00010510: 2030 2020 2020 0d0a 2020 2020 2020 2020   0    ..        
+00010520: 2020 2020 2020 2020 666f 7220 7472 6163          for trac
+00010530: 6b20 696e 2073 656c 662e 7472 6163 6b73  k in self.tracks
+00010540: 2e66 696e 6461 6c6c 2827 5472 6163 6b27  .findall('Track'
+00010550: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00010560: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+00010570: 203d 2069 6e74 2874 7261 636b 2e67 6574   = int(track.get
+00010580: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
+00010590: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+000105a0: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
+000105b0: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+000105c0: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+000105d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000105e0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+000105f0: 6769 745f 6c65 6e67 7468 203d 206c 656e  git_length = len
+00010600: 2873 7472 2874 7261 636b 5f69 6429 290d  (str(track_id)).
+00010610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010620: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010630: 6469 6769 745f 6c65 6e67 7468 203e 206d  digit_length > m
+00010640: 6178 5f6c 656e 6774 683a 0d0a 2020 2020  ax_length:..    
+00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010660: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+00010670: 6c65 6e67 7468 203d 2064 6967 6974 5f6c  length = digit_l
+00010680: 656e 6774 680d 0a20 2020 2020 2020 2020  ength..         
+00010690: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
+000106a0: 7472 6163 6b5f 6469 6769 7420 3d20 6d61  track_digit = ma
+000106b0: 785f 6c65 6e67 7468 2020 2020 2020 2020  x_length        
+000106c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000106d0: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
+000106e0: 6163 6b20 696e 2073 656c 662e 7472 6163  ack in self.trac
+000106f0: 6b73 2e66 696e 6461 6c6c 2827 5472 6163  ks.findall('Trac
+00010700: 6b27 293a 0d0a 2020 2020 2020 2020 2020  k'):..          
+00010710: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
+00010720: 6964 203d 2069 6e74 2874 7261 636b 2e67  id = int(track.g
+00010730: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
+00010740: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+00010750: 2020 2020 2020 2020 2020 2069 6620 7472             if tr
+00010760: 6163 6b5f 6964 2069 6e20 7365 6c66 2e66  ack_id in self.f
+00010770: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+00010780: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00010790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000107a0: 2e5f 7472 6163 6b5f 636f 6d70 7574 6572  ._track_computer
+000107b0: 2874 7261 636b 2c20 7472 6163 6b5f 6964  (track, track_id
+000107c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000107d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000107e0: 636f 756e 7420 2b3d 2031 0d0a 2020 2020  count += 1..    
+000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010800: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+00010810: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+00010820: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00010830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010840: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+00010850: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
+00010860: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+00010870: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010880: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+00010890: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a20  ge is not None: 
+000108a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000108b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000108c0: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
+000108d0: 616e 6e65 6c5f 786d 6c28 290d 0a20 2020  annel_xml()..   
+000108e0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+000108f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010900: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00010910: 6c66 2e67 7261 7068 5f73 706c 6974 2e69  lf.graph_split.i
+00010920: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010940: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 2020 6461 7567 6874 6572 5f74 7261 636b    daughter_track
+00010970: 5f69 6420 3d20 2069 6e74 2866 6c6f 6174  _id =  int(float
+00010980: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
+00010990: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000109a0: 5b69 6e74 2866 6c6f 6174 286b 2929 5d5b  [int(float(k))][
+000109b0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+000109c0: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 2020 2070 6172 656e 745f 7472 6163 6b5f     parent_track_
+000109f0: 6964 203d 2069 6e74 2866 6c6f 6174 2873  id = int(float(s
+00010a00: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
+00010a10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00010a20: 6e74 2866 6c6f 6174 2876 2929 5d5b 7365  nt(float(v))][se
+00010a30: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
+00010a40: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2073 656c 662e 6772 6170 685f 7472 6163   self.graph_trac
+00010a70: 6b73 5b64 6175 6768 7465 725f 7472 6163  ks[daughter_trac
+00010a80: 6b5f 6964 5d20 3d20 7061 7265 6e74 5f74  k_id] = parent_t
+00010a90: 7261 636b 5f69 640d 0a20 2020 2020 2020  rack_id..       
+00010aa0: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
+00010ab0: 6574 5f61 7474 7269 6275 7465 7328 290d  et_attributes().
+00010ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ad0: 2069 6620 7365 6c66 2e61 7574 6f65 6e63   if self.autoenc
+00010ae0: 6f64 6572 5f6d 6f64 656c 2061 6e64 2073  oder_model and s
+00010af0: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
+00010b00: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b20: 2020 2070 7269 6e74 2827 4765 7474 696e     print('Gettin
+00010b30: 6720 6175 746f 656e 636f 6465 7220 636c  g autoencoder cl
+00010b40: 6f75 6473 2729 0d0a 2020 2020 2020 2020  ouds')..        
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010b60: 656c 662e 5f61 7373 6967 6e5f 636c 7573  elf._assign_clus
+00010b70: 7465 725f 636c 6173 7328 290d 0a20 2020  ter_class()..   
+00010b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b90: 2020 2020 7072 696e 7428 2743 7265 6174      print('Creat
+00010ba0: 696e 6720 6d61 7374 6572 2078 6d6c 2729  ing master xml')
+00010bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010bc0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00010bd0: 7265 6174 655f 6d61 7374 6572 5f78 6d6c  reate_master_xml
+00010be0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00010bf0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00010c00: 2030 200d 0a20 2020 2020 2020 2020 2020   0 ..           
+00010c10: 2020 2020 2066 6f72 2074 7261 636b 5f69       for track_i
+00010c20: 6420 696e 2073 656c 662e 6669 6c74 6572  d in self.filter
+00010c30: 6564 5f74 7261 636b 5f69 6473 3a0d 0a20  ed_track_ids:.. 
+00010c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c60: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+00010c70: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+00010c80: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010cb0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010cc0: 6c61 6265 6c20 3d20 224a 7573 7420 6f6e  label = "Just on
+00010cd0: 6520 6d6f 7265 2074 6869 6e67 220d 0a20  e more thing".. 
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d00: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00010d10: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
+00010d20: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 206c 656e 2873 656c 662e 6669 6c74     len(self.filt
-00010d70: 6572 6564 5f74 7261 636b 5f69 6473 292c  ered_track_ids),
-00010d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010da0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d50: 2020 2020 302c 0d0a 2020 2020 2020 2020      0,..        
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2020 2020 2020 6c65 6e28 7365 6c66          len(self
+00010d90: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+00010da0: 6964 7329 2c0d 0a20 2020 2020 2020 2020  ids),..         
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00010de0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
-00010df0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010e20: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-00010e30: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
-00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010e70: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
-00010e80: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ea0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00010eb0: 6669 6e61 6c5f 7472 6163 6b73 2874 7261  final_tracks(tra
-00010ec0: 636b 5f69 6429 200d 0a0d 0a20 2020 2020  ck_id) ....     
-00010ed0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00010ee0: 6c66 2e66 6f75 7269 6572 3a0d 0a20 2020  lf.fourier:..   
+00010dd0: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010df0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010e00: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010e10: 7368 6f77 2829 0d0a 2020 2020 2020 2020  show()..        
+00010e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+00010e50: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e80: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010e90: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
+00010ea0: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
+00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010ed0: 656c 662e 5f66 696e 616c 5f74 7261 636b  elf._final_track
+00010ee0: 7328 7472 6163 6b5f 6964 2920 0d0a 0d0a  s(track_id) ....
 00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f00: 7072 696e 7428 2763 6f6d 7075 7469 6e67  print('computing
-00010f10: 2046 6f75 7269 6572 2729 0d0a 2020 2020   Fourier')..    
-00010f20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010f30: 656c 662e 5f63 6f6d 7075 7465 5f70 6865  elf._compute_phe
-00010f40: 6e6f 7479 7065 7328 2920 2020 2020 2020  notypes()       
-00010f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010f70: 2020 2073 656c 662e 5f74 656d 706f 7261     self._tempora
-00010f80: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
-00010f90: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00010fa0: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
-00010fb0: 205f 6372 6561 7465 5f6d 6173 7465 725f   _create_master_
-00010fc0: 786d 6c28 7365 6c66 293a 0d0a 2020 2020  xml(self):..    
-00010fd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010fe0: 200d 0a20 2020 2020 2020 2020 2020 666f   ..           fo
-00010ff0: 7220 5370 6f74 6f62 6a65 6374 2069 6e20  r Spotobject in 
-00011000: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-00011010: 726f 6f74 2e69 7465 7228 2753 706f 7427  root.iter('Spot'
-00011020: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
-00011050: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-00011060: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
-00011070: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 6966 2063 656c 6c5f 6964 2069      if cell_id i
-000110a0: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
-000110b0: 6f74 5f70 726f 7065 7274 6965 732e 6b65  ot_properties.ke
-000110c0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00010f00: 6966 2073 656c 662e 666f 7572 6965 723a  if self.fourier:
+00010f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010f20: 2020 2020 2070 7269 6e74 2827 636f 6d70       print('comp
+00010f30: 7574 696e 6720 466f 7572 6965 7227 290d  uting Fourier').
+00010f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f50: 2020 2020 7365 6c66 2e5f 636f 6d70 7574      self._comput
+00010f60: 655f 7068 656e 6f74 7970 6573 2829 2020  e_phenotypes()  
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010f90: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+00010fa0: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
+00010fb0: 636b 6d61 7465 2829 0d0a 2020 2020 2020  ckmate()..      
+00010fc0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00010fd0: 2020 6465 6620 5f63 7265 6174 655f 6d61    def _create_ma
+00010fe0: 7374 6572 5f78 6d6c 2873 656c 6629 3a0d  ster_xml(self):.
+00010ff0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+00011000: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00011010: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
+00011020: 7420 696e 2073 656c 662e 6d61 7374 6572  t in self.master
+00011030: 5f78 6d6c 5f72 6f6f 742e 6974 6572 2827  _xml_root.iter('
+00011040: 5370 6f74 2729 3a0d 0a20 2020 2020 2020  Spot'):..       
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
+00011070: 203d 2069 6e74 2853 706f 746f 626a 6563   = int(Spotobjec
+00011080: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
+00011090: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2020 2020 2020 2020 2069 6620 6365 6c6c           if cell
+000110c0: 5f69 6420 696e 2073 656c 662e 756e 6971  _id in self.uniq
+000110d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000110e0: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
 000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-00011120: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00011130: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-00011140: 5f69 645d 2e6b 6579 7328 293a 0d0a 0d0a  _id].keys():....
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
-00011180: 626a 6563 742e 7365 7428 6b2c 2073 7472  bject.set(k, str
-00011190: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000111a0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-000111b0: 6c5f 6964 5d5b 6b5d 2929 2020 200d 0a0d  l_id][k]))   ...
-000111c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-000111f0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
-00011200: 725f 786d 6c5f 7472 6565 2e77 7269 7465  r_xml_tree.write
-00011210: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
-00011220: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
-00011230: 7468 2c20 7365 6c66 2e6d 6173 7465 725f  th, self.master_
-00011240: 786d 6c5f 6e61 6d65 2929 0d0a 2020 2020  xml_name))..    
-00011250: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011110: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011130: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011140: 6b20 696e 2073 656c 662e 756e 6971 7565  k in self.unique
+00011150: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011160: 5b63 656c 6c5f 6964 5d2e 6b65 7973 2829  [cell_id].keys()
+00011170: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 5370 6f74 6f62 6a65 6374 2e73 6574 286b  Spotobject.set(k
+000111b0: 2c20 7374 7228 7365 6c66 2e75 6e69 7175  , str(self.uniqu
+000111c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000111d0: 735b 6365 6c6c 5f69 645d 5b6b 5d29 2920  s[cell_id][k])) 
+000111e0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000111f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011200: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00011210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011220: 6d61 7374 6572 5f78 6d6c 5f74 7265 652e  master_xml_tree.
+00011230: 7772 6974 6528 6f73 2e70 6174 682e 6a6f  write(os.path.jo
+00011240: 696e 2873 656c 662e 6d61 7374 6572 5f78  in(self.master_x
+00011250: 6d6c 5f70 6174 682c 2073 656c 662e 6d61  ml_path, self.ma
+00011260: 7374 6572 5f78 6d6c 5f6e 616d 6529 290d  ster_xml_name)).
+00011270: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-000112b0: 2064 6566 205f 6173 7369 676e 5f63 6c75   def _assign_clu
-000112c0: 7374 6572 5f63 6c61 7373 2873 656c 6629  ster_class(self)
-000112d0: 3a0d 0a20 2020 2020 2020 2020 2020 0d0a  :..           ..
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 2020 7365 6c66 2e61 7865 7320 3d20      self.axes = 
-00011300: 7365 6c66 2e61 7865 732e 7265 706c 6163  self.axes.replac
-00011310: 6528 2254 222c 2022 2229 0d0a 2020 2020  e("T", "")..    
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011340: 2020 2020 2020 666f 7220 636f 756e 742c        for count,
-00011350: 2074 696d 655f 6b65 7920 696e 2065 6e75   time_key in enu
-00011360: 6d65 7261 7465 2873 656c 662e 5f74 696d  merate(self._tim
-00011370: 6564 5f63 656e 7472 6f69 642e 6b65 7973  ed_centroid.keys
-00011380: 2829 293a 0d0a 2020 2020 2020 2020 2020  ()):..          
-00011390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000113b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000113c0: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
-000113d0: 6473 203d 2073 656c 662e 5f74 696d 6564  ds = self._timed
-000113e0: 5f63 656e 7472 6f69 645b 7469 6d65 5f6b  _centroid[time_k
-000113f0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00011420: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00011430: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00011460: 5f62 6172 2e6c 6162 656c 203d 2022 4175  _bar.label = "Au
-00011470: 746f 656e 636f 6465 7220 666f 7220 7265  toencoder for re
-00011480: 6669 6e69 6e67 2070 6f69 6e74 2063 6c6f  fining point clo
-00011490: 7564 7322 0d0a 2020 2020 2020 2020 2020  uds"..          
-000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-000114c0: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-000114d0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000112b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000112d0: 0d0a 2020 2020 6465 6620 5f61 7373 6967  ..    def _assig
+000112e0: 6e5f 636c 7573 7465 725f 636c 6173 7328  n_cluster_class(
+000112f0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00011300: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011310: 2020 2020 2020 2020 2073 656c 662e 6178           self.ax
+00011320: 6573 203d 2073 656c 662e 6178 6573 2e72  es = self.axes.r
+00011330: 6570 6c61 6365 2822 5422 2c20 2222 290d  eplace("T", "").
+00011340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011350: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011360: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00011370: 6f75 6e74 2c20 7469 6d65 5f6b 6579 2069  ount, time_key i
+00011380: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
+00011390: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+000113a0: 2e6b 6579 7328 2929 3a0d 0a20 2020 2020  .keys()):..     
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 2020 2074 7265 652c 2073 706f 745f 6365     tree, spot_ce
+000113f0: 6e74 726f 6964 7320 3d20 7365 6c66 2e5f  ntroids = self._
+00011400: 7469 6d65 645f 6365 6e74 726f 6964 5b74  timed_centroid[t
+00011410: 696d 655f 6b65 795d 0d0a 2020 2020 2020  ime_key]..      
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+00011440: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+00011450: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00011480: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
+00011490: 3d20 2241 7574 6f65 6e63 6f64 6572 2066  = "Autoencoder f
+000114a0: 6f72 2072 6566 696e 696e 6720 706f 696e  or refining poin
+000114b0: 7420 636c 6f75 6473 220d 0a20 2020 2020  t clouds"..     
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000114e0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+000114f0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
 00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011530: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
 00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-00011560: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
-00011570: 6b65 7973 2829 2920 2b20 312c 0d0a 2020  keys()) + 1,..  
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115b0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011570: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00011580: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+00011590: 726f 6964 2e6b 6579 7328 2929 202b 2031  roid.keys()) + 1
+000115a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000115e0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
-000115f0: 616c 7565 203d 2020 636f 756e 7420 0d0a  alue =  count ..
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011620: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011630: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
-00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011650: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
-00011660: 7661 6c20 3d20 436c 7573 7465 7269 6e67  val = Clustering
-00011670: 2873 656c 662e 6163 6365 6c65 7261 746f  (self.accelerato
-00011680: 722c 2073 656c 662e 6465 7669 6365 732c  r, self.devices,
-00011690: 2073 656c 662e 7365 675f 696d 6167 655b   self.seg_image[
-000116a0: 696e 7428 7469 6d65 5f6b 6579 292c 3a5d  int(time_key),:]
-000116b0: 2c20 2073 656c 662e 6178 6573 2c20 7365  ,  self.axes, se
-000116c0: 6c66 2e6e 756d 5f70 6f69 6e74 732c 2073  lf.num_points, s
-000116d0: 656c 662e 6175 746f 656e 636f 6465 725f  elf.autoencoder_
-000116e0: 6d6f 6465 6c2c 206b 6579 203d 2074 696d  model, key = tim
-000116f0: 655f 6b65 792c 2070 726f 6772 6573 735f  e_key, progress_
-00011700: 6261 723d 7365 6c66 2e70 726f 6772 6573  bar=self.progres
-00011710: 735f 6261 722c 2062 6174 6368 5f73 697a  s_bar, batch_siz
-00011720: 6520 3d20 7365 6c66 2e62 6174 6368 5f73  e = self.batch_s
-00011730: 697a 652c 2073 6361 6c65 5f7a 3d73 656c  ize, scale_z=sel
-00011740: 662e 7363 616c 655f 7a2c 2073 6361 6c65  f.scale_z, scale
-00011750: 5f78 793d 2073 656c 662e 7363 616c 655f  _xy= self.scale_
-00011760: 7879 2c20 6365 6e74 6572 203d 2073 656c  xy, center = sel
-00011770: 662e 6365 6e74 6572 2920 2020 2020 2020  f.center)       
-00011780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011790: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
-000117a0: 7374 6572 5f65 7661 6c2e 5f63 7265 6174  ster_eval._creat
-000117b0: 655f 636c 7573 7465 725f 6c61 6265 6c73  e_cluster_labels
-000117c0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000117d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000117e0: 696d 6564 5f63 6c75 7374 6572 5f6c 6162  imed_cluster_lab
-000117f0: 656c 203d 2063 6c75 7374 6572 5f65 7661  el = cluster_eva
-00011800: 6c2e 7469 6d65 645f 636c 7573 7465 725f  l.timed_cluster_
-00011810: 6c61 6265 6c20 0d0a 2020 2020 2020 2020  label ..        
-00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011830: 2020 206f 7574 7075 745f 6c61 6265 6c73     output_labels
-00011840: 2c20 206f 7574 7075 745f 636c 7573 7465  ,  output_cluste
-00011850: 725f 6365 6e74 726f 6964 2c20 6f75 7470  r_centroid, outp
-00011860: 7574 5f63 6c6f 7564 5f65 6363 656e 7472  ut_cloud_eccentr
-00011870: 6963 6974 792c 206f 7574 7075 745f 6c61  icity, output_la
-00011880: 7267 6573 745f 6569 6765 6e76 6563 746f  rgest_eigenvecto
-00011890: 722c 206f 7574 7075 745f 6c61 7267 6573  r, output_larges
-000118a0: 745f 6569 6765 6e76 616c 7565 2c20 6f75  t_eigenvalue, ou
-000118b0: 7470 7574 5f64 696d 656e 7369 6f6e 732c  tput_dimensions,
-000118c0: 206f 7574 7075 745f 636c 6f75 645f 7375   output_cloud_su
-000118d0: 7266 6163 655f 6172 6561 203d 2074 696d  rface_area = tim
-000118e0: 6564 5f63 6c75 7374 6572 5f6c 6162 656c  ed_cluster_label
-000118f0: 5b74 696d 655f 6b65 795d 0d0a 2020 2020  [time_key]..    
-00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
-00011920: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00011930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011940: 6361 6c65 5f32 203d 2031 0d0a 2020 2020  cale_2 = 1..    
+000115d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000115e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00011610: 6261 722e 7661 6c75 6520 3d20 2063 6f75  bar.value =  cou
+00011620: 6e74 200d 0a20 2020 2020 2020 2020 2020  nt ..           
+00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011640: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00011650: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+00011660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011670: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00011680: 7465 725f 6576 616c 203d 2043 6c75 7374  ter_eval = Clust
+00011690: 6572 696e 6728 7365 6c66 2e61 6363 656c  ering(self.accel
+000116a0: 6572 6174 6f72 2c20 7365 6c66 2e64 6576  erator, self.dev
+000116b0: 6963 6573 2c20 7365 6c66 2e73 6567 5f69  ices, self.seg_i
+000116c0: 6d61 6765 5b69 6e74 2874 696d 655f 6b65  mage[int(time_ke
+000116d0: 7929 2c3a 5d2c 2020 7365 6c66 2e61 7865  y),:],  self.axe
+000116e0: 732c 2073 656c 662e 6e75 6d5f 706f 696e  s, self.num_poin
+000116f0: 7473 2c20 7365 6c66 2e61 7574 6f65 6e63  ts, self.autoenc
+00011700: 6f64 6572 5f6d 6f64 656c 2c20 6b65 7920  oder_model, key 
+00011710: 3d20 7469 6d65 5f6b 6579 2c20 7072 6f67  = time_key, prog
+00011720: 7265 7373 5f62 6172 3d73 656c 662e 7072  ress_bar=self.pr
+00011730: 6f67 7265 7373 5f62 6172 2c20 6261 7463  ogress_bar, batc
+00011740: 685f 7369 7a65 203d 2073 656c 662e 6261  h_size = self.ba
+00011750: 7463 685f 7369 7a65 2c20 7363 616c 655f  tch_size, scale_
+00011760: 7a3d 7365 6c66 2e73 6361 6c65 5f7a 2c20  z=self.scale_z, 
+00011770: 7363 616c 655f 7879 3d20 7365 6c66 2e73  scale_xy= self.s
+00011780: 6361 6c65 5f78 792c 2063 656e 7465 7220  cale_xy, center 
+00011790: 3d20 7365 6c66 2e63 656e 7465 7229 2020  = self.center)  
+000117a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117c0: 2020 636c 7573 7465 725f 6576 616c 2e5f    cluster_eval._
+000117d0: 6372 6561 7465 5f63 6c75 7374 6572 5f6c  create_cluster_l
+000117e0: 6162 656c 7328 290d 0a20 2020 2020 2020  abels()..       
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 2020 2020 7469 6d65 645f 636c 7573 7465      timed_cluste
+00011810: 725f 6c61 6265 6c20 3d20 636c 7573 7465  r_label = cluste
+00011820: 725f 6576 616c 2e74 696d 6564 5f63 6c75  r_eval.timed_clu
+00011830: 7374 6572 5f6c 6162 656c 200d 0a20 2020  ster_label ..   
+00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011850: 2020 2020 2020 2020 6f75 7470 7574 5f6c          output_l
+00011860: 6162 656c 732c 2020 6f75 7470 7574 5f63  abels,  output_c
+00011870: 6c75 7374 6572 5f63 656e 7472 6f69 642c  luster_centroid,
+00011880: 206f 7574 7075 745f 636c 6f75 645f 6563   output_cloud_ec
+00011890: 6365 6e74 7269 6369 7479 2c20 6f75 7470  centricity, outp
+000118a0: 7574 5f6c 6172 6765 7374 5f65 6967 656e  ut_largest_eigen
+000118b0: 7665 6374 6f72 2c20 6f75 7470 7574 5f6c  vector, output_l
+000118c0: 6172 6765 7374 5f65 6967 656e 7661 6c75  argest_eigenvalu
+000118d0: 652c 206f 7574 7075 745f 6469 6d65 6e73  e, output_dimens
+000118e0: 696f 6e73 2c20 6f75 7470 7574 5f63 6c6f  ions, output_clo
+000118f0: 7564 5f73 7572 6661 6365 5f61 7265 6120  ud_surface_area 
+00011900: 3d20 7469 6d65 645f 636c 7573 7465 725f  = timed_cluster_
+00011910: 6c61 6265 6c5b 7469 6d65 5f6b 6579 5d0d  label[time_key].
+00011920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011930: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00011940: 655f 3120 3d20 310d 0a20 2020 2020 2020  e_1 = 1..       
 00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00011970: 7261 6e67 6528 6c65 6e28 6f75 7470 7574  range(len(output
-00011980: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
-00011990: 6429 293a 0d0a 2020 2020 2020 2020 2020  d)):..          
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 2020 2020 2020 2020 2020 6365 6e74 726f            centro
-000119c0: 6964 203d 206f 7574 7075 745f 636c 7573  id = output_clus
-000119d0: 7465 725f 6365 6e74 726f 6964 5b69 5d0d  ter_centroid[i].
-000119e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a00: 2020 2020 2071 7561 6c69 7479 203d 206f       quality = o
-00011a10: 7574 7075 745f 6c61 7267 6573 745f 6569  utput_largest_ei
-00011a20: 6765 6e76 616c 7565 5b69 5d0d 0a20 2020  genvalue[i]..   
-00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-00011a60: 6d70 5f66 6972 7374 797a 203d 206f 7574  mp_firstyz = out
-00011a70: 7075 745f 636c 6f75 645f 6563 6365 6e74  put_cloud_eccent
-00011a80: 7269 6369 7479 5b69 5d0d 0a20 2020 2020  ricity[i]..     
-00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00011ab0: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
-00011ac0: 6e73 696f 6e20 3d20 6f75 7470 7574 5f64  nsion = output_d
-00011ad0: 696d 656e 7369 6f6e 735b 695d 200d 0a20  imensions[i] .. 
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
-00011b10: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
-00011b20: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
-00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
-00011b60: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
-00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011ba0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011bb0: 696f 6e5b 315d 203d 3d20 313a 0d0a 2020  ion[1] == 1:..  
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bf0: 7363 616c 655f 3220 3d20 7365 6c66 2e79  scale_2 = self.y
-00011c00: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
-00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
-00011c40: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
-00011c50: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
-00011c90: 2e7a 6361 6c69 6272 6174 696f 6e0d 0a20  .zcalibration.. 
-00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cc0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011cd0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011ce0: 696f 6e5b 315d 203d 3d20 303a 0d0a 2020  ion[1] == 0:..  
-00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d20: 7363 616c 655f 3220 3d20 7365 6c66 2e78  scale_2 = self.x
-00011d30: 6361 6c69 6272 6174 696f 6e20 2020 0d0a  calibration   ..
-00011d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d60: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011d70: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011d80: 305d 203d 3d20 313a 0d0a 2020 2020 2020  0] == 1:..      
-00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011db0: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-00011dc0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00011dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011e00: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011e10: 656e 7369 6f6e 5b31 5d20 3d3d 2030 3a0d  ension[1] == 0:.
-00011e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-00011e60: 662e 7863 616c 6962 7261 7469 6f6e 2020  f.xcalibration  
-00011e70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
-00011ea0: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
-00011eb0: 6e5b 305d 203d 3d20 313a 0d0a 2020 2020  n[0] == 1:..    
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
-00011ef0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00011f00: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011f30: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
-00011f40: 696d 656e 7369 6f6e 5b31 5d20 3d3d 2032  imension[1] == 2
-00011f50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 2073 6361 6c65 5f32 203d 2073       scale_2 = s
-00011f90: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00011fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
-00011fe0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00011ff0: 5b30 5d20 3d3d 2030 3a0d 0a20 2020 2020  [0] == 0:..     
-00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012020: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
-00012030: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00012040: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012060: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012070: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-00012080: 6d65 6e73 696f 6e5b 315d 203d 3d20 313a  mension[1] == 1:
-00012090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
-000120d0: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
-000120e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
-00012110: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00012120: 5b30 5d20 3d3d 2030 3a0d 0a20 2020 2020  [0] == 0:..     
-00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012150: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
-00012160: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00012170: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000121a0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-000121b0: 6d65 6e73 696f 6e5b 315d 203d 3d20 323a  mension[1] == 2:
-000121c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
-00012200: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
-00012210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011960: 2020 2020 7363 616c 655f 3220 3d20 310d      scale_2 = 1.
+00011970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011980: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011990: 6920 696e 2072 616e 6765 286c 656e 286f  i in range(len(o
+000119a0: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
+000119b0: 6e74 726f 6964 2929 3a0d 0a20 2020 2020  ntroid)):..     
+000119c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000119e0: 656e 7472 6f69 6420 3d20 6f75 7470 7574  entroid = output
+000119f0: 5f63 6c75 7374 6572 5f63 656e 7472 6f69  _cluster_centroi
+00011a00: 645b 695d 0d0a 2020 2020 2020 2020 2020  d[i]..          
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 2020 2020 2020 2020 2020 7175 616c 6974            qualit
+00011a30: 7920 3d20 6f75 7470 7574 5f6c 6172 6765  y = output_large
+00011a40: 7374 5f65 6967 656e 7661 6c75 655b 695d  st_eigenvalue[i]
+00011a50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a70: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+00011a80: 7479 5f63 6f6d 705f 6669 7273 7479 7a20  ty_comp_firstyz 
+00011a90: 3d20 6f75 7470 7574 5f63 6c6f 7564 5f65  = output_cloud_e
+00011aa0: 6363 656e 7472 6963 6974 795b 695d 0d0a  ccentricity[i]..
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2020 2020 6573 7365 6e74 7269 6369 7479      essentricity
+00011ae0: 5f64 696d 656e 7369 6f6e 203d 206f 7574  _dimension = out
+00011af0: 7075 745f 6469 6d65 6e73 696f 6e73 5b69  put_dimensions[i
+00011b00: 5d20 0d0a 2020 2020 2020 2020 2020 2020  ] ..            
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b20: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011b30: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011b40: 6e5b 305d 203d 3d20 323a 0d0a 2020 2020  n[0] == 2:..    
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b70: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
+00011b80: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00011b90: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00011ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011bc0: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00011bd0: 696d 656e 7369 6f6e 5b31 5d20 3d3d 2031  imension[1] == 1
+00011be0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 2020 2020 2073 6361 6c65 5f32 203d 2073       scale_2 = s
+00011c20: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00011c30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c50: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011c60: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011c70: 6e5b 305d 203d 3d20 323a 0d0a 2020 2020  n[0] == 2:..    
+00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ca0: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
+00011cb0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
+00011cc0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011cf0: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
+00011d00: 696d 656e 7369 6f6e 5b31 5d20 3d3d 2030  imension[1] == 0
+00011d10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2073 6361 6c65 5f32 203d 2073       scale_2 = s
+00011d50: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+00011d60: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d80: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00011d90: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00011da0: 7369 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20  sion[0] == 1:.. 
+00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dd0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011de0: 3120 3d20 7365 6c66 2e79 6361 6c69 6272  1 = self.ycalibr
+00011df0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00011e30: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+00011e40: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00011e80: 3d20 7365 6c66 2e78 6361 6c69 6272 6174  = self.xcalibrat
+00011e90: 696f 6e20 200d 0a0d 0a20 2020 2020 2020  ion  ....       
+00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011eb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011ec0: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
+00011ed0: 656e 7369 6f6e 5b30 5d20 3d3d 2031 3a0d  ension[0] == 1:.
+00011ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f00: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+00011f10: 655f 3120 3d20 7365 6c66 2e79 6361 6c69  e_1 = self.ycali
+00011f20: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f50: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
+00011f60: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
+00011f70: 203d 3d20 323a 0d0a 2020 2020 2020 2020   == 2:..        
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fa0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011fb0: 3220 3d20 7365 6c66 2e7a 6361 6c69 6272  2 = self.zcalibr
+00011fc0: 6174 696f 6e20 2020 2020 2020 2020 2020  ation           
+00011fd0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ff0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00012000: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00012010: 6e73 696f 6e5b 305d 203d 3d20 303a 0d0a  nsion[0] == 0:..
+00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00012050: 5f31 203d 2073 656c 662e 7863 616c 6962  _1 = self.xcalib
+00012060: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012090: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+000120a0: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+000120b0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
+000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120e0: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+000120f0: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
+00012100: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00012110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012120: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00012130: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00012140: 6e73 696f 6e5b 305d 203d 3d20 303a 0d0a  nsion[0] == 0:..
+00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00012180: 5f31 203d 2073 656c 662e 7863 616c 6962  _1 = self.xcalib
+00012190: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121c0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+000121d0: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+000121e0: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+00012220: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
+00012230: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
 00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00012290: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
-000122d0: 7869 7320 3d20 6f75 7470 7574 5f6c 6172  xis = output_lar
-000122e0: 6765 7374 5f65 6967 656e 7665 6374 6f72  gest_eigenvector
-000122f0: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012310: 2020 2020 2020 2020 2073 7572 6661 6365           surface
-00012320: 5f61 7265 6120 3d20 6f75 7470 7574 5f63  _area = output_c
-00012330: 6c6f 7564 5f73 7572 6661 6365 5f61 7265  loud_surface_are
-00012340: 615b 695d 202a 2073 656c 662e 7a63 616c  a[i] * self.zcal
-00012350: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
-00012360: 7963 616c 6962 7261 7469 6f6e 202a 2073  ycalibration * s
-00012370: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-00012380: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123a0: 2020 2020 2020 6469 7374 2c20 696e 6465        dist, inde
-000123b0: 7820 3d20 7472 6565 2e71 7565 7279 2863  x = tree.query(c
-000123c0: 656e 7472 6f69 6429 0d0a 2020 2020 2020  entroid)..      
-000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000123f0: 6469 7573 203d 2071 7561 6c69 7479 202a  dius = quality *
-00012400: 206d 6174 682e 706f 7728 7365 6c66 2e7a   math.pow(self.z
-00012410: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-00012420: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
-00012430: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
-00012440: 696f 6e2c 2031 2e30 2f33 2e30 290d 0a20  ion, 1.0/3.0).. 
-00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012470: 2020 2069 6620 6469 7374 203c 2071 7561     if dist < qua
-00012480: 6c69 7479 3a0d 0a20 2020 2020 2020 2020  lity:..         
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2020 2063 6c6f 7365 7374 5f63 656e 7472     closest_centr
-000124c0: 6f69 6420 3d20 7370 6f74 5f63 656e 7472  oid = spot_centr
-000124d0: 6f69 6473 5b69 6e64 6578 5d0d 0a20 2020  oids[index]..   
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
-00012510: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
-00012520: 696e 7428 7469 6d65 5f6b 6579 292c 636c  int(time_key),cl
-00012530: 6f73 6573 745f 6365 6e74 726f 6964 5b30  osest_centroid[0
-00012540: 5d2c 2063 6c6f 7365 7374 5f63 656e 7472  ], closest_centr
-00012550: 6f69 645b 315d 2c20 636c 6f73 6573 745f  oid[1], closest_
-00012560: 6365 6e74 726f 6964 5b32 5d29 0d0a 2020  centroid[2])..  
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012590: 2020 2020 2020 2020 2020 636c 6f73 6573            closes
-000125a0: 745f 6365 6c6c 5f69 6420 3d20 7365 6c66  t_cell_id = self
-000125b0: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-000125c0: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-000125d0: 5f63 656e 7472 6f69 645d 0d0a 2020 2020  _centroid]..    
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012600: 2020 2020 2020 2020 6d61 736b 5f76 6563          mask_vec
-00012610: 746f 7220 3d20 5b20 666c 6f61 7428 7365  tor = [ float(se
-00012620: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012630: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00012640: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
-00012650: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-00012660: 645f 785f 6b65 795d 292c 2066 6c6f 6174  d_x_key]), float
-00012670: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00012680: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012690: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-000126a0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-000126b0: 726f 6964 5f79 5f6b 6579 5d29 2c20 666c  roid_y_key]), fl
-000126c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000126d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000126e0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-000126f0: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00012700: 656e 7472 6f69 645f 7a5f 6b65 795d 2920  entroid_z_key]) 
-00012710: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012730: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012740: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-00012750: 616e 6775 6c61 725f 6368 616e 6765 2863  angular_change(c
-00012760: 656c 6c5f 6178 6973 2c20 6d61 736b 5f76  ell_axis, mask_v
-00012770: 6563 746f 7229 0d0a 2020 2020 2020 2020  ector)..        
-00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000122c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000122f0: 656c 6c5f 6178 6973 203d 206f 7574 7075  ell_axis = outpu
+00012300: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
+00012310: 6563 746f 725b 695d 0d0a 2020 2020 2020  ector[i]..      
+00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012330: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00012340: 7266 6163 655f 6172 6561 203d 206f 7574  rface_area = out
+00012350: 7075 745f 636c 6f75 645f 7375 7266 6163  put_cloud_surfac
+00012360: 655f 6172 6561 5b69 5d20 2a20 7365 6c66  e_area[i] * self
+00012370: 2e7a 6361 6c69 6272 6174 696f 6e20 2a20  .zcalibration * 
+00012380: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+00012390: 6e20 2a20 7365 6c66 2e78 6361 6c69 6272  n * self.xcalibr
+000123a0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2020 2020 2020 2020 2020 2064 6973 742c             dist,
+000123d0: 2069 6e64 6578 203d 2074 7265 652e 7175   index = tree.qu
+000123e0: 6572 7928 6365 6e74 726f 6964 290d 0a20  ery(centroid).. 
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012410: 2020 2072 6164 6975 7320 3d20 7175 616c     radius = qual
+00012420: 6974 7920 2a20 6d61 7468 2e70 6f77 2873  ity * math.pow(s
+00012430: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00012440: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
+00012450: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
+00012460: 6962 7261 7469 6f6e 2c20 312e 302f 332e  ibration, 1.0/3.
+00012470: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012490: 2020 2020 2020 2020 6966 2064 6973 7420          if dist 
+000124a0: 3c20 7175 616c 6974 793a 0d0a 2020 2020  < quality:..    
+000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 2020 2020 2020 2020 636c 6f73 6573 745f          closest_
+000124e0: 6365 6e74 726f 6964 203d 2073 706f 745f  centroid = spot_
+000124f0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00012500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012520: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00012530: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
+00012540: 6420 3d20 2869 6e74 2874 696d 655f 6b65  d = (int(time_ke
+00012550: 7929 2c63 6c6f 7365 7374 5f63 656e 7472  y),closest_centr
+00012560: 6f69 645b 305d 2c20 636c 6f73 6573 745f  oid[0], closest_
+00012570: 6365 6e74 726f 6964 5b31 5d2c 2063 6c6f  centroid[1], clo
+00012580: 7365 7374 5f63 656e 7472 6f69 645b 325d  sest_centroid[2]
+00012590: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000125c0: 6c6f 7365 7374 5f63 656c 6c5f 6964 203d  losest_cell_id =
+000125d0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000125e0: 745f 6365 6e74 726f 6964 5b66 7261 6d65  t_centroid[frame
+000125f0: 5f73 706f 745f 6365 6e74 726f 6964 5d0d  _spot_centroid].
+00012600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012620: 2020 2020 2020 2020 2020 2020 206d 6173               mas
+00012630: 6b5f 7665 6374 6f72 203d 205b 2066 6c6f  k_vector = [ flo
+00012640: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00012650: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00012660: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00012670: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+00012680: 6e74 726f 6964 5f78 5f6b 6579 5d29 2c20  ntroid_x_key]), 
+00012690: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+000126a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000126b0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+000126c0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
+000126d0: 6b63 656e 7472 6f69 645f 795f 6b65 795d  kcentroid_y_key]
+000126e0: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
+000126f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00012700: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00012710: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
+00012720: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
+00012730: 6579 5d29 205d 0d0a 2020 2020 2020 2020  ey]) ]..        
+00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012760: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+00012770: 736b 203d 2061 6e67 756c 6172 5f63 6861  sk = angular_cha
+00012780: 6e67 6528 6365 6c6c 5f61 7869 732c 206d  nge(cell_axis, m
+00012790: 6173 6b5f 7665 6374 6f72 290d 0a20 2020  ask_vector)..   
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-000127e0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000127f0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00012800: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00012810: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
-00012820: 6579 203a 2063 656c 6c5f 6178 6973 5f6d  ey : cell_axis_m
-00012830: 6173 6b7d 290d 0a20 2020 2020 2020 2020  ask})..         
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012860: 2020 2069 6620 7365 6c66 2e75 6e69 7175     if self.uniqu
-00012870: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012880: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012890: 6c6c 5f69 6429 5d5b 7365 6c66 2e72 6164  ll_id)][self.rad
-000128a0: 6975 735f 6b65 795d 203e 2030 3a0d 0a20  ius_key] > 0:.. 
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000128f0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00012900: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00012910: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00012920: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
-00012930: 6f6d 705f 6669 7273 746b 6579 203a 2065  omp_firstkey : e
-00012940: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012950: 5f66 6972 7374 797a 5b30 5d20 2a20 7363  _firstyz[0] * sc
-00012960: 616c 655f 317d 290d 0a20 2020 2020 2020  ale_1})..       
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000129a0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000129b0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-000129c0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-000129d0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-000129e0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-000129f0: 636f 6e64 6b65 7920 3a20 6563 6365 6e74  condkey : eccent
-00012a00: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00012a10: 7479 7a5b 315d 202a 2073 6361 6c65 5f32  tyz[1] * scale_2
-00012a20: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a50: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012a60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012a70: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012a80: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00012a90: 287b 7365 6c66 2e73 7572 6661 6365 5f61  ({self.surface_a
-00012aa0: 7265 615f 6b65 7920 3a20 7375 7266 6163  rea_key : surfac
-00012ab0: 655f 6172 6561 7d29 0d0a 2020 2020 2020  e_area})..      
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00012af0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012b00: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00012b10: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
-00012b20: 7570 6461 7465 287b 7365 6c66 2e71 7561  update({self.qua
-00012b30: 6c69 7479 5f6b 6579 203a 2071 7561 6c69  lity_key : quali
-00012b40: 7479 7d29 0d0a 2020 2020 2020 2020 2020  ty})..          
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b70: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00012b80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00012b90: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00012ba0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00012bb0: 7465 287b 7365 6c66 2e72 6164 6975 735f  te({self.radius_
-00012bc0: 6b65 7920 3a20 7261 6469 7573 207d 290d  key : radius }).
-00012bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bf0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00012c00: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000127c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012800: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012810: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00012820: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00012830: 7b73 656c 662e 6365 6c6c 6178 6973 5f6d  {self.cellaxis_m
+00012840: 6173 6b5f 6b65 7920 3a20 6365 6c6c 5f61  ask_key : cell_a
+00012850: 7869 735f 6d61 736b 7d29 0d0a 2020 2020  xis_mask})..    
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012880: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012890: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000128a0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+000128b0: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
+000128c0: 662e 7261 6469 7573 5f6b 6579 5d20 3e20  f.radius_key] > 
+000128d0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012900: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00012910: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012920: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012930: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00012940: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
+00012950: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
+00012960: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
+00012970: 5f63 6f6d 705f 6669 7273 7479 7a5b 305d  _comp_firstyz[0]
+00012980: 202a 2073 6361 6c65 5f31 7d29 0d0a 2020   * scale_1})..  
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129c0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+000129d0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000129e0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+000129f0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012a00: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00012a10: 6d70 5f73 6563 6f6e 646b 6579 203a 2065  mp_secondkey : e
+00012a20: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00012a30: 5f66 6972 7374 797a 5b31 5d20 2a20 7363  _firstyz[1] * sc
+00012a40: 616c 655f 327d 290d 0a20 2020 2020 2020  ale_2})..       
+00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00012a80: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00012a90: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+00012aa0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00012ab0: 7064 6174 6528 7b73 656c 662e 7375 7266  pdate({self.surf
+00012ac0: 6163 655f 6172 6561 5f6b 6579 203a 2073  ace_area_key : s
+00012ad0: 7572 6661 6365 5f61 7265 617d 290d 0a20  urface_area}).. 
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b10: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00012b20: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00012b30: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00012b40: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00012b50: 662e 7175 616c 6974 795f 6b65 7920 3a20  f.quality_key : 
+00012b60: 7175 616c 6974 797d 290d 0a20 2020 2020  quality})..     
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012ba0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00012bb0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00012bc0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00012bd0: 2e75 7064 6174 6528 7b73 656c 662e 7261  .update({self.ra
+00012be0: 6469 7573 5f6b 6579 203a 2072 6164 6975  dius_key : radiu
+00012bf0: 7320 7d29 0d0a 2020 2020 2020 2020 2020  s })..          
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00012c20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012c70: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00012c80: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00012c90: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00012ca0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-00012cb0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00012cc0: 7273 746b 6579 203a 202d 317d 290d 0a20  rstkey : -1}).. 
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00012d10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00012d20: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00012d30: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00012d40: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
-00012d50: 6f6d 705f 7365 636f 6e64 6b65 7920 3a20  omp_secondkey : 
-00012d60: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00012da0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00012db0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00012dc0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00012dd0: 7465 287b 7365 6c66 2e73 7572 6661 6365  te({self.surface
-00012de0: 5f61 7265 615f 6b65 7920 3a20 2d31 7d29  _area_key : -1})
-00012df0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012e30: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012e40: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012e50: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00012e60: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
-00012e70: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ea0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012eb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00012ec0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00012ed0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00012ee0: 7064 6174 6528 7b73 656c 662e 7261 6469  pdate({self.radi
-00012ef0: 7573 5f6b 6579 203a 202d 3120 7d29 0d0a  us_key : -1 })..
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f30: 2020 200d 0a0d 0a0d 0a0d 0a0d 0a20 2020     ..........   
+00012c50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00012c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00012ca0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012cb0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00012cc0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012cd0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00012ce0: 6d70 5f66 6972 7374 6b65 7920 3a20 2d31  mp_firstkey : -1
+00012cf0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d20: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00012d30: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012d40: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012d50: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00012d60: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
+00012d70: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
+00012d80: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012dc0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00012dd0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00012de0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+00012df0: 2e75 7064 6174 6528 7b73 656c 662e 7375  .update({self.su
+00012e00: 7266 6163 655f 6172 6561 5f6b 6579 203a  rface_area_key :
+00012e10: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012e50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00012e60: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
+00012e70: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
+00012e80: 6174 6528 7b73 656c 662e 7175 616c 6974  ate({self.qualit
+00012e90: 795f 6b65 7920 3a20 2d31 7d29 0d0a 2020  y_key : -1})..  
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00012ee0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012ef0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00012f00: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012f10: 2e72 6164 6975 735f 6b65 7920 3a20 2d31  .radius_key : -1
+00012f20: 207d 290d 0a20 2020 2020 2020 2020 2020   })..           
+00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f60: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012f70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012f80: 7220 286b 2c76 2920 696e 2073 656c 662e  r (k,v) in self.
-00012f90: 726f 6f74 5f73 706f 7473 2e69 7465 6d73  root_spots.items
-00012fa0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2020 2020 2020 2073 656c 662e 726f 6f74         self.root
-00012fd0: 5f73 706f 7473 5b6b 5d20 3d20 7365 6c66  _spots[k] = self
-00012fe0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00012ff0: 7065 7274 6965 735b 6b5d 2020 2020 2020  perties[k]      
-00013000: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00013010: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00013020: 636f 6d70 7574 655f 7068 656e 6f74 7970  compute_phenotyp
-00013030: 6573 2873 656c 6629 3a0d 0a0d 0a20 2020  es(self):....   
-00013040: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00013050: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-00013060: 7472 6163 6b73 2e69 7465 6d73 2829 3a0d  tracks.items():.
-00013070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013080: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013090: 2020 2074 7261 636b 5f69 6420 3d20 6b0d     track_id = k.
-000130a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000130b0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-000130c0: 7469 6573 203d 2073 656c 662e 756e 6971  ties = self.uniq
-000130d0: 7565 5f74 7261 636b 5f70 726f 7065 7274  ue_track_propert
-000130e0: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-000130f0: 2020 2020 2020 2020 7472 6163 6b73 203d          tracks =
-00013100: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00013110: 636b 735b 6b5d 0d0a 2020 2020 2020 2020  cks[k]..        
-00013120: 2020 2020 2020 2020 5a20 3d20 7472 6163          Z = trac
-00013130: 6b73 5b3a 2c32 5d0d 0a20 2020 2020 2020  ks[:,2]..       
-00013140: 2020 2020 2020 2020 2059 203d 2074 7261           Y = tra
-00013150: 636b 735b 3a2c 335d 0d0a 2020 2020 2020  cks[:,3]..      
-00013160: 2020 2020 2020 2020 2020 5820 3d20 7472            X = tr
-00013170: 6163 6b73 5b3a 2c34 5d0d 0a20 2020 2020  acks[:,4]..     
-00013180: 2020 2020 2020 2020 2020 2074 696d 6520             time 
-00013190: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-000131a0: 7274 6965 735b 3a2c 305d 0d0a 2020 2020  rties[:,0]..    
-000131b0: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-000131c0: 7565 5f69 6473 203d 2074 7261 636b 6c65  ue_ids = trackle
-000131d0: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-000131e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000131f0: 2020 2075 6e69 7175 655f 6964 735f 7365     unique_ids_se
-00013200: 7420 3d20 7365 7428 756e 6971 7565 5f69  t = set(unique_i
-00013210: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-00013220: 2020 2020 2067 656e 6572 6174 696f 6e5f       generation_
-00013230: 6964 7320 3d20 7472 6163 6b6c 6574 5f70  ids = tracklet_p
-00013240: 726f 7065 7274 6965 735b 3a2c 325d 0d0a  roperties[:,2]..
-00013250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013260: 7261 6469 7573 203d 2074 7261 636b 6c65  radius = trackle
-00013270: 745f 7072 6f70 6572 7469 6573 5b3a 2c33  t_properties[:,3
-00013280: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013290: 2020 2076 6f6c 756d 6520 3d20 7472 6163     volume = trac
-000132a0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-000132b0: 3a2c 345d 0d0a 2020 2020 2020 2020 2020  :,4]..          
-000132c0: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
-000132d0: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
-000132e0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-000132f0: 6965 735b 3a2c 355d 0d0a 2020 2020 2020  ies[:,5]..      
-00013300: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-00013310: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00013320: 6e64 203d 2074 7261 636b 6c65 745f 7072  nd = tracklet_pr
-00013330: 6f70 6572 7469 6573 5b3a 2c36 5d0d 0a20  operties[:,6].. 
-00013340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013350: 7572 6661 6365 5f61 7265 6120 3d20 7472  urface_area = tr
-00013360: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00013370: 735b 3a2c 375d 0d0a 2020 2020 2020 2020  s[:,7]..        
-00013380: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013390: 2020 2020 2020 2020 2069 6e74 656e 7369           intensi
-000133a0: 7479 203d 2074 7261 636b 6c65 745f 7072  ty = tracklet_pr
-000133b0: 6f70 6572 7469 6573 5b3a 2c38 5d0d 0a20  operties[:,8].. 
-000133c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000133d0: 7065 6564 203d 2074 7261 636b 6c65 745f  peed = tracklet_
-000133e0: 7072 6f70 6572 7469 6573 5b3a 2c39 5d0d  properties[:,9].
-000133f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013400: 206d 6f74 696f 6e5f 616e 676c 6520 3d20   motion_angle = 
-00013410: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00013420: 6965 735b 3a2c 3130 5d0d 0a20 2020 2020  ies[:,10]..     
-00013430: 2020 2020 2020 2020 2020 2061 6363 656c             accel
-00013440: 6572 6174 696f 6e20 3d20 7472 6163 6b6c  eration = trackl
-00013450: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00013460: 3131 5d0d 0a20 2020 2020 2020 2020 2020  11]..           
-00013470: 2020 2020 2064 6973 7461 6e63 655f 6365       distance_ce
-00013480: 6c6c 5f6d 6173 6b20 3d20 7472 6163 6b6c  ll_mask = trackl
-00013490: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000134a0: 3132 5d0d 0a20 2020 2020 2020 2020 2020  12]..           
-000134b0: 2020 2020 2072 6164 6961 6c5f 616e 676c       radial_angl
-000134c0: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-000134d0: 7065 7274 6965 735b 3a2c 3133 5d0d 0a20  perties[:,13].. 
-000134e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000134f0: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-00013500: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00013510: 6965 735b 3a2c 3134 5d0d 0a0d 0a0d 0a20  ies[:,14]...... 
-00013520: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00013530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013540: 2075 6e69 7175 655f 6666 745f 7072 6f70   unique_fft_prop
-00013550: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
-00013560: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00013570: 2020 2020 2020 756e 6971 7565 5f63 6c75        unique_clu
-00013580: 7374 6572 5f70 726f 7065 7274 6965 735f  ster_properties_
-00013590: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-000135a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000135b0: 656c 662e 756e 6971 7565 5f66 6674 5f70  elf.unique_fft_p
-000135c0: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-000135d0: 6964 5d20 3d20 7b7d 0d0a 2020 2020 2020  id] = {}..      
-000135e0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000135f0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-00013600: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00013610: 645d 203d 207b 7d0d 0a0d 0a20 2020 2020  d] = {}....     
-00013620: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00013630: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-00013640: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
-00013650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013660: 2020 756e 6971 7565 5f64 796e 616d 6963    unique_dynamic
-00013670: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013680: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
-00013690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000136a0: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
-000136b0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-000136c0: 5d20 3d20 7b7d 0d0a 2020 2020 2020 2020  ] = {}..        
-000136d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000136e0: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-000136f0: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00013700: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00013710: 2020 2020 2020 2065 7870 616e 6465 645f         expanded_
-00013720: 7469 6d65 203d 206e 702e 7a65 726f 7328  time = np.zeros(
-00013730: 7365 6c66 2e74 656e 6420 2d20 7365 6c66  self.tend - self
-00013740: 2e74 7374 6172 7420 2b20 3129 0d0a 2020  .tstart + 1)..  
-00013750: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00013760: 696e 745f 7361 6d70 6c65 203d 2065 7870  int_sample = exp
-00013770: 616e 6465 645f 7469 6d65 2e73 6861 7065  anded_time.shape
-00013780: 5b30 5d0d 0a20 2020 2020 2020 2020 2020  [0]..           
-00013790: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000137a0: 6e67 6528 6c65 6e28 6578 7061 6e64 6564  nge(len(expanded
-000137b0: 5f74 696d 6529 293a 0d0a 2020 2020 2020  _time)):..      
-000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137d0: 2065 7870 616e 6465 645f 7469 6d65 5b69   expanded_time[i
-000137e0: 5d20 3d20 6920 0d0a 2020 2020 2020 2020  ] = i ..        
-000137f0: 2020 2020 2020 2020 666f 7220 6375 7272          for curr
-00013800: 656e 745f 756e 6971 7565 5f69 6420 696e  ent_unique_id in
-00013810: 2075 6e69 7175 655f 6964 735f 7365 743a   unique_ids_set:
-00013820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013830: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00013840: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
-00013850: 6564 5f69 6e74 656e 7369 7479 203d 206e  ed_intensity = n
-00013860: 702e 7a65 726f 7328 7365 6c66 2e74 656e  p.zeros(self.ten
-00013870: 6420 2d20 7365 6c66 2e74 7374 6172 7420  d - self.tstart 
-00013880: 2b20 3129 0d0a 2020 2020 2020 2020 2020  + 1)..          
-00013890: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000138a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138c0: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-000138d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000138e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000138f0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
-00013900: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013910: 656e 745f 7920 3d20 5b5d 0d0a 2020 2020  ent_y = []..    
-00013920: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013930: 7572 7265 6e74 5f78 203d 205b 5d0d 0a20  urrent_x = [].. 
-00013940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013950: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
-00013960: 6974 7920 3d20 5b5d 0d0a 2020 2020 2020  ity = []..      
-00013970: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013980: 7265 6e74 5f72 6164 6975 7320 3d20 5b5d  rent_radius = []
-00013990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000139a0: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
-000139b0: 756d 6520 3d20 5b5d 0d0a 2020 2020 2020  ume = []..      
-000139c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000139d0: 7265 6e74 5f73 7065 6564 203d 205b 5d0d  rent_speed = [].
-000139e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000139f0: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
-00013a00: 6f6e 5f61 6e67 6c65 203d 205b 5d0d 0a20  on_angle = [].. 
-00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a20: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
-00013a30: 7261 7469 6f6e 203d 205b 5d0d 0a20 2020  ration = []..   
-00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-00013a60: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00013a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a80: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00013a90: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00013aa0: 7273 7420 3d20 5b5d 0d0a 2020 2020 2020  rst = []..      
-00013ab0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013ac0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013ad0: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
-00013ae0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013af0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-00013b00: 7572 6661 6365 5f61 7265 6120 3d20 5b5d  urface_area = []
-00013b10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00013b20: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
-00013b30: 6164 6961 6c5f 616e 676c 6520 3d20 5b5d  adial_angle = []
-00013b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013b50: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
-00013b60: 6c5f 6178 6973 5f6d 6173 6b20 3d20 5b5d  l_axis_mask = []
-00013b70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013b80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013b90: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
-00013ba0: 2069 6e20 7261 6e67 6528 7469 6d65 2e73   in range(time.s
-00013bb0: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
-00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bd0: 2020 2020 2069 6620 6375 7272 656e 745f       if current_
-00013be0: 756e 6971 7565 5f69 6420 3d3d 2075 6e69  unique_id == uni
-00013bf0: 7175 655f 6964 735b 6a5d 3a0d 0a20 2020  que_ids[j]:..   
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013c20: 7272 656e 745f 7469 6d65 2e61 7070 656e  rrent_time.appen
-00013c30: 6428 7469 6d65 5b6a 5d29 0d0a 2020 2020  d(time[j])..    
-00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013c60: 7265 6e74 5f7a 2e61 7070 656e 6428 5a5b  rent_z.append(Z[
-00013c70: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c90: 2020 2020 2020 6375 7272 656e 745f 792e        current_y.
-00013ca0: 6170 7065 6e64 2859 5b6a 5d29 0d0a 2020  append(Y[j])..  
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013cd0: 7572 7265 6e74 5f78 2e61 7070 656e 6428  urrent_x.append(
-00013ce0: 585b 6a5d 290d 0a20 2020 2020 2020 2020  X[j])..         
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 2020 2020 6578 7061 6e64 6564          expanded
-00013d10: 5f69 6e74 656e 7369 7479 5b69 6e74 2874  _intensity[int(t
-00013d20: 696d 655b 6a5d 295d 203d 2069 6e74 656e  ime[j])] = inten
-00013d30: 7369 7479 5b6a 5d0d 0a20 2020 2020 2020  sity[j]..       
-00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d50: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013d60: 745f 696e 7465 6e73 6974 792e 6170 7065  t_intensity.appe
-00013d70: 6e64 2869 6e74 656e 7369 7479 5b6a 5d29  nd(intensity[j])
-00013d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013da0: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
-00013db0: 732e 6170 7065 6e64 2872 6164 6975 735b  s.append(radius[
-00013dc0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
-00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013de0: 2020 2020 2020 6375 7272 656e 745f 766f        current_vo
-00013df0: 6c75 6d65 2e61 7070 656e 6428 766f 6c75  lume.append(volu
-00013e00: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013e30: 5f73 7065 6564 2e61 7070 656e 6428 7370  _speed.append(sp
-00013e40: 6565 645b 6a5d 290d 0a20 2020 2020 2020  eed[j])..       
-00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013e70: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2e61  t_motion_angle.a
-00013e80: 7070 656e 6428 6d6f 7469 6f6e 5f61 6e67  ppend(motion_ang
-00013e90: 6c65 5b6a 5d29 0d0a 2020 2020 2020 2020  le[j])..        
-00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013eb0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013ec0: 5f61 6363 656c 6572 6174 696f 6e2e 6170  _acceleration.ap
-00013ed0: 7065 6e64 2861 6363 656c 6572 6174 696f  pend(acceleratio
-00013ee0: 6e5b 6a5d 290d 0a20 2020 2020 2020 2020  n[j])..         
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013f10: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00013f20: 736b 2e61 7070 656e 6428 6469 7374 616e  sk.append(distan
-00013f30: 6365 5f63 656c 6c5f 6d61 736b 5b6a 5d29  ce_cell_mask[j])
-00013f40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f60: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-00013f70: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00013f80: 7374 2e61 7070 656e 6428 6563 6365 6e74  st.append(eccent
-00013f90: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00013fa0: 745b 6a5d 290d 0a20 2020 2020 2020 2020  t[j])..         
-00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fc0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013fd0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013fe0: 705f 7365 636f 6e64 2e61 7070 656e 6428  p_second.append(
-00013ff0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00014000: 705f 7365 636f 6e64 5b6a 5d29 0d0a 2020  p_second[j])..  
-00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014030: 7572 7265 6e74 5f73 7572 6661 6365 5f61  urrent_surface_a
-00014040: 7265 612e 6170 7065 6e64 2873 7572 6661  rea.append(surfa
-00014050: 6365 5f61 7265 615b 6a5d 290d 0a20 2020  ce_area[j])..   
-00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014070: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00014080: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
-00014090: 6c65 2e61 7070 656e 6428 7261 6469 616c  le.append(radial
-000140a0: 5f61 6e67 6c65 5b6a 5d29 0d0a 2020 2020  _angle[j])..    
-000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000140d0: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-000140e0: 6173 6b2e 6170 7065 6e64 2863 656c 6c5f  ask.append(cell_
-000140f0: 6178 6973 5f6d 6173 6b5b 6a5d 290d 0a20  axis_mask[j]).. 
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014110: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
-00014120: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014130: 656e 745f 7469 6d65 2c20 6474 7970 653d  ent_time, dtype=
-00014140: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014160: 6375 7272 656e 745f 696e 7465 6e73 6974  current_intensit
-00014170: 7920 3d20 6e70 2e61 7361 7272 6179 2863  y = np.asarray(c
-00014180: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
-00014190: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000141a0: 3332 290d 0a0d 0a0d 0a0d 0a20 2020 2020  32)........     
-000141b0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000141c0: 7272 656e 745f 7261 6469 7573 203d 206e  rrent_radius = n
-000141d0: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-000141e0: 745f 7261 6469 7573 2c20 6474 7970 653d  t_radius, dtype=
-000141f0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014210: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
-00014220: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014230: 656e 745f 766f 6c75 6d65 2c20 6474 7970  ent_volume, dtyp
-00014240: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00014270: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-00014280: 7420 3d20 6e70 2e61 7361 7272 6179 2863  t = np.asarray(c
-00014290: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-000142a0: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
-000142b0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-000142c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000142d0: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-000142e0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000142f0: 7365 636f 6e64 203d 206e 702e 6173 6172  second = np.asar
-00014300: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
-00014310: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00014320: 636f 6e64 2c20 6474 7970 653d 6e70 2e66  cond, dtype=np.f
-00014330: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00014340: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00014350: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
-00014360: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00014370: 7272 656e 745f 7375 7266 6163 655f 6172  rrent_surface_ar
-00014380: 6561 2c20 6474 7970 653d 6e70 2e66 6c6f  ea, dtype=np.flo
-00014390: 6174 3332 290d 0a0d 0a20 2020 2020 2020  at32)....       
-000143a0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000143b0: 656e 745f 7370 6565 6420 3d20 6e70 2e61  ent_speed = np.a
-000143c0: 7361 7272 6179 2863 7572 7265 6e74 5f73  sarray(current_s
-000143d0: 7065 6564 2c20 6474 7970 653d 6e70 2e66  peed, dtype=np.f
-000143e0: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-000143f0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00014400: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00014410: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00014420: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
-00014430: 6c65 2c20 6474 7970 653d 6e70 2e66 6c6f  le, dtype=np.flo
-00014440: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014450: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014460: 745f 6163 6365 6c65 7261 7469 6f6e 203d  t_acceleration =
-00014470: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014480: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
-00014490: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000144a0: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-000144b0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000144c0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000144d0: 736b 203d 206e 702e 6173 6172 7261 7928  sk = np.asarray(
-000144e0: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-000144f0: 5f63 656c 6c5f 6d61 736b 2c20 6474 7970  _cell_mask, dtyp
-00014500: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014520: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
-00014530: 5f61 6e67 6c65 203d 206e 702e 6173 6172  _angle = np.asar
-00014540: 7261 7928 6375 7272 656e 745f 7261 6469  ray(current_radi
-00014550: 616c 5f61 6e67 6c65 2c20 6474 7970 653d  al_angle, dtype=
-00014560: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
-00014590: 735f 6d61 736b 203d 206e 702e 6173 6172  s_mask = np.asar
-000145a0: 7261 7928 6375 7272 656e 745f 6365 6c6c  ray(current_cell
-000145b0: 5f61 7869 735f 6d61 736b 2c20 6474 7970  _axis_mask, dtyp
-000145c0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
-000145d0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000145e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000145f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014610: 6966 2070 6f69 6e74 5f73 616d 706c 6520  if point_sample 
-00014620: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 2020 2020 2020 7866 5f73 616d 706c 6520        xf_sample 
-00014650: 3d20 6666 7466 7265 7128 706f 696e 745f  = fftfreq(point_
-00014660: 7361 6d70 6c65 2c20 7365 6c66 2e74 6361  sample, self.tca
-00014670: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2020 2020 2020 2020 2020 2020 6666 7473              ffts
-000146a0: 7472 6970 5f73 616d 706c 6520 3d20 6666  trip_sample = ff
-000146b0: 7428 6578 7061 6e64 6564 5f69 6e74 656e  t(expanded_inten
-000146c0: 7369 7479 290d 0a20 2020 2020 2020 2020  sity)..         
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
-000146f0: 7361 6d70 6c65 203d 206e 702e 6162 7328  sample = np.abs(
-00014700: 6666 7473 7472 6970 5f73 616d 706c 6529  fftstrip_sample)
-00014710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014730: 2020 7866 5f73 616d 706c 6520 3d20 7866    xf_sample = xf
-00014740: 5f73 616d 706c 655b 3020 3a20 6c65 6e28  _sample[0 : len(
-00014750: 7866 5f73 616d 706c 6529 202f 2f20 325d  xf_sample) // 2]
-00014760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
-00014790: 6520 3d20 6666 7474 6f74 616c 5f73 616d  e = ffttotal_sam
-000147a0: 706c 655b 3020 3a20 6c65 6e28 6666 7474  ple[0 : len(fftt
-000147b0: 6f74 616c 5f73 616d 706c 6529 202f 2f20  otal_sample) // 
-000147c0: 325d 0d0a 0d0a 2020 2020 2020 2020 2020  2]....          
-000147d0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-000147e0: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
-000147f0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-00014800: 756e 6971 7565 5f69 645d 203d 2065 7870  unique_id] = exp
-00014810: 616e 6465 645f 7469 6d65 2c20 6578 7061  anded_time, expa
-00014820: 6e64 6564 5f69 6e74 656e 7369 7479 2c20  nded_intensity, 
-00014830: 7866 5f73 616d 706c 652c 2066 6674 746f  xf_sample, fftto
-00014840: 7461 6c5f 7361 6d70 6c65 0d0a 2020 2020  tal_sample..    
-00014850: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00014860: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-00014870: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00014880: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00014890: 5f69 645d 203d 2020 6375 7272 656e 745f  _id] =  current_
-000148a0: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-000148b0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-000148c0: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-000148d0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-000148e0: 745f 756e 6971 7565 5f69 645d 203d 2063  t_unique_id] = c
-000148f0: 7572 7265 6e74 5f74 696d 652c 2063 7572  urrent_time, cur
-00014900: 7265 6e74 5f7a 2c20 6375 7272 656e 745f  rent_z, current_
-00014910: 792c 2063 7572 7265 6e74 5f78 2c20 6375  y, current_x, cu
-00014920: 7272 656e 745f 7261 6469 7573 2c20 6375  rrent_radius, cu
-00014930: 7272 656e 745f 766f 6c75 6d65 2c20 6375  rrent_volume, cu
-00014940: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00014950: 7479 5f63 6f6d 705f 6669 7273 742c 2063  ty_comp_first, c
-00014960: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00014970: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
-00014980: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
-00014990: 5f61 7265 610d 0a20 2020 2020 2020 2020  _area..         
-000149a0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000149b0: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-000149c0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
-000149d0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
-000149e0: 3d20 6375 7272 656e 745f 7469 6d65 2c20  = current_time, 
-000149f0: 6375 7272 656e 745f 7370 6565 642c 2063  current_speed, c
-00014a00: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
-00014a10: 676c 652c 2063 7572 7265 6e74 5f61 6363  gle, current_acc
-00014a20: 656c 6572 6174 696f 6e2c 2063 7572 7265  eleration, curre
-00014a30: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
-00014a40: 5f6d 6173 6b2c 2063 7572 7265 6e74 5f72  _mask, current_r
-00014a50: 6164 6961 6c5f 616e 676c 652c 2063 7572  adial_angle, cur
-00014a60: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
-00014a70: 6173 6b0d 0a20 2020 2020 2020 2020 2020  ask..           
-00014a80: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014a90: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
-00014aa0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
-00014ab0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
-00014ac0: 7175 655f 6964 3a75 6e69 7175 655f 6666  que_id:unique_ff
-00014ad0: 745f 7072 6f70 6572 7469 6573 5f74 7261  t_properties_tra
-00014ae0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
-00014af0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
-00014b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014b10: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
-00014b20: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
-00014b30: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
-00014b40: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00014b50: 643a 756e 6971 7565 5f63 6c75 7374 6572  d:unique_cluster
-00014b60: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00014b70: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00014b80: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
-00014b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ba0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
-00014bb0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
-00014bc0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00014bd0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00014be0: 3a75 6e69 7175 655f 7368 6170 655f 7072  :unique_shape_pr
-00014bf0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00014c00: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-00014c10: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
-00014c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014c30: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-00014c40: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-00014c50: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
-00014c60: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
-00014c70: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
-00014c80: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00014c90: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-00014ca0: 6964 5d7d 290d 0a0d 0a20 2020 2064 6566  id]})....    def
-00014cb0: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
-00014cc0: 5f73 706f 7473 2873 656c 662c 2066 7261  _spots(self, fra
-00014cd0: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
-00014ce0: 6c5f 6964 2c20 7472 6163 6b5f 6964 293a  l_id, track_id):
-00014cf0: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-00014d00: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
-00014d10: 2063 656e 7472 6f69 6473 2c20 6c61 6265   centroids, labe
-00014d20: 6c73 2c20 766f 6c75 6d65 2c20 696e 7465  ls, volume, inte
-00014d30: 6e73 6974 795f 6d65 616e 2c20 696e 7465  nsity_mean, inte
-00014d40: 6e73 6974 795f 746f 7461 6c2c 2062 6f75  nsity_total, bou
-00014d50: 6e64 696e 675f 626f 7865 7320 3d20 7365  nding_boxes = se
-00014d60: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
-00014d70: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
-00014d80: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
-00014d90: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
-00014da0: 2070 6978 656c 7465 7374 6c6f 6361 7469   pixeltestlocati
-00014db0: 6f6e 203d 2028 7a2c 792c 7829 0d0a 2020  on = (z,y,x)..  
-00014dc0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
-00014dd0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
-00014de0: 7279 2870 6978 656c 7465 7374 6c6f 6361  ry(pixeltestloca
-00014df0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
-00014e00: 2020 2020 2020 2062 626f 7820 3d20 626f         bbox = bo
-00014e10: 756e 6469 6e67 5f62 6f78 6573 5b69 6e64  unding_boxes[ind
-00014e20: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
-00014e30: 2073 697a 657a 203d 2061 6273 2862 626f   sizez = abs(bbo
-00014e40: 785b 305d 202d 2062 626f 785b 335d 290d  x[0] - bbox[3]).
-00014e50: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00014e60: 6579 203d 2061 6273 2862 626f 785b 315d  ey = abs(bbox[1]
-00014e70: 202d 2062 626f 785b 345d 290d 0a20 2020   - bbox[4])..   
-00014e80: 2020 2020 2020 2020 2073 697a 6578 203d           sizex =
-00014e90: 2061 6273 2862 626f 785b 325d 202d 2062   abs(bbox[2] - b
-00014ea0: 626f 785b 355d 2920 0d0a 2020 2020 2020  box[5]) ..      
-00014eb0: 2020 2020 2020 7665 746f 5f76 6f6c 756d        veto_volum
-00014ec0: 6520 3d20 7369 7a65 7820 2a20 7369 7a65  e = sizex * size
-00014ed0: 7920 2a20 7369 7a65 7a0d 0a20 2020 2020  y * sizez..     
-00014ee0: 2020 2020 2020 2076 6574 6f5f 7261 6469         veto_radi
-00014ef0: 7573 203d 206d 6174 682e 706f 7728 3320  us = math.pow(3 
-00014f00: 2a20 7665 746f 5f76 6f6c 756d 6520 2f20  * veto_volume / 
-00014f10: 2834 202a 206d 6174 682e 7069 292c 2031  (4 * math.pi), 1
-00014f20: 2e30 202f 2033 2e30 290d 0a0d 0a20 2020  .0 / 3.0)....   
-00014f30: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
-00014f40: 6e20 3d20 2863 656e 7472 6f69 6473 5b69  n = (centroids[i
-00014f50: 6e64 6578 5d5b 305d 202a 2073 656c 662e  ndex][0] * self.
-00014f60: 7a63 616c 6962 7261 7469 6f6e 2c20 6365  zcalibration, ce
-00014f70: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
-00014f80: 5d2a 7365 6c66 2e79 6361 6c69 6272 6174  ]*self.ycalibrat
-00014f90: 696f 6e2c 2063 656e 7472 6f69 6473 5b69  ion, centroids[i
-00014fa0: 6e64 6578 5d5b 325d 2a73 656c 662e 7863  ndex][2]*self.xc
-00014fb0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
-00014fc0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
-00014fd0: 203d 206d 6174 682e 706f 7728 766f 6c75   = math.pow(volu
-00014fe0: 6d65 5b69 6e64 6578 5d2c 2031 2e30 2f33  me[index], 1.0/3
-00014ff0: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
-00015000: 2052 4144 4955 5320 3d20 6d61 7468 2e70   RADIUS = math.p
-00015010: 6f77 2876 6f6c 756d 655b 696e 6465 785d  ow(volume[index]
-00015020: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
-00015030: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
-00015040: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
-00015050: 7a63 616c 6962 7261 7469 6f6e 2c20 312e  zcalibration, 1.
-00015060: 302f 332e 3029 200d 0a0d 0a20 2020 2020  0/3.0) ....     
-00015070: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00015080: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
-00015090: 656e 7472 6f69 6420 3d20 7365 6c66 2e5f  entroid = self._
-000150a0: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
-000150b0: 7428 6672 616d 652c 206c 6f63 6174 696f  t(frame, locatio
-000150c0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-000150d0: 6966 2064 6973 7420 3c3d 2032 202a 2076  if dist <= 2 * v
-000150e0: 6574 6f5f 7261 6469 7573 3a0d 0a20 2020  eto_radius:..   
-000150f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015100: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-00015110: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015120: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015140: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
-00015150: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
-00015160: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
-00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015180: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00015190: 203a 2069 6e74 2866 7261 6d65 292c 0d0a   : int(frame),..
-000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151b0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
-000151c0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-000151d0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-000151e0: 5b30 5d2a 2073 656c 662e 7a63 616c 6962  [0]* self.zcalib
-000151f0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-00015220: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
-00015230: 6964 735b 696e 6465 785d 5b31 5d2a 2073  ids[index][1]* s
-00015240: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-00015250: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00015260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015270: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
-00015280: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
-00015290: 6465 785d 5b32 5d2a 2073 656c 662e 7863  dex][2]* self.xc
-000152a0: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
-000152b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152c0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-000152d0: 6964 5f6b 6579 3a20 696e 7428 7472 6163  id_key: int(trac
-000152e0: 6b5f 6964 292c 0d0a 2020 2020 2020 2020  k_id),..        
-000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015300: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-00015310: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
-00015320: 7428 696e 7465 6e73 6974 795f 746f 7461  t(intensity_tota
-00015330: 6c5b 696e 6465 785d 2929 2c0d 0a20 2020  l[index])),..   
-00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015350: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
-00015360: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
-00015370: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
-00015380: 6d65 616e 5b69 6e64 6578 5d29 292c 0d0a  mean[index])),..
-00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153a0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-000153b0: 6975 735f 6b65 7920 3a20 2866 6c6f 6174  ius_key : (float
-000153c0: 2852 4144 4955 5329 292c 0d0a 2020 2020  (RADIUS)),..    
-000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153e0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
-000153f0: 5f6b 6579 203a 2028 666c 6f61 7428 5155  _key : (float(QU
-00015400: 414c 4954 5929 292c 0d0a 2020 2020 2020  ALITY)),..      
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 2020 7365 6c66 2e64 6973 7461 6e63 655f    self.distance_
-00015430: 6365 6c6c 5f6d 6173 6b5f 6b65 793a 2066  cell_mask_key: f
-00015440: 6c6f 6174 2864 6973 7461 6e63 655f 6365  loat(distance_ce
-00015450: 6c6c 5f6d 6173 6b29 2c0d 0a20 2020 2020  ll_mask),..     
-00015460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015470: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
-00015480: 726f 6964 5f7a 5f6b 6579 3a20 666c 6f61  roid_z_key: floa
-00015490: 7428 6d61 736b 6365 6e74 726f 6964 5b30  t(maskcentroid[0
-000154a0: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
-000154b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000154c0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
-000154d0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-000154e0: 6365 6e74 726f 6964 5b31 5d29 2c0d 0a20  centroid[1]),.. 
-000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015500: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-00015510: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
-00015520: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
-00015530: 6964 5b32 5d29 200d 0a0d 0a20 2020 2020  id[2]) ....     
-00015540: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00015550: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00015560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015570: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-00015580: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-00015590: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-000155a0: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
-000155b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000155c0: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
-000155d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000155e0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-000155f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015600: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
-00015610: 6528 7b73 656c 662e 746f 7461 6c5f 696e  e({self.total_in
-00015620: 7465 6e73 6974 795f 6b65 793a 202d 317d  tensity_key: -1}
-00015630: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015640: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00015650: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-00015660: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-00015670: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
-00015680: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-00015690: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
-000156a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000156b0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-000156c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000156d0: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
-000156e0: 7465 287b 7365 6c66 2e72 6164 6975 735f  te({self.radius_
-000156f0: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
-00015700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015710: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-00015720: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015730: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
-00015740: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
-00015750: 5f6b 6579 3a20 2d31 7d29 0d0a 0d0a 0d0a  _key: -1})......
-00015760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015780: 2020 200d 0a20 2020 2064 6566 205f 6469     ..    def _di
-00015790: 6374 5f75 7064 6174 6528 7365 6c66 2c20  ct_update(self, 
-000157a0: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
-000157b0: 6964 733a 204c 6973 742c 2020 6365 6c6c  ids: List,  cell
-000157c0: 5f69 643a 2069 6e74 2c20 7472 6163 6b5f  _id: int, track_
-000157d0: 6964 3a20 696e 742c 2073 6f75 7263 655f  id: int, source_
-000157e0: 6964 3a20 696e 742c 2074 6172 6765 745f  id: int, target_
-000157f0: 6964 3a20 696e 7429 3a0d 0a0d 0a20 0d0a  id: int):.... ..
-00015800: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
-00015810: 6f6e 5f69 6420 3d20 7365 6c66 2e67 656e  on_id = self.gen
-00015820: 6572 6174 696f 6e5f 6469 6374 5b63 656c  eration_dict[cel
-00015830: 6c5f 6964 5d0d 0a20 2020 2020 2020 2074  l_id]..        t
-00015840: 7261 636b 6c65 745f 6964 203d 2073 656c  racklet_id = sel
-00015850: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
-00015860: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
-00015870: 200d 0a0d 0a20 2020 2020 2020 2075 6e69   ....        uni
-00015880: 7175 655f 6964 203d 2073 7472 2874 7261  que_id = str(tra
-00015890: 636b 5f69 6429 202b 2020 7374 7228 6765  ck_id) +  str(ge
-000158a0: 6e65 7261 7469 6f6e 5f69 6429 202b 2073  neration_id) + s
-000158b0: 7472 2874 7261 636b 6c65 745f 6964 290d  tr(tracklet_id).
-000158c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000158d0: 2020 2076 6563 5f6d 6173 6b20 3d20 5b66     vec_mask = [f
-000158e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000158f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015900: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00015910: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-00015920: 5f78 5f6b 6579 5d29 2c20 666c 6f61 7428  _x_key]), float(
-00015930: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015940: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015950: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00015960: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
-00015970: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
-00015980: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015990: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000159a0: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
-000159b0: 6e74 726f 6964 5f7a 5f6b 6579 5d29 205d  ntroid_z_key]) ]
-000159c0: 0d0a 0d0a 2020 2020 2020 2020 7665 635f  ....        vec_
-000159d0: 6365 6c6c 203d 205b 666c 6f61 7428 7365  cell = [float(se
-000159e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000159f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015a00: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
-00015a10: 7369 645f 6b65 795d 2920 2c20 0d0a 2020  sid_key]) , ..  
-00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a30: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00015a40: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015a50: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015a60: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
-00015a70: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
-00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a90: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00015aa0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00015ab0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015ac0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
-00015ad0: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a0d  zposid_key])]...
-00015ae0: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
-00015af0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
-00015b00: 7665 635f 6d61 736b 2c20 7665 635f 6365  vec_mask, vec_ce
-00015b10: 6c6c 290d 0a0d 0a20 2020 2020 2020 2073  ll)....        s
-00015b20: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015b30: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00015b40: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00015b50: 7b73 656c 662e 7261 6469 616c 5f61 6e67  {self.radial_ang
-00015b60: 6c65 5f6b 6579 203a 2061 6e67 6c65 7d29  le_key : angle})
-00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b80: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00015b90: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
-00015ba0: 6964 732e 6170 7065 6e64 2873 7472 2875  ids.append(str(u
-00015bb0: 6e69 7175 655f 6964 2929 0d0a 2020 2020  nique_id))..    
-00015bc0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015bd0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015be0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015bf0: 6461 7465 287b 7365 6c66 2e75 6e69 7175  date({self.uniqu
-00015c00: 6569 645f 6b65 7920 3a20 7374 7228 756e  eid_key : str(un
-00015c10: 6971 7565 5f69 6429 7d29 0d0a 2020 2020  ique_id)})..    
-00015c20: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015c30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015c40: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015c50: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
-00015c60: 6c65 7469 645f 6b65 7920 3a20 7374 7228  letid_key : str(
-00015c70: 7472 6163 6b6c 6574 5f69 6429 7d29 200d  tracklet_id)}) .
-00015c80: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00015c90: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015ca0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015cb0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015cc0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
-00015cd0: 203a 2073 7472 2867 656e 6572 6174 696f   : str(generatio
-00015ce0: 6e5f 6964 297d 2920 0d0a 2020 2020 2020  n_id)}) ..      
-00015cf0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015d00: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015d10: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015d20: 7465 287b 7365 6c66 2e74 7261 636b 6964  te({self.trackid
-00015d30: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
-00015d40: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
-00015d50: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015d60: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015d70: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015d80: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
-00015d90: 676c 655f 6b65 7920 3a20 302e 307d 290d  gle_key : 0.0}).
-00015da0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00015db0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015dc0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015dd0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015de0: 7370 6565 645f 6b65 7920 3a20 302e 307d  speed_key : 0.0}
-00015df0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00015e00: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015e10: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015e20: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015e30: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-00015e40: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
-00015e50: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015e60: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015e70: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015e80: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
-00015e90: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00015ea0: 7374 6b65 7920 3a20 2d31 7d29 0d0a 2020  stkey : -1})..  
-00015eb0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015ec0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015ed0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015ee0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00015ef0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00015f00: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
-00015f10: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00015f20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015f30: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015f40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015f50: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-00015f60: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00015f70: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015f80: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015f90: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015fa0: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
-00015fb0: 5f6d 6173 6b5f 6b65 7920 3a20 2d31 7d29  _mask_key : -1})
-00015fc0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
-00015fd0: 6f75 7263 655f 6964 2069 7320 6e6f 7420  ource_id is not 
-00015fe0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00015ff0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00016000: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016010: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00016020: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
-00016030: 6964 5f6b 6579 203a 2069 6e74 2873 6f75  id_key : int(sou
-00016040: 7263 655f 6964 297d 290d 0a20 2020 2020  rce_id)})..     
-00016050: 2020 2020 2020 2076 6563 5f31 203d 205b         vec_1 = [
-00016060: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00016070: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016080: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00016090: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-000160a0: 2920 2d20 666c 6f61 7428 7365 6c66 2e75  ) - float(self.u
-000160b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000160c0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
-000160d0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-000160e0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016100: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00016110: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016120: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00016130: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
-00016140: 6964 5f6b 6579 5d29 202d 2066 6c6f 6174  id_key]) - float
-00016150: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-00016160: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00016170: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-00016180: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
-00016190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000161a0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-000161b0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000161c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000161d0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-000161e0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
-000161f0: 2d20 2066 6c6f 6174 2873 656c 662e 756e  -  float(self.un
-00016200: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016210: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00016220: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00016230: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
-00016240: 2020 2020 2073 7065 6564 203d 206e 702e       speed = np.
-00016250: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
-00016260: 312c 2076 6563 5f31 2929 2f73 656c 662e  1, vec_1))/self.
-00016270: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
-00016280: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00016290: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000162a0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000162b0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000162c0: 2e73 7065 6564 5f6b 6579 203a 2073 7065  .speed_key : spe
-000162d0: 6564 7d29 0d0a 0d0a 2020 2020 2020 2020  ed})....        
-000162e0: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-000162f0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00016300: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
-00016310: 3129 0d0a 0d0a 2020 2020 2020 2020 2020  1)....          
-00016320: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016330: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016340: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016350: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
-00016360: 616e 676c 655f 6b65 7920 3a20 6d6f 7469  angle_key : moti
-00016370: 6f6e 5f61 6e67 6c65 7d29 200d 0a0d 0a20  on_angle}) .... 
-00016380: 2020 2020 2020 2020 2020 2069 6620 736f             if so
-00016390: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
-000163a0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-000163b0: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-000163c0: 2020 2020 2020 2020 2070 7265 5f73 6f75           pre_sou
-000163d0: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
-000163e0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
-000163f0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
-00016400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016410: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016420: 2020 2020 2020 2076 6563 5f32 203d 205b         vec_2 = [
-00016430: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00016440: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016450: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00016460: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00016470: 2920 2d20 3220 2a20 666c 6f61 7428 7365  ) - 2 * float(se
-00016480: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016490: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
-000164a0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
-000164b0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
-000164c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000164d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000164e0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
-000164f0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00016500: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
-00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016520: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-00016530: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016540: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00016550: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
-00016560: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
-00016570: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016580: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016590: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-000165a0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-000165b0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-000165c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000165d0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-000165e0: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
-000165f0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016610: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00016620: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016630: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016640: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
-00016650: 706f 7369 645f 6b65 795d 2920 2d20 2032  posid_key]) -  2
-00016660: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
-00016670: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016680: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-00016690: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-000166a0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
-000166b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000166c0: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
-000166d0: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
-000166e0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-000166f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016700: 2020 2020 2020 2061 6363 203d 206e 702e         acc = np.
-00016710: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
-00016720: 322c 2076 6563 5f32 2929 2f73 656c 662e  2, vec_2))/self.
-00016730: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
-00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016750: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00016760: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00016770: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016780: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00016790: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
-000167a0: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
-000167b0: 3a20 6163 637d 290d 0a20 2020 2020 2020  : acc})..       
-000167c0: 2065 6c69 6620 736f 7572 6365 5f69 6420   elif source_id 
-000167d0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
-000167e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000167f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016800: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00016810: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
-00016820: 6f72 6569 645f 6b65 7920 3a20 4e6f 6e65  oreid_key : None
-00016830: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
-00016840: 200d 0a0d 0a20 2020 2020 2020 2069 6620   ....        if 
-00016850: 7461 7267 6574 5f69 6420 6973 206e 6f74  target_id is not
-00016860: 204e 6f6e 653a 2020 2020 2020 200d 0a20   None:       .. 
-00016870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016880: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016890: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000168a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000168b0: 662e 6166 7465 7269 645f 6b65 7920 3a20  f.afterid_key : 
-000168c0: 696e 7428 7461 7267 6574 5f69 6429 7d29  int(target_id)})
-000168d0: 200d 0a20 2020 2020 2020 2065 6c69 6620   ..        elif 
-000168e0: 7461 7267 6574 5f69 6420 6973 204e 6f6e  target_id is Non
-000168f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00016900: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016910: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016920: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00016930: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
-00016940: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
-00016950: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00016960: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
-00016970: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
-00016980: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
-00016990: 2920 2020 200d 0a0d 0a0d 0a20 2020 2064  )    ......    d
-000169a0: 6566 205f 7465 6d70 6f72 616c 5f70 6c6f  ef _temporal_plo
-000169b0: 7473 5f74 7261 636b 6d61 7465 2873 656c  ts_trackmate(sel
-000169c0: 6629 3a0d 0a20 2020 200d 0a20 2020 200d  f):..    ..    .
-000169d0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
-000169e0: 2020 2020 2020 2073 656c 662e 4174 7472         self.Attr
-000169f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00016a00: 2020 2020 2020 2073 7461 7274 7469 6d65         starttime
-00016a10: 203d 2069 6e74 286d 696e 2873 656c 662e   = int(min(self.
-00016a20: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
-00016a30: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
-00016a40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00016a50: 6e64 7469 6d65 203d 2069 6e74 286d 6178  ndtime = int(max
-00016a60: 2873 656c 662e 416c 6c56 616c 7565 735b  (self.AllValues[
-00016a70: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00016a80: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
-00016a90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00016aa0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00016ab0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00016ac0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00016ad0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
-00016ae0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016af0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016b00: 7469 635f 7661 725f 6469 7370 5f7a 203d  tic_var_disp_z =
-00016b10: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016b20: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016b30: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
-00016b40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016b50: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016b60: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
-00016b70: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016b80: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016b90: 6963 5f6d 6561 6e5f 6469 7370 5f78 203d  ic_mean_disp_x =
-00016ba0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016bb0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016bc0: 635f 7661 725f 6469 7370 5f78 203d 205b  c_var_disp_x = [
-00016bd0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00016be0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016bf0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
-00016c00: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016c10: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016c20: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00016c30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016c40: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016c50: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
-00016c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016c70: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00016c80: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
-00016c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ca0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00016cb0: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
-00016cc0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016cd0: 662e 6d69 746f 7469 635f 7661 725f 6163  f.mitotic_var_ac
-00016ce0: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-00016cf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00016d00: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
-00016d10: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
-00016d20: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016d30: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00016d40: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
-00016d50: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
-00016d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d70: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00016d80: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
-00016d90: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
-00016da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016db0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00016dc0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00016dd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016de0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00016df0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00016e00: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
-00016e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016e20: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016e30: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
-00016e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016e50: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00016e60: 6d65 616e 5f64 6973 705f 7920 3d20 5b5d  mean_disp_y = []
-00016e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016e80: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00016e90: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
-00016ea0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016eb0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00016ec0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00016ed0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-00016ee0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00016ef0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00016f00: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
-00016f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016f20: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00016f30: 616e 5f72 6164 6975 7320 3d20 5b5d 0d0a  an_radius = []..
-00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f50: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016f60: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00016f70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016f80: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00016f90: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
-00016fa0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016fb0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00016fc0: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
-00016fd0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016fe0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00016ff0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f61  n_mitotic_mean_a
-00017000: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00017010: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017020: 6e5f 6d69 746f 7469 635f 7661 725f 6163  n_mitotic_var_ac
-00017030: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-00017040: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00017050: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00017060: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00017070: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
-00017080: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017090: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000170a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000170b0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000170c0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000170d0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-000170e0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000170f0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00017100: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017110: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00017120: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00017130: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00017140: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017150: 5f6d 6561 6e5f 6469 7370 5f7a 203d 205b  _mean_disp_z = [
-00017160: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017170: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00017180: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
-00017190: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000171a0: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
-000171b0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
-000171c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000171d0: 6c6c 5f76 6172 5f64 6973 705f 7920 3d20  ll_var_disp_y = 
-000171e0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-000171f0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00017200: 6561 6e5f 6469 7370 5f78 203d 205b 5d0d  ean_disp_x = [].
-00017210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017220: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00017230: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
-00017240: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017250: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
-00017260: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00017270: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017280: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
-00017290: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000172a0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-000172b0: 6e5f 7370 6565 6420 3d20 5b5d 0d0a 2020  n_speed = []..  
-000172c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000172d0: 6c66 2e61 6c6c 5f76 6172 5f73 7065 6564  lf.all_var_speed
-000172e0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000172f0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017300: 6c5f 6d65 616e 5f61 6363 203d 205b 5d0d  l_mean_acc = [].
-00017310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017320: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
-00017330: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
-00017340: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00017350: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
-00017360: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00017370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017380: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00017390: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000173a0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000173b0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000173c0: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
-000173d0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
-00017400: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00017410: 3d20 5b5d 0d0a 0d0a 0d0a 2020 2020 2020  = []......      
-00017420: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00017430: 6f74 735f 7472 6163 6b73 203d 207b 7d0d  ots_tracks = {}.
-00017440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017450: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00017460: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00017470: 726f 7065 7274 6965 732e 6974 656d 7328  roperties.items(
-00017480: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00017490: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 616c 6c5f 7370 6f74 7320 3d20 7365    all_spots = se
-000174c0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-000174d0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
-000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174f0: 2020 2020 6966 2073 656c 662e 7472 6163      if self.trac
-00017500: 6b69 645f 6b65 7920 696e 2061 6c6c 5f73  kid_key in all_s
-00017510: 706f 7473 3a0d 0a20 2020 2020 2020 2020  pots:..         
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00017540: 735b 6b5d 203d 2061 6c6c 5f73 706f 7473  s[k] = all_spots
-00017550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017560: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00017570: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00017580: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
-00017590: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000175a0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-000175b0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-000175c0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-000175d0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-000175e0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-000175f0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00017620: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00017630: 6e20 7471 646d 2872 616e 6765 2873 7461  n tqdm(range(sta
-00017640: 7274 7469 6d65 2c20 656e 6474 696d 6529  rttime, endtime)
-00017650: 2c20 746f 7461 6c3d 656e 6474 696d 6520  , total=endtime 
-00017660: 2d20 7374 6172 7474 696d 6529 3a0d 0a20  - starttime):.. 
-00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017680: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017690: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000176a0: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-000176b0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-000176c0: 6c66 2e5f 636f 6d70 7574 655f 7465 6d70  lf._compute_temp
-000176d0: 6f72 616c 2c20 692c 2061 6c6c 5f73 706f  oral, i, all_spo
-000176e0: 7473 5f74 7261 636b 7329 290d 0a20 0d0a  ts_tracks)).. ..
-000176f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017700: 2020 2020 5b72 2e72 6573 756c 7428 2920      [r.result() 
-00017710: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
-00017720: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
-00017730: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
-00017740: 295d 0d0a 0d0a 0d0a 2020 2020 6465 6620  )]......    def 
-00017750: 5f63 6f6d 7075 7465 5f74 656d 706f 7261  _compute_tempora
-00017760: 6c28 7365 6c66 2c20 692c 2061 6c6c 5f73  l(self, i, all_s
-00017770: 706f 7473 5f74 7261 636b 7329 3a20 2020  pots_tracks):   
-00017780: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-000177b0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
-000177c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000177d0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-000177e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000177f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017800: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00017810: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017820: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00017830: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017840: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
-00017850: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00017860: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017870: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-00017880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017890: 2020 2020 206d 6974 6f74 6963 5f64 6972       mitotic_dir
-000178a0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000178b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000178c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000178d0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-000178e0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00017910: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00017920: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017930: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00017940: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017950: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017960: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-00017970: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017980: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00017990: 7469 635f 7261 6469 7573 203d 205b 5d0d  tic_radius = [].
-000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000179c0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179e0: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
-000179f0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017a00: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017a10: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00017a20: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00017a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a40: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017a50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017a60: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
-00017a70: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
-00017aa0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012f50: 2020 2020 2020 2020 0d0a 0d0a 0d0a 0d0a          ........
+00012f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fa0: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00012fb0: 7365 6c66 2e72 6f6f 745f 7370 6f74 732e  self.root_spots.
+00012fc0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012ff0: 2e72 6f6f 745f 7370 6f74 735b 6b5d 203d  .root_spots[k] =
+00013000: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00013010: 745f 7072 6f70 6572 7469 6573 5b6b 5d20  t_properties[k] 
+00013020: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013030: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013040: 6465 6620 5f63 6f6d 7075 7465 5f70 6865  def _compute_phe
+00013050: 6e6f 7479 7065 7328 7365 6c66 293a 0d0a  notypes(self):..
+00013060: 0d0a 2020 2020 2020 2020 2020 666f 7220  ..          for 
+00013070: 286b 2c76 2920 696e 2073 656c 662e 756e  (k,v) in self.un
+00013080: 6971 7565 5f74 7261 636b 732e 6974 656d  ique_tracks.item
+00013090: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+000130a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000130b0: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+000130c0: 203d 206b 0d0a 2020 2020 2020 2020 2020   = k..          
+000130d0: 2020 2020 2020 7472 6163 6b6c 6574 5f70        tracklet_p
+000130e0: 726f 7065 7274 6965 7320 3d20 7365 6c66  roperties = self
+000130f0: 2e75 6e69 7175 655f 7472 6163 6b5f 7072  .unique_track_pr
+00013100: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
+00013110: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00013120: 636b 7320 3d20 7365 6c66 2e75 6e69 7175  cks = self.uniqu
+00013130: 655f 7472 6163 6b73 5b6b 5d0d 0a20 2020  e_tracks[k]..   
+00013140: 2020 2020 2020 2020 2020 2020 205a 203d               Z =
+00013150: 2074 7261 636b 735b 3a2c 325d 0d0a 2020   tracks[:,2]..  
+00013160: 2020 2020 2020 2020 2020 2020 2020 5920                Y 
+00013170: 3d20 7472 6163 6b73 5b3a 2c33 5d0d 0a20  = tracks[:,3].. 
+00013180: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+00013190: 203d 2074 7261 636b 735b 3a2c 345d 0d0a   = tracks[:,4]..
+000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131b0: 7469 6d65 203d 2074 7261 636b 6c65 745f  time = tracklet_
+000131c0: 7072 6f70 6572 7469 6573 5b3a 2c30 5d0d  properties[:,0].
+000131d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000131e0: 2075 6e69 7175 655f 6964 7320 3d20 7472   unique_ids = tr
+000131f0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00013200: 735b 3a2c 315d 0d0a 2020 2020 2020 2020  s[:,1]..        
+00013210: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+00013220: 6473 5f73 6574 203d 2073 6574 2875 6e69  ds_set = set(uni
+00013230: 7175 655f 6964 7329 0d0a 2020 2020 2020  que_ids)..      
+00013240: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+00013250: 7469 6f6e 5f69 6473 203d 2074 7261 636b  tion_ids = track
+00013260: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00013270: 2c32 5d0d 0a20 2020 2020 2020 2020 2020  ,2]..           
+00013280: 2020 2020 2072 6164 6975 7320 3d20 7472       radius = tr
+00013290: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000132a0: 735b 3a2c 335d 0d0a 2020 2020 2020 2020  s[:,3]..        
+000132b0: 2020 2020 2020 2020 766f 6c75 6d65 203d          volume =
+000132c0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+000132d0: 7469 6573 5b3a 2c34 5d0d 0a20 2020 2020  ties[:,4]..     
+000132e0: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
+000132f0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00013300: 7374 203d 2074 7261 636b 6c65 745f 7072  st = tracklet_pr
+00013310: 6f70 6572 7469 6573 5b3a 2c35 5d0d 0a20  operties[:,5].. 
+00013320: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00013330: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013340: 5f73 6563 6f6e 6420 3d20 7472 6163 6b6c  _second = trackl
+00013350: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+00013360: 365d 0d0a 2020 2020 2020 2020 2020 2020  6]..            
+00013370: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+00013380: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00013390: 6572 7469 6573 5b3a 2c37 5d0d 0a20 2020  erties[:,7]..   
+000133a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000133b0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000133c0: 7465 6e73 6974 7920 3d20 7472 6163 6b6c  tensity = trackl
+000133d0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000133e0: 385d 0d0a 2020 2020 2020 2020 2020 2020  8]..            
+000133f0: 2020 2020 7370 6565 6420 3d20 7472 6163      speed = trac
+00013400: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00013410: 3a2c 395d 0d0a 2020 2020 2020 2020 2020  :,9]..          
+00013420: 2020 2020 2020 6d6f 7469 6f6e 5f61 6e67        motion_ang
+00013430: 6c65 203d 2074 7261 636b 6c65 745f 7072  le = tracklet_pr
+00013440: 6f70 6572 7469 6573 5b3a 2c31 305d 0d0a  operties[:,10]..
+00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013460: 6163 6365 6c65 7261 7469 6f6e 203d 2074  acceleration = t
+00013470: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00013480: 6573 5b3a 2c31 315d 0d0a 2020 2020 2020  es[:,11]..      
+00013490: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+000134a0: 6365 5f63 656c 6c5f 6d61 736b 203d 2074  ce_cell_mask = t
+000134b0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000134c0: 6573 5b3a 2c31 325d 0d0a 2020 2020 2020  es[:,12]..      
+000134d0: 2020 2020 2020 2020 2020 7261 6469 616c            radial
+000134e0: 5f61 6e67 6c65 203d 2074 7261 636b 6c65  _angle = trackle
+000134f0: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
+00013500: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
+00013510: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+00013520: 736b 203d 2074 7261 636b 6c65 745f 7072  sk = tracklet_pr
+00013530: 6f70 6572 7469 6573 5b3a 2c31 345d 0d0a  operties[:,14]..
+00013540: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00013550: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00013560: 2020 2020 2020 756e 6971 7565 5f66 6674        unique_fft
+00013570: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013580: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
+00013590: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+000135a0: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
+000135b0: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
+000135c0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+000135d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000135e0: 6666 745f 7072 6f70 6572 7469 6573 5b74  fft_properties[t
+000135f0: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
+00013600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013610: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00013620: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
+00013630: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 0d0a  ack_id] = {}....
+00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013650: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00013660: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00013670: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00013680: 2020 2020 2020 2075 6e69 7175 655f 6479         unique_dy
+00013690: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
+000136a0: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
+000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136c0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+000136d0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
+000136e0: 636b 5f69 645d 203d 207b 7d0d 0a20 2020  ck_id] = {}..   
+000136f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013700: 662e 756e 6971 7565 5f64 796e 616d 6963  f.unique_dynamic
+00013710: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+00013720: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
+00013730: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+00013740: 6e64 6564 5f74 696d 6520 3d20 6e70 2e7a  nded_time = np.z
+00013750: 6572 6f73 2873 656c 662e 7465 6e64 202d  eros(self.tend -
+00013760: 2073 656c 662e 7473 7461 7274 202b 2031   self.tstart + 1
+00013770: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013780: 2020 2070 6f69 6e74 5f73 616d 706c 6520     point_sample 
+00013790: 3d20 6578 7061 6e64 6564 5f74 696d 652e  = expanded_time.
+000137a0: 7368 6170 655b 305d 0d0a 2020 2020 2020  shape[0]..      
+000137b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000137c0: 696e 2072 616e 6765 286c 656e 2865 7870  in range(len(exp
+000137d0: 616e 6465 645f 7469 6d65 2929 3a0d 0a20  anded_time)):.. 
+000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137f0: 2020 2020 2020 6578 7061 6e64 6564 5f74        expanded_t
+00013800: 696d 655b 695d 203d 2069 200d 0a20 2020  ime[i] = i ..   
+00013810: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00013820: 2063 7572 7265 6e74 5f75 6e69 7175 655f   current_unique_
+00013830: 6964 2069 6e20 756e 6971 7565 5f69 6473  id in unique_ids
+00013840: 5f73 6574 3a0d 0a20 2020 2020 2020 2020  _set:..         
+00013850: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013860: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00013870: 7870 616e 6465 645f 696e 7465 6e73 6974  xpanded_intensit
+00013880: 7920 3d20 6e70 2e7a 6572 6f73 2873 656c  y = np.zeros(sel
+00013890: 662e 7465 6e64 202d 2073 656c 662e 7473  f.tend - self.ts
+000138a0: 7461 7274 202b 2031 290d 0a20 2020 2020  tart + 1)..     
+000138b0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000138e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000138f0: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
+00013900: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013910: 7272 656e 745f 7a20 3d20 5b5d 0d0a 2020  rrent_z = []..  
+00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013930: 2063 7572 7265 6e74 5f79 203d 205b 5d0d   current_y = [].
+00013940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013950: 2020 2020 6375 7272 656e 745f 7820 3d20      current_x = 
+00013960: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00013970: 2020 2020 2020 2063 7572 7265 6e74 5f69         current_i
+00013980: 6e74 656e 7369 7479 203d 205b 5d0d 0a20  ntensity = [].. 
+00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139a0: 2020 6375 7272 656e 745f 7261 6469 7573    current_radius
+000139b0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000139c0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+000139d0: 745f 766f 6c75 6d65 203d 205b 5d0d 0a20  t_volume = [].. 
+000139e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139f0: 2020 6375 7272 656e 745f 7370 6565 6420    current_speed 
+00013a00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00013a10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013a20: 5f6d 6f74 696f 6e5f 616e 676c 6520 3d20  _motion_angle = 
+00013a30: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00013a40: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00013a50: 6363 656c 6572 6174 696f 6e20 3d20 5b5d  cceleration = []
+00013a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013a70: 2020 2020 2063 7572 7265 6e74 5f64 6973       current_dis
+00013a80: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00013a90: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00013aa0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013ab0: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00013ac0: 6d70 5f66 6972 7374 203d 205b 5d0d 0a20  mp_first = [].. 
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ae0: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00013af0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00013b00: 6e64 203d 205b 5d0d 0a20 2020 2020 2020  nd = []..       
+00013b10: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013b20: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
+00013b30: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00013b40: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013b50: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00013b60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00013b70: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013b80: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
+00013b90: 203d 205b 5d20 0d0a 2020 2020 2020 2020   = [] ..        
+00013ba0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bc0: 666f 7220 6a20 696e 2072 616e 6765 2874  for j in range(t
+00013bd0: 696d 652e 7368 6170 655b 305d 293a 0d0a  ime.shape[0]):..
+00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bf0: 2020 2020 2020 2020 2020 6966 2063 7572            if cur
+00013c00: 7265 6e74 5f75 6e69 7175 655f 6964 203d  rent_unique_id =
+00013c10: 3d20 756e 6971 7565 5f69 6473 5b6a 5d3a  = unique_ids[j]:
+00013c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c40: 2020 2063 7572 7265 6e74 5f74 696d 652e     current_time.
+00013c50: 6170 7065 6e64 2874 696d 655b 6a5d 290d  append(time[j]).
+00013c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2020 6375 7272 656e 745f 7a2e 6170 7065    current_z.appe
+00013c90: 6e64 285a 5b6a 5d29 0d0a 2020 2020 2020  nd(Z[j])..      
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cb0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013cc0: 6e74 5f79 2e61 7070 656e 6428 595b 6a5d  nt_y.append(Y[j]
+00013cd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cf0: 2020 2020 6375 7272 656e 745f 782e 6170      current_x.ap
+00013d00: 7065 6e64 2858 5b6a 5d29 0d0a 2020 2020  pend(X[j])..    
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00013d30: 616e 6465 645f 696e 7465 6e73 6974 795b  anded_intensity[
+00013d40: 696e 7428 7469 6d65 5b6a 5d29 5d20 3d20  int(time[j])] = 
+00013d50: 696e 7465 6e73 6974 795b 6a5d 0d0a 2020  intensity[j]..  
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013d80: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
+00013d90: 2e61 7070 656e 6428 696e 7465 6e73 6974  .append(intensit
+00013da0: 795b 6a5d 290d 0a20 2020 2020 2020 2020  y[j])..         
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dc0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013dd0: 7261 6469 7573 2e61 7070 656e 6428 7261  radius.append(ra
+00013de0: 6469 7573 5b6a 5d29 0d0a 2020 2020 2020  dius[j])..      
+00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e00: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013e10: 6e74 5f76 6f6c 756d 652e 6170 7065 6e64  nt_volume.append
+00013e20: 2876 6f6c 756d 655b 6a5d 290d 0a20 2020  (volume[j])..   
+00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e40: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013e50: 7272 656e 745f 7370 6565 642e 6170 7065  rrent_speed.appe
+00013e60: 6e64 2873 7065 6564 5b6a 5d29 0d0a 2020  nd(speed[j])..  
+00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013e90: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
+00013ea0: 676c 652e 6170 7065 6e64 286d 6f74 696f  gle.append(motio
+00013eb0: 6e5f 616e 676c 655b 6a5d 290d 0a20 2020  n_angle[j])..   
+00013ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ed0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013ee0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00013ef0: 6f6e 2e61 7070 656e 6428 6163 6365 6c65  on.append(accele
+00013f00: 7261 7469 6f6e 5b6a 5d29 0d0a 2020 2020  ration[j])..    
+00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f20: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013f30: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+00013f40: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 2864  ll_mask.append(d
+00013f50: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00013f60: 6b5b 6a5d 290d 0a20 2020 2020 2020 2020  k[j])..         
+00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f80: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013f90: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013fa0: 705f 6669 7273 742e 6170 7065 6e64 2865  p_first.append(e
+00013fb0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013fc0: 5f66 6972 7374 5b6a 5d29 0d0a 2020 2020  _first[j])..    
+00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fe0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013ff0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00014000: 795f 636f 6d70 5f73 6563 6f6e 642e 6170  y_comp_second.ap
+00014010: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
+00014020: 795f 636f 6d70 5f73 6563 6f6e 645b 6a5d  y_comp_second[j]
+00014030: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014050: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
+00014060: 6163 655f 6172 6561 2e61 7070 656e 6428  ace_area.append(
+00014070: 7375 7266 6163 655f 6172 6561 5b6a 5d29  surface_area[j])
+00014080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140a0: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
+000140b0: 6c5f 616e 676c 652e 6170 7065 6e64 2872  l_angle.append(r
+000140c0: 6164 6961 6c5f 616e 676c 655b 6a5d 290d  adial_angle[j]).
+000140d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000140e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140f0: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
+00014100: 7869 735f 6d61 736b 2e61 7070 656e 6428  xis_mask.append(
+00014110: 6365 6c6c 5f61 7869 735f 6d61 736b 5b6a  cell_axis_mask[j
+00014120: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00014130: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00014140: 696d 6520 3d20 6e70 2e61 7361 7272 6179  ime = np.asarray
+00014150: 2863 7572 7265 6e74 5f74 696d 652c 2064  (current_time, d
+00014160: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014180: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
+00014190: 656e 7369 7479 203d 206e 702e 6173 6172  ensity = np.asar
+000141a0: 7261 7928 6375 7272 656e 745f 696e 7465  ray(current_inte
+000141b0: 6e73 6974 792c 2064 7479 7065 3d6e 702e  nsity, dtype=np.
+000141c0: 666c 6f61 7433 3229 0d0a 0d0a 0d0a 0d0a  float32)........
+000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141e0: 2020 2063 7572 7265 6e74 5f72 6164 6975     current_radiu
+000141f0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
+00014200: 7572 7265 6e74 5f72 6164 6975 732c 2064  urrent_radius, d
+00014210: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014230: 2020 2020 2063 7572 7265 6e74 5f76 6f6c       current_vol
+00014240: 756d 6520 3d20 6e70 2e61 7361 7272 6179  ume = np.asarray
+00014250: 2863 7572 7265 6e74 5f76 6f6c 756d 652c  (current_volume,
+00014260: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00014270: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00014280: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+00014290: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+000142a0: 5f66 6972 7374 203d 206e 702e 6173 6172  _first = np.asar
+000142b0: 7261 7928 6375 7272 656e 745f 6563 6365  ray(current_ecce
+000142c0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+000142d0: 7273 742c 2064 7479 7065 3d6e 702e 666c  rst, dtype=np.fl
+000142e0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+000142f0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014300: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00014310: 636f 6d70 5f73 6563 6f6e 6420 3d20 6e70  comp_second = np
+00014320: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00014330: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00014340: 6d70 5f73 6563 6f6e 642c 2064 7479 7065  mp_second, dtype
+00014350: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014370: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
+00014380: 5f61 7265 6120 3d20 6e70 2e61 7361 7272  _area = np.asarr
+00014390: 6179 2863 7572 7265 6e74 5f73 7572 6661  ay(current_surfa
+000143a0: 6365 5f61 7265 612c 2064 7479 7065 3d6e  ce_area, dtype=n
+000143b0: 702e 666c 6f61 7433 3229 0d0a 0d0a 2020  p.float32)....  
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2063 7572 7265 6e74 5f73 7065 6564 203d   current_speed =
+000143e0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+000143f0: 656e 745f 7370 6565 642c 2064 7479 7065  ent_speed, dtype
+00014400: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014420: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
+00014430: 616e 676c 6520 3d20 6e70 2e61 7361 7272  angle = np.asarr
+00014440: 6179 2863 7572 7265 6e74 5f6d 6f74 696f  ay(current_motio
+00014450: 6e5f 616e 676c 652c 2064 7479 7065 3d6e  n_angle, dtype=n
+00014460: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+00014470: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00014480: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
+00014490: 696f 6e20 3d20 6e70 2e61 7361 7272 6179  ion = np.asarray
+000144a0: 2863 7572 7265 6e74 5f61 6363 656c 6572  (current_acceler
+000144b0: 6174 696f 6e2c 2064 7479 7065 3d6e 702e  ation, dtype=np.
+000144c0: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+000144d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000144e0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+000144f0: 6c6c 5f6d 6173 6b20 3d20 6e70 2e61 7361  ll_mask = np.asa
+00014500: 7272 6179 2863 7572 7265 6e74 5f64 6973  rray(current_dis
+00014510: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
+00014520: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00014530: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00014540: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00014550: 6164 6961 6c5f 616e 676c 6520 3d20 6e70  adial_angle = np
+00014560: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00014570: 5f72 6164 6961 6c5f 616e 676c 652c 2064  _radial_angle, d
+00014580: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000145a0: 2020 2020 2063 7572 7265 6e74 5f63 656c       current_cel
+000145b0: 6c5f 6178 6973 5f6d 6173 6b20 3d20 6e70  l_axis_mask = np
+000145c0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+000145d0: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b2c  _cell_axis_mask,
+000145e0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000145f0: 3229 0d0a 0d0a 0d0a 2020 2020 2020 2020  2)......        
+00014600: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00014610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014630: 2020 2020 2069 6620 706f 696e 745f 7361       if point_sa
+00014640: 6d70 6c65 203e 2030 3a0d 0a20 2020 2020  mple > 0:..     
+00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014660: 2020 2020 2020 2020 2020 2078 665f 7361             xf_sa
+00014670: 6d70 6c65 203d 2066 6674 6672 6571 2870  mple = fftfreq(p
+00014680: 6f69 6e74 5f73 616d 706c 652c 2073 656c  oint_sample, sel
+00014690: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
+000146a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 2066 6674 7374 7269 705f 7361 6d70 6c65   fftstrip_sample
+000146d0: 203d 2066 6674 2865 7870 616e 6465 645f   = fft(expanded_
+000146e0: 696e 7465 6e73 6974 7929 0d0a 2020 2020  intensity)..    
+000146f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014700: 2020 2020 2020 2020 2020 2020 6666 7474              fftt
+00014710: 6f74 616c 5f73 616d 706c 6520 3d20 6e70  otal_sample = np
+00014720: 2e61 6273 2866 6674 7374 7269 705f 7361  .abs(fftstrip_sa
+00014730: 6d70 6c65 290d 0a20 2020 2020 2020 2020  mple)..         
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
+00014760: 203d 2078 665f 7361 6d70 6c65 5b30 203a   = xf_sample[0 :
+00014770: 206c 656e 2878 665f 7361 6d70 6c65 2920   len(xf_sample) 
+00014780: 2f2f 2032 5d0d 0a20 2020 2020 2020 2020  // 2]..         
+00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147a0: 2020 2020 2020 2066 6674 746f 7461 6c5f         ffttotal_
+000147b0: 7361 6d70 6c65 203d 2066 6674 746f 7461  sample = ffttota
+000147c0: 6c5f 7361 6d70 6c65 5b30 203a 206c 656e  l_sample[0 : len
+000147d0: 2866 6674 746f 7461 6c5f 7361 6d70 6c65  (ffttotal_sample
+000147e0: 2920 2f2f 2032 5d0d 0a0d 0a20 2020 2020  ) // 2]....     
+000147f0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00014800: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+00014810: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00014820: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+00014830: 3d20 6578 7061 6e64 6564 5f74 696d 652c  = expanded_time,
+00014840: 2065 7870 616e 6465 645f 696e 7465 6e73   expanded_intens
+00014850: 6974 792c 2078 665f 7361 6d70 6c65 2c20  ity, xf_sample, 
+00014860: 6666 7474 6f74 616c 5f73 616d 706c 650d  ffttotal_sample.
+00014870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014880: 2020 2020 756e 6971 7565 5f63 6c75 7374      unique_clust
+00014890: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
+000148a0: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+000148b0: 6e69 7175 655f 6964 5d20 3d20 2063 7572  nique_id] =  cur
+000148c0: 7265 6e74 5f74 696d 650d 0a20 2020 2020  rent_time..     
+000148d0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000148e0: 6971 7565 5f73 6861 7065 5f70 726f 7065  ique_shape_prope
+000148f0: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00014900: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00014910: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
+00014920: 2c20 6375 7272 656e 745f 7a2c 2063 7572  , current_z, cur
+00014930: 7265 6e74 5f79 2c20 6375 7272 656e 745f  rent_y, current_
+00014940: 782c 2063 7572 7265 6e74 5f72 6164 6975  x, current_radiu
+00014950: 732c 2063 7572 7265 6e74 5f76 6f6c 756d  s, current_volum
+00014960: 652c 2063 7572 7265 6e74 5f65 6363 656e  e, current_eccen
+00014970: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00014980: 7374 2c20 6375 7272 656e 745f 6563 6365  st, current_ecce
+00014990: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+000149a0: 636f 6e64 2c20 6375 7272 656e 745f 7375  cond, current_su
+000149b0: 7266 6163 655f 6172 6561 0d0a 2020 2020  rface_area..    
+000149c0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000149d0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+000149e0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+000149f0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00014a00: 5f69 645d 203d 2063 7572 7265 6e74 5f74  _id] = current_t
+00014a10: 696d 652c 2063 7572 7265 6e74 5f73 7065  ime, current_spe
+00014a20: 6564 2c20 6375 7272 656e 745f 6d6f 7469  ed, current_moti
+00014a30: 6f6e 5f61 6e67 6c65 2c20 6375 7272 656e  on_angle, curren
+00014a40: 745f 6163 6365 6c65 7261 7469 6f6e 2c20  t_acceleration, 
+00014a50: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
+00014a60: 5f63 656c 6c5f 6d61 736b 2c20 6375 7272  _cell_mask, curr
+00014a70: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
+00014a80: 2c20 6375 7272 656e 745f 6365 6c6c 5f61  , current_cell_a
+00014a90: 7869 735f 6d61 736b 0d0a 2020 2020 2020  xis_mask..      
+00014aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00014ab0: 662e 756e 6971 7565 5f66 6674 5f70 726f  f.unique_fft_pro
+00014ac0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00014ad0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+00014ae0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+00014af0: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00014b00: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
+00014b10: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
+00014b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b30: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014b40: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
+00014b50: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+00014b60: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+00014b70: 7175 655f 6964 3a75 6e69 7175 655f 636c  que_id:unique_cl
+00014b80: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00014b90: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00014ba0: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00014bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014bc0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00014bd0: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
+00014be0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
+00014bf0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
+00014c00: 7565 5f69 643a 756e 6971 7565 5f73 6861  ue_id:unique_sha
+00014c10: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
+00014c20: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
+00014c30: 6e69 7175 655f 6964 5d7d 290d 0a20 2020  nique_id]})..   
+00014c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c50: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
+00014c60: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
+00014c70: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
+00014c80: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
+00014c90: 6964 3a75 6e69 7175 655f 6479 6e61 6d69  id:unique_dynami
+00014ca0: 635f 7072 6f70 6572 7469 6573 5f74 7261  c_properties_tra
+00014cb0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00014cc0: 6971 7565 5f69 645d 7d29 0d0a 0d0a 2020  ique_id]})....  
+00014cd0: 2020 6465 6620 5f73 6563 6f6e 645f 6368    def _second_ch
+00014ce0: 616e 6e65 6c5f 7370 6f74 7328 7365 6c66  annel_spots(self
+00014cf0: 2c20 6672 616d 652c 207a 2c20 792c 2078  , frame, z, y, x
+00014d00: 2c20 6365 6c6c 5f69 642c 2074 7261 636b  , cell_id, track
+00014d10: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
+00014d20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00014d30: 7472 6565 2c20 6365 6e74 726f 6964 732c  tree, centroids,
+00014d40: 206c 6162 656c 732c 2076 6f6c 756d 652c   labels, volume,
+00014d50: 2069 6e74 656e 7369 7479 5f6d 6561 6e2c   intensity_mean,
+00014d60: 2069 6e74 656e 7369 7479 5f74 6f74 616c   intensity_total
+00014d70: 2c20 626f 756e 6469 6e67 5f62 6f78 6573  , bounding_boxes
+00014d80: 203d 2073 656c 662e 5f74 696d 6564 5f63   = self._timed_c
+00014d90: 6861 6e6e 656c 5f73 6567 5f69 6d61 6765  hannel_seg_image
+00014da0: 5b73 7472 2869 6e74 2866 6c6f 6174 2866  [str(int(float(f
+00014db0: 7261 6d65 2929 295d 0d0a 2020 2020 2020  rame)))]..      
+00014dc0: 2020 2020 2020 7069 7865 6c74 6573 746c        pixeltestl
+00014dd0: 6f63 6174 696f 6e20 3d20 287a 2c79 2c78  ocation = (z,y,x
+00014de0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00014df0: 6973 742c 2069 6e64 6578 203d 2074 7265  ist, index = tre
+00014e00: 652e 7175 6572 7928 7069 7865 6c74 6573  e.query(pixeltes
+00014e10: 746c 6f63 6174 696f 6e29 0d0a 0d0a 0d0a  tlocation)......
+00014e20: 2020 2020 2020 2020 2020 2020 6262 6f78              bbox
+00014e30: 203d 2062 6f75 6e64 696e 675f 626f 7865   = bounding_boxe
+00014e40: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
+00014e50: 2020 2020 2020 7369 7a65 7a20 3d20 6162        sizez = ab
+00014e60: 7328 6262 6f78 5b30 5d20 2d20 6262 6f78  s(bbox[0] - bbox
+00014e70: 5b33 5d29 0d0a 2020 2020 2020 2020 2020  [3])..          
+00014e80: 2020 7369 7a65 7920 3d20 6162 7328 6262    sizey = abs(bb
+00014e90: 6f78 5b31 5d20 2d20 6262 6f78 5b34 5d29  ox[1] - bbox[4])
+00014ea0: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+00014eb0: 7a65 7820 3d20 6162 7328 6262 6f78 5b32  zex = abs(bbox[2
+00014ec0: 5d20 2d20 6262 6f78 5b35 5d29 200d 0a20  ] - bbox[5]) .. 
+00014ed0: 2020 2020 2020 2020 2020 2076 6574 6f5f             veto_
+00014ee0: 766f 6c75 6d65 203d 2073 697a 6578 202a  volume = sizex *
+00014ef0: 2073 697a 6579 202a 2073 697a 657a 0d0a   sizey * sizez..
+00014f00: 2020 2020 2020 2020 2020 2020 7665 746f              veto
+00014f10: 5f72 6164 6975 7320 3d20 6d61 7468 2e70  _radius = math.p
+00014f20: 6f77 2833 202a 2076 6574 6f5f 766f 6c75  ow(3 * veto_volu
+00014f30: 6d65 202f 2028 3420 2a20 6d61 7468 2e70  me / (4 * math.p
+00014f40: 6929 2c20 312e 3020 2f20 332e 3029 0d0a  i), 1.0 / 3.0)..
+00014f50: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00014f60: 6361 7469 6f6e 203d 2028 6365 6e74 726f  cation = (centro
+00014f70: 6964 735b 696e 6465 785d 5b30 5d20 2a20  ids[index][0] * 
+00014f80: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00014f90: 6e2c 2063 656e 7472 6f69 6473 5b69 6e64  n, centroids[ind
+00014fa0: 6578 5d5b 315d 2a73 656c 662e 7963 616c  ex][1]*self.ycal
+00014fb0: 6962 7261 7469 6f6e 2c20 6365 6e74 726f  ibration, centro
+00014fc0: 6964 735b 696e 6465 785d 5b32 5d2a 7365  ids[index][2]*se
+00014fd0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+00014fe0: 0d0a 2020 2020 2020 2020 2020 2020 5155  ..            QU
+00014ff0: 414c 4954 5920 3d20 6d61 7468 2e70 6f77  ALITY = math.pow
+00015000: 2876 6f6c 756d 655b 696e 6465 785d 2c20  (volume[index], 
+00015010: 312e 302f 332e 3029 0d0a 2020 2020 2020  1.0/3.0)..      
+00015020: 2020 2020 2020 5241 4449 5553 203d 206d        RADIUS = m
+00015030: 6174 682e 706f 7728 766f 6c75 6d65 5b69  ath.pow(volume[i
+00015040: 6e64 6578 5d20 2a20 7365 6c66 2e78 6361  ndex] * self.xca
+00015050: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
+00015060: 2e79 6361 6c69 6272 6174 696f 6e20 2a20  .ycalibration * 
+00015070: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00015080: 6e2c 2031 2e30 2f33 2e30 2920 0d0a 0d0a  n, 1.0/3.0) ....
+00015090: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+000150a0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+000150b0: 6d61 736b 6365 6e74 726f 6964 203d 2073  maskcentroid = s
+000150c0: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
+000150d0: 795f 6469 7374 2866 7261 6d65 2c20 6c6f  y_dist(frame, lo
+000150e0: 6361 7469 6f6e 290d 0a20 2020 2020 2020  cation)..       
+000150f0: 2020 2020 2069 6620 6469 7374 203c 3d20       if dist <= 
+00015100: 3220 2a20 7665 746f 5f72 6164 6975 733a  2 * veto_radius:
+00015110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015120: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00015130: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015140: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
+00015150: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00015160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015170: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
+00015180: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
+00015190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151a0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
+000151b0: 645f 6b65 7920 3a20 696e 7428 6672 616d  d_key : int(fram
+000151c0: 6529 2c0d 0a20 2020 2020 2020 2020 2020  e),..           
+000151d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000151e0: 662e 7a70 6f73 6964 5f6b 6579 203a 2066  f.zposid_key : f
+000151f0: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+00015200: 6e64 6578 5d5b 305d 2a20 7365 6c66 2e7a  ndex][0]* self.z
+00015210: 6361 6c69 6272 6174 696f 6e29 2c0d 0a20  calibration),.. 
+00015220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 2020 2020 2020 2073 656c 662e 7970 6f73         self.ypos
+00015240: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+00015250: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00015260: 315d 2a20 7365 6c66 2e79 6361 6c69 6272  1]* self.ycalibr
+00015270: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015290: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
+000152a0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
+000152b0: 6473 5b69 6e64 6578 5d5b 325d 2a20 7365  ds[index][2]* se
+000152c0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+000152d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000152e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000152f0: 7472 6163 6b69 645f 6b65 793a 2069 6e74  trackid_key: int
+00015300: 2874 7261 636b 5f69 6429 2c0d 0a20 2020  (track_id),..   
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00015330: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+00015340: 2866 6c6f 6174 2869 6e74 656e 7369 7479  (float(intensity
+00015350: 5f74 6f74 616c 5b69 6e64 6578 5d29 292c  _total[index])),
+00015360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015370: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015380: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+00015390: 7920 3a20 2866 6c6f 6174 2869 6e74 656e  y : (float(inten
+000153a0: 7369 7479 5f6d 6561 6e5b 696e 6465 785d  sity_mean[index]
+000153b0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+000153c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000153d0: 662e 7261 6469 7573 5f6b 6579 203a 2028  f.radius_key : (
+000153e0: 666c 6f61 7428 5241 4449 5553 2929 2c0d  float(RADIUS)),.
+000153f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015400: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
+00015410: 616c 6974 795f 6b65 7920 3a20 2866 6c6f  ality_key : (flo
+00015420: 6174 2851 5541 4c49 5459 2929 2c0d 0a20  at(QUALITY)),.. 
+00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015440: 2020 2020 2020 2073 656c 662e 6469 7374         self.dist
+00015450: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+00015460: 6579 3a20 666c 6f61 7428 6469 7374 616e  ey: float(distan
+00015470: 6365 5f63 656c 6c5f 6d61 736b 292c 0d0a  ce_cell_mask),..
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+000154a0: 6b63 656e 7472 6f69 645f 7a5f 6b65 793a  kcentroid_z_key:
+000154b0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
+000154c0: 6f69 645b 305d 292c 0d0a 2020 2020 2020  oid[0]),..      
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+000154f0: 6f69 645f 795f 6b65 793a 2066 6c6f 6174  oid_y_key: float
+00015500: 286d 6173 6b63 656e 7472 6f69 645b 315d  (maskcentroid[1]
+00015510: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00015520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015530: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
+00015540: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+00015550: 656e 7472 6f69 645b 325d 2920 0d0a 0d0a  entroid[2]) ....
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 7d0d 0a20 2020 2020 2020 2020 2020 2065  }..            e
+00015580: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00015590: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000155a0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+000155b0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+000155c0: 6c6c 5f69 645d 203d 2073 656c 662e 756e  ll_id] = self.un
+000155d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000155e0: 7469 6573 5b63 656c 6c5f 6964 5d0d 0a20  ties[cell_id].. 
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015600: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00015610: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015620: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00015630: 7570 6461 7465 287b 7365 6c66 2e74 6f74  update({self.tot
+00015640: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
+00015650: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
+00015660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015670: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+00015680: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015690: 6365 6c6c 5f69 645d 2e75 7064 6174 6528  cell_id].update(
+000156a0: 7b73 656c 662e 6d65 616e 5f69 6e74 656e  {self.mean_inten
+000156b0: 7369 7479 5f6b 6579 3a20 2d31 7d29 0d0a  sity_key: -1})..
+000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156d0: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+000156e0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+000156f0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00015700: 2e75 7064 6174 6528 7b73 656c 662e 7261  .update({self.ra
+00015710: 6469 7573 5f6b 6579 3a20 2d31 7d29 0d0a  dius_key: -1})..
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+00015740: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+00015750: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+00015760: 2e75 7064 6174 6528 7b73 656c 662e 7175  .update({self.qu
+00015770: 616c 6974 795f 6b65 793a 202d 317d 290d  ality_key: -1}).
+00015780: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+00015790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157a0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
+000157b0: 6620 5f64 6963 745f 7570 6461 7465 2873  f _dict_update(s
+000157c0: 656c 662c 2075 6e69 7175 655f 7472 6163  elf, unique_trac
+000157d0: 6b6c 6574 5f69 6473 3a20 4c69 7374 2c20  klet_ids: List, 
+000157e0: 2063 656c 6c5f 6964 3a20 696e 742c 2074   cell_id: int, t
+000157f0: 7261 636b 5f69 643a 2069 6e74 2c20 736f  rack_id: int, so
+00015800: 7572 6365 5f69 643a 2069 6e74 2c20 7461  urce_id: int, ta
+00015810: 7267 6574 5f69 643a 2069 6e74 293a 0d0a  rget_id: int):..
+00015820: 0d0a 200d 0a20 2020 2020 2020 2067 656e  .. ..        gen
+00015830: 6572 6174 696f 6e5f 6964 203d 2073 656c  eration_id = sel
+00015840: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
+00015850: 745b 6365 6c6c 5f69 645d 0d0a 2020 2020  t[cell_id]..    
+00015860: 2020 2020 7472 6163 6b6c 6574 5f69 6420      tracklet_id 
+00015870: 3d20 7365 6c66 2e74 7261 636b 6c65 745f  = self.tracklet_
+00015880: 6469 6374 5b63 656c 6c5f 6964 5d0d 0a20  dict[cell_id].. 
+00015890: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+000158a0: 2020 756e 6971 7565 5f69 6420 3d20 7374    unique_id = st
+000158b0: 7228 7472 6163 6b5f 6964 2920 2b20 2073  r(track_id) +  s
+000158c0: 7472 2867 656e 6572 6174 696f 6e5f 6964  tr(generation_id
+000158d0: 2920 2b20 7374 7228 7472 6163 6b6c 6574  ) + str(tracklet
+000158e0: 5f69 6429 0d0a 2020 2020 2020 2020 0d0a  _id)..        ..
+000158f0: 2020 2020 2020 2020 7665 635f 6d61 736b          vec_mask
+00015900: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00015910: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015920: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015930: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00015940: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00015950: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00015960: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015970: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015980: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00015990: 5f79 5f6b 6579 5d29 2c20 666c 6f61 7428  _y_key]), float(
+000159a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000159b0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000159c0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+000159d0: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+000159e0: 795d 2920 5d0d 0a0d 0a20 2020 2020 2020  y]) ]....       
+000159f0: 2076 6563 5f63 656c 6c20 3d20 5b66 6c6f   vec_cell = [flo
+00015a00: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015a10: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015a20: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00015a30: 662e 7870 6f73 6964 5f6b 6579 5d29 202c  f.xposid_key]) ,
+00015a40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015a50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015a60: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00015a70: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015a80: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015a90: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00015aa0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00015ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ac0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015ad0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015ae0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00015af0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00015b00: 295d 0d0a 0d0a 2020 2020 2020 2020 616e  )]....        an
+00015b10: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
+00015b20: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
+00015b30: 6563 5f63 656c 6c29 0d0a 0d0a 2020 2020  ec_cell)....    
+00015b40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015b50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015b60: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015b70: 6461 7465 287b 7365 6c66 2e72 6164 6961  date({self.radia
+00015b80: 6c5f 616e 676c 655f 6b65 7920 3a20 616e  l_angle_key : an
+00015b90: 676c 657d 2920 2020 2020 2020 2020 2020  gle})           
+00015ba0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00015bb0: 2020 2020 2075 6e69 7175 655f 7472 6163       unique_trac
+00015bc0: 6b6c 6574 5f69 6473 2e61 7070 656e 6428  klet_ids.append(
+00015bd0: 7374 7228 756e 6971 7565 5f69 6429 290d  str(unique_id)).
+00015be0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015bf0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015c00: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015c10: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015c20: 756e 6971 7565 6964 5f6b 6579 203a 2073  uniqueid_key : s
+00015c30: 7472 2875 6e69 7175 655f 6964 297d 290d  tr(unique_id)}).
+00015c40: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015c50: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015c60: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015c70: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015c80: 7472 6163 6b6c 6574 6964 5f6b 6579 203a  trackletid_key :
+00015c90: 2073 7472 2874 7261 636b 6c65 745f 6964   str(tracklet_id
+00015ca0: 297d 2920 0d0a 2020 2020 2020 2020 7365  )}) ..        se
+00015cb0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015cc0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015cd0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015ce0: 7365 6c66 2e67 656e 6572 6174 696f 6e69  self.generationi
+00015cf0: 645f 6b65 7920 3a20 7374 7228 6765 6e65  d_key : str(gene
+00015d00: 7261 7469 6f6e 5f69 6429 7d29 200d 0a20  ration_id)}) .. 
+00015d10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015d20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015d30: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015d40: 2e75 7064 6174 6528 7b73 656c 662e 7472  .update({self.tr
+00015d50: 6163 6b69 645f 6b65 7920 3a20 7374 7228  ackid_key : str(
+00015d60: 7472 6163 6b5f 6964 297d 290d 0a20 2020  track_id)})..   
+00015d70: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015d80: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015d90: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015da0: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
+00015db0: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 2030  on_angle_key : 0
+00015dc0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
+00015dd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015de0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015df0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015e00: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
+00015e10: 2030 2e30 7d29 0d0a 2020 2020 2020 2020   0.0})..        
+00015e20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00015e30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015e40: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00015e50: 287b 7365 6c66 2e61 6363 656c 6572 6174  ({self.accelerat
+00015e60: 696f 6e5f 6b65 7920 3a20 302e 307d 290d  ion_key : 0.0}).
+00015e70: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015e80: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015e90: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015ea0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015eb0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00015ec0: 705f 6669 7273 746b 6579 203a 202d 317d  p_firstkey : -1}
+00015ed0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015ee0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015ef0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015f00: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00015f10: 662e 6563 6365 6e74 7269 6369 7479 5f63  f.eccentricity_c
+00015f20: 6f6d 705f 7365 636f 6e64 6b65 7920 3a20  omp_secondkey : 
+00015f30: 2d31 7d29 0d0a 2020 2020 2020 2020 7365  -1})..        se
+00015f40: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00015f50: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00015f60: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00015f70: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+00015f80: 615f 6b65 7920 3a20 2d31 7d29 0d0a 2020  a_key : -1})..  
+00015f90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015fa0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015fb0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015fc0: 7570 6461 7465 287b 7365 6c66 2e63 656c  update({self.cel
+00015fd0: 6c61 7869 735f 6d61 736b 5f6b 6579 203a  laxis_mask_key :
+00015fe0: 202d 317d 290d 0a0d 0a20 2020 2020 2020   -1})....       
+00015ff0: 2069 6620 736f 7572 6365 5f69 6420 6973   if source_id is
+00016000: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00016010: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00016020: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00016030: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00016040: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
+00016050: 6566 6f72 6569 645f 6b65 7920 3a20 696e  eforeid_key : in
+00016060: 7428 736f 7572 6365 5f69 6429 7d29 0d0a  t(source_id)})..
+00016070: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
+00016080: 3120 3d20 5b66 6c6f 6174 2873 656c 662e  1 = [float(self.
+00016090: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000160a0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000160b0: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+000160c0: 5f6b 6579 5d29 202d 2066 6c6f 6174 2873  _key]) - float(s
+000160d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000160e0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+000160f0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+00016100: 7870 6f73 6964 5f6b 6579 5d29 2c20 0d0a  xposid_key]), ..
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
+00016130: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00016140: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00016150: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00016160: 2e79 706f 7369 645f 6b65 795d 2920 2d20  .yposid_key]) - 
+00016170: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00016180: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016190: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
+000161a0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+000161b0: 795d 292c 200d 0a20 2020 2020 2020 2020  y]), ..         
+000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161d0: 2020 2066 6c6f 6174 2873 656c 662e 756e     float(self.un
+000161e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000161f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00016200: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00016210: 6579 5d29 202d 2020 666c 6f61 7428 7365  ey]) -  float(se
+00016220: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016230: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00016240: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
+00016250: 706f 7369 645f 6b65 795d 295d 0d0a 2020  posid_key])]..  
+00016260: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
+00016270: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
+00016280: 2876 6563 5f31 2c20 7665 635f 3129 292f  (vec_1, vec_1))/
+00016290: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+000162a0: 6e0d 0a20 2020 2020 2020 2020 2020 2073  n..            s
+000162b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000162c0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000162d0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000162e0: 7b73 656c 662e 7370 6565 645f 6b65 7920  {self.speed_key 
+000162f0: 3a20 7370 6565 647d 290d 0a0d 0a20 2020  : speed})....   
+00016300: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
+00016310: 616e 676c 6520 3d20 616e 6775 6c61 725f  angle = angular_
+00016320: 6368 616e 6765 2876 6563 5f6d 6173 6b2c  change(vec_mask,
+00016330: 2076 6563 5f31 290d 0a0d 0a20 2020 2020   vec_1)....     
+00016340: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00016350: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00016360: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00016370: 2e75 7064 6174 6528 7b73 656c 662e 6d6f  .update({self.mo
+00016380: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 203a  tion_angle_key :
+00016390: 206d 6f74 696f 6e5f 616e 676c 657d 2920   motion_angle}) 
+000163a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000163b0: 6966 2073 6f75 7263 655f 6964 2069 6e20  if source_id in 
+000163c0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
+000163d0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
+000163e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000163f0: 655f 736f 7572 6365 5f69 6420 3d20 7365  e_source_id = se
+00016400: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
+00016410: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
+00016420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016430: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016440: 2020 2020 2020 2020 2020 2020 7665 635f              vec_
+00016450: 3220 3d20 5b66 6c6f 6174 2873 656c 662e  2 = [float(self.
+00016460: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016470: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016480: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+00016490: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
+000164a0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+000164b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+000164c0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+000164d0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+000164e0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
+000164f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016500: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
+00016510: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
+00016520: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+00016530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016540: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00016550: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00016560: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00016570: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00016580: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
+00016590: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
+000165a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000165b0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
+000165c0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
+000165d0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
+000165e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000165f0: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
+00016600: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
+00016610: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
+00016620: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016630: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016640: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00016650: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016660: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00016670: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00016680: 202d 2020 3220 2a20 666c 6f61 7428 7365   -  2 * float(se
+00016690: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000166a0: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+000166b0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
+000166c0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
+000166d0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000166e0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000166f0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
+00016700: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00016710: 6b65 795d 295d 0d0a 2020 2020 2020 2020  key])]..        
+00016720: 2020 2020 2020 2020 2020 2020 6163 6320              acc 
+00016730: 3d20 6e70 2e73 7172 7428 6e70 2e64 6f74  = np.sqrt(np.dot
+00016740: 2876 6563 5f32 2c20 7665 635f 3229 292f  (vec_2, vec_2))/
+00016750: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
+00016760: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00016770: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00016780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016790: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000167a0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+000167b0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+000167c0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+000167d0: 5f6b 6579 203a 2061 6363 7d29 0d0a 2020  _key : acc})..  
+000167e0: 2020 2020 2020 656c 6966 2073 6f75 7263        elif sourc
+000167f0: 655f 6964 2069 7320 4e6f 6e65 3a0d 0a20  e_id is None:.. 
+00016800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016810: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016820: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016830: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00016840: 662e 6265 666f 7265 6964 5f6b 6579 203a  f.beforeid_key :
+00016850: 204e 6f6e 657d 2920 0d0a 2020 2020 2020   None}) ..      
+00016860: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00016870: 2020 6966 2074 6172 6765 745f 6964 2069    if target_id i
+00016880: 7320 6e6f 7420 4e6f 6e65 3a20 2020 2020  s not None:     
+00016890: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000168a0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000168b0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000168c0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000168d0: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
+000168e0: 6579 203a 2069 6e74 2874 6172 6765 745f  ey : int(target_
+000168f0: 6964 297d 2920 0d0a 2020 2020 2020 2020  id)}) ..        
+00016900: 656c 6966 2074 6172 6765 745f 6964 2069  elif target_id i
+00016910: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00016920: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00016930: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016940: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00016950: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
+00016960: 7269 645f 6b65 7920 3a20 4e6f 6e65 7d29  rid_key : None})
+00016970: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00016980: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00016990: 636f 6e64 5f63 6861 6e6e 656c 5f75 7064  cond_channel_upd
+000169a0: 6174 6528 6365 6c6c 5f69 642c 2074 7261  ate(cell_id, tra
+000169b0: 636b 5f69 6429 2020 2020 0d0a 0d0a 0d0a  ck_id)    ......
+000169c0: 2020 2020 6465 6620 5f74 656d 706f 7261      def _tempora
+000169d0: 6c5f 706c 6f74 735f 7472 6163 6b6d 6174  l_plots_trackmat
+000169e0: 6528 7365 6c66 293a 0d0a 2020 2020 0d0a  e(self):..    ..
+000169f0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+00016a00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016a10: 2e41 7474 7220 3d20 7b7d 0d0a 2020 2020  .Attr = {}..    
+00016a20: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00016a30: 7474 696d 6520 3d20 696e 7428 6d69 6e28  ttime = int(min(
+00016a40: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
+00016a50: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00016a60: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00016a70: 2020 2020 656e 6474 696d 6520 3d20 696e      endtime = in
+00016a80: 7428 6d61 7828 7365 6c66 2e41 6c6c 5661  t(max(self.AllVa
+00016a90: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
+00016aa0: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00016ab0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00016ac0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016ad0: 662e 7469 6d65 203d 205b 5d0d 0a20 2020  f.time = []..   
+00016ae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016af0: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00016b00: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+00016b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016b20: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00016b30: 705f 7a20 3d20 5b5d 0d0a 0d0a 2020 2020  p_z = []....    
+00016b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016b50: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00016b60: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+00016b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016b80: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00016b90: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00016ba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016bb0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00016bc0: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00016bd0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016be0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00016bf0: 7820 3d20 5b5d 0d0a 0d0a 2020 2020 2020  x = []....      
+00016c00: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016c10: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
+00016c20: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
+00016c30: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016c40: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00016c50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016c60: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016c70: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00016c80: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016c90: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00016ca0: 7469 635f 7661 725f 7370 6565 6420 3d20  tic_var_speed = 
+00016cb0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016cc0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016cd0: 6963 5f6d 6561 6e5f 6163 6320 3d20 5b5d  ic_mean_acc = []
+00016ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016cf0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00016d00: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00016d10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016d20: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00016d30: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016d40: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+00016d50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016d60: 6974 6f74 6963 5f76 6172 5f64 6972 6563  itotic_var_direc
+00016d70: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00016d80: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016d90: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016da0: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
+00016db0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00016dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016dd0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00016de0: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00016df0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00016e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016e10: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016e20: 616e 5f64 6973 705f 7a20 3d20 5b5d 0d0a  an_disp_z = []..
+00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e40: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016e50: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+00016e60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016e70: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016e80: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
+00016e90: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016ea0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00016eb0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00016ec0: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00016ed0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016ee0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00016ef0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00016f00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016f10: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016f20: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00016f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016f40: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00016f50: 6963 5f6d 6561 6e5f 7261 6469 7573 203d  ic_mean_radius =
+00016f60: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00016f70: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00016f80: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00016f90: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016fa0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00016fb0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f73  n_mitotic_mean_s
+00016fc0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+00016fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016fe0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00016ff0: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+00017000: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017010: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00017020: 6561 6e5f 6163 6320 3d20 5b5d 0d0a 2020  ean_acc = []..  
+00017030: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017040: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00017050: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00017060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017070: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00017080: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00017090: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
+000170a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000170b0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+000170c0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000170d0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+000170e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000170f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00017100: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00017110: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
+00017120: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017130: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00017140: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00017150: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+00017160: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017170: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00017180: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+00017190: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+000171a0: 5f76 6172 5f64 6973 705f 7a20 3d20 5b5d  _var_disp_z = []
+000171b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000171c0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+000171d0: 6e5f 6469 7370 5f79 203d 205b 5d0d 0a20  n_disp_y = [].. 
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000171f0: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00017200: 5f79 203d 205b 5d0d 0a0d 0a20 2020 2020  _y = []....     
+00017210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017220: 616c 6c5f 6d65 616e 5f64 6973 705f 7820  all_mean_disp_x 
+00017230: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017240: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00017250: 6172 5f64 6973 705f 7820 3d20 5b5d 0d0a  ar_disp_x = []..
+00017260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017270: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00017280: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00017290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000172a0: 662e 616c 6c5f 7661 725f 7261 6469 7573  f.all_var_radius
+000172b0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000172c0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000172d0: 6c5f 6d65 616e 5f73 7065 6564 203d 205b  l_mean_speed = [
+000172e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000172f0: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00017300: 7370 6565 6420 3d20 5b5d 0d0a 0d0a 2020  speed = []....  
+00017310: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017320: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 6320  lf.all_mean_acc 
+00017330: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017340: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00017350: 6172 5f61 6363 203d 205b 5d0d 0a0d 0a20  ar_acc = [].... 
+00017360: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017370: 656c 662e 616c 6c5f 6d65 616e 5f64 6972  elf.all_mean_dir
+00017380: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+00017390: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000173a0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+000173b0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000173c0: 6861 6e67 6520 3d20 5b5d 0d0a 0d0a 2020  hange = []....  
+000173d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000173e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
+000173f0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00017400: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017410: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00017420: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00017430: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a20  mask = []...... 
+00017440: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017450: 6c6c 5f73 706f 7473 5f74 7261 636b 7320  ll_spots_tracks 
+00017460: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00017470: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+00017480: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
+00017490: 706f 745f 7072 6f70 6572 7469 6573 2e69  pot_properties.i
+000174a0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+000174b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000174c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000174d0: 2020 2020 2020 2061 6c6c 5f73 706f 7473         all_spots
+000174e0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
+000174f0: 706f 745f 7072 6f70 6572 7469 6573 5b6b  pot_properties[k
+00017500: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017510: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00017520: 2e74 7261 636b 6964 5f6b 6579 2069 6e20  .trackid_key in 
+00017530: 616c 6c5f 7370 6f74 733a 0d0a 2020 2020  all_spots:..    
+00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017550: 2020 2020 2020 616c 6c5f 7370 6f74 735f        all_spots_
+00017560: 7472 6163 6b73 5b6b 5d20 3d20 616c 6c5f  tracks[k] = all_
+00017570: 7370 6f74 730d 0a20 2020 2020 2020 2020  spots..         
+00017580: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00017590: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000175a0: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+000175b0: 7572 6573 203d 205b 5d0d 0a20 2020 2020  ures = []..     
+000175c0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000175d0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
+000175e0: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
+000175f0: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
+00017600: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
+00017610: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
+00017620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017630: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00017640: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00017650: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
+00017660: 6528 7374 6172 7474 696d 652c 2065 6e64  e(starttime, end
+00017670: 7469 6d65 292c 2074 6f74 616c 3d65 6e64  time), total=end
+00017680: 7469 6d65 202d 2073 7461 7274 7469 6d65  time - starttime
+00017690: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000176a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176c0: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
+000176d0: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
+000176e0: 6974 2873 656c 662e 5f63 6f6d 7075 7465  it(self._compute
+000176f0: 5f74 656d 706f 7261 6c2c 2069 2c20 616c  _temporal, i, al
+00017700: 6c5f 7370 6f74 735f 7472 6163 6b73 2929  l_spots_tracks))
+00017710: 0d0a 200d 0a20 2020 2020 2020 2020 2020  .. ..           
+00017720: 2020 2020 2020 2020 205b 722e 7265 7375           [r.resu
+00017730: 6c74 2829 2066 6f72 2072 2069 6e20 636f  lt() for r in co
+00017740: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+00017750: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+00017760: 7475 7265 7329 5d0d 0a0d 0a0d 0a20 2020  tures)]......   
+00017770: 2064 6566 205f 636f 6d70 7574 655f 7465   def _compute_te
+00017780: 6d70 6f72 616c 2873 656c 662c 2069 2c20  mporal(self, i, 
+00017790: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000177a0: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
+000177b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000177c0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000177d0: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177f0: 206d 6974 6f74 6963 5f64 6973 705f 7920   mitotic_disp_y 
+00017800: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017810: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017820: 635f 6469 7370 5f78 203d 205b 5d0d 0a20  c_disp_x = [].. 
+00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017840: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
+00017850: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00017860: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017870: 7469 635f 7370 6565 6420 3d20 5b5d 0d0a  tic_speed = []..
+00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017890: 2020 2020 6d69 746f 7469 635f 6163 6320      mitotic_acc 
+000178a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000178b0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000178c0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000178d0: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+000178e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000178f0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00017900: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00017910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017920: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017930: 635f 6469 7370 5f7a 203d 205b 5d0d 0a20  c_disp_z = [].. 
+00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017950: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00017960: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00017990: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+000179a0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+000179b0: 5f6d 6974 6f74 6963 5f72 6164 6975 7320  _mitotic_radius 
+000179c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000179d0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+000179e0: 746f 7469 635f 7370 6565 6420 3d20 5b5d  totic_speed = []
+000179f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017a00: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017a10: 635f 6163 6320 3d20 5b5d 0d0a 2020 2020  c_acc = []..    
+00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a30: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
+00017a40: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00017a50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017a60: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017a70: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00017a80: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00017a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017aa0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 00017ab0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-00017ac0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00017ac0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
 00017ad0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017ae0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+00017ae0: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
 00017af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b00: 2020 616c 6c5f 7261 6469 7573 203d 205b    all_radius = [
+00017b00: 2020 616c 6c5f 6469 7370 5f78 203d 205b    all_disp_x = [
 00017b10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017b20: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
-00017b30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017b40: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-00017b50: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-00017b60: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017b70: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00017b80: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-00017b90: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00017ba0: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-00017bb0: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a0d  mask = [].......
-00017bc0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017bd0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00017be0: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
-00017bf0: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
-00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00017c40: 5f74 696d 6520 3d20 616c 6c5f 7370 6f74  _time = all_spot
-00017c50: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017c60: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
-00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c80: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017c90: 6963 203d 2061 6c6c 5f73 706f 7473 5f74  ic = all_spots_t
-00017ca0: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
-00017cb0: 7669 6469 6e67 5f6b 6579 5d0d 0a20 2020  viding_key]..   
-00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cf0: 2020 2020 2020 6966 2069 203d 3d20 696e        if i == in
-00017d00: 7428 6375 7272 656e 745f 7469 6d65 293a  t(current_time):
-00017d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d30: 2020 2020 6966 206d 6974 6f74 6963 3a0d      if mitotic:.
-00017d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d60: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017d70: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
-00017d80: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017d90: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
-00017da0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00017db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dc0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017dd0: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
-00017de0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017df0: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
-00017e00: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00017e40: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
-00017e50: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017e60: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
-00017e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 2020 2020 2020 6966 2061 6c6c 5f73          if all_s
-00017ea0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017eb0: 656c 662e 7261 6469 7573 5f6b 6579 5d20  elf.radius_key] 
-00017ec0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
-00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ef0: 206d 6974 6f74 6963 5f72 6164 6975 732e   mitotic_radius.
-00017f00: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00017f10: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00017f20: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f50: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00017b20: 2020 2020 2020 2061 6c6c 5f72 6164 6975         all_radiu
+00017b30: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00017b40: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017b50: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b70: 616c 6c5f 6163 6320 3d20 5b5d 0d0a 2020  all_acc = []..  
+00017b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b90: 2020 616c 6c5f 6469 7265 6374 696f 6e61    all_directiona
+00017ba0: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bc0: 2020 2061 6c6c 5f64 6973 7461 6e63 655f     all_distance_
+00017bd0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00017be0: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+00017bf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00017c00: 286b 2c76 2920 696e 2061 6c6c 5f73 706f  (k,v) in all_spo
+00017c10: 7473 5f74 7261 636b 732e 6974 656d 7328  ts_tracks.items(
+00017c20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017c50: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00017c60: 7272 656e 745f 7469 6d65 203d 2061 6c6c  rrent_time = all
+00017c70: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017c80: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
+00017c90: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+00017ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cb0: 6d69 746f 7469 6320 3d20 616c 6c5f 7370  mitotic = all_sp
+00017cc0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017cd0: 6c66 2e64 6976 6964 696e 675f 6b65 795d  lf.dividing_key]
+00017ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017cf0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d10: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
+00017d20: 3d3d 2069 6e74 2863 7572 7265 6e74 5f74  == int(current_t
+00017d30: 696d 6529 3a0d 0a20 2020 2020 2020 2020  ime):..         
+00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d50: 2020 2020 2020 2020 2069 6620 6d69 746f           if mito
+00017d60: 7469 633a 0d0a 2020 2020 2020 2020 2020  tic:..          
+00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d80: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017d90: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+00017da0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017db0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+00017dc0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00017dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017df0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00017e00: 792e 6170 7065 6e64 2861 6c6c 5f73 706f  y.append(all_spo
+00017e10: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017e20: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00017e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e50: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017e60: 6469 7370 5f78 2e61 7070 656e 6428 616c  disp_x.append(al
+00017e70: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017e80: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
+00017e90: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017eb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017ec0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017ed0: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+00017ee0: 6b65 795d 203e 2030 3a0d 0a20 2020 2020  key] > 0:..     
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f10: 2020 2020 2020 6d69 746f 7469 635f 7261        mitotic_ra
+00017f20: 6469 7573 2e61 7070 656e 6428 616c 6c5f  dius.append(all_
+00017f30: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017f40: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+00017f50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f80: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017f90: 7261 6469 7573 2e61 7070 656e 6428 4e6f  radius.append(No
-00017fa0: 6e65 2920 2020 2020 2020 0d0a 2020 2020  ne)       ..    
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 6d69 746f 7469 635f 7370 6565      mitotic_spee
-00017fe0: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00017ff0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018000: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018030: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
-00018040: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00018050: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00018060: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00018070: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018090: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000180a0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-000180b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000180c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000180d0: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-000180e0: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018110: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00018120: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018130: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018140: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018150: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-00018160: 6173 6b5f 6b65 795d 290d 0a0d 0a0d 0a20  ask_key])...... 
-00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018190: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
-000181a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000181b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181c0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-000181d0: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
-000181e0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000181f0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
-00018200: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
-00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018230: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00018240: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
-00018250: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00018260: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-00018270: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000182a0: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
-000182b0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000182c0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
-000182d0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018300: 2020 2020 2069 6620 616c 6c5f 7370 6f74       if all_spot
-00018310: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018320: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
-00018330: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00018360: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
-00018370: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00018380: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018390: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183c0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00017f70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00017f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fa0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00017fb0: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
+00017fc0: 6e64 284e 6f6e 6529 2020 2020 2020 200d  nd(None)       .
+00017fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ff0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00018000: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+00018010: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00018020: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+00018030: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00018040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018050: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00018060: 7469 635f 6163 632e 6170 7065 6e64 2861  tic_acc.append(a
+00018070: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00018080: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
+00018090: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
+000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180c0: 2020 2020 6d69 746f 7469 635f 6469 7265      mitotic_dire
+000180d0: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+000180e0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+000180f0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+00018100: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+00018110: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018130: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00018140: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+00018150: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
+00018160: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00018170: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+00018180: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+00018190: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 2020 2020 2020 6966 206e 6f74 206d 6974        if not mit
+000181c0: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
+000181d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181e0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000181f0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018200: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
+00018210: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00018220: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018250: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00018260: 7469 635f 6469 7370 5f79 2e61 7070 656e  tic_disp_y.appen
+00018270: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00018280: 6b73 5b6b 5d5b 7365 6c66 2e79 706f 7369  ks[k][self.yposi
+00018290: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000182a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182c0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+000182d0: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
+000182e0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000182f0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00018300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018320: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
+00018330: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00018340: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
+00018350: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
+00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018380: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00018390: 7261 6469 7573 2e61 7070 656e 6428 616c  radius.append(al
+000183a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+000183b0: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
+000183c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 000183d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018400: 6974 6f74 6963 5f72 6164 6975 732e 6170  itotic_radius.ap
-00018410: 7065 6e64 284e 6f6e 6529 2020 2020 2020  pend(None)      
-00018420: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018440: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018450: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
-00018460: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018470: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018480: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
-00018490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000184c0: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
-000184d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000184e0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-000184f0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
-00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018520: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
-00018530: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00018540: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018550: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018560: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-00018570: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00018580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018590: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000185a0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000185b0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-000185c0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000185d0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
-000185e0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-000185f0: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
-00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018610: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00018620: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
-00018630: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00018640: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00018650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018670: 2020 2020 616c 6c5f 6469 7370 5f79 2e61      all_disp_y.a
-00018680: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018690: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
-000186a0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000186d0: 6c6c 5f64 6973 705f 782e 6170 7065 6e64  ll_disp_x.append
-000186e0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000186f0: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
-00018700: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-00018730: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00018740: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
-00018750: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
-00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018770: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018780: 6c5f 7261 6469 7573 2e61 7070 656e 6428  l_radius.append(
-00018790: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000187a0: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
-000187b0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+000183e0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000183f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00018400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018420: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
+00018430: 7573 2e61 7070 656e 6428 4e6f 6e65 2920  us.append(None) 
+00018440: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018470: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f73     non_mitotic_s
+00018480: 7065 6564 2e61 7070 656e 6428 616c 6c5f  peed.append(all_
+00018490: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000184a0: 7365 6c66 2e73 7065 6564 5f6b 6579 5d29  self.speed_key])
+000184b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184d0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+000184e0: 746f 7469 635f 6163 632e 6170 7065 6e64  totic_acc.append
+000184f0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00018500: 735b 6b5d 5b73 656c 662e 6163 6365 6c65  s[k][self.accele
+00018510: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
+00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018540: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00018550: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00018560: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
+00018570: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00018580: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+00018590: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185c0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+000185d0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+000185e0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+000185f0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00018600: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018610: 736b 5f6b 6579 5d29 0d0a 0d0a 2020 2020  sk_key])....    
+00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018630: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00018640: 6c5f 6469 7370 5f7a 2e61 7070 656e 6428  l_disp_z.append(
+00018650: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00018660: 5b6b 5d5b 7365 6c66 2e7a 706f 7369 645f  [k][self.zposid_
+00018670: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00018680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018690: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+000186a0: 705f 792e 6170 7065 6e64 2861 6c6c 5f73  p_y.append(all_s
+000186b0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000186c0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+000186d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000186e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186f0: 2020 2020 616c 6c5f 6469 7370 5f78 2e61      all_disp_x.a
+00018700: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00018710: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
+00018720: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00018730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018740: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00018750: 6620 616c 6c5f 7370 6f74 735f 7472 6163  f all_spots_trac
+00018760: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
+00018770: 735f 6b65 795d 203e 2030 3a0d 0a20 2020  s_key] > 0:..   
+00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187a0: 2020 2061 6c6c 5f72 6164 6975 732e 6170     all_radius.ap
+000187b0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000187c0: 7261 636b 735b 6b5d 5b73 656c 662e 7261  racks[k][self.ra
+000187d0: 6469 7573 5f6b 6579 5d29 0d0a 2020 2020  dius_key])..    
 000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018800: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
-00018810: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
-00018820: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
-00018850: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00018860: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018870: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 2061 6c6c 5f61 6363 2e61 7070 656e 6428   all_acc.append(
-000188b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000188c0: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
-000188d0: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00018900: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00018910: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
-00018920: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00018930: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
-00018940: 6c65 5f6b 6579 5d29 2020 200d 0a20 2020  le_key])   ..   
-00018950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018960: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00018970: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-00018980: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
-00018990: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-000189a0: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-000189b0: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
-000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000189f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018a00: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00018a10: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
-00018a20: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00018a30: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00018a40: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00018a50: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00018a60: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-00018a70: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
-00018aa0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00018ab0: 6628 6d69 746f 7469 635f 6469 7370 5f78  f(mitotic_disp_x
-00018ac0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018ad0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018ae0: 746f 7469 635f 6469 7370 5f7a 203d 206e  totic_disp_z = n
-00018af0: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
-00018b00: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
-00018b10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018b20: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00018b30: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
-00018b40: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
-00018b50: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00018b60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018b70: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00018b80: 635f 6469 7370 5f78 203d 206e 702e 6162  c_disp_x = np.ab
-00018b90: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
-00018ba0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00018bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018bc0: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
-00018bd0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00018be0: 6628 616c 6c5f 6469 7370 5f7a 2929 0d0a  f(all_disp_z))..
-00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c00: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
-00018c10: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00018c20: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
-00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c40: 2020 616c 6c5f 6469 7370 5f78 203d 206e    all_disp_x = n
-00018c50: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
-00018c60: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 0d0a  l_disp_x))......
-00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018cb0: 6c66 2e74 696d 652e 6170 7065 6e64 2869  lf.time.append(i
-00018cc0: 202a 2073 656c 662e 7463 616c 6962 7261   * self.tcalibra
-00018cd0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018cf0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00018d00: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
-00018d10: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
-00018d20: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00018d30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018d40: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00018d50: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
-00018d60: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
-00018d70: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
-00018d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018d90: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00018da0: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
-00018db0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
-00018dc0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00018dd0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018de0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-00018df0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00018e00: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-00018e10: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018e20: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018e30: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
-00018e40: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00018e50: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00018e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e70: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018e80: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
-00018e90: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00018ea0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ec0: 2020 2066 696c 7465 7265 645f 7661 6c75     filtered_valu
-00018ed0: 6573 203d 205b 7661 6c20 666f 7220 7661  es = [val for va
-00018ee0: 6c20 696e 206d 6974 6f74 6963 5f72 6164  l in mitotic_rad
-00018ef0: 6975 7320 6966 2076 616c 2069 7320 6e6f  ius if val is no
-00018f00: 7420 4e6f 6e65 5d0d 0a20 2020 2020 2020  t None]..       
-00018f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018f20: 662e 6d69 746f 7469 635f 6d65 616e 5f72  f.mitotic_mean_r
-00018f30: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00018f40: 6d65 616e 2866 696c 7465 7265 645f 7661  mean(filtered_va
-00018f50: 6c75 6573 2929 0d0a 2020 2020 2020 2020  lues))..        
-00018f60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f80: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00018f90: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
-00018fa0: 286e 702e 7374 6428 6669 6c74 6572 6564  (np.std(filtered
-00018fb0: 5f76 616c 7565 7329 290d 0a20 2020 2020  _values))..     
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00018fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018fe0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018ff0: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
-00019000: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00019010: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-00019020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019030: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00019040: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
-00019050: 702e 7374 6428 6d69 746f 7469 635f 7370  p.std(mitotic_sp
-00019060: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00019070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019080: 662e 6d69 746f 7469 635f 6d65 616e 5f61  f.mitotic_mean_a
-00019090: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-000190a0: 6e28 6d69 746f 7469 635f 6163 6329 290d  n(mitotic_acc)).
-000190b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000190d0: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
-000190e0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-000190f0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00019100: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019110: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00019120: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00019130: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00019140: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
-00019150: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00019160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019170: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00019180: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00019190: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-000191a0: 2e73 7464 286d 6974 6f74 6963 5f64 6972  .std(mitotic_dir
-000191b0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-000191c0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000191d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000191e0: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
-000191f0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00019200: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00019210: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00019220: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00019230: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019240: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00019250: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00019260: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00019270: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
-00019280: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
-00019290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000192a0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000192b0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-000192c0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-000192d0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000192e0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-000192f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019300: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00019310: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00019320: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00019330: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00019360: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-00019370: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00019380: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
-00019390: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000193a0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-000193b0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000193c0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-000193d0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-000193e0: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-000193f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019400: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019410: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00019420: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00019430: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
-00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019450: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00019460: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-00019470: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00019480: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
-00019490: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000194a0: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
-000194b0: 645f 7661 6c75 6573 203d 205b 7661 6c20  d_values = [val 
-000194c0: 666f 7220 7661 6c20 696e 206e 6f6e 5f6d  for val in non_m
-000194d0: 6974 6f74 6963 5f72 6164 6975 7320 6966  itotic_radius if
-000194e0: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
-000194f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00019500: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019510: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
-00019520: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
-00019530: 616e 2866 696c 7465 7265 645f 7661 6c75  an(filtered_valu
-00019540: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
-00019550: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019570: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00019580: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00019590: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
-000195a0: 6564 5f76 616c 7565 7329 290d 0a0d 0a20  ed_values)).... 
-000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-000195d0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
-000195e0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-000195f0: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
-00019600: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019610: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019620: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00019630: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00019640: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00019650: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-00019660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019670: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00019680: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-00019690: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-000196a0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
-000196b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000196c0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-000196d0: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-000196e0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
-000196f0: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
-00019700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019710: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00019720: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00019730: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-00019740: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00019750: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00019760: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-00019770: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00019780: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00019790: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000197a0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-000197b0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-000197c0: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
-000197d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000197e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000197f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00019800: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00019810: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019820: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00019830: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00019840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019850: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00019860: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
-00019870: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00019880: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00019890: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000198a0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
-000198b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000198c0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-000198d0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
-000198e0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-000198f0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00019900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019910: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
-00019920: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00019930: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
-00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00019960: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-00019970: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
-00019980: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019990: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000199a0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
-000199b0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-000199c0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-000199d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000199e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-000199f0: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
-00019a00: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
-00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a20: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00019a30: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-00019a40: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
-00019a50: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00019a60: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
-00019a70: 6564 5f76 616c 7565 7320 3d20 5b76 616c  ed_values = [val
-00019a80: 2066 6f72 2076 616c 2069 6e20 616c 6c5f   for val in all_
-00019a90: 7261 6469 7573 2069 6620 7661 6c20 6973  radius if val is
-00019aa0: 206e 6f74 204e 6f6e 655d 0d0a 2020 2020   not None]..    
-00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ac0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
-00019ad0: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
-00019ae0: 6561 6e28 6669 6c74 6572 6564 5f76 616c  ean(filtered_val
-00019af0: 7565 7329 290d 0a20 2020 2020 2020 2020  ues))..         
-00019b00: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b20: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
-00019b30: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
-00019b40: 7464 2866 696c 7465 7265 645f 7661 6c75  td(filtered_valu
-00019b50: 6573 2929 0d0a 0d0a 2020 2020 2020 2020  es))....        
-00019b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019b70: 2e61 6c6c 5f6d 6561 6e5f 7370 6565 642e  .all_mean_speed.
-00019b80: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-00019b90: 6c6c 5f73 7065 6564 2929 0d0a 2020 2020  ll_speed))..    
-00019ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bb0: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
-00019bc0: 6564 2e61 7070 656e 6428 6e70 2e73 7464  ed.append(np.std
-00019bd0: 2861 6c6c 5f73 7065 6564 2929 0d0a 0d0a  (all_speed))....
-00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bf0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00019c00: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
-00019c10: 6d65 616e 2861 6c6c 5f61 6363 2929 0d0a  mean(all_acc))..
-00019c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c30: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00019c40: 5f61 6363 2e61 7070 656e 6428 6e70 2e73  _acc.append(np.s
-00019c50: 7464 2861 6c6c 5f61 6363 2929 0d0a 0d0a  td(all_acc))....
-00019c60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019c70: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00019c80: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00019c90: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00019ca0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7265  np.mean(all_dire
-00019cb0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-00019cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019cd0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00019ce0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00019cf0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00019d00: 7374 6428 616c 6c5f 6469 7265 6374 696f  std(all_directio
-00019d10: 6e61 6c5f 6368 616e 6765 2929 0d0a 0d0a  nal_change))....
-00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d30: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00019d40: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-00019d50: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
-00019d60: 6561 6e28 616c 6c5f 6469 7374 616e 6365  ean(all_distance
-00019d70: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d90: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00019da0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00019db0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
-00019dc0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-00019dd0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-00019de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019df0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00019e00: 0d0a 6465 6620 626f 756e 6461 7279 5f70  ..def boundary_p
-00019e10: 6f69 6e74 7328 6d61 736b 2c20 7863 616c  oints(mask, xcal
-00019e20: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
-00019e30: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
-00019e40: 7469 6f6e 293a 0d0a 0d0a 2020 2020 6e64  tion):....    nd
-00019e50: 696d 203d 206c 656e 286d 6173 6b2e 7368  im = len(mask.sh
-00019e60: 6170 6529 0d0a 2020 2020 7469 6d65 645f  ape)..    timed_
-00019e70: 6d61 736b 203d 207b 7d0d 0a20 2020 206d  mask = {}..    m
-00019e80: 6173 6b20 3d20 6d61 736b 203e 2030 0d0a  ask = mask > 0..
-00019e90: 2020 2020 6d61 736b 203d 206d 6173 6b2e      mask = mask.
-00019ea0: 6173 7479 7065 2827 7569 6e74 3827 290d  astype('uint8').
-00019eb0: 0a20 2020 2023 2059 5820 7368 6170 6564  .    # YX shaped
-00019ec0: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
-00019ed0: 6e64 696d 203d 3d20 323a 0d0a 2020 2020  ndim == 2:..    
-00019ee0: 2020 2020 0d0a 2020 2020 2020 2020 626f      ..        bo
-00019ef0: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
-00019f00: 756e 6461 7269 6573 286d 6173 6b29 0d0a  undaries(mask)..
-00019f10: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
-00019f20: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
-00019f30: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-00019f40: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
-00019f50: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-00019f60: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-00019f70: 203e 2030 290d 0a20 2020 2020 2020 2072   > 0)..        r
-00019f80: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
-00019f90: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
-00019fa0: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
-00019fb0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00019fc0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
-00019fd0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-00019fe0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
-00019ff0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
-0001a000: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-0001a010: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-0001a020: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-0001a030: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-0001a040: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
-0001a050: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-0001a060: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-0001a070: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
-0001a080: 696f 6e0d 0a0d 0a20 2020 2020 2020 2074  ion....        t
-0001a090: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
-0001a0a0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
-0001a0b0: 6573 290d 0a20 2020 2020 2020 2023 2054  es)..        # T
-0001a0c0: 6869 7320 6f62 6a65 6374 2063 6f6e 7461  his object conta
-0001a0d0: 696e 7320 6c69 7374 206f 6620 616c 6c20  ins list of all 
-0001a0e0: 7468 6520 706f 696e 7473 2066 6f72 2061  the points for a
-0001a0f0: 6c6c 2074 6865 206c 6162 656c 7320 696e  ll the labels in
-0001a100: 2074 6865 204d 6173 6b20 696d 6167 6520   the Mask image 
-0001a110: 7769 7468 2074 6865 206c 6162 656c 2069  with the label i
-0001a120: 6420 616e 6420 766f 6c75 6d65 206f 6620  d and volume of 
-0001a130: 6561 6368 206c 6162 656c 0d0a 2020 2020  each label..    
-0001a140: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-0001a150: 7472 2830 295d 203d 205b 7472 6565 2c20  tr(0)] = [tree, 
-0001a160: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-0001a170: 656e 7472 6f69 645d 0d0a 0d0a 2020 2020  entroid]....    
-0001a180: 2320 5459 5820 7368 6170 6564 206f 626a  # TYX shaped obj
-0001a190: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-0001a1a0: 203d 3d20 333a 0d0a 0d0a 0d0a 2020 2020   == 3:......    
-0001a1b0: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
-0001a1c0: 6d28 7261 6e67 6528 302c 206d 6173 6b2e  m(range(0, mask.
-0001a1d0: 7368 6170 655b 305d 2929 3a0d 0a20 2020  shape[0])):..   
-0001a1e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0001a200: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
-0001a210: 6f75 6e64 6172 6965 7328 6d61 736b 5b69  oundaries(mask[i
-0001a220: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
-0001a230: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
-0001a240: 726f 6964 203d 2028 302c 2920 2b20 636f  roid = (0,) + co
-0001a250: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
-0001a260: 6f75 6e64 6172 7929 200d 0a20 2020 2020  oundary) ..     
-0001a270: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-0001a280: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
-0001a290: 756e 6461 7279 203e 2030 290d 0a20 2020  undary > 0)..   
-0001a2a0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-0001a2b0: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
-0001a2c0: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
-0001a2d0: 7261 7928 696e 6469 6365 732c 2064 7479  ray(indices, dty
-0001a2e0: 7065 3d6e 702e 666c 6f61 7433 3229 292e  pe=np.float32)).
-0001a2f0: 636f 7079 2829 0d0a 0d0a 2020 2020 2020  copy()....      
-0001a300: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-0001a310: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
-0001a320: 7265 616c 5f69 6e64 6963 6573 2929 3a0d  real_indices)):.
-0001a330: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a340: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-0001a350: 6365 735b 6a5d 5b30 5d20 3d20 7265 616c  ces[j][0] = real
-0001a360: 5f69 6e64 6963 6573 5b6a 5d5b 305d 202a  _indices[j][0] *
-0001a370: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
-0001a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a390: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-0001a3a0: 6a5d 5b31 5d20 3d20 7265 616c 5f69 6e64  j][1] = real_ind
-0001a3b0: 6963 6573 5b6a 5d5b 315d 202a 2078 6361  ices[j][1] * xca
-0001a3c0: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
-0001a3d0: 2020 2020 2020 2020 2020 2020 2074 7265               tre
-0001a3e0: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
-0001a3f0: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
-0001a400: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001a410: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
-0001a420: 7374 7228 6929 5d20 3d20 5b74 7265 652c  str(i)] = [tree,
-0001a430: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
-0001a440: 6365 6e74 726f 6964 5d0d 0a20 2020 2020  centroid]..     
-0001a450: 2020 2020 2020 200d 0a20 2020 2023 2054         ..    # T
-0001a460: 5a59 5820 7368 6170 6564 206f 626a 6563  ZYX shaped objec
-0001a470: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
-0001a480: 3d20 343a 0d0a 2020 2020 2020 2020 7072  = 4:..        pr
-0001a490: 696e 7428 274d 616b 696e 6720 6d61 736b  int('Making mask
-0001a4a0: 2069 6e20 3444 2729 0d0a 2020 2020 2020   in 4D')..      
-0001a4b0: 2020 626f 756e 6461 7279 203d 206e 702e    boundary = np.
-0001a4c0: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
-0001a4d0: 2020 2020 5b6d 6173 6b2e 7368 6170 655b      [mask.shape[
-0001a4e0: 305d 2c20 6d61 736b 2e73 6861 7065 5b31  0], mask.shape[1
-0001a4f0: 5d2c 206d 6173 6b2e 7368 6170 655b 325d  ], mask.shape[2]
-0001a500: 2c20 6d61 736b 2e73 6861 7065 5b33 5d5d  , mask.shape[3]]
-0001a510: 2c20 6474 7970 653d 6e70 2e75 696e 7438  , dtype=np.uint8
-0001a520: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-0001a530: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001a540: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
-0001a550: 655b 305d 293a 0d0a 2020 2020 2020 2020  e[0]):..        
-0001a560: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001a570: 2020 626f 756e 6461 7279 5b69 2c3a 5d20    boundary[i,:] 
-0001a580: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
-0001a590: 7328 6d61 736b 5b69 2c3a 5d29 0d0a 2020  s(mask[i,:])..  
-0001a5a0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
-0001a5b0: 6365 6e74 726f 6964 203d 2063 6f6d 7075  centroid = compu
-0001a5c0: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
-0001a5d0: 6461 7279 5b69 2c3a 5d29 200d 0a20 2020  dary[i,:]) ..   
-0001a5e0: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-0001a5f0: 203d 206e 702e 7768 6572 6528 626f 756e   = np.where(boun
-0001a600: 6461 7279 5b69 2c3a 5d20 3e20 3029 0d0a  dary[i,:] > 0)..
-0001a610: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001a620: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-0001a630: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-0001a640: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
-0001a650: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
-0001a660: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-0001a670: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-0001a680: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
-0001a690: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
-0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-0001a6c0: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
-0001a6d0: 6365 735b 6a5d 5b30 5d20 2a20 7a63 616c  ces[j][0] * zcal
-0001a6e0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-0001a6f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001a700: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-0001a710: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-0001a720: 6a5d 5b31 5d20 2a20 7963 616c 6962 7261  j][1] * ycalibra
-0001a730: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-0001a740: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-0001a750: 6e64 6963 6573 5b6a 5d5b 325d 203d 2072  ndices[j][2] = r
-0001a760: 6561 6c5f 696e 6469 6365 735b 6a5d 5b32  eal_indices[j][2
-0001a770: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
-0001a780: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a790: 7472 6565 203d 2073 7061 7469 616c 2e63  tree = spatial.c
-0001a7a0: 4b44 5472 6565 2872 6561 6c5f 696e 6469  KDTree(real_indi
-0001a7b0: 6365 7329 0d0a 2020 2020 2020 2020 2020  ces)..          
-0001a7c0: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
-0001a7d0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
-0001a7e0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
-0001a7f0: 7472 6f69 645d 0d0a 2020 2020 7072 696e  troid]..    prin
-0001a800: 7428 2743 6f6d 7075 7465 6420 7468 6520  t('Computed the 
-0001a810: 626f 756e 6461 7279 2070 6f69 6e74 7327  boundary points'
-0001a820: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
-0001a830: 7469 6d65 645f 6d61 736b 2c20 626f 756e  timed_mask, boun
-0001a840: 6461 7279 2020 2020 2020 2020 0d0a 0d0a  dary        ....
-0001a850: 6465 6620 636f 6d70 7574 655f 6365 6e74  def compute_cent
-0001a860: 726f 6964 2862 696e 6172 795f 696d 6167  roid(binary_imag
-0001a870: 6529 3a0d 0a20 2020 2023 2045 6e73 7572  e):..    # Ensur
-0001a880: 6520 6269 6e61 7279 2069 6d61 6765 2069  e binary image i
-0001a890: 7320 6120 4e75 6d50 7920 6172 7261 790d  s a NumPy array.
-0001a8a0: 0a20 2020 2062 696e 6172 795f 696d 6167  .    binary_imag
-0001a8b0: 6520 3d20 6e70 2e61 7272 6179 2862 696e  e = np.array(bin
-0001a8c0: 6172 795f 696d 6167 6529 0d0a 0d0a 2020  ary_image)....  
-0001a8d0: 2020 7768 6974 655f 7069 7865 6c73 203d    white_pixels =
-0001a8e0: 206e 702e 7768 6572 6528 6269 6e61 7279   np.where(binary
-0001a8f0: 5f69 6d61 6765 203d 3d20 3129 0d0a 2020  _image == 1)..  
-0001a900: 2020 6e75 6d5f 7069 7865 6c73 203d 206c    num_pixels = l
-0001a910: 656e 2877 6869 7465 5f70 6978 656c 735b  en(white_pixels[
-0001a920: 305d 290d 0a0d 0a20 2020 2023 2043 6f6d  0])....    # Com
-0001a930: 7075 7465 2074 6865 2063 656e 7472 6f69  pute the centroi
-0001a940: 6420 6f66 2074 6865 2077 6869 7465 2070  d of the white p
-0001a950: 6978 656c 7320 696e 2074 6865 2062 6f75  ixels in the bou
-0001a960: 6e64 6172 7920 696d 6167 650d 0a20 2020  ndary image..   
-0001a970: 2063 656e 7472 6f69 6420 3d20 6e70 2e7a   centroid = np.z
-0001a980: 6572 6f73 2862 696e 6172 795f 696d 6167  eros(binary_imag
-0001a990: 652e 6e64 696d 290d 0a20 2020 2066 6f72  e.ndim)..    for
-0001a9a0: 2064 696d 2069 6e20 7261 6e67 6528 6269   dim in range(bi
-0001a9b0: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
-0001a9c0: 3a0d 0a20 2020 2020 2020 2063 656e 7472  :..        centr
-0001a9d0: 6f69 645b 6469 6d5d 203d 2077 6869 7465  oid[dim] = white
-0001a9e0: 5f70 6978 656c 735b 6469 6d5d 2e73 756d  _pixels[dim].sum
-0001a9f0: 2829 202f 206e 756d 5f70 6978 656c 730d  () / num_pixels.
-0001aa00: 0a0d 0a20 2020 2072 6574 7572 6e20 6365  ...    return ce
-0001aa10: 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a 200d  ntroid........ .
-0001aa20: 0a0d 0a64 6566 2067 6574 5f63 7376 5f64  ...def get_csv_d
-0001aa30: 6174 6128 6373 7629 3a0d 0a0d 0a20 2020  ata(csv):....   
-0001aa40: 2020 2020 2064 6174 6173 6574 203d 2070       dataset = p
-0001aa50: 642e 7265 6164 5f63 7376 280d 0a20 2020  d.read_csv(..   
-0001aa60: 2020 2020 2020 2020 2063 7376 2c20 6465           csv, de
-0001aa70: 6c69 6d69 7465 723d 222c 222c 2065 6e63  limiter=",", enc
-0001aa80: 6f64 696e 673d 2275 6e69 636f 6465 5f65  oding="unicode_e
-0001aa90: 7363 6170 6522 2c20 6c6f 775f 6d65 6d6f  scape", low_memo
-0001aaa0: 7279 3d46 616c 7365 0d0a 2020 2020 2020  ry=False..      
-0001aab0: 2020 295b 333a 5d0d 0a20 2020 2020 2020    )[3:]..       
-0001aac0: 2064 6174 6173 6574 5f69 6e64 6578 203d   dataset_index =
-0001aad0: 2064 6174 6173 6574 2e69 6e64 6578 0d0a   dataset.index..
-0001aae0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-0001aaf0: 6174 6173 6574 2c20 6461 7461 7365 745f  ataset, dataset_
-0001ab00: 696e 6465 780d 0a20 2020 200d 0a64 6566  index..    ..def
-0001ab10: 2067 6574 5f73 706f 745f 6461 7461 7365   get_spot_datase
-0001ab20: 7428 7370 6f74 5f64 6174 6173 6574 2c20  t(spot_dataset, 
-0001ab30: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001ab40: 706f 745f 6b65 7973 2c20 7863 616c 6962  pot_keys, xcalib
-0001ab50: 7261 7469 6f6e 2c20 7963 616c 6962 7261  ration, ycalibra
-0001ab60: 7469 6f6e 2c20 7a63 616c 6962 7261 7469  tion, zcalibrati
-0001ab70: 6f6e 2c20 4174 7472 6962 7574 6542 6f78  on, AttributeBox
-0001ab80: 6e61 6d65 2c20 6465 7465 6374 696f 6e63  name, detectionc
-0001ab90: 6861 6e6e 656c 293a 0d0a 2020 2020 2020  hannel):..      
-0001aba0: 2020 416c 6c56 616c 7565 7320 3d20 7b7d    AllValues = {}
-0001abb0: 0d0a 2020 2020 2020 2020 706f 7369 7820  ..        posix 
-0001abc0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001abd0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-0001abe0: 7822 5d0d 0a20 2020 2020 2020 2070 6f73  x"]..        pos
-0001abf0: 6979 203d 2074 7261 636b 5f61 6e61 6c79  iy = track_analy
-0001ac00: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
-0001ac10: 6f73 6979 225d 0d0a 2020 2020 2020 2020  osiy"]..        
-0001ac20: 706f 7369 7a20 3d20 7472 6163 6b5f 616e  posiz = track_an
-0001ac30: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001ac40: 5b22 706f 7369 7a22 5d0d 0a20 2020 2020  ["posiz"]..     
-0001ac50: 2020 2066 7261 6d65 203d 2074 7261 636b     frame = track
-0001ac60: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001ac70: 6579 735b 2266 7261 6d65 225d 0d0a 2020  eys["frame"]..  
-0001ac80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001ac90: 4c6f 6361 7469 6f6e 5820 3d20 280d 0a20  LocationX = (.. 
-0001aca0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001acb0: 6461 7461 7365 745b 706f 7369 785d 2e61  dataset[posix].a
-0001acc0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001acd0: 2078 6361 6c69 6272 6174 696f 6e0d 0a20   xcalibration.. 
-0001ace0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001acf0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001ad00: 4c6f 6361 7469 6f6e 5920 3d20 280d 0a20  LocationY = (.. 
-0001ad10: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001ad20: 6461 7461 7365 745b 706f 7369 795d 2e61  dataset[posiy].a
-0001ad30: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001ad40: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
-0001ad50: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001ad60: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001ad70: 4c6f 6361 7469 6f6e 5a20 3d20 280d 0a20  LocationZ = (.. 
-0001ad80: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
-0001ad90: 6461 7461 7365 745b 706f 7369 7a5d 2e61  dataset[posiz].a
-0001ada0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
-0001adb0: 207a 6361 6c69 6272 6174 696f 6e0d 0a20   zcalibration.. 
-0001adc0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
-0001add0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
-0001ade0: 4c6f 6361 7469 6f6e 5420 3d20 2873 706f  LocationT = (spo
-0001adf0: 745f 6461 7461 7365 745b 6672 616d 655d  t_dataset[frame]
-0001ae00: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001ae10: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001ae20: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
-0001ae30: 2020 2020 2069 676e 6f72 655f 7661 6c75       ignore_valu
-0001ae40: 6573 203d 205b 7472 6163 6b5f 616e 616c  es = [track_anal
-0001ae50: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001ae60: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-0001ae70: 2c74 7261 636b 5f61 6e61 6c79 7369 735f  ,track_analysis_
-0001ae80: 7370 6f74 5f6b 6579 735b 2274 6f74 616c  spot_keys["total
-0001ae90: 5f69 6e74 656e 7369 7479 225d 5d0d 0a20  _intensity"]].. 
-0001aea0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-0001aeb0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001aec0: 6973 5f73 706f 745f 6b65 7973 2e69 7465  is_spot_keys.ite
-0001aed0: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
-0001aee0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
-0001aef0: 6374 696f 6e63 6861 6e6e 656c 203d 3d20  ctionchannel == 
-0001af00: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-0001af10: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
-0001af20: 2022 6d65 616e 5f69 6e74 656e 7369 7479   "mean_intensity
-0001af30: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
-0001af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af50: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
-0001af60: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001af70: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
-0001af80: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
-0001af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afa0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
-0001afb0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
-0001afc0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001afd0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
-0001afe0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
-0001aff0: 3d3d 2022 746f 7461 6c5f 696e 7465 6e73  == "total_intens
-0001b000: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
-0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b020: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
-0001b030: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001b040: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
-0001b050: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
-0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b070: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001b080: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
-0001b090: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-0001b0a0: 2266 6c6f 6174 2229 2020 2020 2020 200d  "float")       .
-0001b0b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001b0c0: 2020 2069 6620 7620 6e6f 7420 696e 2069     if v not in i
-0001b0d0: 676e 6f72 655f 7661 6c75 6573 3a0d 0a20  gnore_values:.. 
-0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001b100: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-0001b110: 6c6c 5661 6c75 6573 5b76 5d20 3d20 7370  llValues[v] = sp
-0001b120: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
-0001b130: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b150: 2020 0d0a 0d0a 2020 2020 2020 2020 416c    ....        Al
-0001b160: 6c56 616c 7565 735b 706f 7369 785d 203d  lValues[posix] =
-0001b170: 2072 6f75 6e64 284c 6f63 6174 696f 6e58   round(LocationX
-0001b180: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
-0001b190: 5661 6c75 6573 5b70 6f73 6979 5d20 3d20  Values[posiy] = 
-0001b1a0: 726f 756e 6428 4c6f 6361 7469 6f6e 592c  round(LocationY,
-0001b1b0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
-0001b1c0: 616c 7565 735b 706f 7369 7a5d 203d 2072  alues[posiz] = r
-0001b1d0: 6f75 6e64 284c 6f63 6174 696f 6e5a 2c33  ound(LocationZ,3
-0001b1e0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
-0001b1f0: 6c75 6573 5b66 7261 6d65 5d20 3d20 726f  lues[frame] = ro
-0001b200: 756e 6428 4c6f 6361 7469 6f6e 542c 3329  und(LocationT,3)
-0001b210: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-0001b220: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
-0001b230: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001b240: 732e 6170 7065 6e64 2841 7474 7269 6275  s.append(Attribu
-0001b250: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
-0001b260: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
-0001b270: 656e 616d 6520 696e 2041 6c6c 5661 6c75  ename in AllValu
-0001b280: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
-0001b290: 2020 2020 2020 2020 2020 4174 7472 6962            Attrib
-0001b2a0: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
-0001b2b0: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
-0001b2c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001b2d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001b2e0: 2020 7265 7475 726e 2041 7474 7269 6275    return Attribu
-0001b2f0: 7465 6964 732c 2041 6c6c 5661 6c75 6573  teids, AllValues
-0001b300: 2020 2020 200d 0a20 2020 200d 0a0d 0a64       ..    ....d
-0001b310: 6566 2067 6574 5f74 7261 636b 5f64 6174  ef get_track_dat
-0001b320: 6173 6574 2874 7261 636b 5f64 6174 6173  aset(track_datas
-0001b330: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
-0001b340: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
-0001b350: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
-0001b360: 636b 5f6b 6579 732c 2054 7261 636b 4174  ck_keys, TrackAt
-0001b370: 7472 6962 7574 6542 6f78 6e61 6d65 293a  tributeBoxname):
-0001b380: 0d0a 2020 2020 416c 6c54 7261 636b 5661  ..    AllTrackVa
-0001b390: 6c75 6573 203d 207b 7d0d 0a20 2020 2074  lues = {}..    t
-0001b3a0: 7261 636b 5f69 6420 3d20 7472 6163 6b5f  rack_id = track_
-0001b3b0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001b3c0: 7973 5b22 7472 6163 6b5f 6964 225d 0d0a  ys["track_id"]..
-0001b3d0: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
-0001b3e0: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
-0001b3f0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
-0001b400: 290d 0a0d 0a20 2020 2041 6c6c 5472 6163  )....    AllTrac
-0001b410: 6b56 616c 7565 735b 7472 6163 6b5f 6964  kValues[track_id
-0001b420: 5d20 3d20 5469 640d 0a0d 0a20 2020 2066  ] = Tid....    f
-0001b430: 6f72 2028 6b2c 2076 2920 696e 2074 7261  or (k, v) in tra
-0001b440: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001b450: 6b5f 6b65 7973 2e69 7465 6d73 2829 3a0d  k_keys.items():.
-0001b460: 0a20 2020 2020 2020 2078 203d 2074 7261  .        x = tra
-0001b470: 636b 5f64 6174 6173 6574 5b76 5d2e 6173  ck_dataset[v].as
-0001b480: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001b490: 2020 2020 2020 206d 696e 7661 6c20 3d20         minval = 
-0001b4a0: 6d69 6e28 7829 0d0a 2020 2020 2020 2020  min(x)..        
-0001b4b0: 6d61 7876 616c 203d 206d 6178 2878 290d  maxval = max(x).
-0001b4c0: 0a0d 0a20 2020 2020 2020 2069 6620 6d69  ...        if mi
-0001b4d0: 6e76 616c 203e 2030 2061 6e64 206d 6178  nval > 0 and max
-0001b4e0: 7661 6c20 3c3d 2031 3a0d 0a20 2020 2020  val <= 1:..     
-0001b4f0: 2020 2020 2020 2078 203d 2078 202b 2031         x = x + 1
-0001b500: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
-0001b510: 7261 636b 5661 6c75 6573 5b74 7261 636b  rackValues[track
-0001b520: 5f69 645d 5b6b 5d20 3d20 726f 756e 6428  _id][k] = round(
-0001b530: 782c 2033 290d 0a0d 0a20 2020 2054 7261  x, 3)....    Tra
-0001b540: 636b 4174 7472 6962 7574 6569 6473 203d  ckAttributeids =
-0001b550: 205b 5472 6163 6b41 7474 7269 6275 7465   [TrackAttribute
-0001b560: 426f 786e 616d 655d 202b 206c 6973 7428  Boxname] + list(
-0001b570: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-0001b580: 7261 636b 5f6b 6579 732e 6b65 7973 2829  rack_keys.keys()
-0001b590: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
-0001b5a0: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001b5b0: 732c 2041 6c6c 5472 6163 6b56 616c 7565  s, AllTrackValue
-0001b5c0: 730d 0a20 2020 200d 0a64 6566 2067 6574  s..    ..def get
-0001b5d0: 5f65 6467 6573 5f64 6174 6173 6574 2865  _edges_dataset(e
-0001b5e0: 6467 6573 5f64 6174 6173 6574 2c20 6564  dges_dataset, ed
-0001b5f0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
-0001b600: 782c 2074 7261 636b 5f61 6e61 6c79 7369  x, track_analysi
-0001b610: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
-0001b620: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-0001b630: 735f 6b65 7973 293a 0d0a 0d0a 2020 2020  s_keys):....    
-0001b640: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001b650: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001b660: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
-0001b670: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001b680: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
-0001b690: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
-0001b6a0: 6564 6765 735f 6461 7461 7365 745b 7472  edges_dataset[tr
-0001b6b0: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
-0001b6c0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001b6d0: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
-0001b6e0: 6572 6528 5469 6420 3d3d 2030 290d 0a20  ere(Tid == 0).. 
-0001b6f0: 2020 2020 2020 206d 6178 7472 6163 6b5f         maxtrack_
-0001b700: 6964 203d 206d 6178 2854 6964 290d 0a20  id = max(Tid).. 
-0001b710: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
-0001b720: 5f69 6e64 6963 6573 203d 2065 6467 6573  _indices = edges
-0001b730: 5f64 6174 6173 6574 5f69 6e64 6578 5b69  _dataset_index[i
-0001b740: 6e64 6963 6573 5d0d 0a20 2020 2020 2020  ndices]..       
-0001b750: 2054 6964 5b63 6f6e 6469 7469 6f6e 5f69   Tid[condition_i
-0001b760: 6e64 6963 6573 5d20 3d20 6d61 7874 7261  ndices] = maxtra
-0001b770: 636b 5f69 6420 2b20 310d 0a20 2020 2020  ck_id + 1..     
-0001b780: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001b790: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001b7a0: 640d 0a0d 0a20 2020 2020 2020 2066 6f72  d....        for
-0001b7b0: 206b 2069 6e20 7472 6163 6b5f 616e 616c   k in track_anal
-0001b7c0: 7973 6973 5f65 6467 6573 5f6b 6579 732e  ysis_edges_keys.
-0001b7d0: 7661 6c75 6573 2829 3a0d 0a0d 0a20 2020  values():....   
-0001b7e0: 2020 2020 2020 2020 2069 6620 6b20 213d           if k !=
-0001b7f0: 2074 7261 636b 5f69 643a 0d0a 2020 2020   track_id:..    
-0001b800: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-0001b810: 6564 6765 735f 6461 7461 7365 745b 6b5d  edges_dataset[k]
-0001b820: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001b830: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001b840: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001b850: 6573 5b6b 5d20 3d20 7820 2020 0d0a 2020  es[k] = x   ..  
-0001b860: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001b870: 2072 6574 7572 6e20 416c 6c45 6467 6573   return AllEdges
-0001b880: 5661 6c75 6573 2020 200d 0a20 2020 200d  Values   ..    .
-0001b890: 0a20 2020 2020 2020 0d0a 2020 2020 0d0a  .       ..    ..
-0001b8a0: 6465 6620 7363 616c 655f 7661 6c75 6528  def scale_value(
-0001b8b0: 782c 2073 6361 6c65 203d 2032 3535 202a  x, scale = 255 *
-0001b8c0: 2032 3535 293a 0d0a 0d0a 0d0a 2020 2020   255):......    
-0001b8d0: 2072 6574 7572 6e20 7820 2a20 7363 616c   return x * scal
-0001b8e0: 6520 2020 0d0a 2020 2020 0d0a 0d0a 0d0a  e   ..    ......
-0001b8f0: 6465 6620 7072 6f62 5f73 6967 6d6f 6964  def prob_sigmoid
-0001b900: 2878 293a 0d0a 2020 2020 7265 7475 726e  (x):..    return
-0001b910: 2031 202d 206d 6174 682e 6578 7028 2d78   1 - math.exp(-x
-0001b920: 290d 0a0d 0a0d 0a64 6566 2061 6e67 756c  )......def angul
-0001b930: 6172 5f63 6861 6e67 6528 7665 635f 302c  ar_change(vec_0,
-0001b940: 2076 6563 5f31 293a 0d0a 2020 2020 2020   vec_1):..      
-0001b950: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
-0001b960: 3020 3d20 7665 635f 3020 2f20 6e70 2e6c  0 = vec_0 / np.l
-0001b970: 696e 616c 672e 6e6f 726d 2876 6563 5f30  inalg.norm(vec_0
-0001b980: 290d 0a20 2020 2020 2020 2076 6563 5f31  )..        vec_1
-0001b990: 203d 2076 6563 5f31 202f 206e 702e 6c69   = vec_1 / np.li
-0001b9a0: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3129  nalg.norm(vec_1)
-0001b9b0: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
-0001b9c0: 3d20 6e70 2e61 7263 636f 7328 6e70 2e63  = np.arccos(np.c
-0001b9d0: 6c69 7028 6e70 2e64 6f74 2876 6563 5f30  lip(np.dot(vec_0
-0001b9e0: 2c20 7665 635f 3129 2c20 2d31 2e30 2c20  , vec_1), -1.0, 
-0001b9f0: 312e 3029 290d 0a20 2020 2020 2020 2061  1.0))..        a
-0001ba00: 6e67 6c65 203d 2061 6e67 6c65 202a 2031  ngle = angle * 1
-0001ba10: 3830 202f 206e 702e 7069 0d0a 2020 2020  80 / np.pi..    
-0001ba20: 2020 2020 7265 7475 726e 2061 6e67 6c65      return angle
-0001ba30: 0d0a 2020 2020 200d 0a0d 0a64 6566 2065  ..     ....def e
-0001ba40: 7661 6c5f 626f 6f6c 2876 616c 7565 293a  val_bool(value):
-0001ba50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ba60: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-0001ba70: 2076 616c 7565 2020 3d3d 2027 5472 7565   value  == 'True
-0001ba80: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
-0001ba90: 2020 2020 2064 6976 5f6b 6579 203d 2054       div_key = T
-0001baa0: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-0001bab0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001bac0: 2020 2020 6469 765f 6b65 7920 3d20 4661      div_key = Fa
-0001bad0: 6c73 6520 0d0a 0d0a 2020 2020 2020 2020  lse ....        
-0001bae0: 7265 7475 726e 2064 6976 5f6b 6579 2020  return div_key  
-0001baf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001bb00: 0d0a 6465 6620 6368 6563 6b5f 616e 645f  ..def check_and_
-0001bb10: 7570 6461 7465 5f6d 6173 6b28 6d61 736b  update_mask(mask
-0001bb20: 2c69 6d61 6765 293a 0d0a 2020 2020 2020  ,image):..      
-0001bb30: 200d 0a20 2020 2020 2020 2069 6620 6c65   ..        if le
-0001bb40: 6e28 6d61 736b 2e73 6861 7065 2920 3c20  n(mask.shape) < 
-0001bb50: 6c65 6e28 696d 6167 652e 7368 6170 6529  len(image.shape)
-0001bb60: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
-0001bb70: 7064 6174 655f 6d61 736b 203d 206e 702e  pdate_mask = np.
-0001bb80: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
-0001bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bba0: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
-0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbc0: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001bbd0: 7065 5b30 5d2c 0d0a 2020 2020 2020 2020  pe[0],..        
-0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbf0: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001bc00: 6170 655b 315d 2c0d 0a20 2020 2020 2020  ape[1],..       
-0001bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc20: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001bc30: 6861 7065 5b32 5d2c 0d0a 2020 2020 2020  hape[2],..      
-0001bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc50: 2020 2020 2020 2020 2020 696d 6167 652e            image.
-0001bc60: 7368 6170 655b 335d 2c0d 0a20 2020 2020  shape[3],..     
-0001bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc80: 2020 2020 2020 205d 2c20 6474 7970 653d         ], dtype=
-0001bc90: 2275 696e 7438 220d 0a20 2020 2020 2020  "uint8"..       
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcb0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0001bcc0: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
-0001bcd0: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
-0001bce0: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
-0001bcf0: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
-0001bd00: 696e 2072 616e 6765 2830 2c20 7570 6461  in range(0, upda
-0001bd10: 7465 5f6d 6173 6b2e 7368 6170 655b 315d  te_mask.shape[1]
-0001bd20: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0001bd30: 2020 2020 2020 2020 2020 7570 6461 7465            update
-0001bd40: 5f6d 6173 6b5b 692c 206a 2c20 3a2c 203a  _mask[i, j, :, :
-0001bd50: 5d20 3d20 6d61 736b 5b69 2c20 3a2c 203a  ] = mask[i, :, :
-0001bd60: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
-0001bd70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001bd80: 2020 7570 6461 7465 5f6d 6173 6b20 3d20    update_mask = 
-0001bd90: 6d61 736b 0d0a 0d0a 2020 2020 2020 2020  mask....        
-0001bda0: 7265 7475 726e 2075 7064 6174 655f 6d61  return update_ma
-0001bdb0: 736b 2020 2020 2020 2020 0d0a 2020 2020  sk        ..    
-0001bdc0: 2020 200d 0a                                ..
+000187f0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00018800: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018820: 2020 2020 2020 2020 2020 2061 6c6c 5f72             all_r
+00018830: 6164 6975 732e 6170 7065 6e64 284e 6f6e  adius.append(Non
+00018840: 6529 2020 2020 2020 200d 0a20 2020 2020  e)       ..     
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00018870: 5f73 7065 6564 2e61 7070 656e 6428 616c  _speed.append(al
+00018880: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00018890: 5d5b 7365 6c66 2e73 7065 6564 5f6b 6579  ][self.speed_key
+000188a0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 2020 2020 2020 616c 6c5f 6163 632e 6170        all_acc.ap
+000188d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+000188e0: 7261 636b 735b 6b5d 5b73 656c 662e 6163  racks[k][self.ac
+000188f0: 6365 6c65 7261 7469 6f6e 5f6b 6579 5d29  celeration_key])
+00018900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018920: 2020 2020 616c 6c5f 6469 7265 6374 696f      all_directio
+00018930: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018940: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00018950: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00018960: 6e5f 616e 676c 655f 6b65 795d 2920 2020  n_angle_key])   
+00018970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2020 2020 616c 6c5f 6469 7374 616e 6365      all_distance
+000189a0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+000189b0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000189c0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+000189d0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+000189e0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00018a20: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00018a30: 6963 5f64 6973 705f 7a20 3d20 6e70 2e61  ic_disp_z = np.a
+00018a40: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
+00018a50: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
+00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a70: 206d 6974 6f74 6963 5f64 6973 705f 7920   mitotic_disp_y 
+00018a80: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00018a90: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
+00018aa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018ab0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00018ac0: 6973 705f 7820 3d20 6e70 2e61 6273 286e  isp_x = np.abs(n
+00018ad0: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
+00018ae0: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
+00018af0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00018b00: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018b10: 7a20 3d20 6e70 2e61 6273 286e 702e 6469  z = np.abs(np.di
+00018b20: 6666 286e 6f6e 5f6d 6974 6f74 6963 5f64  ff(non_mitotic_d
+00018b30: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00018b40: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00018b50: 5f6d 6974 6f74 6963 5f64 6973 705f 7920  _mitotic_disp_y 
+00018b60: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00018b70: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00018b80: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+00018b90: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00018ba0: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
+00018bb0: 6e70 2e61 6273 286e 702e 6469 6666 286e  np.abs(np.diff(n
+00018bc0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018bd0: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00018be0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00018bf0: 6973 705f 7a20 3d20 6e70 2e61 6273 286e  isp_z = np.abs(n
+00018c00: 702e 6469 6666 2861 6c6c 5f64 6973 705f  p.diff(all_disp_
+00018c10: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+00018c20: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00018c30: 705f 7920 3d20 6e70 2e61 6273 286e 702e  p_y = np.abs(np.
+00018c40: 6469 6666 2861 6c6c 5f64 6973 705f 7929  diff(all_disp_y)
+00018c50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018c60: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00018c70: 7820 3d20 6e70 2e61 6273 286e 702e 6469  x = np.abs(np.di
+00018c80: 6666 2861 6c6c 5f64 6973 705f 7829 290d  ff(all_disp_x)).
+00018c90: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cb0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cd0: 2020 2073 656c 662e 7469 6d65 2e61 7070     self.time.app
+00018ce0: 656e 6428 6920 2a20 7365 6c66 2e74 6361  end(i * self.tca
+00018cf0: 6c69 6272 6174 696f 6e29 0d0a 0d0a 0d0a  libration)......
+00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d10: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018d20: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
+00018d30: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00018d40: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
+00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d60: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00018d70: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
+00018d80: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+00018d90: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018db0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00018dc0: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
+00018dd0: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
+00018de0: 6469 7370 5f79 2929 0d0a 2020 2020 2020  disp_y))..      
+00018df0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018e00: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00018e10: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
+00018e20: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
+00018e30: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
+00018e40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018e50: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00018e60: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
+00018e70: 6561 6e28 6d69 746f 7469 635f 6469 7370  ean(mitotic_disp
+00018e80: 5f78 2929 0d0a 2020 2020 2020 2020 2020  _x))..          
+00018e90: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018ea0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00018eb0: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
+00018ec0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00018ed0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018ee0: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
+00018ef0: 5f76 616c 7565 7320 3d20 5b76 616c 2066  _values = [val f
+00018f00: 6f72 2076 616c 2069 6e20 6d69 746f 7469  or val in mitoti
+00018f10: 635f 7261 6469 7573 2069 6620 7661 6c20  c_radius if val 
+00018f20: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00018f50: 6561 6e5f 7261 6469 7573 2e61 7070 656e  ean_radius.appen
+00018f60: 6428 6e70 2e6d 6561 6e28 6669 6c74 6572  d(np.mean(filter
+00018f70: 6564 5f76 616c 7565 7329 290d 0a20 2020  ed_values))..   
+00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00018fa0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018fb0: 7469 635f 7661 725f 7261 6469 7573 2e61  tic_var_radius.a
+00018fc0: 7070 656e 6428 6e70 2e73 7464 2866 696c  ppend(np.std(fil
+00018fd0: 7465 7265 645f 7661 6c75 6573 2929 0d0a  tered_values))..
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ff0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00019000: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00019010: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+00019020: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+00019030: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
+00019040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019050: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00019060: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+00019070: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00019080: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+000190b0: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+000190c0: 702e 6d65 616e 286d 6974 6f74 6963 5f61  p.mean(mitotic_a
+000190d0: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
+000190e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000190f0: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+00019100: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
+00019110: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
+00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019130: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00019140: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+00019150: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00019160: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
+00019170: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00019180: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00019190: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000191a0: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+000191b0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+000191c0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+000191d0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000191e0: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
+000191f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019200: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00019210: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00019220: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+00019230: 6e28 6d69 746f 7469 635f 6469 7374 616e  n(mitotic_distan
+00019240: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019260: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00019270: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
+00019280: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
+00019290: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+000192a0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+000192b0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000192c0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000192d0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000192e0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+000192f0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00019300: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
+00019310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019320: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00019330: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
+00019340: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00019350: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00019360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019370: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00019380: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00019390: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
+000193a0: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+000193b0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+000193c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000193d0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+000193e0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+000193f0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00019400: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+00019410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019420: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00019430: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
+00019440: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00019450: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00019460: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00019470: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00019480: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00019490: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
+000194a0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+000194b0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+000194c0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000194d0: 6c74 6572 6564 5f76 616c 7565 7320 3d20  ltered_values = 
+000194e0: 5b76 616c 2066 6f72 2076 616c 2069 6e20  [val for val in 
+000194f0: 6e6f 6e5f 6d69 746f 7469 635f 7261 6469  non_mitotic_radi
+00019500: 7573 2069 6620 7661 6c20 6973 206e 6f74  us if val is not
+00019510: 204e 6f6e 655d 0d0a 2020 2020 2020 2020   None]..        
+00019520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019530: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00019540: 6e5f 7261 6469 7573 2e61 7070 656e 6428  n_radius.append(
+00019550: 6e70 2e6d 6561 6e28 6669 6c74 6572 6564  np.mean(filtered
+00019560: 5f76 616c 7565 7329 290d 0a20 2020 2020  _values))..     
+00019570: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00019580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019590: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000195a0: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+000195b0: 2e61 7070 656e 6428 6e70 2e73 7464 2866  .append(np.std(f
+000195c0: 696c 7465 7265 645f 7661 6c75 6573 2929  iltered_values))
+000195d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000195e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000195f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7370  _mitotic_mean_sp
+00019600: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
+00019610: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f73  an(non_mitotic_s
+00019620: 7065 6564 2929 0d0a 2020 2020 2020 2020  peed))..        
+00019630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019640: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00019650: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00019660: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+00019670: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
+00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019690: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000196a0: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
+000196b0: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
+000196c0: 6f74 6963 5f61 6363 2929 0d0a 2020 2020  otic_acc))..    
+000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196e0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000196f0: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
+00019700: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00019710: 6963 5f61 6363 2929 0d0a 0d0a 2020 2020  ic_acc))....    
+00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019730: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00019740: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
+00019750: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00019760: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00019770: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
+00019780: 6368 616e 6765 2929 0d0a 2020 2020 2020  change))..      
+00019790: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000197a0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+000197b0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+000197c0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+000197d0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+000197e0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+000197f0: 6765 2929 200d 0a0d 0a20 2020 2020 2020  ge)) ....       
+00019800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019810: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00019820: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00019830: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+00019840: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+00019850: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00019860: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
+00019870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019880: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019890: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000198a0: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
+000198b0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+000198c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+000198d0: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+000198e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000198f0: 616c 6c5f 6d65 616e 5f64 6973 705f 7a2e  all_mean_disp_z.
+00019900: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00019910: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
+00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019930: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00019940: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
+00019950: 7464 2861 6c6c 5f64 6973 705f 7a29 290d  td(all_disp_z)).
+00019960: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019970: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00019980: 6d65 616e 5f64 6973 705f 792e 6170 7065  mean_disp_y.appe
+00019990: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
+000199a0: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+000199b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000199c0: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
+000199d0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+000199e0: 6c6c 5f64 6973 705f 7929 290d 0a0d 0a20  ll_disp_y)).... 
+000199f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a00: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00019a10: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00019a20: 702e 6d65 616e 2861 6c6c 5f64 6973 705f  p.mean(all_disp_
+00019a30: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+00019a40: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019a50: 6c5f 7661 725f 6469 7370 5f78 2e61 7070  l_var_disp_x.app
+00019a60: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
+00019a70: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
+00019a80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00019a90: 696c 7465 7265 645f 7661 6c75 6573 203d  iltered_values =
+00019aa0: 205b 7661 6c20 666f 7220 7661 6c20 696e   [val for val in
+00019ab0: 2061 6c6c 5f72 6164 6975 7320 6966 2076   all_radius if v
+00019ac0: 616c 2069 7320 6e6f 7420 4e6f 6e65 5d0d  al is not None].
+00019ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ae0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00019af0: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
+00019b00: 286e 702e 6d65 616e 2866 696c 7465 7265  (np.mean(filtere
+00019b10: 645f 7661 6c75 6573 2929 0d0a 2020 2020  d_values))..    
+00019b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019b40: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00019b50: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
+00019b60: 286e 702e 7374 6428 6669 6c74 6572 6564  (np.std(filtered
+00019b70: 5f76 616c 7565 7329 290d 0a0d 0a20 2020  _values))....   
+00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b90: 2073 656c 662e 616c 6c5f 6d65 616e 5f73   self.all_mean_s
+00019ba0: 7065 6564 2e61 7070 656e 6428 6e70 2e6d  peed.append(np.m
+00019bb0: 6561 6e28 616c 6c5f 7370 6565 6429 290d  ean(all_speed)).
+00019bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019bd0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00019be0: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
+00019bf0: 702e 7374 6428 616c 6c5f 7370 6565 6429  p.std(all_speed)
+00019c00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019c10: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019c20: 6c5f 6d65 616e 5f61 6363 2e61 7070 656e  l_mean_acc.appen
+00019c30: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6163  d(np.mean(all_ac
+00019c40: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+00019c50: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019c60: 6c5f 7661 725f 6163 632e 6170 7065 6e64  l_var_acc.append
+00019c70: 286e 702e 7374 6428 616c 6c5f 6163 6329  (np.std(all_acc)
+00019c80: 290d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  )........       
+00019c90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019ca0: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
+00019cb0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+00019cc0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00019cd0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019ce0: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00019cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019d00: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
+00019d10: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00019d20: 6428 6e70 2e73 7464 2861 6c6c 5f64 6972  d(np.std(all_dir
+00019d30: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00019d40: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019d50: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00019d60: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+00019d70: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00019d80: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
+00019d90: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00019da0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019db0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00019dc0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+00019dd0: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00019de0: 2e73 7464 2861 6c6c 5f64 6973 7461 6e63  .std(all_distanc
+00019df0: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+00019e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00019e20: 2020 2020 200d 0a64 6566 2062 6f75 6e64       ..def bound
+00019e30: 6172 795f 706f 696e 7473 286d 6173 6b2c  ary_points(mask,
+00019e40: 2078 6361 6c69 6272 6174 696f 6e2c 2079   xcalibration, y
+00019e50: 6361 6c69 6272 6174 696f 6e2c 207a 6361  calibration, zca
+00019e60: 6c69 6272 6174 696f 6e29 3a0d 0a0d 0a20  libration):.... 
+00019e70: 2020 206e 6469 6d20 3d20 6c65 6e28 6d61     ndim = len(ma
+00019e80: 736b 2e73 6861 7065 290d 0a20 2020 2074  sk.shape)..    t
+00019e90: 696d 6564 5f6d 6173 6b20 3d20 7b7d 0d0a  imed_mask = {}..
+00019ea0: 2020 2020 6d61 736b 203d 206d 6173 6b20      mask = mask 
+00019eb0: 3e20 300d 0a20 2020 206d 6173 6b20 3d20  > 0..    mask = 
+00019ec0: 6d61 736b 2e61 7374 7970 6528 2775 696e  mask.astype('uin
+00019ed0: 7438 2729 0d0a 2020 2020 2320 5958 2073  t8')..    # YX s
+00019ee0: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+00019ef0: 2020 6966 206e 6469 6d20 3d3d 2032 3a0d    if ndim == 2:.
+00019f00: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00019f10: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
+00019f20: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
+00019f30: 736b 290d 0a20 2020 2020 2020 2072 6567  sk)..        reg
+00019f40: 696f 6e63 656e 7472 6f69 6420 3d20 2830  ioncentroid = (0
+00019f50: 2c29 202b 2063 6f6d 7075 7465 5f63 656e  ,) + compute_cen
+00019f60: 7472 6f69 6428 626f 756e 6461 7279 2920  troid(boundary) 
+00019f70: 0d0a 2020 2020 2020 2020 696e 6469 6365  ..        indice
+00019f80: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00019f90: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+00019fa0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+00019fb0: 203d 206e 702e 7472 616e 7370 6f73 6528   = np.transpose(
+00019fc0: 6e70 2e61 7361 7272 6179 2869 6e64 6963  np.asarray(indic
+00019fd0: 6573 2c20 6474 7970 653d 6e70 2e66 6c6f  es, dtype=np.flo
+00019fe0: 6174 3332 2929 2e63 6f70 7928 290d 0a0d  at32)).copy()...
+00019ff0: 0a20 2020 2020 2020 2066 6f72 206a 2069  .        for j i
+0001a000: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+0001a010: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+0001a020: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001a030: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+0001a040: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+0001a050: 6a5d 5b30 5d20 2a20 7963 616c 6962 7261  j][0] * ycalibra
+0001a060: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+0001a070: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+0001a080: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+0001a090: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
+0001a0a0: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+0001a0b0: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
+0001a0c0: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
+0001a0d0: 696e 6469 6365 7329 0d0a 2020 2020 2020  indices)..      
+0001a0e0: 2020 2320 5468 6973 206f 626a 6563 7420    # This object 
+0001a0f0: 636f 6e74 6169 6e73 206c 6973 7420 6f66  contains list of
+0001a100: 2061 6c6c 2074 6865 2070 6f69 6e74 7320   all the points 
+0001a110: 666f 7220 616c 6c20 7468 6520 6c61 6265  for all the labe
+0001a120: 6c73 2069 6e20 7468 6520 4d61 736b 2069  ls in the Mask i
+0001a130: 6d61 6765 2077 6974 6820 7468 6520 6c61  mage with the la
+0001a140: 6265 6c20 6964 2061 6e64 2076 6f6c 756d  bel id and volum
+0001a150: 6520 6f66 2065 6163 6820 6c61 6265 6c0d  e of each label.
+0001a160: 0a20 2020 2020 2020 2074 696d 6564 5f6d  .        timed_m
+0001a170: 6173 6b5b 7374 7228 3029 5d20 3d20 5b74  ask[str(0)] = [t
+0001a180: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
+0001a190: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a0d  gioncentroid]...
+0001a1a0: 0a20 2020 2023 2054 5958 2073 6861 7065  .    # TYX shape
+0001a1b0: 6420 6f62 6a65 6374 0d0a 2020 2020 6966  d object..    if
+0001a1c0: 206e 6469 6d20 3d3d 2033 3a0d 0a0d 0a0d   ndim == 3:.....
+0001a1d0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0001a1e0: 6e20 7471 646d 2872 616e 6765 2830 2c20  n tqdm(range(0, 
+0001a1f0: 6d61 736b 2e73 6861 7065 5b30 5d29 293a  mask.shape[0])):
+0001a200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a210: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0001a220: 2020 2020 626f 756e 6461 7279 203d 2066      boundary = f
+0001a230: 696e 645f 626f 756e 6461 7269 6573 286d  ind_boundaries(m
+0001a240: 6173 6b5b 692c 3a5d 290d 0a20 2020 2020  ask[i,:])..     
+0001a250: 2020 2020 2020 2020 2020 2072 6567 696f             regio
+0001a260: 6e63 656e 7472 6f69 6420 3d20 2830 2c29  ncentroid = (0,)
+0001a270: 202b 2063 6f6d 7075 7465 5f63 656e 7472   + compute_centr
+0001a280: 6f69 6428 626f 756e 6461 7279 2920 0d0a  oid(boundary) ..
+0001a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2a0: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+0001a2b0: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
+0001a2c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a2d0: 2020 7265 616c 5f69 6e64 6963 6573 203d    real_indices =
+0001a2e0: 206e 702e 7472 616e 7370 6f73 6528 6e70   np.transpose(np
+0001a2f0: 2e61 7361 7272 6179 2869 6e64 6963 6573  .asarray(indices
+0001a300: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+0001a310: 3332 2929 2e63 6f70 7928 290d 0a0d 0a20  32)).copy().... 
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a330: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+0001a340: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+0001a350: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+0001a360: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001a370: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
+0001a380: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001a390: 5b30 5d20 2a20 7963 616c 6962 7261 7469  [0] * ycalibrati
+0001a3a0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+0001a3b0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+0001a3c0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+0001a3d0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+0001a3e0: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
+0001a3f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a400: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+0001a410: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+0001a420: 6469 6365 7329 0d0a 0d0a 2020 2020 2020  dices)....      
+0001a430: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
+0001a440: 6d61 736b 5b73 7472 2869 295d 203d 205b  mask[str(i)] = [
+0001a450: 7472 6565 2c20 696e 6469 6365 732c 2072  tree, indices, r
+0001a460: 6567 696f 6e63 656e 7472 6f69 645d 0d0a  egioncentroid]..
+0001a470: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001a480: 2020 2320 545a 5958 2073 6861 7065 6420    # TZYX shaped 
+0001a490: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+0001a4a0: 6469 6d20 3d3d 2034 3a0d 0a20 2020 2020  dim == 4:..     
+0001a4b0: 2020 2070 7269 6e74 2827 4d61 6b69 6e67     print('Making
+0001a4c0: 206d 6173 6b20 696e 2034 4427 290d 0a20   mask in 4D').. 
+0001a4d0: 2020 2020 2020 2062 6f75 6e64 6172 7920         boundary 
+0001a4e0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
+0001a4f0: 2020 2020 2020 2020 205b 6d61 736b 2e73           [mask.s
+0001a500: 6861 7065 5b30 5d2c 206d 6173 6b2e 7368  hape[0], mask.sh
+0001a510: 6170 655b 315d 2c20 6d61 736b 2e73 6861  ape[1], mask.sha
+0001a520: 7065 5b32 5d2c 206d 6173 6b2e 7368 6170  pe[2], mask.shap
+0001a530: 655b 335d 5d2c 2064 7479 7065 3d6e 702e  e[3]], dtype=np.
+0001a540: 7569 6e74 380d 0a20 2020 2020 2020 2029  uint8..        )
+0001a550: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
+0001a560: 696e 2072 616e 6765 2830 2c20 6d61 736b  in range(0, mask
+0001a570: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
+0001a580: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001a590: 2020 2020 2020 2062 6f75 6e64 6172 795b         boundary[
+0001a5a0: 692c 3a5d 203d 2066 696e 645f 626f 756e  i,:] = find_boun
+0001a5b0: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
+0001a5c0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0001a5d0: 6567 696f 6e63 656e 7472 6f69 6420 3d20  egioncentroid = 
+0001a5e0: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
+0001a5f0: 2862 6f75 6e64 6172 795b 692c 3a5d 2920  (boundary[i,:]) 
+0001a600: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+0001a610: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+0001a620: 2862 6f75 6e64 6172 795b 692c 3a5d 203e  (boundary[i,:] >
+0001a630: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001a640: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
+0001a650: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
+0001a660: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
+0001a670: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+0001a680: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
+0001a690: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0001a6a0: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
+0001a6b0: 7265 616c 5f69 6e64 6963 6573 2929 3a0d  real_indices)):.
+0001a6c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001a6d0: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+0001a6e0: 6365 735b 6a5d 5b30 5d20 3d20 7265 616c  ces[j][0] = real
+0001a6f0: 5f69 6e64 6963 6573 5b6a 5d5b 305d 202a  _indices[j][0] *
+0001a700: 207a 6361 6c69 6272 6174 696f 6e0d 0a20   zcalibration.. 
+0001a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a720: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
+0001a730: 6a5d 5b31 5d20 3d20 7265 616c 5f69 6e64  j][1] = real_ind
+0001a740: 6963 6573 5b6a 5d5b 315d 202a 2079 6361  ices[j][1] * yca
+0001a750: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001a770: 6561 6c5f 696e 6469 6365 735b 6a5d 5b32  eal_indices[j][2
+0001a780: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
+0001a790: 5b6a 5d5b 325d 202a 2078 6361 6c69 6272  [j][2] * xcalibr
+0001a7a0: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
+0001a7b0: 2020 2020 2074 7265 6520 3d20 7370 6174       tree = spat
+0001a7c0: 6961 6c2e 634b 4454 7265 6528 7265 616c  ial.cKDTree(real
+0001a7d0: 5f69 6e64 6963 6573 290d 0a20 2020 2020  _indices)..     
+0001a7e0: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+0001a7f0: 6b5b 7374 7228 6929 5d20 3d20 5b74 7265  k[str(i)] = [tre
+0001a800: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+0001a810: 6f6e 6365 6e74 726f 6964 5d0d 0a20 2020  oncentroid]..   
+0001a820: 2070 7269 6e74 2827 436f 6d70 7574 6564   print('Computed
+0001a830: 2074 6865 2062 6f75 6e64 6172 7920 706f   the boundary po
+0001a840: 696e 7473 2729 0d0a 0d0a 2020 2020 7265  ints')....    re
+0001a850: 7475 726e 2074 696d 6564 5f6d 6173 6b2c  turn timed_mask,
+0001a860: 2062 6f75 6e64 6172 7920 2020 2020 2020   boundary       
+0001a870: 200d 0a0d 0a64 6566 2063 6f6d 7075 7465   ....def compute
+0001a880: 5f63 656e 7472 6f69 6428 6269 6e61 7279  _centroid(binary
+0001a890: 5f69 6d61 6765 293a 0d0a 2020 2020 2320  _image):..    # 
+0001a8a0: 456e 7375 7265 2062 696e 6172 7920 696d  Ensure binary im
+0001a8b0: 6167 6520 6973 2061 204e 756d 5079 2061  age is a NumPy a
+0001a8c0: 7272 6179 0d0a 2020 2020 6269 6e61 7279  rray..    binary
+0001a8d0: 5f69 6d61 6765 203d 206e 702e 6172 7261  _image = np.arra
+0001a8e0: 7928 6269 6e61 7279 5f69 6d61 6765 290d  y(binary_image).
+0001a8f0: 0a0d 0a20 2020 2077 6869 7465 5f70 6978  ...    white_pix
+0001a900: 656c 7320 3d20 6e70 2e77 6865 7265 2862  els = np.where(b
+0001a910: 696e 6172 795f 696d 6167 6520 3d3d 2031  inary_image == 1
+0001a920: 290d 0a20 2020 206e 756d 5f70 6978 656c  )..    num_pixel
+0001a930: 7320 3d20 6c65 6e28 7768 6974 655f 7069  s = len(white_pi
+0001a940: 7865 6c73 5b30 5d29 0d0a 0d0a 2020 2020  xels[0])....    
+0001a950: 2320 436f 6d70 7574 6520 7468 6520 6365  # Compute the ce
+0001a960: 6e74 726f 6964 206f 6620 7468 6520 7768  ntroid of the wh
+0001a970: 6974 6520 7069 7865 6c73 2069 6e20 7468  ite pixels in th
+0001a980: 6520 626f 756e 6461 7279 2069 6d61 6765  e boundary image
+0001a990: 0d0a 2020 2020 6365 6e74 726f 6964 203d  ..    centroid =
+0001a9a0: 206e 702e 7a65 726f 7328 6269 6e61 7279   np.zeros(binary
+0001a9b0: 5f69 6d61 6765 2e6e 6469 6d29 0d0a 2020  _image.ndim)..  
+0001a9c0: 2020 666f 7220 6469 6d20 696e 2072 616e    for dim in ran
+0001a9d0: 6765 2862 696e 6172 795f 696d 6167 652e  ge(binary_image.
+0001a9e0: 6e64 696d 293a 0d0a 2020 2020 2020 2020  ndim):..        
+0001a9f0: 6365 6e74 726f 6964 5b64 696d 5d20 3d20  centroid[dim] = 
+0001aa00: 7768 6974 655f 7069 7865 6c73 5b64 696d  white_pixels[dim
+0001aa10: 5d2e 7375 6d28 2920 2f20 6e75 6d5f 7069  ].sum() / num_pi
+0001aa20: 7865 6c73 0d0a 0d0a 2020 2020 7265 7475  xels....    retu
+0001aa30: 726e 2063 656e 7472 6f69 640d 0a0d 0a0d  rn centroid.....
+0001aa40: 0a0d 0a20 0d0a 0d0a 6465 6620 6765 745f  ... ....def get_
+0001aa50: 6373 765f 6461 7461 2863 7376 293a 0d0a  csv_data(csv):..
+0001aa60: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
+0001aa70: 7420 3d20 7064 2e72 6561 645f 6373 7628  t = pd.read_csv(
+0001aa80: 0d0a 2020 2020 2020 2020 2020 2020 6373  ..            cs
+0001aa90: 762c 2064 656c 696d 6974 6572 3d22 2c22  v, delimiter=","
+0001aaa0: 2c20 656e 636f 6469 6e67 3d22 756e 6963  , encoding="unic
+0001aab0: 6f64 655f 6573 6361 7065 222c 206c 6f77  ode_escape", low
+0001aac0: 5f6d 656d 6f72 793d 4661 6c73 650d 0a20  _memory=False.. 
+0001aad0: 2020 2020 2020 2029 5b33 3a5d 0d0a 2020         )[3:]..  
+0001aae0: 2020 2020 2020 6461 7461 7365 745f 696e        dataset_in
+0001aaf0: 6465 7820 3d20 6461 7461 7365 742e 696e  dex = dataset.in
+0001ab00: 6465 780d 0a20 2020 2020 2020 2072 6574  dex..        ret
+0001ab10: 7572 6e20 6461 7461 7365 742c 2064 6174  urn dataset, dat
+0001ab20: 6173 6574 5f69 6e64 6578 0d0a 2020 2020  aset_index..    
+0001ab30: 0d0a 6465 6620 6765 745f 7370 6f74 5f64  ..def get_spot_d
+0001ab40: 6174 6173 6574 2873 706f 745f 6461 7461  ataset(spot_data
+0001ab50: 7365 742c 2074 7261 636b 5f61 6e61 6c79  set, track_analy
+0001ab60: 7369 735f 7370 6f74 5f6b 6579 732c 2078  sis_spot_keys, x
+0001ab70: 6361 6c69 6272 6174 696f 6e2c 2079 6361  calibration, yca
+0001ab80: 6c69 6272 6174 696f 6e2c 207a 6361 6c69  libration, zcali
+0001ab90: 6272 6174 696f 6e2c 2041 7474 7269 6275  bration, Attribu
+0001aba0: 7465 426f 786e 616d 652c 2064 6574 6563  teBoxname, detec
+0001abb0: 7469 6f6e 6368 616e 6e65 6c29 3a0d 0a20  tionchannel):.. 
+0001abc0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001abd0: 203d 207b 7d0d 0a20 2020 2020 2020 2070   = {}..        p
+0001abe0: 6f73 6978 203d 2074 7261 636b 5f61 6e61  osix = track_ana
+0001abf0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001ac00: 2270 6f73 6978 225d 0d0a 2020 2020 2020  "posix"]..      
+0001ac10: 2020 706f 7369 7920 3d20 7472 6163 6b5f    posiy = track_
+0001ac20: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001ac30: 7973 5b22 706f 7369 7922 5d0d 0a20 2020  ys["posiy"]..   
+0001ac40: 2020 2020 2070 6f73 697a 203d 2074 7261       posiz = tra
+0001ac50: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001ac60: 5f6b 6579 735b 2270 6f73 697a 225d 0d0a  _keys["posiz"]..
+0001ac70: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
+0001ac80: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001ac90: 706f 745f 6b65 7973 5b22 6672 616d 6522  pot_keys["frame"
+0001aca0: 5d0d 0a20 2020 2020 2020 200d 0a20 2020  ]..        ..   
+0001acb0: 2020 2020 204c 6f63 6174 696f 6e58 203d       LocationX =
+0001acc0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001acd0: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+0001ace0: 6978 5d2e 6173 7479 7065 2822 666c 6f61  ix].astype("floa
+0001acf0: 7422 2920 2f20 7863 616c 6962 7261 7469  t") / xcalibrati
+0001ad00: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+0001ad10: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+0001ad20: 2020 2020 204c 6f63 6174 696f 6e59 203d       LocationY =
+0001ad30: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001ad40: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+0001ad50: 6979 5d2e 6173 7479 7065 2822 666c 6f61  iy].astype("floa
+0001ad60: 7422 2920 2f20 7963 616c 6962 7261 7469  t") / ycalibrati
+0001ad70: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+0001ad80: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+0001ad90: 2020 2020 204c 6f63 6174 696f 6e5a 203d       LocationZ =
+0001ada0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
+0001adb0: 7370 6f74 5f64 6174 6173 6574 5b70 6f73  spot_dataset[pos
+0001adc0: 697a 5d2e 6173 7479 7065 2822 666c 6f61  iz].astype("floa
+0001add0: 7422 2920 2f20 7a63 616c 6962 7261 7469  t") / zcalibrati
+0001ade0: 6f6e 0d0a 2020 2020 2020 2020 292e 6173  on..        ).as
+0001adf0: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+0001ae00: 2020 2020 204c 6f63 6174 696f 6e54 203d       LocationT =
+0001ae10: 2028 7370 6f74 5f64 6174 6173 6574 5b66   (spot_dataset[f
+0001ae20: 7261 6d65 5d2e 6173 7479 7065 2822 666c  rame].astype("fl
+0001ae30: 6f61 7422 2929 2e61 7374 7970 6528 2269  oat")).astype("i
+0001ae40: 6e74 2229 0d0a 2020 2020 2020 2020 0d0a  nt")..        ..
+0001ae50: 0d0a 2020 2020 2020 2020 6967 6e6f 7265  ..        ignore
+0001ae60: 5f76 616c 7565 7320 3d20 5b74 7261 636b  _values = [track
+0001ae70: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001ae80: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
+0001ae90: 6974 7922 5d2c 7472 6163 6b5f 616e 616c  ity"],track_anal
+0001aea0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001aeb0: 746f 7461 6c5f 696e 7465 6e73 6974 7922  total_intensity"
+0001aec0: 5d5d 0d0a 2020 2020 2020 2020 666f 7220  ]]..        for 
+0001aed0: 286b 2c76 2920 696e 2074 7261 636b 5f61  (k,v) in track_a
+0001aee0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001aef0: 732e 6974 656d 7328 293a 0d0a 0d0a 2020  s.items():....  
+0001af00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001af10: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+0001af20: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
+0001af30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001af40: 206b 203d 3d20 226d 6561 6e5f 696e 7465   k == "mean_inte
+0001af50: 6e73 6974 795f 6368 3222 3a0d 0a20 2020  nsity_ch2":..   
+0001af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af70: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0001af80: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001af90: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
+0001afa0: 6e74 656e 7369 7479 225d 0d0a 2020 2020  ntensity"]..    
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afc0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001afd0: 5b76 616c 7565 5d20 3d20 7370 6f74 5f64  [value] = spot_d
+0001afe0: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
+0001aff0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b010: 6966 206b 203d 3d20 2274 6f74 616c 5f69  if k == "total_i
+0001b020: 6e74 656e 7369 7479 5f63 6832 223a 0d0a  ntensity_ch2":..
+0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b040: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0001b050: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+0001b060: 735f 7370 6f74 5f6b 6579 735b 2274 6f74  s_spot_keys["tot
+0001b070: 616c 5f69 6e74 656e 7369 7479 225d 0d0a  al_intensity"]..
+0001b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b090: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
+0001b0a0: 6c75 6573 5b76 616c 7565 5d20 3d20 7370  lues[value] = sp
+0001b0b0: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+0001b0c0: 7479 7065 2822 666c 6f61 7422 2920 2020  type("float")   
+0001b0d0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0001b0e0: 2020 2020 2020 2020 6966 2076 206e 6f74          if v not
+0001b0f0: 2069 6e20 6967 6e6f 7265 5f76 616c 7565   in ignore_value
+0001b100: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001b110: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b130: 2020 2020 416c 6c56 616c 7565 735b 765d      AllValues[v]
+0001b140: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
+0001b150: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+0001b160: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0001b170: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+0001b180: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
+0001b190: 6978 5d20 3d20 726f 756e 6428 4c6f 6361  ix] = round(Loca
+0001b1a0: 7469 6f6e 582c 3329 0d0a 2020 2020 2020  tionX,3)..      
+0001b1b0: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
+0001b1c0: 795d 203d 2072 6f75 6e64 284c 6f63 6174  y] = round(Locat
+0001b1d0: 696f 6e59 2c33 290d 0a20 2020 2020 2020  ionY,3)..       
+0001b1e0: 2041 6c6c 5661 6c75 6573 5b70 6f73 697a   AllValues[posiz
+0001b1f0: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
+0001b200: 6f6e 5a2c 3329 0d0a 2020 2020 2020 2020  onZ,3)..        
+0001b210: 416c 6c56 616c 7565 735b 6672 616d 655d  AllValues[frame]
+0001b220: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+0001b230: 6e54 2c33 290d 0a20 2020 2020 2020 2041  nT,3)..        A
+0001b240: 7474 7269 6275 7465 6964 7320 3d20 5b5d  ttributeids = []
+0001b250: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+0001b260: 7574 6569 6473 2e61 7070 656e 6428 4174  uteids.append(At
+0001b270: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
+0001b280: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
+0001b290: 7269 6275 7465 6e61 6d65 2069 6e20 416c  ributename in Al
+0001b2a0: 6c56 616c 7565 732e 6b65 7973 2829 3a0d  lValues.keys():.
+0001b2b0: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
+0001b2c0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
+0001b2d0: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
+0001b2e0: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
+0001b2f0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
+0001b300: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
+0001b310: 7472 6962 7574 6569 6473 2c20 416c 6c56  tributeids, AllV
+0001b320: 616c 7565 7320 2020 2020 0d0a 2020 2020  alues     ..    
+0001b330: 0d0a 0d0a 6465 6620 6765 745f 7472 6163  ....def get_trac
+0001b340: 6b5f 6461 7461 7365 7428 416c 6c54 7261  k_dataset(AllTra
+0001b350: 636b 5661 6c75 6573 2c20 7472 6163 6b5f  ckValues, track_
+0001b360: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
+0001b370: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001b380: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
+0001b390: 735f 7472 6163 6b5f 6b65 7973 2c20 5472  s_track_keys, Tr
+0001b3a0: 6163 6b41 7474 7269 6275 7465 426f 786e  ackAttributeBoxn
+0001b3b0: 616d 6529 3a0d 0a20 2020 0d0a 2020 2020  ame):..   ..    
+0001b3c0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
+0001b3d0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001b3e0: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
+0001b3f0: 0a20 2020 2054 6964 203d 2069 6e74 2874  .    Tid = int(t
+0001b400: 7261 636b 5f64 6174 6173 6574 5b74 7261  rack_dataset[tra
+0001b410: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
+0001b420: 6c6f 6174 2229 290d 0a0d 0a20 2020 2041  loat"))....    A
+0001b430: 6c6c 5472 6163 6b56 616c 7565 735b 5469  llTrackValues[Ti
+0001b440: 645d 203d 207b 7d0d 0a0d 0a20 2020 2066  d] = {}....    f
+0001b450: 6f72 2028 6b2c 2076 2920 696e 2074 7261  or (k, v) in tra
+0001b460: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
+0001b470: 6b5f 6b65 7973 2e69 7465 6d73 2829 3a0d  k_keys.items():.
+0001b480: 0a20 2020 2020 2020 2078 203d 2074 7261  .        x = tra
+0001b490: 636b 5f64 6174 6173 6574 5b76 5d2e 6173  ck_dataset[v].as
+0001b4a0: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001b4b0: 2020 2020 2020 206d 696e 7661 6c20 3d20         minval = 
+0001b4c0: 6d69 6e28 7829 0d0a 2020 2020 2020 2020  min(x)..        
+0001b4d0: 6d61 7876 616c 203d 206d 6178 2878 290d  maxval = max(x).
+0001b4e0: 0a0d 0a20 2020 2020 2020 2069 6620 6d69  ...        if mi
+0001b4f0: 6e76 616c 203e 2030 2061 6e64 206d 6178  nval > 0 and max
+0001b500: 7661 6c20 3c3d 2031 3a0d 0a20 2020 2020  val <= 1:..     
+0001b510: 2020 2020 2020 2078 203d 2078 202b 2031         x = x + 1
+0001b520: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
+0001b530: 7261 636b 5661 6c75 6573 5b54 6964 5d5b  rackValues[Tid][
+0001b540: 6b5d 203d 2072 6f75 6e64 2878 2c20 3329  k] = round(x, 3)
+0001b550: 0d0a 0d0a 2020 2020 5472 6163 6b41 7474  ....    TrackAtt
+0001b560: 7269 6275 7465 6964 7320 3d20 5b54 7261  ributeids = [Tra
+0001b570: 636b 4174 7472 6962 7574 6542 6f78 6e61  ckAttributeBoxna
+0001b580: 6d65 5d20 2b20 6c69 7374 2874 7261 636b  me] + list(track
+0001b590: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001b5a0: 6b65 7973 2e6b 6579 7328 2929 0d0a 0d0a  keys.keys())....
+0001b5b0: 2020 2020 7265 7475 726e 2054 7261 636b      return Track
+0001b5c0: 4174 7472 6962 7574 6569 6473 2c20 416c  Attributeids, Al
+0001b5d0: 6c54 7261 636b 5661 6c75 6573 0d0a 2020  lTrackValues..  
+0001b5e0: 2020 0d0a 6465 6620 6765 745f 6564 6765    ..def get_edge
+0001b5f0: 735f 6461 7461 7365 7428 6564 6765 735f  s_dataset(edges_
+0001b600: 6461 7461 7365 742c 2065 6467 6573 5f64  dataset, edges_d
+0001b610: 6174 6173 6574 5f69 6e64 6578 2c20 7472  ataset_index, tr
+0001b620: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001b630: 745f 6b65 7973 2c20 7472 6163 6b5f 616e  t_keys, track_an
+0001b640: 616c 7973 6973 5f65 6467 6573 5f6b 6579  alysis_edges_key
+0001b650: 7329 3a0d 0a0d 0a20 2020 2020 2020 2041  s):....        A
+0001b660: 6c6c 4564 6765 7356 616c 7565 7320 3d20  llEdgesValues = 
+0001b670: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
+0001b680: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
+0001b690: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001b6a0: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
+0001b6b0: 2020 2020 2054 6964 203d 2065 6467 6573       Tid = edges
+0001b6c0: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
+0001b6d0: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
+0001b6e0: 2229 0d0a 2020 2020 2020 2020 696e 6469  ")..        indi
+0001b6f0: 6365 7320 3d20 6e70 2e77 6865 7265 2854  ces = np.where(T
+0001b700: 6964 203d 3d20 3029 0d0a 2020 2020 2020  id == 0)..      
+0001b710: 2020 6d61 7874 7261 636b 5f69 6420 3d20    maxtrack_id = 
+0001b720: 6d61 7828 5469 6429 0d0a 2020 2020 2020  max(Tid)..      
+0001b730: 2020 636f 6e64 6974 696f 6e5f 696e 6469    condition_indi
+0001b740: 6365 7320 3d20 6564 6765 735f 6461 7461  ces = edges_data
+0001b750: 7365 745f 696e 6465 785b 696e 6469 6365  set_index[indice
+0001b760: 735d 0d0a 2020 2020 2020 2020 5469 645b  s]..        Tid[
+0001b770: 636f 6e64 6974 696f 6e5f 696e 6469 6365  condition_indice
+0001b780: 735d 203d 206d 6178 7472 6163 6b5f 6964  s] = maxtrack_id
+0001b790: 202b 2031 0d0a 2020 2020 2020 2020 416c   + 1..        Al
+0001b7a0: 6c45 6467 6573 5661 6c75 6573 5b74 7261  lEdgesValues[tra
+0001b7b0: 636b 5f69 645d 203d 2054 6964 0d0a 0d0a  ck_id] = Tid....
+0001b7c0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+0001b7d0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001b7e0: 6564 6765 735f 6b65 7973 2e76 616c 7565  edges_keys.value
+0001b7f0: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001b800: 2020 2020 6966 206b 2021 3d20 7472 6163      if k != trac
+0001b810: 6b5f 6964 3a0d 0a20 2020 2020 2020 2020  k_id:..         
+0001b820: 2020 2020 2020 2078 203d 2065 6467 6573         x = edges
+0001b830: 5f64 6174 6173 6574 5b6b 5d2e 6173 7479  _dataset[k].asty
+0001b840: 7065 2822 666c 6f61 7422 290d 0a0d 0a20  pe("float").... 
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001b860: 6c6c 4564 6765 7356 616c 7565 735b 6b5d  llEdgesValues[k]
+0001b870: 203d 2078 2020 200d 0a20 2020 2020 2020   = x   ..       
+0001b880: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+0001b890: 726e 2041 6c6c 4564 6765 7356 616c 7565  rn AllEdgesValue
+0001b8a0: 7320 2020 0d0a 2020 2020 0d0a 2020 2020  s   ..    ..    
+0001b8b0: 2020 200d 0a20 2020 200d 0a64 6566 2073     ..    ..def s
+0001b8c0: 6361 6c65 5f76 616c 7565 2878 2c20 7363  cale_value(x, sc
+0001b8d0: 616c 6520 3d20 3235 3520 2a20 3235 3529  ale = 255 * 255)
+0001b8e0: 3a0d 0a0d 0a0d 0a20 2020 2020 7265 7475  :......     retu
+0001b8f0: 726e 2078 202a 2073 6361 6c65 2020 200d  rn x * scale   .
+0001b900: 0a20 2020 200d 0a0d 0a0d 0a64 6566 2070  .    ......def p
+0001b910: 726f 625f 7369 676d 6f69 6428 7829 3a0d  rob_sigmoid(x):.
+0001b920: 0a20 2020 2072 6574 7572 6e20 3120 2d20  .    return 1 - 
+0001b930: 6d61 7468 2e65 7870 282d 7829 0d0a 0d0a  math.exp(-x)....
+0001b940: 0d0a 6465 6620 616e 6775 6c61 725f 6368  ..def angular_ch
+0001b950: 616e 6765 2876 6563 5f30 2c20 7665 635f  ange(vec_0, vec_
+0001b960: 3129 3a0d 0a20 2020 2020 2020 200d 0a20  1):..        .. 
+0001b970: 2020 2020 2020 2076 6563 5f30 203d 2076         vec_0 = v
+0001b980: 6563 5f30 202f 206e 702e 6c69 6e61 6c67  ec_0 / np.linalg
+0001b990: 2e6e 6f72 6d28 7665 635f 3029 0d0a 2020  .norm(vec_0)..  
+0001b9a0: 2020 2020 2020 7665 635f 3120 3d20 7665        vec_1 = ve
+0001b9b0: 635f 3120 2f20 6e70 2e6c 696e 616c 672e  c_1 / np.linalg.
+0001b9c0: 6e6f 726d 2876 6563 5f31 290d 0a20 2020  norm(vec_1)..   
+0001b9d0: 2020 2020 2061 6e67 6c65 203d 206e 702e       angle = np.
+0001b9e0: 6172 6363 6f73 286e 702e 636c 6970 286e  arccos(np.clip(n
+0001b9f0: 702e 646f 7428 7665 635f 302c 2076 6563  p.dot(vec_0, vec
+0001ba00: 5f31 292c 202d 312e 302c 2031 2e30 2929  _1), -1.0, 1.0))
+0001ba10: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
+0001ba20: 3d20 616e 676c 6520 2a20 3138 3020 2f20  = angle * 180 / 
+0001ba30: 6e70 2e70 690d 0a20 2020 2020 2020 2072  np.pi..        r
+0001ba40: 6574 7572 6e20 616e 676c 650d 0a20 2020  eturn angle..   
+0001ba50: 2020 0d0a 0d0a 6465 6620 6576 616c 5f62    ....def eval_b
+0001ba60: 6f6f 6c28 7661 6c75 6529 3a0d 0a20 2020  ool(value):..   
+0001ba70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0001ba80: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
+0001ba90: 6520 203d 3d20 2754 7275 6527 3a20 0d0a  e  == 'True': ..
+0001baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bab0: 6469 765f 6b65 7920 3d20 5472 7565 0d0a  div_key = True..
+0001bac0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001bad0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001bae0: 6976 5f6b 6579 203d 2046 616c 7365 200d  iv_key = False .
+0001baf0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001bb00: 6e20 6469 765f 6b65 7920 2020 2020 2020  n div_key       
+0001bb10: 2020 2020 2020 2020 200d 0a0d 0a64 6566           ....def
+0001bb20: 2063 6865 636b 5f61 6e64 5f75 7064 6174   check_and_updat
+0001bb30: 655f 6d61 736b 286d 6173 6b2c 696d 6167  e_mask(mask,imag
+0001bb40: 6529 3a0d 0a20 2020 2020 2020 0d0a 2020  e):..       ..  
+0001bb50: 2020 2020 2020 6966 206c 656e 286d 6173        if len(mas
+0001bb60: 6b2e 7368 6170 6529 203c 206c 656e 2869  k.shape) < len(i
+0001bb70: 6d61 6765 2e73 6861 7065 293a 0d0a 2020  mage.shape):..  
+0001bb80: 2020 2020 2020 2020 2020 7570 6461 7465            update
+0001bb90: 5f6d 6173 6b20 3d20 6e70 2e7a 6572 6f73  _mask = np.zeros
+0001bba0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0001bbb0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+0001bbc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbe0: 2020 696d 6167 652e 7368 6170 655b 305d    image.shape[0]
+0001bbf0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc10: 2020 2069 6d61 6765 2e73 6861 7065 5b31     image.shape[1
+0001bc20: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc40: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001bc50: 325d 2c0d 0a20 2020 2020 2020 2020 2020  2],..           
+0001bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc70: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001bc80: 5b33 5d2c 0d0a 2020 2020 2020 2020 2020  [3],..          
+0001bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bca0: 2020 5d2c 2064 7479 7065 3d22 7569 6e74    ], dtype="uint
+0001bcb0: 3822 0d0a 2020 2020 2020 2020 2020 2020  8"..            
+0001bcc0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+0001bcd0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0001bce0: 2069 6e20 7261 6e67 6528 302c 2075 7064   in range(0, upd
+0001bcf0: 6174 655f 6d61 736b 2e73 6861 7065 5b30  ate_mask.shape[0
+0001bd00: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+0001bd10: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0001bd20: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
+0001bd30: 736b 2e73 6861 7065 5b31 5d29 3a0d 0a0d  sk.shape[1]):...
+0001bd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bd50: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
+0001bd60: 5b69 2c20 6a2c 203a 2c20 3a5d 203d 206d  [i, j, :, :] = m
+0001bd70: 6173 6b5b 692c 203a 2c20 3a5d 0d0a 2020  ask[i, :, :]..  
+0001bd80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+0001bd90: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+0001bda0: 6174 655f 6d61 736b 203d 206d 6173 6b0d  ate_mask = mask.
+0001bdb0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+0001bdc0: 6e20 7570 6461 7465 5f6d 6173 6b20 2020  n update_mask   
+0001bdd0: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
```

### Comparing `napatrackmater-3.9.5/napatrackmater/Trackvector.py` & `napatrackmater-3.9.6/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/__init__.py` & `napatrackmater-3.9.6/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/clustering.py` & `napatrackmater-3.9.6/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.9.6/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/fate_mapping.py` & `napatrackmater-3.9.6/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater/pretrained.py` & `napatrackmater-3.9.6/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.9.6/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.5
+Version: 3.9.6
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.5/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.9.6/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.5/setup.py` & `napatrackmater-3.9.6/setup.py`

 * *Files identical despite different names*

