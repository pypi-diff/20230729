# Comparing `tmp/napatrackmater-3.8.9.tar.gz` & `tmp/napatrackmater-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.8.9.tar", last modified: Sun Jul  9 21:11:55 2023, max compression
+gzip compressed data, was "napatrackmater-3.9.0.tar", last modified: Sat Jul 29 15:03:27 2023, max compression
```

## Comparing `napatrackmater-3.8.9.tar` & `napatrackmater-3.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:55.135350 napatrackmater-3.8.9/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.9/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:11:55.129768 napatrackmater-3.8.9/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.9/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:54.863864 napatrackmater-3.8.9/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.9/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.9/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   113282 2023-07-09 21:10:58.000000 napatrackmater-3.8.9/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.9/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.9/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-07-08 08:48:33.000000 napatrackmater-3.8.9/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.9/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.9/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.9/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-09 21:11:04.000000 napatrackmater-3.8.9/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:55.090648 napatrackmater-3.8.9/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-09 21:11:55.138307 napatrackmater-3.8.9/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.9/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.454446 napatrackmater-3.9.0/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:03:27.454108 napatrackmater-3.9.0/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.452114 napatrackmater-3.9.0/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   114228 2023-07-29 15:02:11.000000 napatrackmater-3.9.0/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 15:02:18.000000 napatrackmater-3.9.0/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:03:27.453537 napatrackmater-3.9.0/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 15:03:27.000000 napatrackmater-3.9.0/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 15:03:27.454534 napatrackmater-3.9.0/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.0/setup.py
```

### Comparing `napatrackmater-3.8.9/LICENSE` & `napatrackmater-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/PKG-INFO` & `napatrackmater-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.9
+Version: 3.9.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
-Author: Varun Kapoor, Mari Tolonen
+Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `napatrackmater-3.8.9/README.md` & `napatrackmater-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.9.0/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.9.0/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/Trackmate.py` & `napatrackmater-3.9.0/napatrackmater/Trackmate.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,6605 +477,6664 @@
 00001dc0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
 00001dd0: 735f 6b65 7973 5b22 7370 6565 6422 5d0d  s_keys["speed"].
 00001de0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
 00001df0: 7370 6c61 6365 6d65 6e74 5f6b 6579 203d  splacement_key =
 00001e00: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
 00001e10: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
 00001e20: 2264 6973 706c 6163 656d 656e 7422 5d0d  "displacement"].
-00001e30: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-00001e40: 6765 5f74 696d 655f 6b65 7920 3d20 7365  ge_time_key = se
-00001e50: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00001e60: 735f 6564 6765 735f 6b65 7973 5b22 6564  s_edges_keys["ed
-00001e70: 6765 5f74 696d 6522 5d0d 0a20 2020 2020  ge_time"]..     
-00001e80: 2020 2073 656c 662e 6564 6765 5f78 5f6c     self.edge_x_l
-00001e90: 6f63 6174 696f 6e5f 6b65 7920 3d20 7365  ocation_key = se
-00001ea0: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00001eb0: 735f 6564 6765 735f 6b65 7973 5b22 6564  s_edges_keys["ed
-00001ec0: 6765 5f78 5f6c 6f63 6174 696f 6e22 5d0d  ge_x_location"].
-00001ed0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-00001ee0: 6765 5f79 5f6c 6f63 6174 696f 6e5f 6b65  ge_y_location_ke
-00001ef0: 7920 3d20 7365 6c66 2e74 7261 636b 5f61  y = self.track_a
-00001f00: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
-00001f10: 7973 5b22 6564 6765 5f79 5f6c 6f63 6174  ys["edge_y_locat
-00001f20: 696f 6e22 5d0d 0a20 2020 2020 2020 2073  ion"]..        s
-00001f30: 656c 662e 6564 6765 5f7a 5f6c 6f63 6174  elf.edge_z_locat
-00001f40: 696f 6e5f 6b65 7920 3d20 7365 6c66 2e74  ion_key = self.t
-00001f50: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
-00001f60: 6765 735f 6b65 7973 5b22 6564 6765 5f7a  ges_keys["edge_z
-00001f70: 5f6c 6f63 6174 696f 6e22 5d0d 0a20 2020  _location"]..   
-00001f80: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00001f90: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00001fa0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-00001fb0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00001fc0: 6b5f 6d69 746f 7369 735f 6c61 6265 6c20  k_mitosis_label 
-00001fd0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
-00001fe0: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
-00001ff0: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
-00002000: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00002010: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-00002020: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
-00002030: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
-00002040: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
-00002050: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
-00002060: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
-00002070: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-00002080: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00002090: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-000020a0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-000020b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000020c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000020d0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-000020e0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000020f0: 745f 6365 6e74 726f 6964 203d 207b 7d0d  t_centroid = {}.
-00002100: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00002110: 6971 7565 5f74 7261 636b 5f63 656e 7472  ique_track_centr
-00002120: 6f69 6420 3d20 7b7d 0d0a 2020 2020 2020  oid = {}..      
-00002130: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
-00002140: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
-00002150: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
-00002160: 5f63 656c 6c5f 6964 7320 3d20 7b7d 0d0a  _cell_ids = {}..
-00002170: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00002180: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-00002190: 5f70 726f 7065 7274 6965 7320 3d20 7b7d  _properties = {}
-000021a0: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-000021b0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-000021c0: 7020 3d20 7b7d 0d0a 2020 2020 2020 2020  p = {}..        
-000021d0: 7365 6c66 2e65 6467 655f 736f 7572 6365  self.edge_source
-000021e0: 5f6c 6f6f 6b75 7020 3d20 7b7d 0d0a 2020  _lookup = {}..  
-000021f0: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-00002200: 6174 696f 6e5f 6469 6374 203d 207b 7d0d  ation_dict = {}.
-00002210: 0a20 2020 2020 2020 2073 656c 662e 7472  .        self.tr
-00002220: 6163 6b6c 6574 5f64 6963 7420 3d20 7b7d  acklet_dict = {}
-00002230: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-00002240: 7261 7068 5f73 706c 6974 203d 207b 7d0d  raph_split = {}.
-00002250: 0a20 2020 2020 2020 2073 656c 662e 6772  .        self.gr
-00002260: 6170 685f 7472 6163 6b73 203d 207b 7d0d  aph_tracks = {}.
-00002270: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00002280: 696d 6564 5f63 656e 7472 6f69 6420 3d20  imed_centroid = 
-00002290: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
-000022a0: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
-000022b0: 2020 2020 786d 6c5f 7061 7273 6572 203d      xml_parser =
-000022c0: 2065 742e 584d 4c50 6172 7365 7228 6875   et.XMLParser(hu
-000022d0: 6765 5f74 7265 653d 5472 7565 290d 0a20  ge_tree=True).. 
-000022e0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-000022f0: 6173 7465 725f 786d 6c5f 7061 7468 2069  aster_xml_path i
-00002300: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00002310: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-00002320: 7465 725f 786d 6c5f 7061 7468 203d 2050  ter_xml_path = P
-00002330: 6174 6828 272e 2729 0d0a 2020 2020 2020  ath('.')..      
-00002340: 2020 0d0a 2020 2020 2020 2020 6966 2073    ..        if s
-00002350: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-00002360: 6174 682e 6973 5f64 6972 2829 2061 6e64  ath.is_dir() and
-00002370: 2073 656c 662e 786d 6c5f 7061 7468 2069   self.xml_path i
-00002380: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00002390: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000023a0: 6e74 2827 5265 6164 696e 6720 584d 4c27  nt('Reading XML'
-000023b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000023c0: 2020 2073 656c 662e 786d 6c5f 636f 6e74     self.xml_cont
-000023d0: 656e 7420 3d20 6574 2e66 726f 6d73 7472  ent = et.fromstr
-000023e0: 696e 6728 6f70 656e 2873 656c 662e 786d  ing(open(self.xm
-000023f0: 6c5f 7061 7468 292e 7265 6164 2829 2e65  l_path).read().e
-00002400: 6e63 6f64 6528 292c 2078 6d6c 5f70 6172  ncode(), xml_par
-00002410: 7365 7229 0d0a 2020 2020 2020 2020 2020  ser)..          
-00002420: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002430: 2020 2020 2020 2020 7365 6c66 2e66 696c          self.fil
-00002440: 7465 7265 645f 7472 6163 6b5f 6964 7320  tered_track_ids 
-00002450: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2069 6e74 2874 7261 636b 2e67 6574 2873   int(track.get(s
-00002480: 656c 662e 7472 6163 6b69 645f 6b65 7929  elf.trackid_key)
-00002490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000024a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000024b0: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
-000024c0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-000024d0: 6428 224d 6f64 656c 2229 0d0a 2020 2020  d("Model")..    
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 2020 2020 2020 2e66 696e 6428 2246          .find("F
-00002500: 696c 7465 7265 6454 7261 636b 7322 290d  ilteredTracks").
-00002510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002520: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
-00002530: 6e64 616c 6c28 2254 7261 636b 4944 2229  ndall("TrackID")
-00002540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002550: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-00002560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002570: 662e 6d61 785f 7472 6163 6b5f 6964 203d  f.max_track_id =
-00002580: 206d 6178 2873 656c 662e 6669 6c74 6572   max(self.filter
-00002590: 6564 5f74 7261 636b 5f69 6473 2920 2020  ed_track_ids)   
-000025a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000025b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000025c0: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
-000025d0: 6574 5f78 6d6c 5f64 6174 6128 290d 0a20  et_xml_data().. 
-000025e0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-000025f0: 696e 7374 616e 6365 2873 656c 662e 6d61  instance(self.ma
-00002600: 7374 6572 5f78 6d6c 5f70 6174 682c 2073  ster_xml_path, s
-00002610: 7472 293a 2020 2020 2020 0d0a 2020 2020  tr):      ..    
-00002620: 2020 2020 2020 6966 2073 656c 662e 6d61        if self.ma
-00002630: 7374 6572 5f78 6d6c 5f70 6174 682e 6973  ster_xml_path.is
-00002640: 5f66 696c 6528 293a 0d0a 2020 2020 2020  _file():..      
-00002650: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00002660: 5265 6164 696e 6720 4d61 7374 6572 2058  Reading Master X
-00002670: 4d4c 2729 0d0a 2020 2020 2020 2020 2020  ML')..          
-00002680: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00002690: 2020 2020 2020 7365 6c66 2e78 6d6c 5f63        self.xml_c
-000026a0: 6f6e 7465 6e74 203d 2065 742e 6672 6f6d  ontent = et.from
-000026b0: 7374 7269 6e67 286f 7065 6e28 7365 6c66  string(open(self
-000026c0: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
-000026d0: 292e 7265 6164 2829 2e65 6e63 6f64 6528  ).read().encode(
-000026e0: 292c 2078 6d6c 5f70 6172 7365 7229 0d0a  ), xml_parser)..
-000026f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00002700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002710: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-00002720: 6163 6b5f 6964 7320 3d20 5b0d 0a20 2020  ack_ids = [..   
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 2020 2020 2069 6e74 2874 7261           int(tra
-00002750: 636b 2e67 6574 2873 656c 662e 7472 6163  ck.get(self.trac
-00002760: 6b69 645f 6b65 7929 290d 0a20 2020 2020  kid_key))..     
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
-00002790: 2069 6e20 7365 6c66 2e78 6d6c 5f63 6f6e   in self.xml_con
-000027a0: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
-000027b0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2e66 696e 6428 2246 696c 7465 7265 6454  .find("FilteredT
-000027e0: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
-000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 202e 6669 6e64 616c 6c28 2254       .findall("T
-00002810: 7261 636b 4944 2229 0d0a 2020 2020 2020  rackID")..      
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
-00002840: 2020 2020 7365 6c66 2e6d 6178 5f74 7261      self.max_tra
-00002850: 636b 5f69 6420 3d20 6d61 7828 7365 6c66  ck_id = max(self
-00002860: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-00002870: 6964 7329 2020 2020 2020 2020 0d0a 2020  ids)        ..  
-00002880: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00002890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000028a0: 656c 662e 5f67 6574 5f6d 6173 7465 725f  elf._get_master_
-000028b0: 786d 6c5f 6461 7461 2829 0d0a 2020 2020  xml_data()..    
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 2020 200d 0a0d 0a20 2020 2020 0d0a 0d0a     ....     ....
-000028e0: 0d0a 2020 2020 6465 6620 5f63 7265 6174  ..    def _creat
-000028f0: 655f 6368 616e 6e65 6c5f 7472 6565 2873  e_channel_tree(s
-00002900: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-00002910: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
-00002920: 6e6e 656c 5f73 6567 5f69 6d61 6765 203d  nnel_seg_image =
-00002930: 207b 7d0d 0a20 2020 2020 2020 2020 2073   {}..          s
-00002940: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-00002950: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00002960: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00002970: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
-00002980: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
-00002990: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
-000029a0: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
-000029b0: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
-000029c0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
-000029d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000029e0: 6920 696e 2072 616e 6765 2873 656c 662e  i in range(self.
-000029f0: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-00002a00: 652e 7368 6170 655b 305d 293a 0d0a 2020  e.shape[0]):..  
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
-00002a30: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
-00002a40: 626d 6974 2873 656c 662e 5f63 6861 6e6e  bmit(self._chann
-00002a50: 656c 5f63 6f6d 7075 7465 722c 2069 2929  el_computer, i))
-00002a60: 0d0a 2020 2020 2020 2020 2020 0d0a 2020  ..          ..  
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-00002a90: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-00002aa0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002af0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-00002b00: 6265 6c20 3d20 2244 6f69 6e67 2063 6861  bel = "Doing cha
-00002b10: 6e6e 656c 2063 6f6d 7075 7461 7469 6f6e  nnel computation
-00002b20: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00001e30: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00001e40: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
+00001e50: 6365 5f6b 6579 203d 2073 656c 662e 7472  ce_key = self.tr
+00001e60: 6163 6b5f 616e 616c 7973 6973 5f65 6467  ack_analysis_edg
+00001e70: 6573 5f6b 6579 735b 2274 6f74 616c 5f74  es_keys["total_t
+00001e80: 7261 636b 5f64 6973 7461 6e63 6522 5d0d  rack_distance"].
+00001e90: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+00001ea0: 785f 6469 7374 616e 6365 5f74 7261 7665  x_distance_trave
+00001eb0: 6c65 645f 6b65 7920 3d20 7365 6c66 2e74  led_key = self.t
+00001ec0: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00001ed0: 6765 735f 6b65 7973 5b22 6d61 785f 7472  ges_keys["max_tr
+00001ee0: 6163 6b5f 6469 7374 616e 6365 225d 0d0a  ack_distance"]..
+00001ef0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00001f00: 636b 5f64 7572 6174 696f 6e5f 6b65 7920  ck_duration_key 
+00001f10: 3d20 7365 6c66 2e74 7261 636b 5f61 6e61  = self.track_ana
+00001f20: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+00001f30: 5b22 7472 6163 6b5f 6475 7261 7469 6f6e  ["track_duration
+00001f40: 225d 0d0a 2020 2020 2020 2020 0d0a 2020  "]..        ..  
+00001f50: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
+00001f60: 7469 6d65 5f6b 6579 203d 2073 656c 662e  time_key = self.
+00001f70: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001f80: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
+00001f90: 7469 6d65 225d 0d0a 2020 2020 2020 2020  time"]..        
+00001fa0: 7365 6c66 2e65 6467 655f 785f 6c6f 6361  self.edge_x_loca
+00001fb0: 7469 6f6e 5f6b 6579 203d 2073 656c 662e  tion_key = self.
+00001fc0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+00001fd0: 6467 6573 5f6b 6579 735b 2265 6467 655f  dges_keys["edge_
+00001fe0: 785f 6c6f 6361 7469 6f6e 225d 0d0a 2020  x_location"]..  
+00001ff0: 2020 2020 2020 7365 6c66 2e65 6467 655f        self.edge_
+00002000: 795f 6c6f 6361 7469 6f6e 5f6b 6579 203d  y_location_key =
+00002010: 2073 656c 662e 7472 6163 6b5f 616e 616c   self.track_anal
+00002020: 7973 6973 5f65 6467 6573 5f6b 6579 735b  ysis_edges_keys[
+00002030: 2265 6467 655f 795f 6c6f 6361 7469 6f6e  "edge_y_location
+00002040: 225d 0d0a 2020 2020 2020 2020 7365 6c66  "]..        self
+00002050: 2e65 6467 655f 7a5f 6c6f 6361 7469 6f6e  .edge_z_location
+00002060: 5f6b 6579 203d 2073 656c 662e 7472 6163  _key = self.trac
+00002070: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+00002080: 5f6b 6579 735b 2265 6467 655f 7a5f 6c6f  _keys["edge_z_lo
+00002090: 6361 7469 6f6e 225d 0d0a 2020 2020 2020  cation"]..      
+000020a0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+000020b0: 2e75 6e69 7175 655f 7472 6163 6b73 203d  .unique_tracks =
+000020c0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+000020d0: 662e 756e 6971 7565 5f74 7261 636b 5f6d  f.unique_track_m
+000020e0: 6974 6f73 6973 5f6c 6162 656c 203d 207b  itosis_label = {
+000020f0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
+00002100: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
+00002110: 7065 7274 6965 7320 3d20 7b7d 0d0a 2020  perties = {}..  
+00002120: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00002130: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00002140: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002150: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00002160: 6572 5f70 726f 7065 7274 6965 7320 3d20  er_properties = 
+00002170: 7b7d 0d0a 2020 2020 2020 2020 7365 6c66  {}..        self
+00002180: 2e75 6e69 7175 655f 7368 6170 655f 7072  .unique_shape_pr
+00002190: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+000021a0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+000021b0: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+000021c0: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
+000021d0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000021e0: 7370 6f74 5f70 726f 7065 7274 6965 7320  spot_properties 
+000021f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 7365  = {}..        se
+00002200: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
+00002210: 656e 7472 6f69 6420 3d20 7b7d 0d0a 2020  entroid = {}..  
+00002220: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00002230: 655f 7472 6163 6b5f 6365 6e74 726f 6964  e_track_centroid
+00002240: 203d 207b 7d0d 0a20 2020 2020 2020 2073   = {}..        s
+00002250: 656c 662e 726f 6f74 5f73 706f 7473 203d  elf.root_spots =
+00002260: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+00002270: 662e 616c 6c5f 6375 7272 656e 745f 6365  f.all_current_ce
+00002280: 6c6c 5f69 6473 203d 207b 7d0d 0a20 2020  ll_ids = {}..   
+00002290: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+000022a0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+000022b0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
+000022c0: 2020 2020 2020 2073 656c 662e 6564 6765         self.edge
+000022d0: 5f74 6172 6765 745f 6c6f 6f6b 7570 203d  _target_lookup =
+000022e0: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
+000022f0: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
+00002300: 6f6b 7570 203d 207b 7d0d 0a20 2020 2020  okup = {}..     
+00002310: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00002320: 6f6e 5f64 6963 7420 3d20 7b7d 0d0a 2020  on_dict = {}..  
+00002330: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00002340: 6c65 745f 6469 6374 203d 207b 7d0d 0a20  let_dict = {}.. 
+00002350: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
+00002360: 685f 7370 6c69 7420 3d20 7b7d 0d0a 2020  h_split = {}..  
+00002370: 2020 2020 2020 7365 6c66 2e67 7261 7068        self.graph
+00002380: 5f74 7261 636b 7320 3d20 7b7d 0d0a 2020  _tracks = {}..  
+00002390: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
+000023a0: 645f 6365 6e74 726f 6964 203d 207b 7d0d  d_centroid = {}.
+000023b0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+000023c0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+000023d0: 2078 6d6c 5f70 6172 7365 7220 3d20 6574   xml_parser = et
+000023e0: 2e58 4d4c 5061 7273 6572 2868 7567 655f  .XMLParser(huge_
+000023f0: 7472 6565 3d54 7275 6529 0d0a 2020 2020  tree=True)..    
+00002400: 2020 2020 6966 2073 656c 662e 6d61 7374      if self.mast
+00002410: 6572 5f78 6d6c 5f70 6174 6820 6973 204e  er_xml_path is N
+00002420: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00002430: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+00002440: 5f78 6d6c 5f70 6174 6820 3d20 5061 7468  _xml_path = Path
+00002450: 2827 2e27 290d 0a20 2020 2020 2020 200d  ('.')..        .
+00002460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00002470: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
+00002480: 2e69 735f 6469 7228 2920 616e 6420 7365  .is_dir() and se
+00002490: 6c66 2e78 6d6c 5f70 6174 6820 6973 206e  lf.xml_path is n
+000024a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000024b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000024c0: 2752 6561 6469 6e67 2058 4d4c 2729 0d0a  'Reading XML')..
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+000024f0: 203d 2065 742e 6672 6f6d 7374 7269 6e67   = et.fromstring
+00002500: 286f 7065 6e28 7365 6c66 2e78 6d6c 5f70  (open(self.xml_p
+00002510: 6174 6829 2e72 6561 6428 292e 656e 636f  ath).read().enco
+00002520: 6465 2829 2c20 786d 6c5f 7061 7273 6572  de(), xml_parser
+00002530: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002540: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00002550: 2020 2020 2073 656c 662e 6669 6c74 6572       self.filter
+00002560: 6564 5f74 7261 636b 5f69 6473 203d 205b  ed_track_ids = [
+00002570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002580: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00002590: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+000025a0: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000025d0: 7472 6163 6b20 696e 2073 656c 662e 786d  track in self.xm
+000025e0: 6c5f 636f 6e74 656e 742e 6669 6e64 2822  l_content.find("
+000025f0: 4d6f 6465 6c22 290d 0a20 2020 2020 2020  Model")..       
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 202e 6669 6e64 2822 4669 6c74       .find("Filt
+00002620: 6572 6564 5472 6163 6b73 2229 0d0a 2020  eredTracks")..  
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 2020 2020 2e66 696e 6461            .finda
+00002650: 6c6c 2822 5472 6163 6b49 4422 290d 0a20  ll("TrackID").. 
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+00002680: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00002690: 6178 5f74 7261 636b 5f69 6420 3d20 6d61  ax_track_id = ma
+000026a0: 7828 7365 6c66 2e66 696c 7465 7265 645f  x(self.filtered_
+000026b0: 7472 6163 6b5f 6964 7329 2020 2020 2020  track_ids)      
+000026c0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000026d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000026e0: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
+000026f0: 786d 6c5f 6461 7461 2829 0d0a 2020 2020  xml_data()..    
+00002700: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00002710: 7461 6e63 6528 7365 6c66 2e6d 6173 7465  tance(self.maste
+00002720: 725f 786d 6c5f 7061 7468 2c20 7374 7229  r_xml_path, str)
+00002730: 3a20 2020 2020 200d 0a20 2020 2020 2020  :      ..       
+00002740: 2020 2069 6620 7365 6c66 2e6d 6173 7465     if self.maste
+00002750: 725f 786d 6c5f 7061 7468 2e69 735f 6669  r_xml_path.is_fi
+00002760: 6c65 2829 3a0d 0a20 2020 2020 2020 2020  le():..         
+00002770: 2020 2020 2020 7072 696e 7428 2752 6561        print('Rea
+00002780: 6469 6e67 204d 6173 7465 7220 584d 4c27  ding Master XML'
+00002790: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000027a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000027b0: 2020 2073 656c 662e 786d 6c5f 636f 6e74     self.xml_cont
+000027c0: 656e 7420 3d20 6574 2e66 726f 6d73 7472  ent = et.fromstr
+000027d0: 696e 6728 6f70 656e 2873 656c 662e 6d61  ing(open(self.ma
+000027e0: 7374 6572 5f78 6d6c 5f70 6174 6829 2e72  ster_xml_path).r
+000027f0: 6561 6428 292e 656e 636f 6465 2829 2c20  ead().encode(), 
+00002800: 786d 6c5f 7061 7273 6572 290d 0a20 2020  xml_parser)..   
+00002810: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00002820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002830: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+00002840: 5f69 6473 203d 205b 0d0a 2020 2020 2020  _ids = [..      
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 696e 7428 7472 6163 6b2e        int(track.
+00002870: 6765 7428 7365 6c66 2e74 7261 636b 6964  get(self.trackid
+00002880: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
+000028b0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+000028c0: 742e 6669 6e64 2822 4d6f 6465 6c22 290d  t.find("Model").
+000028d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000028e0: 2020 2020 2020 2020 2020 2020 202e 6669               .fi
+000028f0: 6e64 2822 4669 6c74 6572 6564 5472 6163  nd("FilteredTrac
+00002900: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2e66 696e 6461 6c6c 2822 5472 6163    .findall("Trac
+00002930: 6b49 4422 290d 0a20 2020 2020 2020 2020  kID")..         
+00002940: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00002950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002960: 2073 656c 662e 6d61 785f 7472 6163 6b5f   self.max_track_
+00002970: 6964 203d 206d 6178 2873 656c 662e 6669  id = max(self.fi
+00002980: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00002990: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
+000029a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000029b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000029c0: 2e5f 6765 745f 6d61 7374 6572 5f78 6d6c  ._get_master_xml
+000029d0: 5f64 6174 6128 290d 0a20 2020 2020 2020  _data()..       
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029f0: 0d0a 0d0a 2020 2020 200d 0a0d 0a0d 0a20  ....     ...... 
+00002a00: 2020 2064 6566 205f 6372 6561 7465 5f63     def _create_c
+00002a10: 6861 6e6e 656c 5f74 7265 6528 7365 6c66  hannel_tree(self
+00002a20: 293a 0d0a 2020 2020 2020 2020 2020 7365  ):..          se
+00002a30: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
+00002a40: 6c5f 7365 675f 696d 6167 6520 3d20 7b7d  l_seg_image = {}
+00002a50: 0d0a 2020 2020 2020 2020 2020 7365 6c66  ..          self
+00002a60: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+00002a70: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
+00002a80: 5b5d 0d0a 2020 2020 2020 2020 2020 7769  []..          wi
+00002a90: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
+00002aa0: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
+00002ab0: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
+00002ac0: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
+00002ad0: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
+00002ae0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00002af0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00002b00: 6e20 7261 6e67 6528 7365 6c66 2e63 6861  n range(self.cha
+00002b10: 6e6e 656c 5f73 6567 5f69 6d61 6765 2e73  nnel_seg_image.s
+00002b20: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
 00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00002b50: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-00002b60: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
-00002bc0: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
+00002b40: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+00002b50: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+00002b60: 7428 7365 6c66 2e5f 6368 616e 6e65 6c5f  t(self._channel_
+00002b70: 636f 6d70 7574 6572 2c20 6929 290d 0a20  computer, i)).. 
+00002b80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002ba0: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+00002bb0: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+00002bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002be0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+00002be0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00002c20: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
-00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c40: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
-00002c50: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-00002c60: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-00002c70: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00002ca0: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-00002cb0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+00002c00: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00002c10: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+00002c20: 203d 2022 446f 696e 6720 6368 616e 6e65   = "Doing channe
+00002c30: 6c20 636f 6d70 7574 6174 696f 6e22 0d0a  l computation"..
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00002c70: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
+00002c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00002ce0: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-00002cf0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cd0: 2020 2020 206c 656e 2866 7574 7572 6573       len(futures
+00002ce0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
 00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00002d30: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
-00002d40: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002d70: 2e72 6573 756c 7428 290d 0a0d 0a20 0d0a  .result().... ..
-00002d80: 0d0a 2020 2020 6465 6620 5f63 6861 6e6e  ..    def _chann
-00002d90: 656c 5f63 6f6d 7075 7465 7228 7365 6c66  el_computer(self
-00002da0: 2c20 6929 3a0d 0a20 2020 2020 2020 2020  , i):..         
-00002db0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002dc0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00002dd0: 2e69 6d61 6765 2069 7320 6e6f 7420 4e6f  .image is not No
-00002de0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00002df0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
-00002e00: 656e 7369 7479 5f69 6d61 6765 203d 2073  ensity_image = s
-00002e10: 656c 662e 696d 6167 650d 0a20 2020 2020  elf.image..     
-00002e20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00002e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e40: 2020 2020 2020 2020 2020 696e 7465 6e73            intens
-00002e50: 6974 795f 696d 6167 6520 3d20 7365 6c66  ity_image = self
-00002e60: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
-00002e70: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-00002e80: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00002e90: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
-00002ea0: 203d 2072 6567 696f 6e70 726f 7073 2873   = regionprops(s
-00002eb0: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-00002ec0: 696d 6167 655b 692c 3a5d 2c20 696e 7465  image[i,:], inte
-00002ed0: 6e73 6974 795f 696d 6167 655b 692c 3a5d  nsity_image[i,:]
-00002ee0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002ef0: 2020 2063 656e 7472 6f69 6473 203d 205b     centroids = [
-00002f00: 7072 6f70 2e63 656e 7472 6f69 6420 666f  prop.centroid fo
-00002f10: 7220 7072 6f70 2069 6e20 7072 6f70 6572  r prop in proper
-00002f20: 7469 6573 5d0d 0a20 2020 2020 2020 2020  ties]..         
-00002f30: 2020 2020 2020 206c 6162 656c 7320 3d20         labels = 
-00002f40: 5b70 726f 702e 6c61 6265 6c20 666f 7220  [prop.label for 
-00002f50: 7072 6f70 2069 6e20 7072 6f70 6572 7469  prop in properti
-00002f60: 6573 5d0d 0a20 2020 2020 2020 2020 2020  es]..           
-00002f70: 2020 2020 2076 6f6c 756d 6520 3d20 5b70       volume = [p
-00002f80: 726f 702e 6172 6561 2066 6f72 2070 726f  rop.area for pro
-00002f90: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
-00002fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002fb0: 2020 696e 7465 6e73 6974 795f 6d65 616e    intensity_mean
-00002fc0: 203d 205b 7072 6f70 2e69 6e74 656e 7369   = [prop.intensi
-00002fd0: 7479 5f6d 6561 6e20 666f 7220 7072 6f70  ty_mean for prop
-00002fe0: 2069 6e20 7072 6f70 6572 7469 6573 5d0d   in properties].
-00002ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003000: 2069 6e74 656e 7369 7479 5f74 6f74 616c   intensity_total
-00003010: 203d 205b 7072 6f70 2e69 6e74 656e 7369   = [prop.intensi
-00003020: 7479 5f6d 6561 6e20 2a20 7072 6f70 2e61  ty_mean * prop.a
-00003030: 7265 6120 666f 7220 7072 6f70 2069 6e20  rea for prop in 
-00003040: 7072 6f70 6572 7469 6573 5d0d 0a20 2020  properties]..   
-00003050: 2020 2020 2020 2020 2020 2020 2062 6f75               bou
-00003060: 6e64 696e 675f 626f 7865 7320 3d20 5b70  nding_boxes = [p
-00003070: 726f 702e 6262 6f78 2066 6f72 2070 726f  rop.bbox for pro
-00003080: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
-00003090: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000030a0: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
-000030b0: 616c 2e63 4b44 5472 6565 2863 656e 7472  al.cKDTree(centr
-000030c0: 6f69 6473 290d 0a0d 0a20 2020 2020 2020  oids)....       
-000030d0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-000030e0: 696d 6564 5f63 6861 6e6e 656c 5f73 6567  imed_channel_seg
-000030f0: 5f69 6d61 6765 5b73 7472 2869 295d 203d  _image[str(i)] =
-00003100: 2020 7472 6565 2c20 6365 6e74 726f 6964    tree, centroid
-00003110: 732c 206c 6162 656c 732c 2076 6f6c 756d  s, labels, volum
-00003120: 652c 2069 6e74 656e 7369 7479 5f6d 6561  e, intensity_mea
-00003130: 6e2c 2069 6e74 656e 7369 7479 5f74 6f74  n, intensity_tot
-00003140: 616c 2c20 626f 756e 6469 6e67 5f62 6f78  al, bounding_box
-00003150: 6573 0d0a 2020 2020 2020 2020 2020 0d0a  es..          ..
-00003160: 0d0a 2020 2020 6465 6620 5f67 6574 5f61  ..    def _get_a
-00003170: 7474 7269 6275 7465 7328 7365 6c66 293a  ttributes(self):
-00003180: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00003190: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000031a0: 662e 4174 7472 6962 7574 6569 6473 2c20  f.Attributeids, 
-000031b0: 7365 6c66 2e41 6c6c 5661 6c75 6573 203d  self.AllValues =
-000031c0: 2020 6765 745f 7370 6f74 5f64 6174 6173    get_spot_datas
-000031d0: 6574 2873 656c 662e 7370 6f74 5f64 6174  et(self.spot_dat
-000031e0: 6173 6574 2c20 7365 6c66 2e74 7261 636b  aset, self.track
-000031f0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00003200: 6579 732c 2073 656c 662e 7863 616c 6962  eys, self.xcalib
-00003210: 7261 7469 6f6e 2c20 7365 6c66 2e79 6361  ration, self.yca
-00003220: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
-00003230: 7a63 616c 6962 7261 7469 6f6e 2c20 7365  zcalibration, se
-00003240: 6c66 2e41 7474 7269 6275 7465 426f 786e  lf.AttributeBoxn
-00003250: 616d 652c 2073 656c 662e 6465 7465 6374  ame, self.detect
-00003260: 6f72 6368 616e 6e65 6c29 0d0a 2020 2020  orchannel)..    
-00003270: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00003280: 6f62 7469 616e 6564 2073 706f 7420 6174  obtianed spot at
-00003290: 7472 6962 7574 6573 2729 0d0a 2020 2020  tributes')..    
-000032a0: 2020 2020 2020 2020 2073 656c 662e 5472           self.Tr
-000032b0: 6163 6b41 7474 7269 6275 7465 6964 732c  ackAttributeids,
-000032c0: 2073 656c 662e 416c 6c54 7261 636b 5661   self.AllTrackVa
-000032d0: 6c75 6573 203d 2067 6574 5f74 7261 636b  lues = get_track
-000032e0: 5f64 6174 6173 6574 2873 656c 662e 7472  _dataset(self.tr
-000032f0: 6163 6b5f 6461 7461 7365 742c 2020 7365  ack_dataset,  se
-00003300: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00003310: 735f 7370 6f74 5f6b 6579 732c 2073 656c  s_spot_keys, sel
-00003320: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00003330: 5f74 7261 636b 5f6b 6579 732c 2073 656c  _track_keys, sel
-00003340: 662e 5472 6163 6b41 7474 7269 6275 7465  f.TrackAttribute
-00003350: 426f 786e 616d 6529 0d0a 2020 2020 2020  Boxname)..      
-00003360: 2020 2020 2020 2070 7269 6e74 2827 6f62         print('ob
-00003370: 7461 696e 6564 2074 7261 636b 2061 7474  tained track att
-00003380: 7269 6275 7465 7327 290d 0a20 2020 2020  ributes')..     
-00003390: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-000033a0: 4564 6765 7356 616c 7565 7320 3d20 6765  EdgesValues = ge
-000033b0: 745f 6564 6765 735f 6461 7461 7365 7428  t_edges_dataset(
-000033c0: 7365 6c66 2e65 6467 6573 5f64 6174 6173  self.edges_datas
-000033d0: 6574 2c20 7365 6c66 2e65 6467 6573 5f64  et, self.edges_d
-000033e0: 6174 6173 6574 5f69 6e64 6578 2c20 7365  ataset_index, se
-000033f0: 6c66 2e74 7261 636b 5f61 6e61 6c79 7369  lf.track_analysi
-00003400: 735f 7370 6f74 5f6b 6579 732c 2073 656c  s_spot_keys, sel
-00003410: 662e 7472 6163 6b5f 616e 616c 7973 6973  f.track_analysis
-00003420: 5f65 6467 6573 5f6b 6579 7329 0d0a 2020  _edges_keys)..  
-00003430: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00003440: 2827 6f62 7461 696e 6564 2065 6467 6520  ('obtained edge 
-00003450: 6174 7472 6962 7574 6573 2729 0d0a 0d0a  attributes')....
-00003460: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00003470: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003480: 6465 6620 5f67 6574 5f62 6f75 6e64 6172  def _get_boundar
-00003490: 795f 706f 696e 7473 2873 656c 6629 3a0d  y_points(self):.
-000034a0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-000034b0: 2020 2020 7072 696e 7428 2743 6f6d 7075      print('Compu
-000034c0: 7469 6e67 2062 6f75 6e64 6172 7920 706f  ting boundary po
-000034d0: 696e 7473 2729 200d 0a20 2020 2020 2020  ints') ..       
-000034e0: 2069 6620 2073 656c 662e 6d61 736b 2069   if  self.mask i
-000034f0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20  s not None:.... 
-00003500: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00003510: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-00003520: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-00003530: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003540: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003550: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003560: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
-00003570: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
-00003580: 5f6d 6173 6b28 7365 6c66 2e6d 6173 6b2c  _mask(self.mask,
-00003590: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-000035a0: 675f 696d 6167 6529 0d0a 0d0a 2020 2020  g_image)....    
-000035b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000035c0: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-000035d0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000035e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003600: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
-00003610: 655f 6d61 736b 203d 2063 6865 636b 5f61  e_mask = check_a
-00003620: 6e64 5f75 7064 6174 655f 6d61 736b 2873  nd_update_mask(s
-00003630: 656c 662e 6d61 736b 2c20 7365 6c66 2e73  elf.mask, self.s
-00003640: 6567 5f69 6d61 6765 290d 0a20 2020 2020  eg_image)..     
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002d30: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00002d40: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002d60: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
+00002d70: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
+00002d80: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
+00002d90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+00002dc0: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+00002dd0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002df0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002e00: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00002e10: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00002e50: 6172 2e76 616c 7565 203d 2020 7365 6c66  ar.value =  self
+00002e60: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e80: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
+00002e90: 7375 6c74 2829 0d0a 0d0a 200d 0a0d 0a20  sult().... .... 
+00002ea0: 2020 2064 6566 205f 6368 616e 6e65 6c5f     def _channel_
+00002eb0: 636f 6d70 7574 6572 2873 656c 662c 2069  computer(self, i
+00002ec0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00002ed0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00002ee0: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
+00002ef0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+00002f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002f10: 2020 2020 2020 2020 2020 696e 7465 6e73            intens
+00002f20: 6974 795f 696d 6167 6520 3d20 7365 6c66  ity_image = self
+00002f30: 2e69 6d61 6765 0d0a 2020 2020 2020 2020  .image..        
+00002f40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f60: 2020 2020 2020 2069 6e74 656e 7369 7479         intensity
+00002f70: 5f69 6d61 6765 203d 2073 656c 662e 6368  _image = self.ch
+00002f80: 616e 6e65 6c5f 7365 675f 696d 6167 650d  annel_seg_image.
+00002f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002fa0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00002fb0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
+00002fc0: 7265 6769 6f6e 7072 6f70 7328 7365 6c66  regionprops(self
+00002fd0: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+00002fe0: 6765 5b69 2c3a 5d2c 2069 6e74 656e 7369  ge[i,:], intensi
+00002ff0: 7479 5f69 6d61 6765 5b69 2c3a 5d29 0d0a  ty_image[i,:])..
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 6365 6e74 726f 6964 7320 3d20 5b70 726f  centroids = [pro
+00003020: 702e 6365 6e74 726f 6964 2066 6f72 2070  p.centroid for p
+00003030: 726f 7020 696e 2070 726f 7065 7274 6965  rop in propertie
+00003040: 735d 0d0a 2020 2020 2020 2020 2020 2020  s]..            
+00003050: 2020 2020 6c61 6265 6c73 203d 205b 7072      labels = [pr
+00003060: 6f70 2e6c 6162 656c 2066 6f72 2070 726f  op.label for pro
+00003070: 7020 696e 2070 726f 7065 7274 6965 735d  p in properties]
+00003080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003090: 2020 766f 6c75 6d65 203d 205b 7072 6f70    volume = [prop
+000030a0: 2e61 7265 6120 666f 7220 7072 6f70 2069  .area for prop i
+000030b0: 6e20 7072 6f70 6572 7469 6573 5d0d 0a20  n properties].. 
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000030d0: 6e74 656e 7369 7479 5f6d 6561 6e20 3d20  ntensity_mean = 
+000030e0: 5b70 726f 702e 696e 7465 6e73 6974 795f  [prop.intensity_
+000030f0: 6d65 616e 2066 6f72 2070 726f 7020 696e  mean for prop in
+00003100: 2070 726f 7065 7274 6965 735d 0d0a 2020   properties]..  
+00003110: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003120: 7465 6e73 6974 795f 746f 7461 6c20 3d20  tensity_total = 
+00003130: 5b70 726f 702e 696e 7465 6e73 6974 795f  [prop.intensity_
+00003140: 6d65 616e 202a 2070 726f 702e 6172 6561  mean * prop.area
+00003150: 2066 6f72 2070 726f 7020 696e 2070 726f   for prop in pro
+00003160: 7065 7274 6965 735d 0d0a 2020 2020 2020  perties]..      
+00003170: 2020 2020 2020 2020 2020 626f 756e 6469            boundi
+00003180: 6e67 5f62 6f78 6573 203d 205b 7072 6f70  ng_boxes = [prop
+00003190: 2e62 626f 7820 666f 7220 7072 6f70 2069  .bbox for prop i
+000031a0: 6e20 7072 6f70 6572 7469 6573 5d0d 0a0d  n properties]...
+000031b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000031c0: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
+000031d0: 634b 4454 7265 6528 6365 6e74 726f 6964  cKDTree(centroid
+000031e0: 7329 0d0a 0d0a 2020 2020 2020 2020 2020  s)....          
+000031f0: 2020 2020 2020 7365 6c66 2e5f 7469 6d65        self._time
+00003200: 645f 6368 616e 6e65 6c5f 7365 675f 696d  d_channel_seg_im
+00003210: 6167 655b 7374 7228 6929 5d20 3d20 2074  age[str(i)] =  t
+00003220: 7265 652c 2063 656e 7472 6f69 6473 2c20  ree, centroids, 
+00003230: 6c61 6265 6c73 2c20 766f 6c75 6d65 2c20  labels, volume, 
+00003240: 696e 7465 6e73 6974 795f 6d65 616e 2c20  intensity_mean, 
+00003250: 696e 7465 6e73 6974 795f 746f 7461 6c2c  intensity_total,
+00003260: 2062 6f75 6e64 696e 675f 626f 7865 730d   bounding_boxes.
+00003270: 0a20 2020 2020 2020 2020 200d 0a0d 0a20  .          .... 
+00003280: 2020 2064 6566 205f 6765 745f 6174 7472     def _get_attr
+00003290: 6962 7574 6573 2873 656c 6629 3a0d 0a20  ibutes(self):.. 
+000032a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000032b0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+000032c0: 7474 7269 6275 7465 6964 732c 2073 656c  ttributeids, sel
+000032d0: 662e 416c 6c56 616c 7565 7320 3d20 2067  f.AllValues =  g
+000032e0: 6574 5f73 706f 745f 6461 7461 7365 7428  et_spot_dataset(
+000032f0: 7365 6c66 2e73 706f 745f 6461 7461 7365  self.spot_datase
+00003300: 742c 2073 656c 662e 7472 6163 6b5f 616e  t, self.track_an
+00003310: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+00003320: 2c20 7365 6c66 2e78 6361 6c69 6272 6174  , self.xcalibrat
+00003330: 696f 6e2c 2073 656c 662e 7963 616c 6962  ion, self.ycalib
+00003340: 7261 7469 6f6e 2c20 7365 6c66 2e7a 6361  ration, self.zca
+00003350: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
+00003360: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+00003370: 2c20 7365 6c66 2e64 6574 6563 746f 7263  , self.detectorc
+00003380: 6861 6e6e 656c 290d 0a20 2020 2020 2020  hannel)..       
+00003390: 2020 2020 2020 7072 696e 7428 276f 6274        print('obt
+000033a0: 6961 6e65 6420 7370 6f74 2061 7474 7269  ianed spot attri
+000033b0: 6275 7465 7327 290d 0a20 2020 2020 2020  butes')..       
+000033c0: 2020 2020 2020 7365 6c66 2e54 7261 636b        self.Track
+000033d0: 4174 7472 6962 7574 6569 6473 2c20 7365  Attributeids, se
+000033e0: 6c66 2e41 6c6c 5472 6163 6b56 616c 7565  lf.AllTrackValue
+000033f0: 7320 3d20 6765 745f 7472 6163 6b5f 6461  s = get_track_da
+00003400: 7461 7365 7428 7365 6c66 2e74 7261 636b  taset(self.track
+00003410: 5f64 6174 6173 6574 2c20 2073 656c 662e  _dataset,  self.
+00003420: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00003430: 706f 745f 6b65 7973 2c20 7365 6c66 2e74  pot_keys, self.t
+00003440: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
+00003450: 6163 6b5f 6b65 7973 2c20 7365 6c66 2e54  ack_keys, self.T
+00003460: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
+00003470: 6e61 6d65 290d 0a20 2020 2020 2020 2020  name)..         
+00003480: 2020 2020 7072 696e 7428 276f 6274 6169      print('obtai
+00003490: 6e65 6420 7472 6163 6b20 6174 7472 6962  ned track attrib
+000034a0: 7574 6573 2729 0d0a 2020 2020 2020 2020  utes')..        
+000034b0: 2020 2020 2073 656c 662e 416c 6c45 6467       self.AllEdg
+000034c0: 6573 5661 6c75 6573 203d 2067 6574 5f65  esValues = get_e
+000034d0: 6467 6573 5f64 6174 6173 6574 2873 656c  dges_dataset(sel
+000034e0: 662e 6564 6765 735f 6461 7461 7365 742c  f.edges_dataset,
+000034f0: 2073 656c 662e 6564 6765 735f 6461 7461   self.edges_data
+00003500: 7365 745f 696e 6465 782c 2073 656c 662e  set_index, self.
+00003510: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+00003520: 706f 745f 6b65 7973 2c20 7365 6c66 2e74  pot_keys, self.t
+00003530: 7261 636b 5f61 6e61 6c79 7369 735f 6564  rack_analysis_ed
+00003540: 6765 735f 6b65 7973 290d 0a20 2020 2020  ges_keys)..     
+00003550: 2020 2020 2020 2020 7072 696e 7428 276f          print('o
+00003560: 6274 6169 6e65 6420 6564 6765 2061 7474  btained edge att
+00003570: 7269 6275 7465 7327 290d 0a0d 0a20 2020  ributes')....   
+00003580: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003590: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+000035a0: 205f 6765 745f 626f 756e 6461 7279 5f70   _get_boundary_p
+000035b0: 6f69 6e74 7328 7365 6c66 293a 0d0a 2020  oints(self):..  
+000035c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000035d0: 2070 7269 6e74 2827 436f 6d70 7574 696e   print('Computin
+000035e0: 6720 626f 756e 6461 7279 2070 6f69 6e74  g boundary point
+000035f0: 7327 2920 0d0a 2020 2020 2020 2020 6966  s') ..        if
+00003600: 2020 7365 6c66 2e6d 6173 6b20 6973 206e    self.mask is n
+00003610: 6f74 204e 6f6e 653a 0d0a 0d0a 2020 2020  ot None:....    
+00003620: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003630: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00003640: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
 00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
-00003670: 6620 7365 6c66 2e73 6567 5f69 6d61 6765  f self.seg_image
-00003680: 2069 7320 4e6f 6e65 2061 6e64 2073 656c   is None and sel
-00003690: 662e 696d 6167 6520 6973 206e 6f74 204e  f.image is not N
-000036a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000036b0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 2020 2020 2020 7365 6c66 2e75 7064          self.upd
-000036e0: 6174 655f 6d61 736b 203d 2063 6865 636b  ate_mask = check
-000036f0: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
-00003700: 2873 656c 662e 6d61 736b 2c20 7365 6c66  (self.mask, self
-00003710: 2e69 6d61 6765 2920 2020 200d 0a20 2020  .image)    ..   
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003740: 2020 2020 2020 7365 6c66 2e6d 6173 6b20        self.mask 
-00003750: 3d20 7365 6c66 2e75 7064 6174 655f 6d61  = self.update_ma
-00003760: 736b 0d0a 2020 2020 2020 2020 2020 2020  sk..            
-00003770: 7365 6c66 2e74 696d 6564 5f6d 6173 6b2c  self.timed_mask,
-00003780: 2073 656c 662e 626f 756e 6461 7279 203d   self.boundary =
-00003790: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
-000037a0: 2873 656c 662e 6d61 736b 2c20 7365 6c66  (self.mask, self
-000037b0: 2e78 6361 6c69 6272 6174 696f 6e2c 2073  .xcalibration, s
-000037c0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-000037d0: 2c20 7365 6c66 2e7a 6361 6c69 6272 6174  , self.zcalibrat
-000037e0: 696f 6e29 0d0a 2020 2020 2020 2020 656c  ion)..        el
-000037f0: 6966 2073 656c 662e 6d61 736b 2069 7320  if self.mask is 
-00003800: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00003810: 2020 2069 6620 7365 6c66 2e73 6567 5f69     if self.seg_i
-00003820: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-00003830: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003840: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003850: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003860: 662e 7570 6461 7465 5f6d 6173 6b20 3d20  f.update_mask = 
-00003870: 6e70 2e7a 6572 6f73 2873 656c 662e 7365  np.zeros(self.se
-00003880: 675f 696d 6167 652e 7368 6170 652c 2064  g_image.shape, d
-00003890: 7479 7065 3d6e 702e 7569 6e74 3829 0d0a  type=np.uint8)..
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000038c0: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-000038d0: 675f 696d 6167 6520 6973 204e 6f6e 6520  g_image is None 
-000038e0: 616e 6420 7365 6c66 2e69 6d61 6765 2069  and self.image i
-000038f0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a0d 0a20  s not None:.... 
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
-00003920: 6173 6b20 3d20 6e70 2e7a 6572 6f73 2873  ask = np.zeros(s
-00003930: 656c 662e 696d 6167 652e 7368 6170 652c  elf.image.shape,
-00003940: 2064 7479 7065 3d6e 702e 7569 6e74 3829   dtype=np.uint8)
-00003950: 200d 0a20 2020 2020 2020 2020 2020 2065   ..            e
-00003960: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00003660: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00003670: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00003680: 7064 6174 655f 6d61 736b 203d 2063 6865  pdate_mask = che
+00003690: 636b 5f61 6e64 5f75 7064 6174 655f 6d61  ck_and_update_ma
+000036a0: 736b 2873 656c 662e 6d61 736b 2c20 7365  sk(self.mask, se
+000036b0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+000036c0: 6d61 6765 290d 0a0d 0a20 2020 2020 2020  mage)....       
+000036d0: 2020 2020 2069 6620 7365 6c66 2e73 6567       if self.seg
+000036e0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+000036f0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00003700: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 2020 2073 656c 662e 7570 6461 7465 5f6d     self.update_m
+00003730: 6173 6b20 3d20 6368 6563 6b5f 616e 645f  ask = check_and_
+00003740: 7570 6461 7465 5f6d 6173 6b28 7365 6c66  update_mask(self
+00003750: 2e6d 6173 6b2c 2073 656c 662e 7365 675f  .mask, self.seg_
+00003760: 696d 6167 6529 0d0a 2020 2020 2020 2020  image)..        
+00003770: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00003780: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00003790: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
+000037a0: 204e 6f6e 6520 616e 6420 7365 6c66 2e69   None and self.i
+000037b0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+000037c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000037d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
+00003800: 5f6d 6173 6b20 3d20 6368 6563 6b5f 616e  _mask = check_an
+00003810: 645f 7570 6461 7465 5f6d 6173 6b28 7365  d_update_mask(se
+00003820: 6c66 2e6d 6173 6b2c 2073 656c 662e 696d  lf.mask, self.im
+00003830: 6167 6529 2020 2020 0d0a 2020 2020 2020  age)    ..      
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00003860: 2020 2073 656c 662e 6d61 736b 203d 2073     self.mask = s
+00003870: 656c 662e 7570 6461 7465 5f6d 6173 6b0d  elf.update_mask.
+00003880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003890: 662e 7469 6d65 645f 6d61 736b 2c20 7365  f.timed_mask, se
+000038a0: 6c66 2e62 6f75 6e64 6172 7920 3d20 626f  lf.boundary = bo
+000038b0: 756e 6461 7279 5f70 6f69 6e74 7328 7365  undary_points(se
+000038c0: 6c66 2e6d 6173 6b2c 2073 656c 662e 7863  lf.mask, self.xc
+000038d0: 616c 6962 7261 7469 6f6e 2c20 7365 6c66  alibration, self
+000038e0: 2e79 6361 6c69 6272 6174 696f 6e2c 2073  .ycalibration, s
+000038f0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00003900: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+00003910: 7365 6c66 2e6d 6173 6b20 6973 204e 6f6e  self.mask is Non
+00003920: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003930: 6966 2073 656c 662e 7365 675f 696d 6167  if self.seg_imag
+00003940: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003960: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00003970: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
 00003980: 7064 6174 655f 6d61 736b 203d 206e 702e  pdate_mask = np.
-00003990: 7a65 726f 7328 7365 6c66 2e69 6d61 6765  zeros(self.image
-000039a0: 7369 7a65 2c20 6474 7970 653d 6e70 2e75  size, dtype=np.u
-000039b0: 696e 7438 2920 2020 2020 2020 0d0a 2020  int8)       ..  
+00003990: 7a65 726f 7328 7365 6c66 2e73 6567 5f69  zeros(self.seg_i
+000039a0: 6d61 6765 2e73 6861 7065 2c20 6474 7970  mage.shape, dtyp
+000039b0: 653d 6e70 2e75 696e 7438 290d 0a20 2020  e=np.uint8)..   
 000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000039e0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-000039f0: 6b20 3d20 7365 6c66 2e75 7064 6174 655f  k = self.update_
-00003a00: 6d61 736b 0d0a 2020 2020 2020 2020 2020  mask..          
-00003a10: 2020 7365 6c66 2e6d 6173 6b5b 3a2c 3a2c    self.mask[:,:,
-00003a20: 313a 2d31 2c31 3a2d 315d 203d 2031 0d0a  1:-1,1:-1] = 1..
-00003a30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003a40: 2e74 696d 6564 5f6d 6173 6b2c 2073 656c  .timed_mask, sel
-00003a50: 662e 626f 756e 6461 7279 203d 2062 6f75  f.boundary = bou
-00003a60: 6e64 6172 795f 706f 696e 7473 2873 656c  ndary_points(sel
-00003a70: 662e 6d61 736b 2c20 7365 6c66 2e78 6361  f.mask, self.xca
-00003a80: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
-00003a90: 7963 616c 6962 7261 7469 6f6e 2c20 7365  ycalibration, se
-00003aa0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e29  lf.zcalibration)
-00003ab0: 0d0a 0d0a 2020 2020 2020 2020 2020 0d0a  ....          ..
-00003ac0: 0d0a 0d0a 2020 2020 6465 6620 5f67 656e  ....    def _gen
-00003ad0: 6572 6174 655f 6765 6e65 7261 7469 6f6e  erate_generation
-00003ae0: 7328 7365 6c66 2c20 7472 6163 6b29 3a0d  s(self, track):.
-00003af0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
-00003b00: 2020 2020 616c 6c5f 736f 7572 6365 5f69      all_source_i
-00003b10: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-00003b20: 2061 6c6c 5f74 6172 6765 745f 6964 7320   all_target_ids 
-00003b30: 3d20 5b5d 200d 0a0d 0a0d 0a20 2020 2020  = [] ......     
-00003b40: 2020 2066 6f72 2065 6467 6520 696e 2074     for edge in t
-00003b50: 7261 636b 2e66 696e 6461 6c6c 2827 4564  rack.findall('Ed
-00003b60: 6765 2729 3a0d 0a0d 0a20 2020 2020 2020  ge'):....       
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2073 6f75 7263 655f 6964 203d       source_id =
-00003b90: 2069 6e74 2865 6467 652e 6765 7428 7365   int(edge.get(se
-00003ba0: 6c66 2e73 706f 745f 736f 7572 6365 5f69  lf.spot_source_i
-00003bb0: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 2020 2020 2074 6172 6765 745f 6964 203d       target_id =
-00003be0: 2069 6e74 2865 6467 652e 6765 7428 7365   int(edge.get(se
-00003bf0: 6c66 2e73 706f 745f 7461 7267 6574 5f69  lf.spot_target_i
-00003c00: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 2020 2061 6c6c 5f73 6f75 7263 655f       all_source_
-00003c30: 6964 732e 6170 7065 6e64 2873 6f75 7263  ids.append(sourc
-00003c40: 655f 6964 290d 0a20 2020 2020 2020 2020  e_id)..         
-00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c60: 2020 2061 6c6c 5f74 6172 6765 745f 6964     all_target_id
-00003c70: 732e 6170 7065 6e64 2874 6172 6765 745f  s.append(target_
-00003c80: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+000039d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000039e0: 2020 2069 6620 7365 6c66 2e73 6567 5f69     if self.seg_i
+000039f0: 6d61 6765 2069 7320 4e6f 6e65 2061 6e64  mage is None and
+00003a00: 2073 656c 662e 696d 6167 6520 6973 206e   self.image is n
+00003a10: 6f74 204e 6f6e 653a 0d0a 0d0a 2020 2020  ot None:....    
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a30: 7365 6c66 2e75 7064 6174 655f 6d61 736b  self.update_mask
+00003a40: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
+00003a50: 2e69 6d61 6765 2e73 6861 7065 2c20 6474  .image.shape, dt
+00003a60: 7970 653d 6e70 2e75 696e 7438 2920 0d0a  ype=np.uint8) ..
+00003a70: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00003a80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003a90: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00003aa0: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
+00003ab0: 6f73 2873 656c 662e 696d 6167 6573 697a  os(self.imagesiz
+00003ac0: 652c 2064 7479 7065 3d6e 702e 7569 6e74  e, dtype=np.uint
+00003ad0: 3829 2020 2020 2020 200d 0a20 2020 2020  8)       ..     
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003b00: 2020 2020 2073 656c 662e 6d61 736b 203d       self.mask =
+00003b10: 2073 656c 662e 7570 6461 7465 5f6d 6173   self.update_mas
+00003b20: 6b0d 0a20 2020 2020 2020 2020 2020 2073  k..            s
+00003b30: 656c 662e 6d61 736b 5b3a 2c3a 2c31 3a2d  elf.mask[:,:,1:-
+00003b40: 312c 313a 2d31 5d20 3d20 310d 0a20 2020  1,1:-1] = 1..   
+00003b50: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
+00003b60: 6d65 645f 6d61 736b 2c20 7365 6c66 2e62  med_mask, self.b
+00003b70: 6f75 6e64 6172 7920 3d20 626f 756e 6461  oundary = bounda
+00003b80: 7279 5f70 6f69 6e74 7328 7365 6c66 2e6d  ry_points(self.m
+00003b90: 6173 6b2c 2073 656c 662e 7863 616c 6962  ask, self.xcalib
+00003ba0: 7261 7469 6f6e 2c20 7365 6c66 2e79 6361  ration, self.yca
+00003bb0: 6c69 6272 6174 696f 6e2c 2073 656c 662e  libration, self.
+00003bc0: 7a63 616c 6962 7261 7469 6f6e 290d 0a0d  zcalibration)...
+00003bd0: 0a20 2020 2020 2020 2020 200d 0a0d 0a0d  .          .....
+00003be0: 0a20 2020 2064 6566 205f 6765 6e65 7261  .    def _genera
+00003bf0: 7465 5f67 656e 6572 6174 696f 6e73 2873  te_generations(s
+00003c00: 656c 662c 2074 7261 636b 293a 0d0a 2020  elf, track):..  
+00003c10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00003c20: 2061 6c6c 5f73 6f75 7263 655f 6964 7320   all_source_ids 
+00003c30: 3d20 5b5d 0d0a 2020 2020 2020 2020 616c  = []..        al
+00003c40: 6c5f 7461 7267 6574 5f69 6473 203d 205b  l_target_ids = [
+00003c50: 5d20 0d0a 0d0a 0d0a 2020 2020 2020 2020  ] ......        
+00003c60: 666f 7220 6564 6765 2069 6e20 7472 6163  for edge in trac
+00003c70: 6b2e 6669 6e64 616c 6c28 2745 6467 6527  k.findall('Edge'
+00003c80: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
 00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ca0: 2069 6620 736f 7572 6365 5f69 6420 696e   if source_id in
-00003cb0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00003cc0: 745f 6c6f 6f6b 7570 2e6b 6579 7328 293a  t_lookup.keys():
-00003cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003ca0: 2020 736f 7572 6365 5f69 6420 3d20 696e    source_id = in
+00003cb0: 7428 6564 6765 2e67 6574 2873 656c 662e  t(edge.get(self.
+00003cc0: 7370 6f74 5f73 6f75 7263 655f 6964 5f6b  spot_source_id_k
+00003cd0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00003d00: 745f 6c6f 6f6b 7570 5b73 6f75 7263 655f  t_lookup[source_
-00003d10: 6964 5d2e 6170 7065 6e64 2874 6172 6765  id].append(targe
-00003d20: 745f 6964 290d 0a20 2020 2020 2020 2020  t_id)..         
+00003cf0: 2020 7461 7267 6574 5f69 6420 3d20 696e    target_id = in
+00003d00: 7428 6564 6765 2e67 6574 2873 656c 662e  t(edge.get(self.
+00003d10: 7370 6f74 5f74 6172 6765 745f 6964 5f6b  spot_target_id_k
+00003d20: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2065 6c73 653a 2020 2020 2020 0d0a     else:      ..
-00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003d70: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-00003d80: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
-00003d90: 5d20 3d20 5b74 6172 6765 745f 6964 5d0d  ] = [target_id].
-00003da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003dc0: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
-00003dd0: 6f6b 7570 5b74 6172 6765 745f 6964 5d20  okup[target_id] 
-00003de0: 3d20 736f 7572 6365 5f69 6420 0d0a 0d0a  = source_id ....
-00003df0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00003e00: 6c6c 5f73 6f75 7263 655f 6964 732c 2061  ll_source_ids, a
-00003e10: 6c6c 5f74 6172 6765 745f 6964 7320 0d0a  ll_target_ids ..
-00003e20: 0d0a 0d0a 2020 2020 6465 6620 5f63 7265  ....    def _cre
-00003e30: 6174 655f 6765 6e65 7261 7469 6f6e 7328  ate_generations(
-00003e40: 7365 6c66 2c20 616c 6c5f 736f 7572 6365  self, all_source
-00003e50: 5f69 6473 3a20 6c69 7374 293a 0d0a 2020  _ids: list):..  
-00003e60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003e70: 2072 6f6f 745f 6c65 6166 203d 205b 5d0d   root_leaf = [].
-00003e80: 0a20 2020 2020 2020 2072 6f6f 745f 726f  .        root_ro
-00003e90: 6f74 203d 205b 5d0d 0a20 2020 2020 2020  ot = []..       
-00003ea0: 2072 6f6f 745f 7370 6c69 7473 203d 205b   root_splits = [
-00003eb0: 5d0d 0a20 2020 2020 2020 2023 4765 7420  ]..        #Get 
-00003ec0: 7468 6520 726f 6f74 2069 640d 0a20 2020  the root id..   
-00003ed0: 2020 2020 2066 6f72 2073 6f75 7263 655f       for source_
-00003ee0: 6964 2069 6e20 616c 6c5f 736f 7572 6365  id in all_source
-00003ef0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00003f00: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00003f10: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
-00003f20: 6f75 7263 655f 6c6f 6f6b 7570 3a0d 0a20  ource_lookup:.. 
-00003f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003f40: 6f75 7263 655f 7461 7267 6574 5f69 6420  ource_target_id 
-00003f50: 3d20 7365 6c66 2e65 6467 655f 736f 7572  = self.edge_sour
-00003f60: 6365 5f6c 6f6f 6b75 705b 736f 7572 6365  ce_lookup[source
-00003f70: 5f69 645d 0d0a 2020 2020 2020 2020 2020  _id]..          
-00003f80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00003f90: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
-00003fa0: 655f 7461 7267 6574 5f69 6420 3d20 4e6f  e_target_id = No
-00003fb0: 6e65 2020 2020 2020 2020 2020 0d0a 2020  ne          ..  
-00003fc0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00003fd0: 6574 5f74 6172 6765 745f 6964 203d 2073  et_target_id = s
-00003fe0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-00003ff0: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
-00004000: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00004010: 2069 6620 736f 7572 6365 5f74 6172 6765   if source_targe
-00004020: 745f 6964 2069 7320 4e6f 6e65 3a0d 0a20  t_id is None:.. 
-00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004040: 2020 6966 2073 6f75 7263 655f 6964 206e    if source_id n
-00004050: 6f74 2069 6e20 726f 6f74 5f72 6f6f 743a  ot in root_root:
-00004060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004070: 2020 2020 2020 2020 726f 6f74 5f72 6f6f          root_roo
-00004080: 742e 6170 7065 6e64 2873 6f75 7263 655f  t.append(source_
-00004090: 6964 2920 0d0a 2020 2020 2020 2020 2020  id) ..          
-000040a0: 2020 2020 6966 206c 656e 2874 6172 6765      if len(targe
-000040b0: 745f 7461 7267 6574 5f69 6429 203e 2031  t_target_id) > 1
-000040c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000040d0: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
-000040e0: 6964 206e 6f74 2069 6e20 726f 6f74 5f73  id not in root_s
-000040f0: 706c 6974 733a 0d0a 2020 2020 2020 2020  plits:..        
-00004100: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00004110: 6f74 5f73 706c 6974 732e 6170 7065 6e64  ot_splits.append
-00004120: 2873 6f75 7263 655f 6964 290d 0a20 2020  (source_id)..   
-00004130: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
-00004140: 7267 6574 5f74 6172 6765 745f 6964 5b30  rget_target_id[0
-00004150: 5d20 6e6f 7420 696e 2073 656c 662e 6564  ] not in self.ed
-00004160: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-00004170: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004180: 2020 2020 2020 726f 6f74 5f6c 6561 662e        root_leaf.
-00004190: 6170 7065 6e64 2874 6172 6765 745f 7461  append(target_ta
-000041a0: 7267 6574 5f69 645b 305d 2920 2020 2020  rget_id[0])     
-000041b0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-000041c0: 2072 6574 7572 6e20 726f 6f74 5f72 6f6f   return root_roo
-000041d0: 742c 2072 6f6f 745f 7370 6c69 7473 2c20  t, root_splits, 
-000041e0: 726f 6f74 5f6c 6561 660d 0a0d 0a20 2020  root_leaf....   
-000041f0: 2064 6566 205f 736f 7274 5f64 6976 6964   def _sort_divid
-00004200: 696e 675f 6365 6c6c 7328 7365 6c66 2c20  ing_cells(self, 
-00004210: 726f 6f74 5f73 706c 6974 7329 3a0d 0a20  root_splits):.. 
-00004220: 2020 2020 2020 2020 2020 6365 6c6c 5f69            cell_i
-00004230: 645f 7469 6d65 7320 3d20 5b5d 0d0a 2020  d_times = []..  
-00004240: 2020 2020 2020 2020 2063 656c 6c5f 6964           cell_id
-00004250: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00004260: 2020 2066 6f72 2072 6f6f 745f 7370 6c69     for root_spli
-00004270: 7420 696e 2072 6f6f 745f 7370 6c69 7473  t in root_splits
-00004280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004290: 2020 2020 2073 706c 6974 5f63 656c 6c5f       split_cell_
-000042a0: 6964 5f74 696d 6520 3d20 7365 6c66 2e75  id_time = self.u
-000042b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000042c0: 7274 6965 735b 726f 6f74 5f73 706c 6974  rties[root_split
-000042d0: 5d5b 7365 6c66 2e66 7261 6d65 6964 5f6b  ][self.frameid_k
-000042e0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-000042f0: 2020 2020 2020 2063 656c 6c5f 6964 5f74         cell_id_t
-00004300: 696d 6573 2e61 7070 656e 6428 7370 6c69  imes.append(spli
-00004310: 745f 6365 6c6c 5f69 645f 7469 6d65 290d  t_cell_id_time).
-00004320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004330: 2020 2063 656c 6c5f 6964 732e 6170 7065     cell_ids.appe
-00004340: 6e64 2872 6f6f 745f 7370 6c69 7429 0d0a  nd(root_split)..
-00004350: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00004360: 645f 696e 6469 6365 7320 3d20 736f 7274  d_indices = sort
-00004370: 6564 2872 616e 6765 286c 656e 2863 656c  ed(range(len(cel
-00004380: 6c5f 6964 5f74 696d 6573 2929 2c20 6b65  l_id_times)), ke
-00004390: 793d 6c61 6d62 6461 206b 3a20 6365 6c6c  y=lambda k: cell
-000043a0: 5f69 645f 7469 6d65 735b 6b5d 290d 0a20  _id_times[k]).. 
-000043b0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-000043c0: 5f63 656c 6c5f 6964 7320 3d20 5b63 656c  _cell_ids = [cel
-000043d0: 6c5f 6964 735b 695d 2066 6f72 2069 2069  l_ids[i] for i i
-000043e0: 6e20 736f 7274 6564 5f69 6e64 6963 6573  n sorted_indices
-000043f0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00004400: 7265 7475 726e 2073 6f72 7465 645f 6365  return sorted_ce
-00004410: 6c6c 5f69 6473 2020 2020 2020 200d 0a0d  ll_ids       ...
-00004420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004430: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-00004440: 6566 205f 6974 6572 6174 655f 6469 7669  ef _iterate_divi
-00004450: 6469 6e67 5f72 6563 7572 7369 7665 2873  ding_recursive(s
-00004460: 656c 662c 2072 6f6f 745f 6c65 6166 2c20  elf, root_leaf, 
-00004470: 7461 7267 6574 5f63 656c 6c2c 2073 6f72  target_cell, sor
-00004480: 7465 645f 726f 6f74 5f73 706c 6974 732c  ted_root_splits,
-00004490: 2067 656e 5f63 6f75 6e74 2c20 7472 6163   gen_count, trac
-000044a0: 6b6c 6574 5f63 6f75 6e74 2c20 7472 6163  klet_count, trac
-000044b0: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
-000044c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000044d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000044e0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000044f0: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-00004500: 6174 696f 6e5f 6469 6374 5b74 6172 6765  ation_dict[targe
-00004510: 745f 6365 6c6c 5d20 3d20 6765 6e5f 636f  t_cell] = gen_co
-00004520: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-00004530: 2020 2020 2073 656c 662e 7472 6163 6b6c       self.trackl
-00004540: 6574 5f64 6963 745b 7461 7267 6574 5f63  et_dict[target_c
-00004550: 656c 6c5d 203d 2074 7261 636b 6c65 745f  ell] = tracklet_
-00004560: 636f 756e 740d 0a0d 0a20 2020 2020 2020  count....       
-00004570: 2020 2020 2020 2020 2069 6620 7461 7267           if targ
-00004580: 6574 5f63 656c 6c20 3d3d 2072 6f6f 745f  et_cell == root_
-00004590: 6c65 6166 3a0d 0a20 2020 2020 2020 2020  leaf:..         
-000045a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000045b0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-000045c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000045d0: 2020 2020 206e 6578 745f 7461 7267 6574       next_target
-000045e0: 5f63 656c 6c20 3d20 4e6f 6e65 0d0a 2020  _cell = None..  
-000045f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
-00004620: 6e20 736f 7274 6564 5f72 6f6f 745f 7370  n sorted_root_sp
-00004630: 6c69 7473 3a0d 0a20 2020 2020 2020 2020  lits:..         
-00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004650: 2020 6e65 7874 5f67 656e 5f63 6f75 6e74    next_gen_count
-00004660: 203d 2067 656e 5f63 6f75 6e74 202b 2031   = gen_count + 1
-00004670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004680: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004690: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
-000046a0: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-000046b0: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046d0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-000046e0: 6365 6c6c 7320 3d20 7365 6c66 2e65 6467  cells = self.edg
-000046f0: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
-00004700: 7461 7267 6574 5f63 656c 6c5d 0d0a 2020  target_cell]..  
-00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004720: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004730: 7220 6b20 696e 2072 616e 6765 286c 656e  r k in range(len
-00004740: 2874 6172 6765 745f 6365 6c6c 7329 293a  (target_cells)):
-00004750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004770: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
-00004780: 6172 6765 745f 6365 6c6c 203d 2074 6172  arget_cell = tar
-00004790: 6765 745f 6365 6c6c 735b 6b5d 0d0a 2020  get_cells[k]..  
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 7472 6163 6b6c 6574 5f63 6f75 6e74    tracklet_count
-000047d0: 203d 2074 7261 636b 6c65 745f 636f 756e   = tracklet_coun
-000047e0: 7420 2b20 3120 2b20 6b0d 0a20 2020 2020  t + 1 + k..     
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004810: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
-00004820: 7365 6c66 2e5f 756e 6971 7565 5f74 7261  self._unique_tra
-00004830: 636b 6c65 745f 636f 756e 7428 7472 6163  cklet_count(trac
-00004840: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
-00004850: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-00004860: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00003d40: 2020 616c 6c5f 736f 7572 6365 5f69 6473    all_source_ids
+00003d50: 2e61 7070 656e 6428 736f 7572 6365 5f69  .append(source_i
+00003d60: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 616c 6c5f 7461 7267 6574 5f69 6473 2e61  all_target_ids.a
+00003d90: 7070 656e 6428 7461 7267 6574 5f69 6429  ppend(target_id)
+00003da0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003db0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003dc0: 2073 6f75 7263 655f 6964 2069 6e20 7365   source_id in se
+00003dd0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00003de0: 6f6f 6b75 702e 6b65 7973 2829 3a0d 0a20  ookup.keys():.. 
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003e10: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00003e20: 6f6f 6b75 705b 736f 7572 6365 5f69 645d  ookup[source_id]
+00003e30: 2e61 7070 656e 6428 7461 7267 6574 5f69  .append(target_i
+00003e40: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e60: 656c 7365 3a20 2020 2020 200d 0a20 2020  else:      ..   
+00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003e90: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00003ea0: 6b75 705b 736f 7572 6365 5f69 645d 203d  kup[source_id] =
+00003eb0: 205b 7461 7267 6574 5f69 645d 0d0a 2020   [target_id]..  
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ed0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00003ee0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
+00003ef0: 705b 7461 7267 6574 5f69 645d 203d 2073  p[target_id] = s
+00003f00: 6f75 7263 655f 6964 200d 0a0d 0a20 2020  ource_id ....   
+00003f10: 2020 2020 2072 6574 7572 6e20 616c 6c5f       return all_
+00003f20: 736f 7572 6365 5f69 6473 2c20 616c 6c5f  source_ids, all_
+00003f30: 7461 7267 6574 5f69 6473 200d 0a0d 0a0d  target_ids .....
+00003f40: 0a20 2020 2064 6566 205f 6372 6561 7465  .    def _create
+00003f50: 5f67 656e 6572 6174 696f 6e73 2873 656c  _generations(sel
+00003f60: 662c 2061 6c6c 5f73 6f75 7263 655f 6964  f, all_source_id
+00003f70: 733a 206c 6973 7429 3a0d 0a20 2020 2020  s: list):..     
+00003f80: 2020 2020 0d0a 2020 2020 2020 2020 726f      ..        ro
+00003f90: 6f74 5f6c 6561 6620 3d20 5b5d 0d0a 2020  ot_leaf = []..  
+00003fa0: 2020 2020 2020 726f 6f74 5f72 6f6f 7420        root_root 
+00003fb0: 3d20 5b5d 0d0a 2020 2020 2020 2020 726f  = []..        ro
+00003fc0: 6f74 5f73 706c 6974 7320 3d20 5b5d 0d0a  ot_splits = []..
+00003fd0: 2020 2020 2020 2020 2347 6574 2074 6865          #Get the
+00003fe0: 2072 6f6f 7420 6964 0d0a 2020 2020 2020   root id..      
+00003ff0: 2020 666f 7220 736f 7572 6365 5f69 6420    for source_id 
+00004000: 696e 2061 6c6c 5f73 6f75 7263 655f 6964  in all_source_id
+00004010: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004020: 2020 6966 2073 6f75 7263 655f 6964 2069    if source_id i
+00004030: 6e20 7365 6c66 2e65 6467 655f 736f 7572  n self.edge_sour
+00004040: 6365 5f6c 6f6f 6b75 703a 0d0a 2020 2020  ce_lookup:..    
+00004050: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+00004060: 6365 5f74 6172 6765 745f 6964 203d 2073  ce_target_id = s
+00004070: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00004080: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
+00004090: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000040a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+000040b0: 2020 2020 2020 2020 736f 7572 6365 5f74          source_t
+000040c0: 6172 6765 745f 6964 203d 204e 6f6e 6520  arget_id = None 
+000040d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000040e0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+000040f0: 7461 7267 6574 5f69 6420 3d20 7365 6c66  target_id = self
+00004100: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00004110: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
+00004120: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004130: 2073 6f75 7263 655f 7461 7267 6574 5f69   source_target_i
+00004140: 6420 6973 204e 6f6e 653a 0d0a 2020 2020  d is None:..    
+00004150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004160: 6620 736f 7572 6365 5f69 6420 6e6f 7420  f source_id not 
+00004170: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004190: 2020 2020 2072 6f6f 745f 726f 6f74 2e61       root_root.a
+000041a0: 7070 656e 6428 736f 7572 6365 5f69 6429  ppend(source_id)
+000041b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000041c0: 2069 6620 6c65 6e28 7461 7267 6574 5f74   if len(target_t
+000041d0: 6172 6765 745f 6964 2920 3e20 313a 0d0a  arget_id) > 1:..
+000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041f0: 2020 2069 6620 736f 7572 6365 5f69 6420     if source_id 
+00004200: 6e6f 7420 696e 2072 6f6f 745f 7370 6c69  not in root_spli
+00004210: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00004220: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00004230: 7370 6c69 7473 2e61 7070 656e 6428 736f  splits.append(so
+00004240: 7572 6365 5f69 6429 0d0a 2020 2020 2020  urce_id)..      
+00004250: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004260: 745f 7461 7267 6574 5f69 645b 305d 206e  t_target_id[0] n
+00004270: 6f74 2069 6e20 7365 6c66 2e65 6467 655f  ot in self.edge_
+00004280: 7461 7267 6574 5f6c 6f6f 6b75 703a 0d0a  target_lookup:..
+00004290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042a0: 2020 2072 6f6f 745f 6c65 6166 2e61 7070     root_leaf.app
+000042b0: 656e 6428 7461 7267 6574 5f74 6172 6765  end(target_targe
+000042c0: 745f 6964 5b30 5d29 2020 2020 2020 2020  t_id[0])        
+000042d0: 2020 0d0a 0d0a 2020 2020 2020 2020 7265    ....        re
+000042e0: 7475 726e 2072 6f6f 745f 726f 6f74 2c20  turn root_root, 
+000042f0: 726f 6f74 5f73 706c 6974 732c 2072 6f6f  root_splits, roo
+00004300: 745f 6c65 6166 0d0a 0d0a 2020 2020 6465  t_leaf....    de
+00004310: 6620 5f73 6f72 745f 6469 7669 6469 6e67  f _sort_dividing
+00004320: 5f63 656c 6c73 2873 656c 662c 2072 6f6f  _cells(self, roo
+00004330: 745f 7370 6c69 7473 293a 0d0a 2020 2020  t_splits):..    
+00004340: 2020 2020 2020 2063 656c 6c5f 6964 5f74         cell_id_t
+00004350: 696d 6573 203d 205b 5d0d 0a20 2020 2020  imes = []..     
+00004360: 2020 2020 2020 6365 6c6c 5f69 6473 203d        cell_ids =
+00004370: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00004380: 666f 7220 726f 6f74 5f73 706c 6974 2069  for root_split i
+00004390: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043b0: 2020 7370 6c69 745f 6365 6c6c 5f69 645f    split_cell_id_
+000043c0: 7469 6d65 203d 2073 656c 662e 756e 6971  time = self.uniq
+000043d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000043e0: 6573 5b72 6f6f 745f 7370 6c69 745d 5b73  es[root_split][s
+000043f0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+00004400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004410: 2020 2020 6365 6c6c 5f69 645f 7469 6d65      cell_id_time
+00004420: 732e 6170 7065 6e64 2873 706c 6974 5f63  s.append(split_c
+00004430: 656c 6c5f 6964 5f74 696d 6529 0d0a 2020  ell_id_time)..  
+00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004450: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
+00004460: 726f 6f74 5f73 706c 6974 290d 0a20 2020  root_split)..   
+00004470: 2020 2020 2020 2020 736f 7274 6564 5f69          sorted_i
+00004480: 6e64 6963 6573 203d 2073 6f72 7465 6428  ndices = sorted(
+00004490: 7261 6e67 6528 6c65 6e28 6365 6c6c 5f69  range(len(cell_i
+000044a0: 645f 7469 6d65 7329 292c 206b 6579 3d6c  d_times)), key=l
+000044b0: 616d 6264 6120 6b3a 2063 656c 6c5f 6964  ambda k: cell_id
+000044c0: 5f74 696d 6573 5b6b 5d29 0d0a 2020 2020  _times[k])..    
+000044d0: 2020 2020 2020 2073 6f72 7465 645f 6365         sorted_ce
+000044e0: 6c6c 5f69 6473 203d 205b 6365 6c6c 5f69  ll_ids = [cell_i
+000044f0: 6473 5b69 5d20 666f 7220 6920 696e 2073  ds[i] for i in s
+00004500: 6f72 7465 645f 696e 6469 6365 735d 0d0a  orted_indices]..
+00004510: 0d0a 2020 2020 2020 2020 2020 2072 6574  ..           ret
+00004520: 7572 6e20 736f 7274 6564 5f63 656c 6c5f  urn sorted_cell_
+00004530: 6964 7320 2020 2020 2020 0d0a 0d0a 2020  ids       ....  
+00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004550: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+00004560: 5f69 7465 7261 7465 5f64 6976 6964 696e  _iterate_dividin
+00004570: 675f 7265 6375 7273 6976 6528 7365 6c66  g_recursive(self
+00004580: 2c20 726f 6f74 5f6c 6561 662c 2074 6172  , root_leaf, tar
+00004590: 6765 745f 6365 6c6c 2c20 736f 7274 6564  get_cell, sorted
+000045a0: 5f72 6f6f 745f 7370 6c69 7473 2c20 6765  _root_splits, ge
+000045b0: 6e5f 636f 756e 742c 2074 7261 636b 6c65  n_count, trackle
+000045c0: 745f 636f 756e 742c 2074 7261 636b 6c65  t_count, trackle
+000045d0: 745f 636f 756e 745f 7461 6b65 6e29 3a0d  t_count_taken):.
+000045e0: 0a20 2020 2020 2020 2020 2020 200d 0a0d  .            ...
+000045f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004600: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00004610: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004620: 6f6e 5f64 6963 745b 7461 7267 6574 5f63  on_dict[target_c
+00004630: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
+00004640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004650: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
+00004660: 6469 6374 5b74 6172 6765 745f 6365 6c6c  dict[target_cell
+00004670: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
+00004680: 6e74 0d0a 0d0a 2020 2020 2020 2020 2020  nt....          
+00004690: 2020 2020 2020 6966 2074 6172 6765 745f        if target_
+000046a0: 6365 6c6c 203d 3d20 726f 6f74 5f6c 6561  cell == root_lea
+000046b0: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+000046c0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000046f0: 2020 6e65 7874 5f74 6172 6765 745f 6365    next_target_ce
+00004700: 6c6c 203d 204e 6f6e 650d 0a20 2020 2020  ll = None..     
+00004710: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004720: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004730: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
+00004740: 6f72 7465 645f 726f 6f74 5f73 706c 6974  orted_root_split
+00004750: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004760: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00004770: 6578 745f 6765 6e5f 636f 756e 7420 3d20  ext_gen_count = 
+00004780: 6765 6e5f 636f 756e 7420 2b20 310d 0a20  gen_count + 1.. 
+00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047a0: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+000047b0: 6765 745f 6365 6c6c 2069 6e20 7365 6c66  get_cell in self
+000047c0: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+000047d0: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00004800: 6c73 203d 2073 656c 662e 6564 6765 5f74  ls = self.edge_t
+00004810: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
+00004820: 6765 745f 6365 6c6c 5d0d 0a20 2020 2020  get_cell]..     
+00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004840: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00004850: 2069 6e20 7261 6e67 6528 6c65 6e28 7461   in range(len(ta
+00004860: 7267 6574 5f63 656c 6c73 2929 3a0d 0a20  rget_cells)):.. 
 00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
-00004890: 636f 756e 745f 7461 6b65 6e2e 6170 7065  count_taken.appe
-000048a0: 6e64 2874 7261 636b 6c65 745f 636f 756e  nd(tracklet_coun
-000048b0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004890: 2020 2064 6175 6768 7465 725f 7461 7267     daughter_targ
+000048a0: 6574 5f63 656c 6c20 3d20 7461 7267 6574  et_cell = target
+000048b0: 5f63 656c 6c73 5b6b 5d0d 0a20 2020 2020  _cells[k]..     
 000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2020 2020 2020 7365 6c66 2e5f 6974          self._it
-000048e0: 6572 6174 655f 6469 7669 6469 6e67 5f72  erate_dividing_r
-000048f0: 6563 7572 7369 7665 2872 6f6f 745f 6c65  ecursive(root_le
-00004900: 6166 2c20 6461 7567 6874 6572 5f74 6172  af, daughter_tar
-00004910: 6765 745f 6365 6c6c 2c20 736f 7274 6564  get_cell, sorted
-00004920: 5f72 6f6f 745f 7370 6c69 7473 2c20 6e65  _root_splits, ne
-00004930: 7874 5f67 656e 5f63 6f75 6e74 2c20 7472  xt_gen_count, tr
-00004940: 6163 6b6c 6574 5f63 6f75 6e74 2c20 7472  acklet_count, tr
-00004950: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
-00004960: 656e 2920 2020 2020 200d 0a0d 0a20 2020  en)      ....   
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004990: 2020 2069 6620 7461 7267 6574 5f63 656c     if target_cel
-000049a0: 6c20 696e 2073 656c 662e 6564 6765 5f74  l in self.edge_t
-000049b0: 6172 6765 745f 6c6f 6f6b 7570 3a0d 0a20  arget_lookup:.. 
-000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049d0: 2020 206e 6578 745f 7461 7267 6574 5f63     next_target_c
-000049e0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
-000049f0: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b74  _target_lookup[t
-00004a00: 6172 6765 745f 6365 6c6c 5d0d 0a20 2020  arget_cell]..   
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
-00004a30: 6c20 3d20 6e65 7874 5f74 6172 6765 745f  l = next_target_
-00004a40: 6365 6c6c 735b 305d 0d0a 2020 2020 2020  cells[0]..      
-00004a50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00004a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004a70: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2077 6869 6c65 206e 6578 745f 7461     while next_ta
-00004aa0: 7267 6574 5f63 656c 6c20 6e6f 7420 696e  rget_cell not in
-00004ab0: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
-00004ac0: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004ae0: 6c66 2e67 656e 6572 6174 696f 6e5f 6469  lf.generation_di
-00004af0: 6374 5b6e 6578 745f 7461 7267 6574 5f63  ct[next_target_c
-00004b00: 656c 6c5d 203d 2067 656e 5f63 6f75 6e74  ell] = gen_count
-00004b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004b20: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00004b30: 7261 636b 6c65 745f 6469 6374 5b6e 6578  racklet_dict[nex
-00004b40: 745f 7461 7267 6574 5f63 656c 6c5d 203d  t_target_cell] =
-00004b50: 2074 7261 636b 6c65 745f 636f 756e 740d   tracklet_count.
-00004b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b70: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
-00004b80: 5f74 6172 6765 745f 6365 6c6c 2069 6e20  _target_cell in 
-00004b90: 726f 6f74 5f6c 6561 663a 0d0a 2020 2020  root_leaf:..    
+000048d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000048e0: 7261 636b 6c65 745f 636f 756e 7420 3d20  racklet_count = 
+000048f0: 7472 6163 6b6c 6574 5f63 6f75 6e74 202b  tracklet_count +
+00004900: 2031 202b 206b 0d0a 2020 2020 2020 2020   1 + k..        
+00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00004930: 6b6c 6574 5f63 6f75 6e74 203d 2073 656c  klet_count = sel
+00004940: 662e 5f75 6e69 7175 655f 7472 6163 6b6c  f._unique_trackl
+00004950: 6574 5f63 6f75 6e74 2874 7261 636b 6c65  et_count(trackle
+00004960: 745f 636f 756e 745f 7461 6b65 6e2c 2074  t_count_taken, t
+00004970: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049a0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
+000049b0: 6e74 5f74 616b 656e 2e61 7070 656e 6428  nt_taken.append(
+000049c0: 7472 6163 6b6c 6574 5f63 6f75 6e74 290d  tracklet_count).
+000049d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
+00004a00: 7465 5f64 6976 6964 696e 675f 7265 6375  te_dividing_recu
+00004a10: 7273 6976 6528 726f 6f74 5f6c 6561 662c  rsive(root_leaf,
+00004a20: 2064 6175 6768 7465 725f 7461 7267 6574   daughter_target
+00004a30: 5f63 656c 6c2c 2073 6f72 7465 645f 726f  _cell, sorted_ro
+00004a40: 6f74 5f73 706c 6974 732c 206e 6578 745f  ot_splits, next_
+00004a50: 6765 6e5f 636f 756e 742c 2074 7261 636b  gen_count, track
+00004a60: 6c65 745f 636f 756e 742c 2074 7261 636b  let_count, track
+00004a70: 6c65 745f 636f 756e 745f 7461 6b65 6e29  let_count_taken)
+00004a80: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00004a90: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 6966 2074 6172 6765 745f 6365 6c6c 2069  if target_cell i
+00004ac0: 6e20 7365 6c66 2e65 6467 655f 7461 7267  n self.edge_targ
+00004ad0: 6574 5f6c 6f6f 6b75 703a 0d0a 2020 2020  et_lookup:..    
+00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004af0: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+00004b00: 7320 3d20 7365 6c66 2e65 6467 655f 7461  s = self.edge_ta
+00004b10: 7267 6574 5f6c 6f6f 6b75 705b 7461 7267  rget_lookup[targ
+00004b20: 6574 5f63 656c 6c5d 0d0a 2020 2020 2020  et_cell]..      
+00004b30: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00004b40: 7874 5f74 6172 6765 745f 6365 6c6c 203d  xt_target_cell =
+00004b50: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004b60: 6c73 5b30 5d0d 0a20 2020 2020 2020 2020  ls[0]..         
+00004b70: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004bc0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-00004bd0: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
-00004be0: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-00004c10: 6163 6b6c 6574 5f64 6963 745b 7461 7267  acklet_dict[targ
-00004c20: 6574 5f63 656c 6c5d 203d 2074 7261 636b  et_cell] = track
-00004c30: 6c65 745f 636f 756e 740d 0a20 2020 2020  let_count..     
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-00004c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c70: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
-00004c80: 5f74 6172 6765 745f 6365 6c6c 2069 6e20  _target_cell in 
-00004c90: 7365 6c66 2e65 6467 655f 7461 7267 6574  self.edge_target
-00004ca0: 5f6c 6f6f 6b75 703a 0d0a 2020 2020 2020  _lookup:..      
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 2020 2020 6e65 7874 5f74 6172 6765        next_targe
-00004cd0: 745f 6365 6c6c 7320 3d20 7365 6c66 2e65  t_cells = self.e
-00004ce0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00004cf0: 705b 6e65 7874 5f74 6172 6765 745f 6365  p[next_target_ce
-00004d00: 6c6c 5d0d 0a20 2020 2020 2020 2020 2020  ll]..           
+00004bb0: 7768 696c 6520 6e65 7874 5f74 6172 6765  while next_targe
+00004bc0: 745f 6365 6c6c 206e 6f74 2069 6e20 736f  t_cell not in so
+00004bd0: 7274 6564 5f72 6f6f 745f 7370 6c69 7473  rted_root_splits
+00004be0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004bf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004c00: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
+00004c10: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+00004c20: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
+00004c50: 6b6c 6574 5f64 6963 745b 6e65 7874 5f74  klet_dict[next_t
+00004c60: 6172 6765 745f 6365 6c6c 5d20 3d20 7472  arget_cell] = tr
+00004c70: 6163 6b6c 6574 5f63 6f75 6e74 0d0a 2020  acklet_count..  
+00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c90: 2020 2020 2020 6966 206e 6578 745f 7461        if next_ta
+00004ca0: 7267 6574 5f63 656c 6c20 696e 2072 6f6f  rget_cell in roo
+00004cb0: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
+00004ce0: 6572 6174 696f 6e5f 6469 6374 5b74 6172  eration_dict[tar
+00004cf0: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
+00004d00: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
 00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
-00004d30: 6c20 3d20 6e65 7874 5f74 6172 6765 745f  l = next_target_
-00004d40: 6365 6c6c 735b 305d 0d0a 2020 2020 2020  cells[0]..      
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 2020 2020 6966 206e 6578 745f 7461        if next_ta
-00004d70: 7267 6574 5f63 656c 6c20 696e 2072 6f6f  rget_cell in roo
-00004d80: 745f 6c65 6166 3a0d 0a20 2020 2020 2020  t_leaf:..       
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
-00004db0: 6572 6174 696f 6e5f 6469 6374 5b74 6172  eration_dict[tar
-00004dc0: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
-00004dd0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
-00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004df0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-00004e00: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
-00004e10: 6365 6c6c 5d20 3d20 7472 6163 6b6c 6574  cell] = tracklet
-00004e20: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 2020 2062 7265 616b 0d0a 0d0a         break....
-00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e60: 6966 206e 6578 745f 7461 7267 6574 5f63  if next_target_c
-00004e70: 656c 6c20 6973 206e 6f74 204e 6f6e 653a  ell is not None:
-00004e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004e90: 2020 2020 2020 7365 6c66 2e67 656e 6572        self.gener
-00004ea0: 6174 696f 6e5f 6469 6374 5b6e 6578 745f  ation_dict[next_
-00004eb0: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
-00004ec0: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004ee0: 6c66 2e74 7261 636b 6c65 745f 6469 6374  lf.tracklet_dict
-00004ef0: 5b6e 6578 745f 7461 7267 6574 5f63 656c  [next_target_cel
-00004f00: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
-00004f10: 756e 7420 200d 0a20 2020 2020 2020 2020  unt  ..         
-00004f20: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00004f30: 6765 6e5f 636f 756e 7420 3d20 6765 6e5f  gen_count = gen_
-00004f40: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-00004f50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00004f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f70: 2020 2020 2069 6620 6e65 7874 5f74 6172       if next_tar
-00004f80: 6765 745f 6365 6c6c 2069 6e20 7365 6c66  get_cell in self
-00004f90: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
-00004fa0: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2020 7461 7267 6574 5f63 656c 6c73 203d    target_cells =
-00004fd0: 2073 656c 662e 6564 6765 5f74 6172 6765   self.edge_targe
-00004fe0: 745f 6c6f 6f6b 7570 5b6e 6578 745f 7461  t_lookup[next_ta
-00004ff0: 7267 6574 5f63 656c 6c5d 0d0a 2020 2020  rget_cell]..    
-00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005010: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00005020: 2072 616e 6765 286c 656e 2874 6172 6765   range(len(targe
-00005030: 745f 6365 6c6c 7329 293a 0d0a 2020 2020  t_cells)):..    
-00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00005060: 6574 5f63 656c 6c20 3d20 7461 7267 6574  et_cell = target
-00005070: 5f63 656c 6c73 5b6b 5d0d 0a20 2020 2020  _cells[k]..     
+00004d20: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00004d30: 6c65 745f 6469 6374 5b74 6172 6765 745f  let_dict[target_
+00004d40: 6365 6c6c 5d20 3d20 7472 6163 6b6c 6574  cell] = tracklet
+00004d50: 5f63 6f75 6e74 0d0a 2020 2020 2020 2020  _count..        
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d90: 2020 2020 2020 6966 206e 6578 745f 7461        if next_ta
+00004da0: 7267 6574 5f63 656c 6c20 696e 2073 656c  rget_cell in sel
+00004db0: 662e 6564 6765 5f74 6172 6765 745f 6c6f  f.edge_target_lo
+00004dc0: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 206e 6578 745f 7461 7267 6574 5f63     next_target_c
+00004df0: 656c 6c73 203d 2073 656c 662e 6564 6765  ells = self.edge
+00004e00: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b6e  _target_lookup[n
+00004e10: 6578 745f 7461 7267 6574 5f63 656c 6c5d  ext_target_cell]
+00004e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e30: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00004e40: 7874 5f74 6172 6765 745f 6365 6c6c 203d  xt_target_cell =
+00004e50: 206e 6578 745f 7461 7267 6574 5f63 656c   next_target_cel
+00004e60: 6c73 5b30 5d0d 0a20 2020 2020 2020 2020  ls[0]..         
+00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e80: 2020 2069 6620 6e65 7874 5f74 6172 6765     if next_targe
+00004e90: 745f 6365 6c6c 2069 6e20 726f 6f74 5f6c  t_cell in root_l
+00004ea0: 6561 663a 0d0a 2020 2020 2020 2020 2020  eaf:..          
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ec0: 2020 2020 2073 656c 662e 6765 6e65 7261       self.genera
+00004ed0: 7469 6f6e 5f64 6963 745b 7461 7267 6574  tion_dict[target
+00004ee0: 5f63 656c 6c5d 203d 2067 656e 5f63 6f75  _cell] = gen_cou
+00004ef0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f10: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
+00004f20: 5f64 6963 745b 7461 7267 6574 5f63 656c  _dict[target_cel
+00004f30: 6c5d 203d 2074 7261 636b 6c65 745f 636f  l] = tracklet_co
+00004f40: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
+00004f70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004f80: 6e65 7874 5f74 6172 6765 745f 6365 6c6c  next_target_cell
+00004f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
+00004fc0: 6f6e 5f64 6963 745b 6e65 7874 5f74 6172  on_dict[next_tar
+00004fd0: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
+00004fe0: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+00004ff0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005000: 7472 6163 6b6c 6574 5f64 6963 745b 6e65  tracklet_dict[ne
+00005010: 7874 5f74 6172 6765 745f 6365 6c6c 5d20  xt_target_cell] 
+00005020: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
+00005030: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005040: 2020 2020 2020 2020 6e65 7874 5f67 656e          next_gen
+00005050: 5f63 6f75 6e74 203d 2067 656e 5f63 6f75  _count = gen_cou
+00005060: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00005070: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005090: 2020 2020 2020 2020 2020 2074 7261 636b             track
-000050a0: 6c65 745f 636f 756e 7420 3d20 7472 6163  let_count = trac
-000050b0: 6b6c 6574 5f63 6f75 6e74 202b 2031 202b  klet_count + 1 +
-000050c0: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 7472 6163 6b6c 6574 5f63 6f75      tracklet_cou
-000050f0: 6e74 203d 2073 656c 662e 5f75 6e69 7175  nt = self._uniqu
-00005100: 655f 7472 6163 6b6c 6574 5f63 6f75 6e74  e_tracklet_count
-00005110: 2874 7261 636b 6c65 745f 636f 756e 745f  (tracklet_count_
-00005120: 7461 6b65 6e2c 2074 7261 636b 6c65 745f  taken, tracklet_
-00005130: 636f 756e 7429 0d0a 2020 2020 2020 2020  count)..        
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00005160: 5f63 6f75 6e74 5f74 616b 656e 2e61 7070  _count_taken.app
-00005170: 656e 6428 7472 6163 6b6c 6574 5f63 6f75  end(tracklet_cou
-00005180: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
-000051b0: 7465 5f64 6976 6964 696e 675f 7265 6375  te_dividing_recu
-000051c0: 7273 6976 6528 726f 6f74 5f6c 6561 662c  rsive(root_leaf,
-000051d0: 2074 6172 6765 745f 6365 6c6c 2c20 736f   target_cell, so
-000051e0: 7274 6564 5f72 6f6f 745f 7370 6c69 7473  rted_root_splits
-000051f0: 2c20 6e65 7874 5f67 656e 5f63 6f75 6e74  , next_gen_count
-00005200: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-00005210: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
-00005220: 5f74 616b 656e 2920 2020 2020 200d 0a0d  _taken)      ...
-00005230: 0a0d 0a0d 0a20 2020 2064 6566 205f 6974  .....    def _it
-00005240: 6572 6174 655f 6469 7669 6469 6e67 2873  erate_dividing(s
-00005250: 656c 662c 2072 6f6f 745f 726f 6f74 2c20  elf, root_root, 
-00005260: 726f 6f74 5f6c 6561 662c 2072 6f6f 745f  root_leaf, root_
-00005270: 7370 6c69 7473 293a 0d0a 2020 2020 2020  splits):..      
-00005280: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005290: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000052a0: 2067 656e 5f63 6f75 6e74 203d 2030 0d0a   gen_count = 0..
-000052b0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-000052c0: 6b6c 6574 5f63 6f75 6e74 203d 2030 0d0a  klet_count = 0..
-000052d0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-000052e0: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
-000052f0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00005300: 2020 2066 6f72 2072 6f6f 745f 616c 6c20     for root_all 
-00005310: 696e 2072 6f6f 745f 726f 6f74 3a0d 0a20  in root_root:.. 
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2073 656c 662e 6765 6e65 7261 7469     self.generati
-00005340: 6f6e 5f64 6963 745b 726f 6f74 5f61 6c6c  on_dict[root_all
-00005350: 5d20 3d20 6765 6e5f 636f 756e 740d 0a20  ] = gen_count.. 
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2020 2073 656c 662e 7472 6163 6b6c 6574     self.tracklet
-00005380: 5f64 6963 745b 726f 6f74 5f61 6c6c 5d20  _dict[root_all] 
-00005390: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
-000053a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000053b0: 2020 2020 2020 7472 6163 6b6c 6574 5f63        tracklet_c
-000053c0: 6f75 6e74 5f74 616b 656e 2e61 7070 656e  ount_taken.appen
-000053d0: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
-000053e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000053f0: 2020 2020 2020 2069 6620 726f 6f74 5f61         if root_a
-00005400: 6c6c 2069 6e20 7365 6c66 2e65 6467 655f  ll in self.edge_
-00005410: 7461 7267 6574 5f6c 6f6f 6b75 7020 616e  target_lookup an
-00005420: 6420 726f 6f74 5f61 6c6c 206e 6f74 2069  d root_all not i
-00005430: 6e20 726f 6f74 5f73 706c 6974 733a 0d0a  n root_splits:..
+00005090: 2020 6966 206e 6578 745f 7461 7267 6574    if next_target
+000050a0: 5f63 656c 6c20 696e 2073 656c 662e 6564  _cell in self.ed
+000050b0: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
+000050c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000050d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000050e0: 6172 6765 745f 6365 6c6c 7320 3d20 7365  arget_cells = se
+000050f0: 6c66 2e65 6467 655f 7461 7267 6574 5f6c  lf.edge_target_l
+00005100: 6f6f 6b75 705b 6e65 7874 5f74 6172 6765  ookup[next_targe
+00005110: 745f 6365 6c6c 5d0d 0a20 2020 2020 2020  t_cell]..       
+00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2020 2020 2066 6f72 206b 2069 6e20 7261       for k in ra
+00005140: 6e67 6528 6c65 6e28 7461 7267 6574 5f63  nge(len(target_c
+00005150: 656c 6c73 2929 3a0d 0a20 2020 2020 2020  ells)):..       
+00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005170: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00005180: 6365 6c6c 203d 2074 6172 6765 745f 6365  cell = target_ce
+00005190: 6c6c 735b 6b5d 0d0a 2020 2020 2020 2020  lls[k]..        
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
+000051c0: 5f63 6f75 6e74 203d 2074 7261 636b 6c65  _count = trackle
+000051d0: 745f 636f 756e 7420 2b20 3120 2b20 6b0d  t_count + 1 + k.
+000051e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
+00005210: 3d20 7365 6c66 2e5f 756e 6971 7565 5f74  = self._unique_t
+00005220: 7261 636b 6c65 745f 636f 756e 7428 7472  racklet_count(tr
+00005230: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
+00005240: 656e 2c20 7472 6163 6b6c 6574 5f63 6f75  en, tracklet_cou
+00005250: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+00005280: 756e 745f 7461 6b65 6e2e 6170 7065 6e64  unt_taken.append
+00005290: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+000052a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+000052d0: 6469 7669 6469 6e67 5f72 6563 7572 7369  dividing_recursi
+000052e0: 7665 2872 6f6f 745f 6c65 6166 2c20 7461  ve(root_leaf, ta
+000052f0: 7267 6574 5f63 656c 6c2c 2073 6f72 7465  rget_cell, sorte
+00005300: 645f 726f 6f74 5f73 706c 6974 732c 206e  d_root_splits, n
+00005310: 6578 745f 6765 6e5f 636f 756e 742c 2074  ext_gen_count, t
+00005320: 7261 636b 6c65 745f 636f 756e 742c 2074  racklet_count, t
+00005330: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
+00005340: 6b65 6e29 2020 2020 2020 0d0a 0d0a 0d0a  ken)      ......
+00005350: 0d0a 2020 2020 6465 6620 5f69 7465 7261  ..    def _itera
+00005360: 7465 5f64 6976 6964 696e 6728 7365 6c66  te_dividing(self
+00005370: 2c20 726f 6f74 5f72 6f6f 742c 2072 6f6f  , root_root, roo
+00005380: 745f 6c65 6166 2c20 726f 6f74 5f73 706c  t_leaf, root_spl
+00005390: 6974 7329 3a0d 0a20 2020 2020 2020 2020  its):..         
+000053a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000053b0: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+000053c0: 6e5f 636f 756e 7420 3d20 300d 0a20 2020  n_count = 0..   
+000053d0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+000053e0: 745f 636f 756e 7420 3d20 300d 0a20 2020  t_count = 0..   
+000053f0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00005400: 745f 636f 756e 745f 7461 6b65 6e20 3d20  t_count_taken = 
+00005410: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00005420: 666f 7220 726f 6f74 5f61 6c6c 2069 6e20  for root_all in 
+00005430: 726f 6f74 5f72 6f6f 743a 0d0a 2020 2020  root_root:..    
 00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00005460: 6365 6c6c 203d 2073 656c 662e 6564 6765  cell = self.edge
-00005470: 5f74 6172 6765 745f 6c6f 6f6b 7570 5b72  _target_lookup[r
-00005480: 6f6f 745f 616c 6c5d 5b30 5d0d 0a20 2020  oot_all][0]..   
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 2020 2020 2020 7768 696c 6520 7461 7267        while targ
-000054b0: 6574 5f63 656c 6c20 6e6f 7420 696e 2072  et_cell not in r
-000054c0: 6f6f 745f 7370 6c69 7473 3a0d 0a20 2020  oot_splits:..   
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000054f0: 7461 7267 6574 5f63 656c 6c20 696e 2073  target_cell in s
-00005500: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-00005510: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
-00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005530: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005540: 662e 6765 6e65 7261 7469 6f6e 5f64 6963  f.generation_dic
-00005550: 745b 7461 7267 6574 5f63 656c 6c5d 203d  t[target_cell] =
-00005560: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
-000055a0: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-000055b0: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
-000055c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2020 2020 7472 6163 6b6c 6574 5f63        tracklet_c
-000055f0: 6f75 6e74 5f74 616b 656e 2e61 7070 656e  ount_taken.appen
-00005600: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
-00005610: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
-00005640: 6c6c 203d 2073 656c 662e 6564 6765 5f74  ll = self.edge_t
-00005650: 6172 6765 745f 6c6f 6f6b 7570 5b74 6172  arget_lookup[tar
-00005660: 6765 745f 6365 6c6c 5d5b 305d 0d0a 2020  get_cell][0]..  
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005690: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000056c0: 6765 6e65 7261 7469 6f6e 5f64 6963 745b  generation_dict[
-000056d0: 7461 7267 6574 5f63 656c 6c5d 203d 2067  target_cell] = g
-000056e0: 656e 5f63 6f75 6e74 0d0a 2020 2020 2020  en_count..      
+00005450: 7365 6c66 2e67 656e 6572 6174 696f 6e5f  self.generation_
+00005460: 6469 6374 5b72 6f6f 745f 616c 6c5d 203d  dict[root_all] =
+00005470: 2067 656e 5f63 6f75 6e74 0d0a 2020 2020   gen_count..    
+00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005490: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
+000054a0: 6374 5b72 6f6f 745f 616c 6c5d 203d 2074  ct[root_all] = t
+000054b0: 7261 636b 6c65 745f 636f 756e 740d 0a20  racklet_count.. 
+000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054d0: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
+000054e0: 745f 7461 6b65 6e2e 6170 7065 6e64 2874  t_taken.append(t
+000054f0: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 2020 2020 6966 2072 6f6f 745f 616c 6c20      if root_all 
+00005520: 696e 2073 656c 662e 6564 6765 5f74 6172  in self.edge_tar
+00005530: 6765 745f 6c6f 6f6b 7570 2061 6e64 2072  get_lookup and r
+00005540: 6f6f 745f 616c 6c20 6e6f 7420 696e 2072  oot_all not in r
+00005550: 6f6f 745f 7370 6c69 7473 3a0d 0a20 2020  oot_splits:..   
+00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005570: 2020 2020 2020 7461 7267 6574 5f63 656c        target_cel
+00005580: 6c20 3d20 7365 6c66 2e65 6467 655f 7461  l = self.edge_ta
+00005590: 7267 6574 5f6c 6f6f 6b75 705b 726f 6f74  rget_lookup[root
+000055a0: 5f61 6c6c 5d5b 305d 0d0a 2020 2020 2020  _all][0]..      
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 2077 6869 6c65 2074 6172 6765 745f     while target_
+000055d0: 6365 6c6c 206e 6f74 2069 6e20 726f 6f74  cell not in root
+000055e0: 5f73 706c 6974 733a 0d0a 2020 2020 2020  _splits:..      
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 2020 2020 2020 2020 2020 6966 2074 6172            if tar
+00005610: 6765 745f 6365 6c6c 2069 6e20 7365 6c66  get_cell in self
+00005620: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00005630: 6b75 703a 0d0a 2020 2020 2020 2020 2020  kup:..          
+00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005650: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00005660: 656e 6572 6174 696f 6e5f 6469 6374 5b74  eneration_dict[t
+00005670: 6172 6765 745f 6365 6c6c 5d20 3d20 6765  arget_cell] = ge
+00005680: 6e5f 636f 756e 740d 0a20 2020 2020 2020  n_count..       
+00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000056b0: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+000056c0: 7461 7267 6574 5f63 656c 6c5d 203d 2074  target_cell] = t
+000056d0: 7261 636b 6c65 745f 636f 756e 740d 0a20  racklet_count.. 
+000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 7365 6c66 2e74 7261 636b 6c65 745f 6469  self.tracklet_di
-00005720: 6374 5b74 6172 6765 745f 6365 6c6c 5d20  ct[target_cell] 
-00005730: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
-00005740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 7472 6163 6b6c 6574          tracklet
-00005770: 5f63 6f75 6e74 5f74 616b 656e 2e61 7070  _count_taken.app
-00005780: 656e 6428 7472 6163 6b6c 6574 5f63 6f75  end(tracklet_cou
-00005790: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000057c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000057d0: 2020 2020 2020 2023 5374 6172 7420 6f66         #Start of
-000057e0: 2074 7261 636b 2069 7320 6120 6469 7669   track is a divi
-000057f0: 6469 6e67 2063 656c 6c20 2020 2020 2020  ding cell       
-00005800: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005810: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00005820: 6f6f 745f 616c 6c20 696e 2073 656c 662e  oot_all in self.
-00005830: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00005840: 7570 2061 6e64 2072 6f6f 745f 616c 6c20  up and root_all 
-00005850: 696e 2072 6f6f 745f 7370 6c69 7473 3a0d  in root_splits:.
-00005860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005870: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005880: 5f63 656c 6c73 203d 2073 656c 662e 6564  _cells = self.ed
-00005890: 6765 5f74 6172 6765 745f 6c6f 6f6b 7570  ge_target_lookup
-000058a0: 5b72 6f6f 745f 616c 6c5d 0d0a 2020 2020  [root_all]..    
-000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058c0: 2020 2020 2067 656e 5f63 6f75 6e74 203d       gen_count =
-000058d0: 2067 656e 5f63 6f75 6e74 202b 2031 0d0a   gen_count + 1..
+00005700: 2020 2074 7261 636b 6c65 745f 636f 756e     tracklet_coun
+00005710: 745f 7461 6b65 6e2e 6170 7065 6e64 2874  t_taken.append(t
+00005720: 7261 636b 6c65 745f 636f 756e 7429 0d0a  racklet_count)..
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005750: 2020 2020 7461 7267 6574 5f63 656c 6c20      target_cell 
+00005760: 3d20 7365 6c66 2e65 6467 655f 7461 7267  = self.edge_targ
+00005770: 6574 5f6c 6f6f 6b75 705b 7461 7267 6574  et_lookup[target
+00005780: 5f63 656c 6c5d 5b30 5d0d 0a20 2020 2020  _cell][0]..     
+00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000057b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2020 2020 2020 2020 7365 6c66 2e67 656e          self.gen
+000057e0: 6572 6174 696f 6e5f 6469 6374 5b74 6172  eration_dict[tar
+000057f0: 6765 745f 6365 6c6c 5d20 3d20 6765 6e5f  get_cell] = gen_
+00005800: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005830: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+00005840: 7461 7267 6574 5f63 656c 6c5d 203d 2074  target_cell] = t
+00005850: 7261 636b 6c65 745f 636f 756e 740d 0a20  racklet_count.. 
+00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
+00005890: 756e 745f 7461 6b65 6e2e 6170 7065 6e64  unt_taken.append
+000058a0: 2874 7261 636b 6c65 745f 636f 756e 7429  (tracklet_count)
+000058b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058d0: 2020 2020 2020 2020 6272 6561 6b20 0d0a          break ..
 000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-00005900: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
-00005910: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005930: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00005940: 6765 745f 6365 6c6c 203d 2074 6172 6765  get_cell = targe
-00005950: 745f 6365 6c6c 735b 6a5d 0d0a 2020 2020  t_cells[j]..    
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00005980: 6b6c 6574 5f63 6f75 6e74 203d 2074 7261  klet_count = tra
-00005990: 636b 6c65 745f 636f 756e 7420 2b20 3120  cklet_count + 1 
-000059a0: 2b20 6a0d 0a20 2020 2020 2020 2020 2020  + j..           
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2074 7261 636b 6c65 745f 636f       tracklet_co
-000059d0: 756e 7420 3d20 7365 6c66 2e5f 756e 6971  unt = self._uniq
-000059e0: 7565 5f74 7261 636b 6c65 745f 636f 756e  ue_tracklet_coun
-000059f0: 7428 7472 6163 6b6c 6574 5f63 6f75 6e74  t(tracklet_count
-00005a00: 5f74 616b 656e 2c20 7472 6163 6b6c 6574  _taken, tracklet
-00005a10: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-00005a40: 745f 636f 756e 745f 7461 6b65 6e2e 6170  t_count_taken.ap
-00005a50: 7065 6e64 2874 7261 636b 6c65 745f 636f  pend(tracklet_co
-00005a60: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 7365 6c66 2e5f 6974 6572        self._iter
-00005a90: 6174 655f 6469 7669 6469 6e67 5f72 6563  ate_dividing_rec
-00005aa0: 7572 7369 7665 2872 6f6f 745f 6c65 6166  ursive(root_leaf
-00005ab0: 2c20 7461 7267 6574 5f63 656c 6c2c 2072  , target_cell, r
-00005ac0: 6f6f 745f 7370 6c69 7473 2c20 6765 6e5f  oot_splits, gen_
-00005ad0: 636f 756e 742c 2074 7261 636b 6c65 745f  count, tracklet_
-00005ae0: 636f 756e 742c 2074 7261 636b 6c65 745f  count, tracklet_
-00005af0: 636f 756e 745f 7461 6b65 6e29 0d0a 2020  count_taken)..  
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00005b50: 2020 2020 2020 2069 6620 6c65 6e28 726f         if len(ro
-00005b60: 6f74 5f73 706c 6974 7329 203e 2030 3a0d  ot_splits) > 0:.
-00005b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005b80: 2020 2020 2073 6f72 7465 645f 726f 6f74       sorted_root
-00005b90: 5f73 706c 6974 7320 3d20 7365 6c66 2e5f  _splits = self._
-00005ba0: 736f 7274 5f64 6976 6964 696e 675f 6365  sort_dividing_ce
-00005bb0: 6c6c 7328 726f 6f74 5f73 706c 6974 7329  lls(root_splits)
-00005bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005bd0: 2020 2020 2020 6669 7273 745f 7370 6c69        first_spli
-00005be0: 7420 3d20 736f 7274 6564 5f72 6f6f 745f  t = sorted_root_
-00005bf0: 7370 6c69 7473 5b30 5d0d 0a20 2020 2020  splits[0]..     
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005c10: 656c 662e 6765 6e65 7261 7469 6f6e 5f64  elf.generation_d
-00005c20: 6963 745b 6669 7273 745f 7370 6c69 745d  ict[first_split]
-00005c30: 203d 2067 656e 5f63 6f75 6e74 0d0a 2020   = gen_count..  
+000058f0: 2020 2020 2353 7461 7274 206f 6620 7472      #Start of tr
+00005900: 6163 6b20 6973 2061 2064 6976 6964 696e  ack is a dividin
+00005910: 6720 6365 6c6c 2020 2020 2020 2020 2020  g cell          
+00005920: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00005930: 2020 2020 2020 2020 2069 6620 726f 6f74           if root
+00005940: 5f61 6c6c 2069 6e20 7365 6c66 2e65 6467  _all in self.edg
+00005950: 655f 7461 7267 6574 5f6c 6f6f 6b75 7020  e_target_lookup 
+00005960: 616e 6420 726f 6f74 5f61 6c6c 2069 6e20  and root_all in 
+00005970: 726f 6f74 5f73 706c 6974 733a 0d0a 2020  root_splits:..  
+00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005990: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
+000059a0: 6c6c 7320 3d20 7365 6c66 2e65 6467 655f  lls = self.edge_
+000059b0: 7461 7267 6574 5f6c 6f6f 6b75 705b 726f  target_lookup[ro
+000059c0: 6f74 5f61 6c6c 5d0d 0a20 2020 2020 2020  ot_all]..       
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059e0: 2020 6765 6e5f 636f 756e 7420 3d20 6765    gen_count = ge
+000059f0: 6e5f 636f 756e 7420 2b20 310d 0a20 2020  n_count + 1..   
+00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+00005a20: 616e 6765 286c 656e 2874 6172 6765 745f  ange(len(target_
+00005a30: 6365 6c6c 7329 293a 0d0a 2020 2020 2020  cells)):..      
+00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a50: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00005a60: 5f63 656c 6c20 3d20 7461 7267 6574 5f63  _cell = target_c
+00005a70: 656c 6c73 5b6a 5d0d 0a20 2020 2020 2020  ells[j]..       
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00005aa0: 745f 636f 756e 7420 3d20 7472 6163 6b6c  t_count = trackl
+00005ab0: 6574 5f63 6f75 6e74 202b 2031 202b 206a  et_count + 1 + j
+00005ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ae0: 2020 7472 6163 6b6c 6574 5f63 6f75 6e74    tracklet_count
+00005af0: 203d 2073 656c 662e 5f75 6e69 7175 655f   = self._unique_
+00005b00: 7472 6163 6b6c 6574 5f63 6f75 6e74 2874  tracklet_count(t
+00005b10: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
+00005b20: 6b65 6e2c 2074 7261 636b 6c65 745f 636f  ken, tracklet_co
+00005b30: 756e 7429 0d0a 2020 2020 2020 2020 2020  unt)..          
+00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b50: 2020 2020 2020 7472 6163 6b6c 6574 5f63        tracklet_c
+00005b60: 6f75 6e74 5f74 616b 656e 2e61 7070 656e  ount_taken.appen
+00005b70: 6428 7472 6163 6b6c 6574 5f63 6f75 6e74  d(tracklet_count
+00005b80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
+00005bb0: 5f64 6976 6964 696e 675f 7265 6375 7273  _dividing_recurs
+00005bc0: 6976 6528 726f 6f74 5f6c 6561 662c 2074  ive(root_leaf, t
+00005bd0: 6172 6765 745f 6365 6c6c 2c20 726f 6f74  arget_cell, root
+00005be0: 5f73 706c 6974 732c 2067 656e 5f63 6f75  _splits, gen_cou
+00005bf0: 6e74 2c20 7472 6163 6b6c 6574 5f63 6f75  nt, tracklet_cou
+00005c00: 6e74 2c20 7472 6163 6b6c 6574 5f63 6f75  nt, tracklet_cou
+00005c10: 6e74 5f74 616b 656e 290d 0a20 2020 2020  nt_taken)..     
+00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c50: 2020 7365 6c66 2e74 7261 636b 6c65 745f    self.tracklet_
-00005c60: 6469 6374 5b66 6972 7374 5f73 706c 6974  dict[first_split
-00005c70: 5d20 3d20 7472 6163 6b6c 6574 5f63 6f75  ] = tracklet_cou
-00005c80: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-00005c90: 2020 2020 2020 2020 6966 2066 6972 7374          if first
-00005ca0: 5f73 706c 6974 2069 6e20 7365 6c66 2e65  _split in self.e
-00005cb0: 6467 655f 7461 7267 6574 5f6c 6f6f 6b75  dge_target_looku
-00005cc0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
-00005cd0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
-00005ce0: 6574 5f63 656c 6c73 203d 2073 656c 662e  et_cells = self.
-00005cf0: 6564 6765 5f74 6172 6765 745f 6c6f 6f6b  edge_target_look
-00005d00: 7570 5b66 6972 7374 5f73 706c 6974 5d0d  up[first_split].
-00005d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d20: 2020 2020 2020 2020 2067 656e 5f63 6f75           gen_cou
-00005d30: 6e74 203d 2067 656e 5f63 6f75 6e74 202b  nt = gen_count +
-00005d40: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00005d50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005d60: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
-00005d70: 6172 6765 745f 6365 6c6c 7329 293a 0d0a  arget_cells)):..
-00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d90: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-00005da0: 6b6c 6574 5f63 6f75 6e74 203d 2074 7261  klet_count = tra
-00005db0: 636b 6c65 745f 636f 756e 7420 2b20 3120  cklet_count + 1 
-00005dc0: 2b20 690d 0a20 2020 2020 2020 2020 2020  + i..           
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2074 7261 636b 6c65 745f 636f 756e 7420   tracklet_count 
-00005df0: 3d20 7365 6c66 2e5f 756e 6971 7565 5f74  = self._unique_t
-00005e00: 7261 636b 6c65 745f 636f 756e 7428 7472  racklet_count(tr
-00005e10: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
-00005e20: 656e 2c20 7472 6163 6b6c 6574 5f63 6f75  en, tracklet_cou
-00005e30: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2074 7261 636b 6c65 745f 636f 756e 745f   tracklet_count_
-00005e60: 7461 6b65 6e2e 6170 7065 6e64 2874 7261  taken.append(tra
-00005e70: 636b 6c65 745f 636f 756e 7429 0d0a 2020  cklet_count)..  
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00005ea0: 5f63 656c 6c20 3d20 7461 7267 6574 5f63  _cell = target_c
-00005eb0: 656c 6c73 5b69 5d0d 0a20 2020 2020 2020  ells[i]..       
-00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
-00005ee0: 7465 5f64 6976 6964 696e 675f 7265 6375  te_dividing_recu
-00005ef0: 7273 6976 6528 726f 6f74 5f6c 6561 662c  rsive(root_leaf,
-00005f00: 2074 6172 6765 745f 6365 6c6c 2c20 736f   target_cell, so
-00005f10: 7274 6564 5f72 6f6f 745f 7370 6c69 7473  rted_root_splits
-00005f20: 2c20 6765 6e5f 636f 756e 742c 2074 7261  , gen_count, tra
-00005f30: 636b 6c65 745f 636f 756e 742c 2074 7261  cklet_count, tra
-00005f40: 636b 6c65 745f 636f 756e 745f 7461 6b65  cklet_count_take
-00005f50: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-00005f60: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00005f70: 6620 5f75 6e69 7175 655f 7472 6163 6b6c  f _unique_trackl
-00005f80: 6574 5f63 6f75 6e74 2873 656c 662c 2074  et_count(self, t
-00005f90: 7261 636b 6c65 745f 636f 756e 745f 7461  racklet_count_ta
-00005fa0: 6b65 6e2c 2074 7261 636b 6c65 745f 636f  ken, tracklet_co
-00005fb0: 756e 7429 3a0d 0a20 2020 2020 2020 2020  unt):..         
-00005fc0: 2020 0d0a 2020 2020 2020 2020 2020 2077    ..           w
-00005fd0: 6869 6c65 2074 7261 636b 6c65 745f 636f  hile tracklet_co
-00005fe0: 756e 7420 696e 2074 7261 636b 6c65 745f  unt in tracklet_
-00005ff0: 636f 756e 745f 7461 6b65 6e3a 0d0a 2020  count_taken:..  
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 7472 6163 6b6c 6574 5f63 6f75 6e74 2020  tracklet_count  
-00006020: 3d20 7472 6163 6b6c 6574 5f63 6f75 6e74  = tracklet_count
-00006030: 202b 2031 200d 0a20 2020 2020 2020 2020   + 1 ..         
-00006040: 2020 2020 2020 2020 2073 656c 662e 5f75           self._u
-00006050: 6e69 7175 655f 7472 6163 6b6c 6574 5f63  nique_tracklet_c
-00006060: 6f75 6e74 2874 7261 636b 6c65 745f 636f  ount(tracklet_co
-00006070: 756e 745f 7461 6b65 6e2c 2074 7261 636b  unt_taken, track
-00006080: 6c65 745f 636f 756e 7429 0d0a 2020 2020  let_count)..    
-00006090: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-000060a0: 6163 6b6c 6574 5f63 6f75 6e74 2020 2020  acklet_count    
-000060b0: 2020 200d 0a0d 0a0d 0a20 2020 2064 6566     ......    def
-000060c0: 205f 6974 6572 6174 655f 7370 6c69 745f   _iterate_split_
-000060d0: 646f 776e 2873 656c 662c 2072 6f6f 745f  down(self, root_
-000060e0: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
-000060f0: 2072 6f6f 745f 7370 6c69 7473 293a 0d0a   root_splits):..
-00006100: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006110: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
-00006120: 5f64 6976 6964 696e 6728 726f 6f74 5f72  _dividing(root_r
-00006130: 6f6f 742c 2072 6f6f 745f 6c65 6166 2c20  oot, root_leaf, 
-00006140: 726f 6f74 5f73 706c 6974 7329 0d0a 2020  root_splits)..  
-00006150: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006160: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00006170: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006180: 0a20 2020 2064 6566 205f 6765 745f 626f  .    def _get_bo
-00006190: 756e 6461 7279 5f64 6973 7428 7365 6c66  undary_dist(self
-000061a0: 2c20 6672 616d 652c 2074 6573 746c 6f63  , frame, testloc
-000061b0: 6174 696f 6e29 3a0d 0a20 2020 2020 2020  ation):..       
-000061c0: 2020 0d0a 2020 2020 2020 2020 6966 2073    ..        if s
-000061d0: 656c 662e 6d61 736b 2069 7320 6e6f 7420  elf.mask is not 
-000061e0: 4e6f 6e65 3a0d 0a0d 0a20 2020 2020 2020  None:....       
-000061f0: 2020 2020 2020 2020 2074 7265 652c 2069           tree, i
-00006200: 6e64 6963 6573 2c20 6d61 736b 6365 6e74  ndices, maskcent
-00006210: 726f 6964 203d 2073 656c 662e 7469 6d65  roid = self.time
-00006220: 645f 6d61 736b 5b73 7472 2869 6e74 2866  d_mask[str(int(f
-00006230: 6c6f 6174 2866 7261 6d65 2929 295d 0d0a  loat(frame)))]..
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00006260: 2020 2020 2020 2020 2020 2320 4765 7420            # Get 
-00006270: 7468 6520 6c6f 6361 7469 6f6e 2061 6e64  the location and
-00006280: 2064 6973 7461 6e63 6520 746f 2074 6865   distance to the
-00006290: 206e 6561 7265 7374 2062 6f75 6e64 6172   nearest boundar
-000062a0: 7920 706f 696e 740d 0a20 2020 2020 2020  y point..       
-000062b0: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-000062c0: 655f 6365 6c6c 5f6d 6173 6b2c 206c 6f63  e_cell_mask, loc
-000062d0: 6174 696f 6e69 6e64 6578 203d 2074 7265  ationindex = tre
-000062e0: 652e 7175 6572 7928 7465 7374 6c6f 6361  e.query(testloca
-000062f0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00006300: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00006310: 6365 6c6c 5f6d 6173 6b20 3d20 6d61 7828  cell_mask = max(
-00006320: 302c 2064 6973 7461 6e63 655f 6365 6c6c  0, distance_cell
-00006330: 5f6d 6173 6b29 0d0a 2020 2020 2020 2020  _mask)..        
-00006340: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00006350: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00006360: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-00006370: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00006380: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-00006390: 2020 2020 6d61 736b 6365 6e74 726f 6964      maskcentroid
-000063a0: 203d 2028 312c 312c 3129 0d0a 0d0a 2020   = (1,1,1)....  
-000063b0: 2020 2020 2020 7265 7475 726e 2064 6973        return dis
-000063c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
-000063d0: 206d 6173 6b63 656e 7472 6f69 6420 2020   maskcentroid   
-000063e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000063f0: 0d0a 2020 2020 6465 6620 5f67 6c6f 6261  ..    def _globa
-00006400: 6c5f 7472 6163 6b5f 6964 2873 656c 662c  l_track_id(self,
-00006410: 2074 7261 636b 5f69 6429 3a0d 0a20 2020   track_id):..   
-00006420: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00006430: 2020 6e75 6d5f 6469 6769 7473 203d 206c    num_digits = l
-00006440: 656e 2873 7472 2873 656c 662e 6d61 785f  en(str(self.max_
-00006450: 7472 6163 6b5f 6469 6769 7429 290d 0a0d  track_digit))...
-00006460: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
-00006470: 645f 7374 7220 3d20 7374 7228 7472 6163  d_str = str(trac
-00006480: 6b5f 6964 290d 0a20 2020 2020 2020 2069  k_id)..        i
-00006490: 6620 6c65 6e28 7472 6163 6b5f 6964 5f73  f len(track_id_s
-000064a0: 7472 2920 3c20 6e75 6d5f 6469 6769 7473  tr) < num_digits
-000064b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000064c0: 7472 6163 6b5f 6964 5f73 7472 203d 2074  track_id_str = t
-000064d0: 7261 636b 5f69 645f 7374 722e 7a66 696c  rack_id_str.zfil
-000064e0: 6c28 6e75 6d5f 6469 6769 7473 290d 0a20  l(num_digits).. 
-000064f0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-00006500: 3d20 696e 7428 7472 6163 6b5f 6964 5f73  = int(track_id_s
-00006510: 7472 290d 0a20 2020 2020 2020 2072 6574  tr)..        ret
-00006520: 7572 6e20 7472 6163 6b5f 6964 0d0a 2020  urn track_id..  
-00006530: 2020 0d0a 2020 2020 6465 6620 5f67 6c6f    ..    def _glo
-00006540: 6261 6c5f 6765 6e65 7261 7469 6f6e 5f69  bal_generation_i
-00006550: 6428 7365 6c66 2c20 6765 6e65 7261 7469  d(self, generati
-00006560: 6f6e 5f69 6429 3a0d 0a20 2020 2020 2020  on_id):..       
-00006570: 200d 0a20 2020 2020 2020 206e 756d 5f64   ..        num_d
-00006580: 6967 6974 7320 3d20 6c65 6e28 7374 7228  igits = len(str(
-00006590: 7365 6c66 2e6d 6178 5f74 7261 636b 5f64  self.max_track_d
-000065a0: 6967 6974 2929 0d0a 2020 2020 2020 2020  igit))..        
-000065b0: 6765 6e65 7261 7469 6f6e 5f69 645f 7374  generation_id_st
-000065c0: 7220 3d20 7374 7228 6765 6e65 7261 7469  r = str(generati
-000065d0: 6f6e 5f69 6429 0d0a 2020 2020 2020 2020  on_id)..        
-000065e0: 6966 206c 656e 2867 656e 6572 6174 696f  if len(generatio
-000065f0: 6e5f 6964 5f73 7472 2920 3c20 6e75 6d5f  n_id_str) < num_
-00006600: 6469 6769 7473 3a0d 0a20 2020 2020 2020  digits:..       
-00006610: 2020 2020 2020 2020 2067 656e 6572 6174           generat
-00006620: 696f 6e5f 6964 5f73 7472 203d 2067 656e  ion_id_str = gen
-00006630: 6572 6174 696f 6e5f 6964 5f73 7472 2e7a  eration_id_str.z
-00006640: 6669 6c6c 286e 756d 5f64 6967 6974 7329  fill(num_digits)
-00006650: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
-00006660: 7469 6f6e 5f69 6420 3d20 696e 7428 6765  tion_id = int(ge
-00006670: 6e65 7261 7469 6f6e 5f69 645f 7374 7229  neration_id_str)
-00006680: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00006690: 726e 2067 656e 6572 6174 696f 6e5f 6964  rn generation_id
-000066a0: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f74  ......    def _t
-000066b0: 7261 636b 5f63 6f6d 7075 7465 7228 7365  rack_computer(se
-000066c0: 6c66 2c20 7472 6163 6b2c 2074 7261 636b  lf, track, track
-000066d0: 5f69 6429 3a0d 0a20 2020 2020 2020 2020  _id):..         
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006730: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00006740: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006760: 2020 2075 6e69 7175 655f 7472 6163 6b6c     unique_trackl
-00006770: 6574 5f69 6473 203d 205b 5d0d 0a20 2020  et_ids = []..   
-00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 2020 2020 2020 2061 6c6c 5f73 6f75           all_sou
-000067a0: 7263 655f 6964 732c 2061 6c6c 5f74 6172  rce_ids, all_tar
-000067b0: 6765 745f 6964 7320 3d20 2073 656c 662e  get_ids =  self.
-000067c0: 5f67 656e 6572 6174 655f 6765 6e65 7261  _generate_genera
-000067d0: 7469 6f6e 7328 7472 6163 6b29 0d0a 2020  tions(track)..  
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 2020 2020 2020 2020 726f 6f74 5f72            root_r
-00006800: 6f6f 742c 2072 6f6f 745f 7370 6c69 7473  oot, root_splits
-00006810: 2c20 726f 6f74 5f6c 6561 6620 3d20 7365  , root_leaf = se
-00006820: 6c66 2e5f 6372 6561 7465 5f67 656e 6572  lf._create_gener
-00006830: 6174 696f 6e73 2861 6c6c 5f73 6f75 7263  ations(all_sourc
-00006840: 655f 6964 7329 200d 0a20 2020 2020 2020  e_ids) ..       
-00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
-00006870: 7465 5f73 706c 6974 5f64 6f77 6e28 726f  te_split_down(ro
-00006880: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-00006890: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-000068a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000068b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 2020 2020 2020 2020 206e 756d 6265             numbe
-000068e0: 725f 6469 7669 6469 6e67 203d 206c 656e  r_dividing = len
-000068f0: 2872 6f6f 745f 7370 6c69 7473 290d 0a20  (root_splits).. 
+00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005c70: 2020 2020 6966 206c 656e 2872 6f6f 745f      if len(root_
+00005c80: 7370 6c69 7473 2920 3e20 303a 0d0a 2020  splits) > 0:..  
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ca0: 2020 736f 7274 6564 5f72 6f6f 745f 7370    sorted_root_sp
+00005cb0: 6c69 7473 203d 2073 656c 662e 5f73 6f72  lits = self._sor
+00005cc0: 745f 6469 7669 6469 6e67 5f63 656c 6c73  t_dividing_cells
+00005cd0: 2872 6f6f 745f 7370 6c69 7473 290d 0a20  (root_splits).. 
+00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cf0: 2020 2066 6972 7374 5f73 706c 6974 203d     first_split =
+00005d00: 2073 6f72 7465 645f 726f 6f74 5f73 706c   sorted_root_spl
+00005d10: 6974 735b 305d 0d0a 2020 2020 2020 2020  its[0]..        
+00005d20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005d30: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
+00005d40: 5b66 6972 7374 5f73 706c 6974 5d20 3d20  [first_split] = 
+00005d50: 6765 6e5f 636f 756e 740d 0a20 2020 2020  gen_count..     
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005d70: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
+00005d80: 745b 6669 7273 745f 7370 6c69 745d 203d  t[first_split] =
+00005d90: 2074 7261 636b 6c65 745f 636f 756e 740d   tracklet_count.
+00005da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005db0: 2020 2020 2069 6620 6669 7273 745f 7370       if first_sp
+00005dc0: 6c69 7420 696e 2073 656c 662e 6564 6765  lit in self.edge
+00005dd0: 5f74 6172 6765 745f 6c6f 6f6b 7570 3a0d  _target_lookup:.
+00005de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005df0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00005e00: 6365 6c6c 7320 3d20 7365 6c66 2e65 6467  cells = self.edg
+00005e10: 655f 7461 7267 6574 5f6c 6f6f 6b75 705b  e_target_lookup[
+00005e20: 6669 7273 745f 7370 6c69 745d 0d0a 2020  first_split]..  
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 2020 2020 6765 6e5f 636f 756e 7420        gen_count 
+00005e50: 3d20 6765 6e5f 636f 756e 7420 2b20 310d  = gen_count + 1.
+00005e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005e70: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00005e80: 6e20 7261 6e67 6528 6c65 6e28 7461 7267  n range(len(targ
+00005e90: 6574 5f63 656c 6c73 2929 3a0d 0a20 2020  et_cells)):..   
+00005ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005eb0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
+00005ec0: 745f 636f 756e 7420 3d20 7472 6163 6b6c  t_count = trackl
+00005ed0: 6574 5f63 6f75 6e74 202b 2031 202b 2069  et_count + 1 + i
+00005ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00005f00: 6163 6b6c 6574 5f63 6f75 6e74 203d 2073  acklet_count = s
+00005f10: 656c 662e 5f75 6e69 7175 655f 7472 6163  elf._unique_trac
+00005f20: 6b6c 6574 5f63 6f75 6e74 2874 7261 636b  klet_count(track
+00005f30: 6c65 745f 636f 756e 745f 7461 6b65 6e2c  let_count_taken,
+00005f40: 2074 7261 636b 6c65 745f 636f 756e 7429   tracklet_count)
+00005f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f60: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00005f70: 6163 6b6c 6574 5f63 6f75 6e74 5f74 616b  acklet_count_tak
+00005f80: 656e 2e61 7070 656e 6428 7472 6163 6b6c  en.append(trackl
+00005f90: 6574 5f63 6f75 6e74 290d 0a20 2020 2020  et_count)..     
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 2020 2074 6172 6765 745f 6365         target_ce
+00005fc0: 6c6c 203d 2074 6172 6765 745f 6365 6c6c  ll = target_cell
+00005fd0: 735b 695d 0d0a 2020 2020 2020 2020 2020  s[i]..          
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ff0: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+00006000: 6469 7669 6469 6e67 5f72 6563 7572 7369  dividing_recursi
+00006010: 7665 2872 6f6f 745f 6c65 6166 2c20 7461  ve(root_leaf, ta
+00006020: 7267 6574 5f63 656c 6c2c 2073 6f72 7465  rget_cell, sorte
+00006030: 645f 726f 6f74 5f73 706c 6974 732c 2067  d_root_splits, g
+00006040: 656e 5f63 6f75 6e74 2c20 7472 6163 6b6c  en_count, trackl
+00006050: 6574 5f63 6f75 6e74 2c20 7472 6163 6b6c  et_count, trackl
+00006060: 6574 5f63 6f75 6e74 5f74 616b 656e 290d  et_count_taken).
+00006070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006080: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+00006090: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+000060a0: 636f 756e 7428 7365 6c66 2c20 7472 6163  count(self, trac
+000060b0: 6b6c 6574 5f63 6f75 6e74 5f74 616b 656e  klet_count_taken
+000060c0: 2c20 7472 6163 6b6c 6574 5f63 6f75 6e74  , tracklet_count
+000060d0: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
+000060e0: 0a20 2020 2020 2020 2020 2020 7768 696c  .           whil
+000060f0: 6520 7472 6163 6b6c 6574 5f63 6f75 6e74  e tracklet_count
+00006100: 2069 6e20 7472 6163 6b6c 6574 5f63 6f75   in tracklet_cou
+00006110: 6e74 5f74 616b 656e 3a0d 0a20 2020 2020  nt_taken:..     
+00006120: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+00006130: 636b 6c65 745f 636f 756e 7420 203d 2074  cklet_count  = t
+00006140: 7261 636b 6c65 745f 636f 756e 7420 2b20  racklet_count + 
+00006150: 3120 0d0a 2020 2020 2020 2020 2020 2020  1 ..            
+00006160: 2020 2020 2020 7365 6c66 2e5f 756e 6971        self._uniq
+00006170: 7565 5f74 7261 636b 6c65 745f 636f 756e  ue_tracklet_coun
+00006180: 7428 7472 6163 6b6c 6574 5f63 6f75 6e74  t(tracklet_count
+00006190: 5f74 616b 656e 2c20 7472 6163 6b6c 6574  _taken, tracklet
+000061a0: 5f63 6f75 6e74 290d 0a20 2020 2020 2020  _count)..       
+000061b0: 2020 2020 7265 7475 726e 2074 7261 636b      return track
+000061c0: 6c65 745f 636f 756e 7420 2020 2020 2020  let_count       
+000061d0: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f69  ......    def _i
+000061e0: 7465 7261 7465 5f73 706c 6974 5f64 6f77  terate_split_dow
+000061f0: 6e28 7365 6c66 2c20 726f 6f74 5f72 6f6f  n(self, root_roo
+00006200: 742c 2072 6f6f 745f 6c65 6166 2c20 726f  t, root_leaf, ro
+00006210: 6f74 5f73 706c 6974 7329 3a0d 0a20 2020  ot_splits):..   
+00006220: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00006230: 7365 6c66 2e5f 6974 6572 6174 655f 6469  self._iterate_di
+00006240: 7669 6469 6e67 2872 6f6f 745f 726f 6f74  viding(root_root
+00006250: 2c20 726f 6f74 5f6c 6561 662c 2072 6f6f  , root_leaf, roo
+00006260: 745f 7370 6c69 7473 290d 0a20 2020 2020  t_splits)..     
+00006270: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006290: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000062a0: 2020 6465 6620 5f67 6574 5f62 6f75 6e64    def _get_bound
+000062b0: 6172 795f 6469 7374 2873 656c 662c 2066  ary_dist(self, f
+000062c0: 7261 6d65 2c20 7465 7374 6c6f 6361 7469  rame, testlocati
+000062d0: 6f6e 293a 0d0a 2020 2020 2020 2020 200d  on):..         .
+000062e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000062f0: 2e6d 6173 6b20 6973 206e 6f74 204e 6f6e  .mask is not Non
+00006300: 653a 0d0a 0d0a 2020 2020 2020 2020 2020  e:....          
+00006310: 2020 2020 2020 7472 6565 2c20 696e 6469        tree, indi
+00006320: 6365 732c 206d 6173 6b63 656e 7472 6f69  ces, maskcentroi
+00006330: 6420 3d20 7365 6c66 2e74 696d 6564 5f6d  d = self.timed_m
+00006340: 6173 6b5b 7374 7228 696e 7428 666c 6f61  ask[str(int(floa
+00006350: 7428 6672 616d 6529 2929 5d0d 0a20 2020  t(frame)))]..   
+00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006370: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006380: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
+00006390: 206c 6f63 6174 696f 6e20 616e 6420 6469   location and di
+000063a0: 7374 616e 6365 2074 6f20 7468 6520 6e65  stance to the ne
+000063b0: 6172 6573 7420 626f 756e 6461 7279 2070  arest boundary p
+000063c0: 6f69 6e74 0d0a 2020 2020 2020 2020 2020  oint..          
+000063d0: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
+000063e0: 656c 6c5f 6d61 736b 2c20 6c6f 6361 7469  ell_mask, locati
+000063f0: 6f6e 696e 6465 7820 3d20 7472 6565 2e71  onindex = tree.q
+00006400: 7565 7279 2874 6573 746c 6f63 6174 696f  uery(testlocatio
+00006410: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+00006420: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+00006430: 6c5f 6d61 736b 203d 206d 6178 2830 2c20  l_mask = max(0, 
+00006440: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00006450: 736b 290d 0a20 2020 2020 2020 2020 2020  sk)..           
+00006460: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00006470: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00006480: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+00006490: 655f 6365 6c6c 5f6d 6173 6b20 3d20 300d  e_cell_mask = 0.
+000064a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064b0: 206d 6173 6b63 656e 7472 6f69 6420 3d20   maskcentroid = 
+000064c0: 2831 2c31 2c31 290d 0a0d 0a20 2020 2020  (1,1,1)....     
+000064d0: 2020 2072 6574 7572 6e20 6469 7374 616e     return distan
+000064e0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
+000064f0: 736b 6365 6e74 726f 6964 2020 2020 2020  skcentroid      
+00006500: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
+00006510: 2020 2064 6566 205f 676c 6f62 616c 5f74     def _global_t
+00006520: 7261 636b 5f69 6428 7365 6c66 2c20 7472  rack_id(self, tr
+00006530: 6163 6b5f 6964 293a 0d0a 2020 2020 2020  ack_id):..      
+00006540: 2020 2020 200d 0a20 2020 2020 2020 206e       ..        n
+00006550: 756d 5f64 6967 6974 7320 3d20 6c65 6e28  um_digits = len(
+00006560: 7374 7228 7365 6c66 2e6d 6178 5f74 7261  str(self.max_tra
+00006570: 636b 5f64 6967 6974 2929 0d0a 0d0a 2020  ck_digit))....  
+00006580: 2020 2020 2020 7472 6163 6b5f 6964 5f73        track_id_s
+00006590: 7472 203d 2073 7472 2874 7261 636b 5f69  tr = str(track_i
+000065a0: 6429 0d0a 2020 2020 2020 2020 6966 206c  d)..        if l
+000065b0: 656e 2874 7261 636b 5f69 645f 7374 7229  en(track_id_str)
+000065c0: 203c 206e 756d 5f64 6967 6974 733a 0d0a   < num_digits:..
+000065d0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+000065e0: 636b 5f69 645f 7374 7220 3d20 7472 6163  ck_id_str = trac
+000065f0: 6b5f 6964 5f73 7472 2e7a 6669 6c6c 286e  k_id_str.zfill(n
+00006600: 756d 5f64 6967 6974 7329 0d0a 2020 2020  um_digits)..    
+00006610: 2020 2020 7472 6163 6b5f 6964 203d 2069      track_id = i
+00006620: 6e74 2874 7261 636b 5f69 645f 7374 7229  nt(track_id_str)
+00006630: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00006640: 2074 7261 636b 5f69 640d 0a20 2020 200d   track_id..    .
+00006650: 0a20 2020 2064 6566 205f 676c 6f62 616c  .    def _global
+00006660: 5f67 656e 6572 6174 696f 6e5f 6964 2873  _generation_id(s
+00006670: 656c 662c 2067 656e 6572 6174 696f 6e5f  elf, generation_
+00006680: 6964 293a 0d0a 2020 2020 2020 2020 0d0a  id):..        ..
+00006690: 2020 2020 2020 2020 6e75 6d5f 6469 6769          num_digi
+000066a0: 7473 203d 206c 656e 2873 7472 2873 656c  ts = len(str(sel
+000066b0: 662e 6d61 785f 7472 6163 6b5f 6469 6769  f.max_track_digi
+000066c0: 7429 290d 0a20 2020 2020 2020 2067 656e  t))..        gen
+000066d0: 6572 6174 696f 6e5f 6964 5f73 7472 203d  eration_id_str =
+000066e0: 2073 7472 2867 656e 6572 6174 696f 6e5f   str(generation_
+000066f0: 6964 290d 0a20 2020 2020 2020 2069 6620  id)..        if 
+00006700: 6c65 6e28 6765 6e65 7261 7469 6f6e 5f69  len(generation_i
+00006710: 645f 7374 7229 203c 206e 756d 5f64 6967  d_str) < num_dig
+00006720: 6974 733a 0d0a 2020 2020 2020 2020 2020  its:..          
+00006730: 2020 2020 2020 6765 6e65 7261 7469 6f6e        generation
+00006740: 5f69 645f 7374 7220 3d20 6765 6e65 7261  _id_str = genera
+00006750: 7469 6f6e 5f69 645f 7374 722e 7a66 696c  tion_id_str.zfil
+00006760: 6c28 6e75 6d5f 6469 6769 7473 290d 0a20  l(num_digits).. 
+00006770: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
+00006780: 6e5f 6964 203d 2069 6e74 2867 656e 6572  n_id = int(gener
+00006790: 6174 696f 6e5f 6964 5f73 7472 290d 0a0d  ation_id_str)...
+000067a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000067b0: 6765 6e65 7261 7469 6f6e 5f69 640d 0a0d  generation_id...
+000067c0: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
+000067d0: 6b5f 636f 6d70 7574 6572 2873 656c 662c  k_computer(self,
+000067e0: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+000067f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006810: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00006820: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006840: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00006850: 7265 6e74 5f63 656c 6c5f 6964 7320 3d20  rent_cell_ids = 
+00006860: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006880: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+00006890: 6964 7320 3d20 5b5d 0d0a 2020 2020 2020  ids = []..      
+000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068b0: 2020 2020 2020 616c 6c5f 736f 7572 6365        all_source
+000068c0: 5f69 6473 2c20 616c 6c5f 7461 7267 6574  _ids, all_target
+000068d0: 5f69 6473 203d 2020 7365 6c66 2e5f 6765  _ids =  self._ge
+000068e0: 6e65 7261 7465 5f67 656e 6572 6174 696f  nerate_generatio
+000068f0: 6e73 2874 7261 636b 290d 0a20 2020 2020  ns(track)..     
 00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006910: 2020 2020 2020 2020 2020 2023 2044 6574             # Det
-00006920: 6572 6d69 6e65 2069 6620 6120 7472 6163  ermine if a trac
-00006930: 6b20 6861 7320 6469 7669 7369 6f6e 7320  k has divisions 
-00006940: 6f72 206e 6f6e 650d 0a20 2020 2020 2020  or none..       
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2069 6620 6c65 6e28 726f 6f74       if len(root
-00006970: 5f73 706c 6974 7329 203e 2030 3a0d 0a20  _splits) > 0:.. 
-00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000069a0: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-000069b0: 5f6d 6974 6f73 6973 5f6c 6162 656c 5b74  _mitosis_label[t
-000069c0: 7261 636b 5f69 645d 203d 205b 312c 206e  rack_id] = [1, n
-000069d0: 756d 6265 725f 6469 7669 6469 6e67 5d0d  umber_dividing].
-000069e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a00: 2064 6976 6964 696e 675f 7472 616a 6563   dividing_trajec
-00006a10: 746f 7279 203d 2054 7275 650d 0a20 2020  tory = True..   
+00006910: 2020 2020 2020 2072 6f6f 745f 726f 6f74         root_root
+00006920: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+00006930: 6f6f 745f 6c65 6166 203d 2073 656c 662e  oot_leaf = self.
+00006940: 5f63 7265 6174 655f 6765 6e65 7261 7469  _create_generati
+00006950: 6f6e 7328 616c 6c5f 736f 7572 6365 5f69  ons(all_source_i
+00006960: 6473 2920 0d0a 2020 2020 2020 2020 2020  ds) ..          
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+00006990: 7370 6c69 745f 646f 776e 2872 6f6f 745f  split_down(root_
+000069a0: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
+000069b0: 2072 6f6f 745f 7370 6c69 7473 290d 0a20   root_splits).. 
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069f0: 2020 2020 2020 2020 6e75 6d62 6572 5f64          number_d
+00006a00: 6976 6964 696e 6720 3d20 6c65 6e28 726f  ividing = len(ro
+00006a10: 6f74 5f73 706c 6974 7329 0d0a 2020 2020  ot_splits)..    
 00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006a40: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
-00006a50: 7420 696e 2073 656c 662e 416c 6c54 7261  t in self.AllTra
-00006a60: 636b 4964 733a 0d0a 2020 2020 2020 2020  ckIds:..        
+00006a30: 2020 2020 2020 2020 2320 4465 7465 726d          # Determ
+00006a40: 696e 6520 6966 2061 2074 7261 636b 2068  ine if a track h
+00006a50: 6173 2064 6976 6973 696f 6e73 206f 7220  as divisions or 
+00006a60: 6e6f 6e65 0d0a 2020 2020 2020 2020 2020  none..          
 00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006a90: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
-00006aa0: 656e 6428 696e 7428 7472 6163 6b5f 6964  end(int(track_id
-00006ab0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 6966 2069 6e74 2874 7261 636b      if int(track
-00006ae0: 5f69 6429 206e 6f74 2069 6e20 7365 6c66  _id) not in self
-00006af0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-00006b00: 733a 2020 2020 200d 0a20 2020 2020 2020  s:     ..       
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00006b30: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-00006b40: 6473 2e61 7070 656e 6428 696e 7428 7472  ds.append(int(tr
-00006b50: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00006a80: 2020 6966 206c 656e 2872 6f6f 745f 7370    if len(root_sp
+00006a90: 6c69 7473 2920 3e20 303a 0d0a 2020 2020  lits) > 0:..    
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006ac0: 2e75 6e69 7175 655f 7472 6163 6b5f 6d69  .unique_track_mi
+00006ad0: 746f 7369 735f 6c61 6265 6c5b 7472 6163  tosis_label[trac
+00006ae0: 6b5f 6964 5d20 3d20 5b31 2c20 6e75 6d62  k_id] = [1, numb
+00006af0: 6572 5f64 6976 6964 696e 675d 0d0a 2020  er_dividing]..  
+00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b10: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00006b20: 7669 6469 6e67 5f74 7261 6a65 6374 6f72  viding_trajector
+00006b30: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
+00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b50: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
+00006b60: 2874 7261 636b 5f69 6429 206e 6f74 2069  (track_id) not i
+00006b70: 6e20 7365 6c66 2e41 6c6c 5472 6163 6b49  n self.AllTrackI
+00006b80: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
 00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00006bd0: 7565 5f74 7261 636b 5f6d 6974 6f73 6973  ue_track_mitosis
-00006be0: 5f6c 6162 656c 5b74 7261 636b 5f69 645d  _label[track_id]
-00006bf0: 203d 205b 302c 2030 5d0d 0a20 2020 2020   = [0, 0]..     
-00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c10: 2020 2020 2020 2020 2020 2064 6976 6964             divid
-00006c20: 696e 675f 7472 616a 6563 746f 7279 203d  ing_trajectory =
-00006c30: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
-00006c60: 7261 636b 5f69 6429 206e 6f74 2069 6e20  rack_id) not in 
-00006c70: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-00006c80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-00006cb0: 7261 636b 4964 732e 6170 7065 6e64 2869  rackIds.append(i
-00006cc0: 6e74 2874 7261 636b 5f69 6429 290d 0a20  nt(track_id)).. 
+00006ba0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+00006bb0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+00006bc0: 2869 6e74 2874 7261 636b 5f69 6429 290d  (int(track_id)).
+00006bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bf0: 2069 6620 696e 7428 7472 6163 6b5f 6964   if int(track_id
+00006c00: 2920 6e6f 7420 696e 2073 656c 662e 4469  ) not in self.Di
+00006c10: 7669 6469 6e67 5472 6163 6b49 6473 3a20  vidingTrackIds: 
+00006c20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+00006c50: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
+00006c60: 6170 7065 6e64 2869 6e74 2874 7261 636b  append(int(track
+00006c70: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00006ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006cb0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00006cc0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
 00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006cf0: 6620 696e 7428 7472 6163 6b5f 6964 2920  f int(track_id) 
-00006d00: 6e6f 7420 696e 2073 656c 662e 4e6f 726d  not in self.Norm
-00006d10: 616c 5472 6163 6b49 6473 3a20 2020 200d  alTrackIds:    .
-00006d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-00006d50: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-00006d60: 696e 7428 7472 6163 6b5f 6964 2929 0d0a  int(track_id))..
-00006d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006d80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00006d90: 7220 6c65 6166 2069 6e20 726f 6f74 5f6c  r leaf in root_l
-00006da0: 6561 663a 0d0a 2020 2020 2020 2020 2020  eaf:..          
+00006ce0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00006cf0: 7472 6163 6b5f 6d69 746f 7369 735f 6c61  track_mitosis_la
+00006d00: 6265 6c5b 7472 6163 6b5f 6964 5d20 3d20  bel[track_id] = 
+00006d10: 5b30 2c20 305d 0d0a 2020 2020 2020 2020  [0, 0]..        
+00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d30: 2020 2020 2020 2020 6469 7669 6469 6e67          dividing
+00006d40: 5f74 7261 6a65 6374 6f72 7920 3d20 4661  _trajectory = Fa
+00006d50: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
+00006d80: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
+00006d90: 662e 416c 6c54 7261 636b 4964 733a 0d0a  f.AllTrackIds:..
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
-00006dd0: 6c65 6166 203d 2073 656c 662e 6564 6765  leaf = self.edge
-00006de0: 5f73 6f75 7263 655f 6c6f 6f6b 7570 5b6c  _source_lookup[l
-00006df0: 6561 665d 0d0a 2020 2020 2020 2020 2020  eaf]..          
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00006e20: 5f63 656c 6c5f 6964 732e 6170 7065 6e64  _cell_ids.append
-00006e30: 286c 6561 6629 200d 0a20 2020 2020 2020  (leaf) ..       
+00006dc0: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+00006dd0: 6b49 6473 2e61 7070 656e 6428 696e 7428  kIds.append(int(
+00006de0: 7472 6163 6b5f 6964 2929 0d0a 2020 2020  track_id))..    
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00006e10: 6e74 2874 7261 636b 5f69 6429 206e 6f74  nt(track_id) not
+00006e20: 2069 6e20 7365 6c66 2e4e 6f72 6d61 6c54   in self.NormalT
+00006e30: 7261 636b 4964 733a 2020 2020 0d0a 2020  rackIds:    ..  
 00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006e60: 2e5f 6469 6374 5f75 7064 6174 6528 756e  ._dict_update(un
-00006e70: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
-00006e80: 732c 206c 6561 662c 2074 7261 636b 5f69  s, leaf, track_i
-00006e90: 642c 2073 6f75 7263 655f 6c65 6166 2c20  d, source_leaf, 
-00006ea0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00006ed0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00006ee0: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
-00006ef0: 7465 287b 7365 6c66 2e64 6976 6964 696e  te({self.dividin
-00006f00: 675f 6b65 7920 3a20 6469 7669 6469 6e67  g_key : dividing
-00006f10: 5f74 7261 6a65 6374 6f72 797d 290d 0a20  _trajectory}).. 
+00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e60: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
+00006e70: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+00006e80: 2874 7261 636b 5f69 6429 290d 0a0d 0a20  (track_id)).... 
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+00006eb0: 6561 6620 696e 2072 6f6f 745f 6c65 6166  eaf in root_leaf
+00006ec0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ee0: 2020 2020 2020 736f 7572 6365 5f6c 6561        source_lea
+00006ef0: 6620 3d20 7365 6c66 2e65 6467 655f 736f  f = self.edge_so
+00006f00: 7572 6365 5f6c 6f6f 6b75 705b 6c65 6166  urce_lookup[leaf
+00006f10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00006f50: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
-00006f60: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
-00006f70: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
-00006f80: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
-00006f90: 7669 6469 6e67 7d29 0d0a 0d0a 2020 2020  viding})....    
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2020 2020 2020 2020 666f 7220 736f 7572          for sour
-00006fc0: 6365 5f69 6420 696e 2061 6c6c 5f73 6f75  ce_id in all_sou
-00006fd0: 7263 655f 6964 733a 0d0a 2020 2020 2020  rce_ids:..      
-00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 7461 7267 6574 5f69 6473 203d 2073    target_ids = s
-00007010: 656c 662e 6564 6765 5f74 6172 6765 745f  elf.edge_target_
-00007020: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
-00007030: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00006f30: 2020 2020 2020 6375 7272 656e 745f 6365        current_ce
+00006f40: 6c6c 5f69 6473 2e61 7070 656e 6428 6c65  ll_ids.append(le
+00006f50: 6166 2920 0d0a 2020 2020 2020 2020 2020  af) ..          
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
+00006f80: 6963 745f 7570 6461 7465 2875 6e69 7175  ict_update(uniqu
+00006f90: 655f 7472 6163 6b6c 6574 5f69 6473 2c20  e_tracklet_ids, 
+00006fa0: 6c65 6166 2c20 7472 6163 6b5f 6964 2c20  leaf, track_id, 
+00006fb0: 736f 7572 6365 5f6c 6561 662c 204e 6f6e  source_leaf, Non
+00006fc0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fe0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00006ff0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00007000: 6573 5b6c 6561 665d 2e75 7064 6174 6528  es[leaf].update(
+00007010: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
+00007020: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
+00007030: 616a 6563 746f 7279 7d29 0d0a 2020 2020  ajectory})..    
 00007040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007050: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00007060: 6e74 5f63 656c 6c5f 6964 732e 6170 7065  nt_cell_ids.appe
-00007070: 6e64 2873 6f75 7263 655f 6964 290d 0a20  nd(source_id).. 
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070a0: 2020 2020 2020 2023 526f 6f74 0d0a 2020         #Root..  
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007050: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007060: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00007070: 7072 6f70 6572 7469 6573 5b6c 6561 665d  properties[leaf]
+00007080: 2e75 7064 6174 6528 7b73 656c 662e 6e75  .update({self.nu
+00007090: 6d62 6572 5f64 6976 6964 696e 675f 6b65  mber_dividing_ke
+000070a0: 7920 3a20 6e75 6d62 6572 5f64 6976 6964  y : number_divid
+000070b0: 696e 677d 290d 0a0d 0a20 2020 2020 2020  ing})....       
 000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000070e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000070f0: 735b 736f 7572 6365 5f69 645d 2e75 7064  s[source_id].upd
-00007100: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00007110: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00007120: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00007160: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00007170: 6965 735b 736f 7572 6365 5f69 645d 2e75  ies[source_id].u
-00007180: 7064 6174 6528 7b73 656c 662e 6e75 6d62  pdate({self.numb
-00007190: 6572 5f64 6976 6964 696e 675f 6b65 7920  er_dividing_key 
-000071a0: 3a20 6e75 6d62 6572 5f64 6976 6964 696e  : number_dividin
-000071b0: 677d 290d 0a20 2020 2020 2020 2020 2020  g})..           
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000071e0: 736f 7572 6365 5f69 6420 6e6f 7420 696e  source_id not in
-000071f0: 2061 6c6c 5f74 6172 6765 745f 6964 733a   all_target_ids:
-00007200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 2020 2020 2066 6f72 2073 6f75 7263 655f       for source_
+000070e0: 6964 2069 6e20 616c 6c5f 736f 7572 6365  id in all_source
+000070f0: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
+00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007110: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00007120: 6172 6765 745f 6964 7320 3d20 7365 6c66  arget_ids = self
+00007130: 2e65 6467 655f 7461 7267 6574 5f6c 6f6f  .edge_target_loo
+00007140: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00007180: 6365 6c6c 5f69 6473 2e61 7070 656e 6428  cell_ids.append(
+00007190: 736f 7572 6365 5f69 6429 0d0a 2020 2020  source_id)..    
+000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 2020 2020 2352 6f6f 740d 0a20 2020 2020      #Root..     
+000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007200: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
+00007210: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
+00007220: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
+00007230: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
+00007240: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
 00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2020 2020 666f 7220 7461 7267 6574 5f69      for target_i
-00007270: 6420 696e 2074 6172 6765 745f 6964 733a  d in target_ids:
-00007280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072b0: 2020 2020 2073 656c 662e 5f64 6963 745f       self._dict_
-000072c0: 7570 6461 7465 2875 6e69 7175 655f 7472  update(unique_tr
-000072d0: 6163 6b6c 6574 5f69 6473 2c20 736f 7572  acklet_ids, sour
-000072e0: 6365 5f69 642c 2074 7261 636b 5f69 642c  ce_id, track_id,
-000072f0: 204e 6f6e 652c 2074 6172 6765 745f 6964   None, target_id
-00007300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007280: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00007290: 5b73 6f75 7263 655f 6964 5d2e 7570 6461  [source_id].upda
+000072a0: 7465 287b 7365 6c66 2e6e 756d 6265 725f  te({self.number_
+000072b0: 6469 7669 6469 6e67 5f6b 6579 203a 206e  dividing_key : n
+000072c0: 756d 6265 725f 6469 7669 6469 6e67 7d29  umber_dividing})
+000072d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000072e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072f0: 2020 2020 2020 2020 2020 6966 2073 6f75            if sou
+00007300: 7263 655f 6964 206e 6f74 2069 6e20 616c  rce_id not in al
+00007310: 6c5f 7461 7267 6574 5f69 6473 3a0d 0a20  l_target_ids:.. 
 00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00007340: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00007350: 735b 7461 7267 6574 5f69 645d 2e75 7064  s[target_id].upd
-00007360: 6174 6528 7b73 656c 662e 6469 7669 6469  ate({self.dividi
-00007370: 6e67 5f6b 6579 203a 2064 6976 6964 696e  ng_key : dividin
-00007380: 675f 7472 616a 6563 746f 7279 7d29 0d0a  g_trajectory})..
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00007350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 2066 6f72 2074 6172 6765 745f 6964 2069   for target_id i
+00007390: 6e20 7461 7267 6574 5f69 6473 3a0d 0a20  n target_ids:.. 
 000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000073d0: 706f 745f 7072 6f70 6572 7469 6573 5b74  pot_properties[t
-000073e0: 6172 6765 745f 6964 5d2e 7570 6461 7465  arget_id].update
-000073f0: 287b 7365 6c66 2e6e 756d 6265 725f 6469  ({self.number_di
-00007400: 7669 6469 6e67 5f6b 6579 203a 206e 756d  viding_key : num
-00007410: 6265 725f 6469 7669 6469 6e67 7d29 0d0a  ber_dividing})..
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 7365 6c66 2e5f 6469 6374 5f75 7064    self._dict_upd
+000073e0: 6174 6528 756e 6971 7565 5f74 7261 636b  ate(unique_track
+000073f0: 6c65 745f 6964 732c 2073 6f75 7263 655f  let_ids, source_
+00007400: 6964 2c20 7472 6163 6b5f 6964 2c20 4e6f  id, track_id, No
+00007410: 6e65 2c20 7461 7267 6574 5f69 6429 0d0a  ne, target_id)..
 00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007440: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007470: 2020 2020 2020 2020 2020 2020 2023 4e6f               #No
-00007480: 726d 616c 2020 2020 2020 2020 0d0a 2020  rmal        ..  
-00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 2020 2020 2020 2020 2020 736f 7572              sour
-000074c0: 6365 5f73 6f75 7263 655f 6964 203d 2073  ce_source_id = s
-000074d0: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
-000074e0: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
-000074f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2066 6f72 2074 6172 6765 745f 6964 2069   for target_id i
-00007530: 6e20 7461 7267 6574 5f69 6473 3a0d 0a20  n target_ids:.. 
+00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007450: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00007460: 706f 745f 7072 6f70 6572 7469 6573 5b74  pot_properties[t
+00007470: 6172 6765 745f 6964 5d2e 7570 6461 7465  arget_id].update
+00007480: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
+00007490: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
+000074a0: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000074f0: 5f70 726f 7065 7274 6965 735b 7461 7267  _properties[targ
+00007500: 6574 5f69 645d 2e75 7064 6174 6528 7b73  et_id].update({s
+00007510: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
+00007520: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
+00007530: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
 00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2073 656c 662e 5f64 6963 745f 7570     self._dict_up
-00007580: 6461 7465 2875 6e69 7175 655f 7472 6163  date(unique_trac
-00007590: 6b6c 6574 5f69 6473 2c20 736f 7572 6365  klet_ids, source
-000075a0: 5f69 642c 2074 7261 636b 5f69 642c 2073  _id, track_id, s
-000075b0: 6f75 7263 655f 736f 7572 6365 5f69 642c  ource_source_id,
-000075c0: 2074 6172 6765 745f 6964 2920 0d0a 2020   target_id) ..  
-000075d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00007610: 6f74 5f70 726f 7065 7274 6965 735b 7461  ot_properties[ta
-00007620: 7267 6574 5f69 645d 2e75 7064 6174 6528  rget_id].update(
-00007630: 7b73 656c 662e 6469 7669 6469 6e67 5f6b  {self.dividing_k
-00007640: 6579 203a 2064 6976 6964 696e 675f 7472  ey : dividing_tr
-00007650: 616a 6563 746f 7279 7d29 200d 0a20 2020  ajectory}) ..   
+00007560: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007590: 2020 2020 2020 2020 2020 234e 6f72 6d61            #Norma
+000075a0: 6c20 2020 2020 2020 200d 0a20 2020 2020  l        ..     
+000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075d0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
+000075e0: 736f 7572 6365 5f69 6420 3d20 7365 6c66  source_id = self
+000075f0: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
+00007600: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
+00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007630: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00007640: 7220 7461 7267 6574 5f69 6420 696e 2074  r target_id in t
+00007650: 6172 6765 745f 6964 733a 0d0a 2020 2020  arget_ids:..    
 00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-000076a0: 745f 7072 6f70 6572 7469 6573 5b74 6172  t_properties[tar
-000076b0: 6765 745f 6964 5d2e 7570 6461 7465 287b  get_id].update({
-000076c0: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
-000076d0: 6469 6e67 5f6b 6579 203a 206e 756d 6265  ding_key : numbe
-000076e0: 725f 6469 7669 6469 6e67 7d29 0d0a 2020  r_dividing})..  
+00007690: 7365 6c66 2e5f 6469 6374 5f75 7064 6174  self._dict_updat
+000076a0: 6528 756e 6971 7565 5f74 7261 636b 6c65  e(unique_trackle
+000076b0: 745f 6964 732c 2073 6f75 7263 655f 6964  t_ids, source_id
+000076c0: 2c20 7472 6163 6b5f 6964 2c20 736f 7572  , track_id, sour
+000076d0: 6365 5f73 6f75 7263 655f 6964 2c20 7461  ce_source_id, ta
+000076e0: 7267 6574 5f69 6429 200d 0a20 2020 2020  rget_id) ..     
 000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007760: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 2066 6f72 2063 7572 7265 6e74 5f72 6f6f   for current_roo
-00007790: 7420 696e 2072 6f6f 745f 726f 6f74 3a0d  t in root_root:.
-000077a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2020 7365 6c66 2e72 6f6f 745f 7370      self.root_sp
-000077d0: 6f74 735b 696e 7428 6375 7272 656e 745f  ots[int(current_
-000077e0: 726f 6f74 295d 203d 2073 656c 662e 756e  root)] = self.un
-000077f0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00007800: 7469 6573 5b69 6e74 2863 7572 7265 6e74  ties[int(current
-00007810: 5f72 6f6f 7429 5d0d 0a20 2020 2020 2020  _root)]..       
+00007710: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007720: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00007730: 7072 6f70 6572 7469 6573 5b74 6172 6765  properties[targe
+00007740: 745f 6964 5d2e 7570 6461 7465 287b 7365  t_id].update({se
+00007750: 6c66 2e64 6976 6964 696e 675f 6b65 7920  lf.dividing_key 
+00007760: 3a20 6469 7669 6469 6e67 5f74 7261 6a65  : dividing_traje
+00007770: 6374 6f72 797d 2920 0d0a 2020 2020 2020  ctory}) ..      
+00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000077b0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000077c0: 726f 7065 7274 6965 735b 7461 7267 6574  roperties[target
+000077d0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
+000077e0: 662e 6e75 6d62 6572 5f64 6976 6964 696e  f.number_dividin
+000077f0: 675f 6b65 7920 3a20 6e75 6d62 6572 5f64  g_key : number_d
+00007800: 6976 6964 696e 677d 290d 0a20 2020 2020  ividing})..     
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00007830: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
 00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2073 656c 662e 616c 6c5f 6375 7272     self.all_curr
-00007860: 656e 745f 6365 6c6c 5f69 6473 5b69 6e74  ent_cell_ids[int
-00007870: 2874 7261 636b 5f69 6429 5d20 3d20 6375  (track_id)] = cu
-00007880: 7272 656e 745f 6365 6c6c 5f69 6473 0d0a  rrent_cell_ids..
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000078b0: 6920 696e 2072 616e 6765 286c 656e 2863  i in range(len(c
-000078c0: 7572 7265 6e74 5f63 656c 6c5f 6964 7329  urrent_cell_ids)
-000078d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 6b20 3d20 696e 7428 6375 7272 656e    k = int(curren
-00007930: 745f 6365 6c6c 5f69 6473 5b69 5d29 2020  t_cell_ids[i])  
-00007940: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2020 616c 6c5f 6469 6374          all_dict
-00007970: 5f76 616c 7565 7320 3d20 7365 6c66 2e75  _values = self.u
-00007980: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00007990: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000079c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079e0: 2020 2074 203d 2069 6e74 2866 6c6f 6174     t = int(float
-000079f0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00007a00: 5b73 656c 662e 6672 616d 6569 645f 6b65  [self.frameid_ke
-00007a10: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
+00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007860: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007890: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000078a0: 7220 6375 7272 656e 745f 726f 6f74 2069  r current_root i
+000078b0: 6e20 726f 6f74 5f72 6f6f 743a 0d0a 2020  n root_root:..  
+000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078e0: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
+000078f0: 5b69 6e74 2863 7572 7265 6e74 5f72 6f6f  [int(current_roo
+00007900: 7429 5d20 3d20 7365 6c66 2e75 6e69 7175  t)] = self.uniqu
+00007910: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00007920: 735b 696e 7428 6375 7272 656e 745f 726f  s[int(current_ro
+00007930: 6f74 295d 0d0a 2020 2020 2020 2020 2020  ot)]..          
+00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007950: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 7365 6c66 2e61 6c6c 5f63 7572 7265 6e74  self.all_current
+00007980: 5f63 656c 6c5f 6964 735b 696e 7428 7472  _cell_ids[int(tr
+00007990: 6163 6b5f 6964 295d 203d 2063 7572 7265  ack_id)] = curre
+000079a0: 6e74 5f63 656c 6c5f 6964 730d 0a20 2020  nt_cell_ids..   
+000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079c0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000079d0: 6e20 7261 6e67 6528 6c65 6e28 6375 7272  n range(len(curr
+000079e0: 656e 745f 6365 6c6c 5f69 6473 2929 3a0d  ent_cell_ids)):.
+000079f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 2020 2020 2020 2020 2020 7a20 3d20 666c            z = fl
-00007a40: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00007a50: 7565 735b 7365 6c66 2e7a 706f 7369 645f  ues[self.zposid_
-00007a60: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00007a30: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00007a40: 203d 2069 6e74 2863 7572 7265 6e74 5f63   = int(current_c
+00007a50: 656c 6c5f 6964 735b 695d 2920 2020 200d  ell_ids[i])    .
+00007a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 2020 2020 2020 2020 2079 203d 2066             y = f
-00007a90: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00007aa0: 6c75 6573 5b73 656c 662e 7970 6f73 6964  lues[self.yposid
-00007ab0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00007a80: 2020 2020 2061 6c6c 5f64 6963 745f 7661       all_dict_va
+00007a90: 6c75 6573 203d 2073 656c 662e 756e 6971  lues = self.uniq
+00007aa0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00007ab0: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
 00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-00007ae0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00007af0: 616c 7565 735b 7365 6c66 2e78 706f 7369  alues[self.xposi
-00007b00: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00007ad0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 7420 3d20 696e 7428 666c 6f61 7428 616c  t = int(float(al
+00007b10: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00007b20: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d29  lf.frameid_key])
+00007b30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2020 2020 2020 2020 2020 7370 6f74 5f63            spot_c
-00007b60: 656e 7472 6f69 6420 3d20 2872 6f75 6e64  entroid = (round
-00007b70: 287a 292f 7365 6c66 2e7a 6361 6c69 6272  (z)/self.zcalibr
-00007b80: 6174 696f 6e2c 2072 6f75 6e64 2879 292f  ation, round(y)/
-00007b90: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-00007ba0: 6e2c 2072 6f75 6e64 2878 292f 7365 6c66  n, round(x)/self
-00007bb0: 2e78 6361 6c69 6272 6174 696f 6e29 0d0a  .xcalibration)..
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
-00007bf0: 656e 7472 6f69 6420 3d20 2874 2c72 6f75  entroid = (t,rou
-00007c00: 6e64 287a 292f 7365 6c66 2e7a 6361 6c69  nd(z)/self.zcali
-00007c10: 6272 6174 696f 6e2c 2072 6f75 6e64 2879  bration, round(y
-00007c20: 292f 7365 6c66 2e79 6361 6c69 6272 6174  )/self.ycalibrat
-00007c30: 696f 6e2c 2072 6f75 6e64 2878 292f 7365  ion, round(x)/se
-00007c40: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
-00007c50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00007b50: 2020 2020 2020 207a 203d 2066 6c6f 6174         z = float
+00007b60: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00007b70: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
+00007b80: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ba0: 2020 2020 2020 2020 7920 3d20 666c 6f61          y = floa
+00007bb0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00007bc0: 735b 7365 6c66 2e79 706f 7369 645f 6b65  s[self.yposid_ke
+00007bd0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 2020 2020 2020 2020 2078 203d 2066 6c6f           x = flo
+00007c00: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00007c10: 6573 5b73 656c 662e 7870 6f73 6964 5f6b  es[self.xposid_k
+00007c20: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c40: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00007c50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00007c80: 7175 655f 7370 6f74 5f63 656e 7472 6f69  que_spot_centroi
-00007c90: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
-00007ca0: 7472 6f69 645d 203d 206b 0d0a 2020 2020  troid] = k..    
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00007ce0: 6b5f 6365 6e74 726f 6964 5b66 7261 6d65  k_centroid[frame
-00007cf0: 5f73 706f 745f 6365 6e74 726f 6964 5d20  _spot_centroid] 
-00007d00: 3d20 7472 6163 6b5f 6964 0d0a 0d0a 2020  = track_id....  
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 2020 6966 2073 7472 2874 2920 696e 2073    if str(t) in s
-00007d40: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-00007d50: 6f69 643a 0d0a 2020 2020 2020 2020 2020  oid:..          
-00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d80: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
-00007d90: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
-00007da0: 6d65 645f 6365 6e74 726f 6964 5b73 7472  med_centroid[str
-00007db0: 2874 295d 0d0a 2020 2020 2020 2020 2020  (t)]..          
-00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c70: 2020 2020 2020 2073 706f 745f 6365 6e74         spot_cent
+00007c80: 726f 6964 203d 2028 726f 756e 6428 7a29  roid = (round(z)
+00007c90: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
+00007ca0: 6f6e 2c20 726f 756e 6428 7929 2f73 656c  on, round(y)/sel
+00007cb0: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+00007cc0: 726f 756e 6428 7829 2f73 656c 662e 7863  round(x)/self.xc
+00007cd0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
+00007d10: 726f 6964 203d 2028 742c 726f 756e 6428  roid = (t,round(
+00007d20: 7a29 2f73 656c 662e 7a63 616c 6962 7261  z)/self.zcalibra
+00007d30: 7469 6f6e 2c20 726f 756e 6428 7929 2f73  tion, round(y)/s
+00007d40: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00007d50: 2c20 726f 756e 6428 7829 2f73 656c 662e  , round(x)/self.
+00007d60: 7863 616c 6962 7261 7469 6f6e 290d 0a0d  xcalibration)...
+00007d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d90: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00007da0: 5f73 706f 745f 6365 6e74 726f 6964 5b66  _spot_centroid[f
+00007db0: 7261 6d65 5f73 706f 745f 6365 6e74 726f  rame_spot_centro
+00007dc0: 6964 5d20 3d20 6b0d 0a20 2020 2020 2020  id] = k..       
 00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2073 706f 745f 6365 6e74 726f 6964 732e   spot_centroids.
-00007df0: 6170 7065 6e64 2873 706f 745f 6365 6e74  append(spot_cent
-00007e00: 726f 6964 290d 0a20 2020 2020 2020 2020  roid)..         
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e30: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
-00007e40: 2e63 4b44 5472 6565 2873 706f 745f 6365  .cKDTree(spot_ce
-00007e50: 6e74 726f 6964 7329 0d0a 2020 2020 2020  ntroids)..      
-00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e80: 2020 2020 2073 656c 662e 5f74 696d 6564       self._timed
-00007e90: 5f63 656e 7472 6f69 645b 7374 7228 7429  _centroid[str(t)
-00007ea0: 5d20 3d20 7472 6565 2c20 7370 6f74 5f63  ] = tree, spot_c
-00007eb0: 656e 7472 6f69 6473 200d 0a20 2020 2020  entroids ..     
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00007ee0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 2073 706f 745f 6365 6e74 726f 6964 7320   spot_centroids 
-00007f20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00007de0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00007df0: 662e 756e 6971 7565 5f74 7261 636b 5f63  f.unique_track_c
+00007e00: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
+00007e10: 6f74 5f63 656e 7472 6f69 645d 203d 2074  ot_centroid] = t
+00007e20: 7261 636b 5f69 640d 0a0d 0a20 2020 2020  rack_id....     
+00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007e50: 6620 7374 7228 7429 2069 6e20 7365 6c66  f str(t) in self
+00007e60: 2e5f 7469 6d65 645f 6365 6e74 726f 6964  ._timed_centroid
+00007e70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e90: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00007ea0: 6565 2c20 7370 6f74 5f63 656e 7472 6f69  ee, spot_centroi
+00007eb0: 6473 203d 2073 656c 662e 5f74 696d 6564  ds = self._timed
+00007ec0: 5f63 656e 7472 6f69 645b 7374 7228 7429  _centroid[str(t)
+00007ed0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00007f00: 6f74 5f63 656e 7472 6f69 6473 2e61 7070  ot_centroids.app
+00007f10: 656e 6428 7370 6f74 5f63 656e 7472 6f69  end(spot_centroi
+00007f20: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
 00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2073 706f 745f 6365 6e74 726f 6964 732e   spot_centroids.
-00007f60: 6170 7065 6e64 2873 706f 745f 6365 6e74  append(spot_cent
-00007f70: 726f 6964 290d 0a20 2020 2020 2020 2020  roid)..         
+00007f40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00007f50: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+00007f60: 4454 7265 6528 7370 6f74 5f63 656e 7472  DTree(spot_centr
+00007f70: 6f69 6473 290d 0a20 2020 2020 2020 2020  oids)..         
 00007f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fa0: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
-00007fb0: 2e63 4b44 5472 6565 2873 706f 745f 6365  .cKDTree(spot_ce
-00007fc0: 6e74 726f 6964 7329 0d0a 2020 2020 2020  ntroids)..      
-00007fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fa0: 2020 7365 6c66 2e5f 7469 6d65 645f 6365    self._timed_ce
+00007fb0: 6e74 726f 6964 5b73 7472 2874 295d 203d  ntroid[str(t)] =
+00007fc0: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
+00007fd0: 726f 6964 7320 0d0a 2020 2020 2020 2020  roids ..        
 00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2020 2073 656c 662e 5f74 696d 6564       self._timed
-00008000: 5f63 656e 7472 6f69 645b 7374 7228 7429  _centroid[str(t)
-00008010: 5d20 3d20 7472 6565 2c20 7370 6f74 5f63  ] = tree, spot_c
-00008020: 656e 7472 6f69 6473 0d0a 2020 2020 2020  entroids..      
-00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008040: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
-00008050: 6620 5f6d 6173 7465 725f 7472 6163 6b5f  f _master_track_
-00008060: 636f 6d70 7574 6572 2873 656c 662c 2074  computer(self, t
-00008070: 7261 636b 2c20 7472 6163 6b5f 6964 293a  rack, track_id):
-00008080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008090: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000080a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000080b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080d0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000080e0: 6e74 5f63 656c 6c5f 6964 7320 3d20 5b5d  nt_cell_ids = []
-000080f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008100: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2020 2020 2020 2061 6c6c 5f73 6f75           all_sou
-00008150: 7263 655f 6964 732c 2061 6c6c 5f74 6172  rce_ids, all_tar
-00008160: 6765 745f 6964 7320 3d20 2073 656c 662e  get_ids =  self.
-00008170: 5f67 656e 6572 6174 655f 6765 6e65 7261  _generate_genera
-00008180: 7469 6f6e 7328 7472 6163 6b29 0d0a 2020  tions(track)..  
-00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081a0: 2020 2020 2020 2020 2020 726f 6f74 5f72            root_r
-000081b0: 6f6f 742c 2072 6f6f 745f 7370 6c69 7473  oot, root_splits
-000081c0: 2c20 726f 6f74 5f6c 6561 6620 3d20 7365  , root_leaf = se
-000081d0: 6c66 2e5f 6372 6561 7465 5f67 656e 6572  lf._create_gener
-000081e0: 6174 696f 6e73 2861 6c6c 5f73 6f75 7263  ations(all_sourc
-000081f0: 655f 6964 7329 200d 0a20 2020 2020 2020  e_ids) ..       
-00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008210: 2020 2020 2073 656c 662e 5f69 7465 7261       self._itera
-00008220: 7465 5f73 706c 6974 5f64 6f77 6e28 726f  te_split_down(ro
-00008230: 6f74 5f72 6f6f 742c 2072 6f6f 745f 6c65  ot_root, root_le
-00008240: 6166 2c20 726f 6f74 5f73 706c 6974 7329  af, root_splits)
-00008250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008260: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008280: 2020 2020 2020 2020 2020 2020 2320 4465              # De
-00008290: 7465 726d 696e 6520 6966 2061 2074 7261  termine if a tra
-000082a0: 636b 2068 6173 2064 6976 6973 696f 6e73  ck has divisions
-000082b0: 206f 7220 6e6f 6e65 0d0a 2020 2020 2020   or none..      
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 6e75 6d62 6572 5f64 6976        number_div
-000082e0: 6964 696e 6720 3d20 6c65 6e28 726f 6f74  iding = len(root
-000082f0: 5f73 706c 6974 7329 0d0a 2020 2020 2020  _splits)..      
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 2020 6966 206c 656e 2872 6f6f        if len(roo
-00008320: 745f 7370 6c69 7473 2920 3e20 303a 0d0a  t_splits) > 0:..
-00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008350: 7365 6c66 2e75 6e69 7175 655f 7472 6163  self.unique_trac
-00008360: 6b5f 6d69 746f 7369 735f 6c61 6265 6c5b  k_mitosis_label[
-00008370: 7472 6163 6b5f 6964 5d20 3d20 5b31 2c20  track_id] = [1, 
-00008380: 6e75 6d62 6572 5f64 6976 6964 696e 675d  number_dividing]
-00008390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 6469 7669 6469 6e67 5f74 7261 6a65    dividing_traje
-000083c0: 6374 6f72 7920 3d20 5472 7565 0d0a 2020  ctory = True..  
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000083f0: 2069 6e74 2874 7261 636b 5f69 6429 206e   int(track_id) n
-00008400: 6f74 2069 6e20 7365 6c66 2e41 6c6c 5472  ot in self.AllTr
-00008410: 6163 6b49 6473 3a0d 0a20 2020 2020 2020  ackIds:..       
+00007ff0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00008000: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00008010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008020: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00008030: 6f74 5f63 656e 7472 6f69 6473 203d 205b  ot_centroids = [
+00008040: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008060: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+00008070: 6f74 5f63 656e 7472 6f69 6473 2e61 7070  ot_centroids.app
+00008080: 656e 6428 7370 6f74 5f63 656e 7472 6f69  end(spot_centroi
+00008090: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000080c0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+000080d0: 4454 7265 6528 7370 6f74 5f63 656e 7472  DTree(spot_centr
+000080e0: 6f69 6473 290d 0a20 2020 2020 2020 2020  oids)..         
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2020 7365 6c66 2e5f 7469 6d65 645f 6365    self._timed_ce
+00008120: 6e74 726f 6964 5b73 7472 2874 295d 203d  ntroid[str(t)] =
+00008130: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
+00008140: 726f 6964 730d 0a20 2020 2020 2020 2020  roids..         
+00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008160: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+00008170: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
+00008180: 7075 7465 7228 7365 6c66 2c20 7472 6163  puter(self, trac
+00008190: 6b2c 2074 7261 636b 5f69 6429 3a0d 0a20  k, track_id):.. 
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081f0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00008200: 6365 6c6c 5f69 6473 203d 205b 5d0d 0a20  cell_ids = [].. 
+00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008220: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008260: 2020 2020 2020 616c 6c5f 736f 7572 6365        all_source
+00008270: 5f69 6473 2c20 616c 6c5f 7461 7267 6574  _ids, all_target
+00008280: 5f69 6473 203d 2020 7365 6c66 2e5f 6765  _ids =  self._ge
+00008290: 6e65 7261 7465 5f67 656e 6572 6174 696f  nerate_generatio
+000082a0: 6e73 2874 7261 636b 290d 0a20 2020 2020  ns(track)..     
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2020 2020 2072 6f6f 745f 726f 6f74         root_root
+000082d0: 2c20 726f 6f74 5f73 706c 6974 732c 2072  , root_splits, r
+000082e0: 6f6f 745f 6c65 6166 203d 2073 656c 662e  oot_leaf = self.
+000082f0: 5f63 7265 6174 655f 6765 6e65 7261 7469  _create_generati
+00008300: 6f6e 7328 616c 6c5f 736f 7572 6365 5f69  ons(all_source_i
+00008310: 6473 2920 0d0a 2020 2020 2020 2020 2020  ds) ..          
+00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008330: 2020 7365 6c66 2e5f 6974 6572 6174 655f    self._iterate_
+00008340: 7370 6c69 745f 646f 776e 2872 6f6f 745f  split_down(root_
+00008350: 726f 6f74 2c20 726f 6f74 5f6c 6561 662c  root, root_leaf,
+00008360: 2072 6f6f 745f 7370 6c69 7473 290d 0a20   root_splits).. 
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 2020 2020 2020 2020 2023 2044 6574 6572           # Deter
+000083b0: 6d69 6e65 2069 6620 6120 7472 6163 6b20  mine if a track 
+000083c0: 6861 7320 6469 7669 7369 6f6e 7320 6f72  has divisions or
+000083d0: 206e 6f6e 650d 0a20 2020 2020 2020 2020   none..         
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 206e 756d 6265 725f 6469 7669 6469     number_dividi
+00008400: 6e67 203d 206c 656e 2872 6f6f 745f 7370  ng = len(root_sp
+00008410: 6c69 7473 290d 0a20 2020 2020 2020 2020  lits)..         
 00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008440: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-00008450: 7065 6e64 2869 6e74 2874 7261 636b 5f69  pend(int(track_i
-00008460: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2069 6620 696e 7428 7472 6163       if int(trac
-00008490: 6b5f 6964 2920 6e6f 7420 696e 2073 656c  k_id) not in sel
-000084a0: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-000084b0: 6473 3a20 2020 2020 0d0a 2020 2020 2020  ds:     ..      
-000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000084e0: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-000084f0: 4964 732e 6170 7065 6e64 2869 6e74 2874  Ids.append(int(t
-00008500: 7261 636b 5f69 6429 290d 0a20 2020 2020  rack_id))..     
-00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008430: 2020 2069 6620 6c65 6e28 726f 6f74 5f73     if len(root_s
+00008440: 706c 6974 7329 203e 2030 3a0d 0a20 2020  plits) > 0:..   
+00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008470: 662e 756e 6971 7565 5f74 7261 636b 5f6d  f.unique_track_m
+00008480: 6974 6f73 6973 5f6c 6162 656c 5b74 7261  itosis_label[tra
+00008490: 636b 5f69 645d 203d 205b 312c 206e 756d  ck_id] = [1, num
+000084a0: 6265 725f 6469 7669 6469 6e67 5d0d 0a20  ber_dividing].. 
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000084d0: 6976 6964 696e 675f 7472 616a 6563 746f  ividing_trajecto
+000084e0: 7279 203d 2054 7275 650d 0a20 2020 2020  ry = True..     
+000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008500: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00008510: 7428 7472 6163 6b5f 6964 2920 6e6f 7420  t(track_id) not 
+00008520: 696e 2073 656c 662e 416c 6c54 7261 636b  in self.AllTrack
+00008530: 4964 733a 0d0a 2020 2020 2020 2020 2020  Ids:..          
 00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00008580: 7175 655f 7472 6163 6b5f 6d69 746f 7369  que_track_mitosi
-00008590: 735f 6c61 6265 6c5b 7472 6163 6b5f 6964  s_label[track_id
-000085a0: 5d20 3d20 5b30 2c20 305d 0d0a 2020 2020  ] = [0, 0]..    
-000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085c0: 2020 2020 2020 2020 2020 2020 6469 7669              divi
-000085d0: 6469 6e67 5f74 7261 6a65 6374 6f72 7920  ding_trajectory 
-000085e0: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008600: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
-00008610: 7472 6163 6b5f 6964 2920 6e6f 7420 696e  track_id) not in
-00008620: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-00008630: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00008550: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+00008560: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+00008570: 6428 696e 7428 7472 6163 6b5f 6964 2929  d(int(track_id))
+00008580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085a0: 2020 6966 2069 6e74 2874 7261 636b 5f69    if int(track_i
+000085b0: 6429 206e 6f74 2069 6e20 7365 6c66 2e44  d) not in self.D
+000085c0: 6976 6964 696e 6754 7261 636b 4964 733a  ividingTrackIds:
+000085d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008600: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+00008610: 2e61 7070 656e 6428 696e 7428 7472 6163  .append(int(trac
+00008620: 6b5f 6964 2929 0d0a 2020 2020 2020 2020  k_id))..        
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-00008660: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-00008670: 696e 7428 7472 6163 6b5f 6964 2929 0d0a  int(track_id))..
+00008650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008660: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00008670: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
 00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086a0: 6966 2069 6e74 2874 7261 636b 5f69 6429  if int(track_id)
-000086b0: 206e 6f74 2069 6e20 7365 6c66 2e4e 6f72   not in self.Nor
-000086c0: 6d61 6c54 7261 636b 4964 733a 2020 2020  malTrackIds:    
-000086d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-00008700: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-00008710: 2869 6e74 2874 7261 636b 5f69 6429 290d  (int(track_id)).
-00008720: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00008730: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00008740: 6f72 206c 6561 6620 696e 2072 6f6f 745f  or leaf in root_
-00008750: 6c65 6166 3a0d 0a20 2020 2020 2020 2020  leaf:..         
+00008690: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000086a0: 5f74 7261 636b 5f6d 6974 6f73 6973 5f6c  _track_mitosis_l
+000086b0: 6162 656c 5b74 7261 636b 5f69 645d 203d  abel[track_id] =
+000086c0: 205b 302c 2030 5d0d 0a20 2020 2020 2020   [0, 0]..       
+000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086e0: 2020 2020 2020 2020 2064 6976 6964 696e           dividin
+000086f0: 675f 7472 616a 6563 746f 7279 203d 2046  g_trajectory = F
+00008700: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2020 2020 6966 2069 6e74 2874 7261        if int(tra
+00008730: 636b 5f69 6429 206e 6f74 2069 6e20 7365  ck_id) not in se
+00008740: 6c66 2e41 6c6c 5472 6163 6b49 6473 3a0d  lf.AllTrackIds:.
+00008750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00008780: 7365 636f 6e64 5f63 6861 6e6e 656c 5f75  second_channel_u
-00008790: 7064 6174 6528 6c65 6166 2c20 7472 6163  pdate(leaf, trac
-000087a0: 6b5f 6964 290d 0a20 2020 2020 2020 2020  k_id)..         
-000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087c0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000087d0: 745f 6365 6c6c 5f69 6473 2e61 7070 656e  t_cell_ids.appen
-000087e0: 6428 6c65 6166 2920 0d0a 2020 2020 2020  d(leaf) ..      
+00008770: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+00008780: 636b 4964 732e 6170 7065 6e64 2869 6e74  ckIds.append(int
+00008790: 2874 7261 636b 5f69 6429 290d 0a20 2020  (track_id))..   
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000087c0: 696e 7428 7472 6163 6b5f 6964 2920 6e6f  int(track_id) no
+000087d0: 7420 696e 2073 656c 662e 4e6f 726d 616c  t in self.Normal
+000087e0: 5472 6163 6b49 6473 3a20 2020 200d 0a20  TrackIds:    .. 
 000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008810: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00008820: 6f70 6572 7469 6573 5b6c 6561 665d 2e75  operties[leaf].u
-00008830: 7064 6174 6528 7b73 656c 662e 6469 7669  pdate({self.divi
-00008840: 6469 6e67 5f6b 6579 203a 2064 6976 6964  ding_key : divid
-00008850: 696e 675f 7472 616a 6563 746f 7279 7d29  ing_trajectory})
-00008860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008880: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00008890: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000088a0: 5b6c 6561 665d 2e75 7064 6174 6528 7b73  [leaf].update({s
-000088b0: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-000088c0: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-000088d0: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
-000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088f0: 2020 2020 2020 2020 2066 6f72 2073 6f75           for sou
-00008900: 7263 655f 6964 2069 6e20 616c 6c5f 736f  rce_id in all_so
-00008910: 7572 6365 5f69 6473 3a0d 0a20 2020 2020  urce_ids:..     
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008940: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
-00008950: 656c 5f75 7064 6174 6528 736f 7572 6365  el_update(source
-00008960: 5f69 642c 2074 7261 636b 5f69 6429 0d0a  _id, track_id)..
-00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008810: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
+00008820: 6163 6b49 6473 2e61 7070 656e 6428 696e  ackIds.append(in
+00008830: 7428 7472 6163 6b5f 6964 2929 0d0a 0d0a  t(track_id))....
+00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008850: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008860: 6c65 6166 2069 6e20 726f 6f74 5f6c 6561  leaf in root_lea
+00008870: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
+00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008890: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
+000088a0: 6f6e 645f 6368 616e 6e65 6c5f 7570 6461  ond_channel_upda
+000088b0: 7465 286c 6561 662c 2074 7261 636b 5f69  te(leaf, track_i
+000088c0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000088f0: 656c 6c5f 6964 732e 6170 7065 6e64 286c  ell_ids.append(l
+00008900: 6561 6629 200d 0a20 2020 2020 2020 2020  eaf) ..         
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00008930: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00008940: 7274 6965 735b 6c65 6166 5d2e 7570 6461  rties[leaf].upda
+00008950: 7465 287b 7365 6c66 2e64 6976 6964 696e  te({self.dividin
+00008960: 675f 6b65 7920 3a20 6469 7669 6469 6e67  g_key : dividing
+00008970: 5f74 7261 6a65 6374 6f72 797d 290d 0a20  _trajectory}).. 
 00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008990: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000089a0: 706f 745f 7072 6f70 6572 7469 6573 5b73  pot_properties[s
-000089b0: 6f75 7263 655f 6964 5d2e 7570 6461 7465  ource_id].update
-000089c0: 287b 7365 6c66 2e64 6976 6964 696e 675f  ({self.dividing_
-000089d0: 6b65 7920 3a20 6469 7669 6469 6e67 5f74  key : dividing_t
-000089e0: 7261 6a65 6374 6f72 797d 290d 0a20 2020  rajectory})..   
-000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+000089b0: 6f74 5f70 726f 7065 7274 6965 735b 6c65  ot_properties[le
+000089c0: 6166 5d2e 7570 6461 7465 287b 7365 6c66  af].update({self
+000089d0: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
+000089e0: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
+000089f0: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
 00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00008a20: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
-00008a30: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
-00008a40: 656c 662e 6e75 6d62 6572 5f64 6976 6964  elf.number_divid
-00008a50: 696e 675f 6b65 7920 3a20 6e75 6d62 6572  ing_key : number
-00008a60: 5f64 6976 6964 696e 677d 290d 0a20 2020  _dividing})..   
-00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 6375 7272 656e 745f 6365 6c6c 5f69 6473  current_cell_ids
-00008aa0: 2e61 7070 656e 6428 736f 7572 6365 5f69  .append(source_i
-00008ab0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b00: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
-00008b10: 726f 6f74 2069 6e20 726f 6f74 5f72 6f6f  root in root_roo
-00008b20: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b40: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
-00008b50: 6f6e 645f 6368 616e 6e65 6c5f 7570 6461  ond_channel_upda
-00008b60: 7465 2863 7572 7265 6e74 5f72 6f6f 742c  te(current_root,
-00008b70: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00008ba0: 656c 662e 726f 6f74 5f73 706f 7473 5b69  elf.root_spots[i
-00008bb0: 6e74 2863 7572 7265 6e74 5f72 6f6f 7429  nt(current_root)
-00008bc0: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
-00008bd0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00008be0: 696e 7428 6375 7272 656e 745f 726f 6f74  int(current_root
-00008bf0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00008c20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00008c30: 6573 5b73 6f75 7263 655f 6964 5d2e 7570  es[source_id].up
-00008c40: 6461 7465 287b 7365 6c66 2e64 6976 6964  date({self.divid
-00008c50: 696e 675f 6b65 7920 3a20 6469 7669 6469  ing_key : dividi
-00008c60: 6e67 5f74 7261 6a65 6374 6f72 797d 290d  ng_trajectory}).
-00008c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c90: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00008ca0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00008cb0: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
-00008cc0: 6528 7b73 656c 662e 6e75 6d62 6572 5f64  e({self.number_d
-00008cd0: 6976 6964 696e 675f 6b65 7920 3a20 6e75  ividing_key : nu
-00008ce0: 6d62 6572 5f64 6976 6964 696e 677d 290d  mber_dividing}).
-00008cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008d30: 616c 6c5f 6375 7272 656e 745f 6365 6c6c  all_current_cell
-00008d40: 5f69 6473 5b69 6e74 2874 7261 636b 5f69  _ids[int(track_i
-00008d50: 6429 5d20 3d20 6375 7272 656e 745f 6365  d)] = current_ce
-00008d60: 6c6c 5f69 6473 0d0a 2020 2020 2020 2020  ll_ids..        
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00008a10: 2020 2020 2020 666f 7220 736f 7572 6365        for source
+00008a20: 5f69 6420 696e 2061 6c6c 5f73 6f75 7263  _id in all_sourc
+00008a30: 655f 6964 733a 0d0a 2020 2020 2020 2020  e_ids:..        
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008a60: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+00008a70: 7570 6461 7465 2873 6f75 7263 655f 6964  update(source_id
+00008a80: 2c20 7472 6163 6b5f 6964 290d 0a20 2020  , track_id)..   
+00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00008ac0: 5f70 726f 7065 7274 6965 735b 736f 7572  _properties[sour
+00008ad0: 6365 5f69 645d 2e75 7064 6174 6528 7b73  ce_id].update({s
+00008ae0: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
+00008af0: 203a 2064 6976 6964 696e 675f 7472 616a   : dividing_traj
+00008b00: 6563 746f 7279 7d29 0d0a 2020 2020 2020  ectory})..      
+00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00008b30: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00008b40: 6f70 6572 7469 6573 5b73 6f75 7263 655f  operties[source_
+00008b50: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00008b60: 2e6e 756d 6265 725f 6469 7669 6469 6e67  .number_dividing
+00008b70: 5f6b 6579 203a 206e 756d 6265 725f 6469  _key : number_di
+00008b80: 7669 6469 6e67 7d29 0d0a 2020 2020 2020  viding})..      
+00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ba0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00008bb0: 7265 6e74 5f63 656c 6c5f 6964 732e 6170  rent_cell_ids.ap
+00008bc0: 7065 6e64 2873 6f75 7263 655f 6964 290d  pend(source_id).
+00008bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c00: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c20: 2066 6f72 2063 7572 7265 6e74 5f72 6f6f   for current_roo
+00008c30: 7420 696e 2072 6f6f 745f 726f 6f74 3a0d  t in root_root:.
+00008c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c60: 2020 2020 7365 6c66 2e5f 7365 636f 6e64      self._second
+00008c70: 5f63 6861 6e6e 656c 5f75 7064 6174 6528  _channel_update(
+00008c80: 6375 7272 656e 745f 726f 6f74 2c20 7472  current_root, tr
+00008c90: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
+00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008cc0: 2e72 6f6f 745f 7370 6f74 735b 696e 7428  .root_spots[int(
+00008cd0: 6375 7272 656e 745f 726f 6f74 295d 203d  current_root)] =
+00008ce0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00008cf0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00008d00: 2863 7572 7265 6e74 5f72 6f6f 7429 5d0d  (current_root)].
+00008d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d30: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00008d40: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00008d50: 736f 7572 6365 5f69 645d 2e75 7064 6174  source_id].updat
+00008d60: 6528 7b73 656c 662e 6469 7669 6469 6e67  e({self.dividing
+00008d70: 5f6b 6579 203a 2064 6976 6964 696e 675f  _key : dividing_
+00008d80: 7472 616a 6563 746f 7279 7d29 0d0a 2020  trajectory})..  
 00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008da0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00008db0: 6c65 6e28 6375 7272 656e 745f 6365 6c6c  len(current_cell
-00008dc0: 5f69 6473 2929 3a0d 0a20 2020 2020 2020  _ids)):..       
-00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008df0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e10: 2020 2020 2020 206b 203d 2069 6e74 2863         k = int(c
-00008e20: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
-00008e30: 695d 2920 2020 0d0a 2020 2020 2020 2020  i])   ..        
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e80: 2020 616c 6c5f 6469 6374 5f76 616c 7565    all_dict_value
-00008e90: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00008ea0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00008eb0: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
-00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ed0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ef0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00008dc0: 745f 7072 6f70 6572 7469 6573 5b73 6f75  t_properties[sou
+00008dd0: 7263 655f 6964 5d2e 7570 6461 7465 287b  rce_id].update({
+00008de0: 7365 6c66 2e6e 756d 6265 725f 6469 7669  self.number_divi
+00008df0: 6469 6e67 5f6b 6579 203a 206e 756d 6265  ding_key : numbe
+00008e00: 725f 6469 7669 6469 6e67 7d29 0d0a 2020  r_dividing})..  
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e40: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00008e50: 5f63 7572 7265 6e74 5f63 656c 6c5f 6964  _current_cell_id
+00008e60: 735b 696e 7428 7472 6163 6b5f 6964 295d  s[int(track_id)]
+00008e70: 203d 2063 7572 7265 6e74 5f63 656c 6c5f   = current_cell_
+00008e80: 6964 730d 0a20 2020 2020 2020 2020 2020  ids..           
+00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008eb0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00008ec0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+00008ed0: 2863 7572 7265 6e74 5f63 656c 6c5f 6964  (current_cell_id
+00008ee0: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
+00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f00: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2020 7420 3d20 696e 7428 666c 6f61 7428    t = int(float(
-00008f30: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00008f40: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-00008f50: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f30: 2020 2020 6b20 3d20 696e 7428 6375 7272      k = int(curr
+00008f40: 656e 745f 6365 6c6c 5f69 6473 5b69 5d29  ent_cell_ids[i])
+00008f50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 2020 2020 2020 2020 207a 203d 2066 6c6f           z = flo
-00008f80: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00008f90: 6573 5b73 656c 662e 7a70 6f73 6964 5f6b  es[self.zposid_k
-00008fa0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 2020 2020 2020 2020 2020 7920 3d20 666c            y = fl
-00008fd0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00008fe0: 7565 735b 7365 6c66 2e79 706f 7369 645f  ues[self.yposid_
-00008ff0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00008f70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00008fa0: 6c6c 5f64 6963 745f 7661 6c75 6573 203d  ll_dict_values =
+00008fb0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00008fc0: 745f 7072 6f70 6572 7469 6573 5b6b 5d0d  t_properties[k].
+00008fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ff0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 2020 2020 2020 2020 2020 2078 203d 2066             x = f
-00009020: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00009030: 6c75 6573 5b73 656c 662e 7870 6f73 6964  lues[self.xposid
-00009040: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009010: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009030: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009040: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
+00009050: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009060: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
+00009070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
-000090a0: 656e 7472 6f69 6420 3d20 2874 2c72 6f75  entroid = (t,rou
-000090b0: 6e64 287a 292f 7365 6c66 2e7a 6361 6c69  nd(z)/self.zcali
-000090c0: 6272 6174 696f 6e2c 2072 6f75 6e64 2879  bration, round(y
-000090d0: 292f 7365 6c66 2e79 6361 6c69 6272 6174  )/self.ycalibrat
-000090e0: 696f 6e2c 2072 6f75 6e64 2878 292f 7365  ion, round(x)/se
-000090f0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
-00009100: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009120: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00009130: 6971 7565 5f73 706f 745f 6365 6e74 726f  ique_spot_centro
-00009140: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
-00009150: 6e74 726f 6964 5d20 3d20 6b0d 0a20 2020  ntroid] = k..   
-00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009090: 2020 2020 2020 7a20 3d20 666c 6f61 7428        z = float(
+000090a0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+000090b0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+000090c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090e0: 2020 2020 2020 2079 203d 2066 6c6f 6174         y = float
+000090f0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00009100: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00009110: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009130: 2020 2020 2020 2020 7820 3d20 666c 6f61          x = floa
+00009140: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00009150: 735b 7365 6c66 2e78 706f 7369 645f 6b65  s[self.xposid_ke
+00009160: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
 00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00009190: 636b 5f63 656e 7472 6f69 645b 6672 616d  ck_centroid[fram
-000091a0: 655f 7370 6f74 5f63 656e 7472 6f69 645d  e_spot_centroid]
-000091b0: 203d 2074 7261 636b 5f69 640d 0a20 2020   = track_id..   
-000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091e0: 0d0a 2020 2020 6465 6620 5f73 6563 6f6e  ..    def _secon
-000091f0: 645f 6368 616e 6e65 6c5f 7570 6461 7465  d_channel_update
-00009200: 2873 656c 662c 2063 656c 6c5f 6964 2c20  (self, cell_id, 
-00009210: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
-00009220: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00009230: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-00009240: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-00009250: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00009260: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009280: 6672 616d 6520 3d20 7365 6c66 2e75 6e69  frame = self.uni
-00009290: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000092a0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000092b0: 5d5b 7365 6c66 2e66 7261 6d65 6964 5f6b  ][self.frameid_k
-000092c0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-000092d0: 2020 2020 207a 203d 2073 656c 662e 756e       z = self.un
-000092e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000092f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00009300: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
-00009310: 6579 5d2f 7365 6c66 2e7a 6361 6c69 6272  ey]/self.zcalibr
-00009320: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-00009330: 2020 2020 2020 2079 203d 2073 656c 662e         y = self.
-00009340: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00009350: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00009360: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
-00009370: 5f6b 6579 5d2f 7365 6c66 2e79 6361 6c69  _key]/self.ycali
-00009380: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00009390: 2020 2020 2020 2020 2078 203d 2073 656c           x = sel
-000093a0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000093b0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000093c0: 6c5f 6964 295d 5b73 656c 662e 7870 6f73  l_id)][self.xpos
-000093d0: 6964 5f6b 6579 5d2f 7365 6c66 2e78 6361  id_key]/self.xca
-000093e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-000093f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009400: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-00009410: 7370 6f74 7328 6672 616d 652c 207a 2c20  spots(frame, z, 
-00009420: 792c 2078 2c20 6365 6c6c 5f69 642c 2074  y, x, cell_id, t
-00009430: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-00009440: 2020 0d0a 2020 2020 6465 6620 5f66 696e    ..    def _fin
-00009450: 616c 5f74 7261 636b 7328 7365 6c66 2c20  al_tracks(self, 
-00009460: 7472 6163 6b5f 6964 293a 0d0a 0d0a 2020  track_id):....  
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00009490: 745f 6365 6c6c 5f69 6473 203d 2073 656c  t_cell_ids = sel
-000094a0: 662e 616c 6c5f 6375 7272 656e 745f 6365  f.all_current_ce
-000094b0: 6c6c 5f69 6473 5b69 6e74 2874 7261 636b  ll_ids[int(track
-000094c0: 5f69 6429 5d0d 0a20 2020 2020 2020 2020  _id)]..         
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
-000094f0: 6c65 7473 203d 207b 7d0d 0a20 2020 2020  lets = {}..     
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-00009520: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009530: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
-00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00009580: 6765 286c 656e 2863 7572 7265 6e74 5f63  ge(len(current_c
-00009590: 656c 6c5f 6964 7329 293a 0d0a 2020 2020  ell_ids)):..    
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
-000095f0: 7428 6375 7272 656e 745f 6365 6c6c 5f69  t(current_cell_i
-00009600: 6473 5b69 5d29 2020 2020 0d0a 2020 2020  ds[i])    ..    
-00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009180: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091b0: 2066 7261 6d65 5f73 706f 745f 6365 6e74   frame_spot_cent
+000091c0: 726f 6964 203d 2028 742c 726f 756e 6428  roid = (t,round(
+000091d0: 7a29 2f73 656c 662e 7a63 616c 6962 7261  z)/self.zcalibra
+000091e0: 7469 6f6e 2c20 726f 756e 6428 7929 2f73  tion, round(y)/s
+000091f0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00009200: 2c20 726f 756e 6428 7829 2f73 656c 662e  , round(x)/self.
+00009210: 7863 616c 6962 7261 7469 6f6e 2920 0d0a  xcalibration) ..
+00009220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00009250: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
+00009260: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
+00009270: 6f69 645d 203d 206b 0d0a 2020 2020 2020  oid] = k..      
+00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000092a0: 6c66 2e75 6e69 7175 655f 7472 6163 6b5f  lf.unique_track_
+000092b0: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
+000092c0: 706f 745f 6365 6e74 726f 6964 5d20 3d20  pot_centroid] = 
+000092d0: 7472 6163 6b5f 6964 0d0a 2020 2020 2020  track_id..      
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00009300: 2020 2064 6566 205f 7365 636f 6e64 5f63     def _second_c
+00009310: 6861 6e6e 656c 5f75 7064 6174 6528 7365  hannel_update(se
+00009320: 6c66 2c20 6365 6c6c 5f69 642c 2074 7261  lf, cell_id, tra
+00009330: 636b 5f69 6429 3a0d 0a20 2020 2020 2020  ck_id):..       
+00009340: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009350: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
+00009360: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
+00009370: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00009380: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00009390: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+000093a0: 6d65 203d 2073 656c 662e 756e 6971 7565  me = self.unique
+000093b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000093c0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+000093d0: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
+000093e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000093f0: 2020 7a20 3d20 7365 6c66 2e75 6e69 7175    z = self.uniqu
+00009400: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00009410: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00009420: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00009430: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
+00009440: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00009450: 2020 2020 7920 3d20 7365 6c66 2e75 6e69      y = self.uni
+00009460: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00009470: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00009480: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00009490: 795d 2f73 656c 662e 7963 616c 6962 7261  y]/self.ycalibra
+000094a0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+000094b0: 2020 2020 2020 7820 3d20 7365 6c66 2e75        x = self.u
+000094c0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000094d0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000094e0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+000094f0: 6b65 795d 2f73 656c 662e 7863 616c 6962  key]/self.xcalib
+00009500: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00009510: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
+00009520: 636f 6e64 5f63 6861 6e6e 656c 5f73 706f  cond_channel_spo
+00009530: 7473 2866 7261 6d65 2c20 7a2c 2079 2c20  ts(frame, z, y, 
+00009540: 782c 2063 656c 6c5f 6964 2c20 7472 6163  x, cell_id, trac
+00009550: 6b5f 6964 290d 0a20 2020 2020 2020 200d  k_id)..        .
+00009560: 0a20 2020 2064 6566 205f 6669 6e61 6c5f  .    def _final_
+00009570: 7472 6163 6b73 2873 656c 662c 2074 7261  tracks(self, tra
+00009580: 636b 5f69 6429 3a0d 0a0d 0a20 2020 2020  ck_id):....     
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+000095b0: 656c 6c5f 6964 7320 3d20 7365 6c66 2e61  ell_ids = self.a
+000095c0: 6c6c 5f63 7572 7265 6e74 5f63 656c 6c5f  ll_current_cell_
+000095d0: 6964 735b 696e 7428 7472 6163 6b5f 6964  ids[int(track_id
+000095e0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+00009610: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
 00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 616c 6c5f 6469 6374 5f76 616c 7565 7320  all_dict_values 
-00009640: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
-00009650: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
-00009660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009680: 2020 2020 2020 756e 6971 7565 5f69 6420        unique_id 
-00009690: 3d20 7374 7228 616c 6c5f 6469 6374 5f76  = str(all_dict_v
-000096a0: 616c 7565 735b 7365 6c66 2e75 6e69 7175  alues[self.uniqu
-000096b0: 6569 645f 6b65 795d 290d 0a20 2020 2020  eid_key])..     
+00009630: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
+00009640: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009650: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009670: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000096a0: 6c65 6e28 6375 7272 656e 745f 6365 6c6c  len(current_cell
+000096b0: 5f69 6473 2929 3a0d 0a20 2020 2020 2020  _ids)):..       
 000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000096e0: 7572 7265 6e74 5f74 7261 636b 5f69 6420  urrent_track_id 
-000096f0: 3d20 7374 7228 616c 6c5f 6469 6374 5f76  = str(all_dict_v
-00009700: 616c 7565 735b 7365 6c66 2e74 7261 636b  alues[self.track
-00009710: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 2020 2020 2020 7420                t 
-00009740: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
-00009750: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00009760: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
-00009770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 2020 206b 203d 2069 6e74 2863         k = int(c
+00009710: 7572 7265 6e74 5f63 656c 6c5f 6964 735b  urrent_cell_ids[
+00009720: 695d 2920 2020 200d 0a20 2020 2020 2020  i])    ..       
+00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009740: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00009750: 5f64 6963 745f 7661 6c75 6573 203d 2073  _dict_values = s
+00009760: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00009770: 7072 6f70 6572 7469 6573 5b6b 5d0d 0a20  properties[k].. 
 00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 2020 207a 203d 2066 6c6f 6174 2861       z = float(a
-000097a0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-000097b0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-000097c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 2020 2020 7920 3d20 666c 6f61 7428        y = float(
-000097f0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-00009800: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00009810: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 2020 2078 203d 2066 6c6f 6174         x = float
-00009840: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-00009850: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
-00009860: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00009890: 745f 7472 6163 6b6c 6574 732c 2063 7572  t_tracklets, cur
-000098a0: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-000098b0: 726f 7065 7274 6965 7320 3d20 7365 6c66  roperties = self
-000098c0: 2e5f 7472 6163 6b6c 6574 5f61 6e64 5f70  ._tracklet_and_p
-000098d0: 726f 7065 7274 6965 7328 616c 6c5f 6469  roperties(all_di
-000098e0: 6374 5f76 616c 7565 732c 2074 2c20 7a2c  ct_values, t, z,
-000098f0: 2079 2c20 782c 206b 2c20 6375 7272 656e   y, x, k, curren
-00009900: 745f 7472 6163 6b5f 6964 2c20 756e 6971  t_track_id, uniq
-00009910: 7565 5f69 642c 2063 7572 7265 6e74 5f74  ue_id, current_t
-00009920: 7261 636b 6c65 7473 2c20 6375 7272 656e  racklets, curren
-00009930: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-00009940: 6572 7469 6573 290d 0a20 2020 2020 2020  erties)..       
-00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009960: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00009970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009980: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00009990: 7265 6e74 5f74 7261 636b 6c65 7473 203d  rent_tracklets =
-000099a0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-000099b0: 656e 745f 7472 6163 6b6c 6574 735b 7374  ent_tracklets[st
-000099c0: 7228 7472 6163 6b5f 6964 295d 2c20 6474  r(track_id)], dt
-000099d0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-000099e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000099f0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00009a00: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-00009a10: 726f 7065 7274 6965 7320 3d20 6e70 2e61  roperties = np.a
-00009a20: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
-00009a30: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009a40: 6965 735b 7374 7228 7472 6163 6b5f 6964  ies[str(track_id
-00009a50: 295d 2c20 6474 7970 653d 6e70 2e66 6c6f  )], dtype=np.flo
-00009a60: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2075 6e69 7175 655f 6964 203d 2073     unique_id = s
+000097b0: 7472 2861 6c6c 5f64 6963 745f 7661 6c75  tr(all_dict_valu
+000097c0: 6573 5b73 656c 662e 756e 6971 7565 6964  es[self.uniqueid
+000097d0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00009800: 656e 745f 7472 6163 6b5f 6964 203d 2073  ent_track_id = s
+00009810: 7472 2861 6c6c 5f64 6963 745f 7661 6c75  tr(all_dict_valu
+00009820: 6573 5b73 656c 662e 7472 6163 6b69 645f  es[self.trackid_
+00009830: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 2020 2020 2074 203d 2069             t = i
+00009860: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
+00009870: 745f 7661 6c75 6573 5b73 656c 662e 6672  t_values[self.fr
+00009880: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
+00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 7a20 3d20 666c 6f61 7428 616c 6c5f    z = float(all_
+000098c0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+000098d0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
+000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009900: 2020 2079 203d 2066 6c6f 6174 2861 6c6c     y = float(all
+00009910: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+00009920: 662e 7970 6f73 6964 5f6b 6579 5d29 0d0a  f.yposid_key])..
+00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009950: 2020 2020 7820 3d20 666c 6f61 7428 616c      x = float(al
+00009960: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009970: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+00009980: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+000099b0: 7261 636b 6c65 7473 2c20 6375 7272 656e  racklets, curren
+000099c0: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+000099d0: 6572 7469 6573 203d 2073 656c 662e 5f74  erties = self._t
+000099e0: 7261 636b 6c65 745f 616e 645f 7072 6f70  racklet_and_prop
+000099f0: 6572 7469 6573 2861 6c6c 5f64 6963 745f  erties(all_dict_
+00009a00: 7661 6c75 6573 2c20 742c 207a 2c20 792c  values, t, z, y,
+00009a10: 2078 2c20 6b2c 2063 7572 7265 6e74 5f74   x, k, current_t
+00009a20: 7261 636b 5f69 642c 2075 6e69 7175 655f  rack_id, unique_
+00009a30: 6964 2c20 6375 7272 656e 745f 7472 6163  id, current_trac
+00009a40: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
+00009a50: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00009a60: 6965 7329 0d0a 2020 2020 2020 2020 2020  ies)..          
 00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00009a80: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
 00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00009ab0: 636b 735b 7472 6163 6b5f 6964 5d20 3d20  cks[track_id] = 
-00009ac0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009ad0: 7320 2020 2020 0d0a 2020 2020 2020 2020  s     ..        
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00009b00: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
-00009b10: 5b74 7261 636b 5f69 645d 203d 2063 7572  [track_id] = cur
-00009b20: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-00009b30: 726f 7065 7274 6965 7320 2020 200d 0a0d  roperties    ...
-00009b40: 0a20 2020 2064 6566 205f 7472 6163 6b6c  .    def _trackl
-00009b50: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
-00009b60: 7328 7365 6c66 2c20 616c 6c5f 6469 6374  s(self, all_dict
-00009b70: 5f76 616c 7565 732c 2074 2c20 7a2c 2079  _values, t, z, y
-00009b80: 2c20 782c 206b 2c20 6375 7272 656e 745f  , x, k, current_
-00009b90: 7472 6163 6b5f 6964 2c20 756e 6971 7565  track_id, unique
-00009ba0: 5f69 642c 2063 7572 7265 6e74 5f74 7261  _id, current_tra
-00009bb0: 636b 6c65 7473 2c20 6375 7272 656e 745f  cklets, current_
-00009bc0: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
-00009bd0: 7469 6573 293a 0d0a 2020 2020 2020 2020  ties):..        
-00009be0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2020 2067 656e 5f69 6420           gen_id 
-00009c10: 3d20 696e 7428 666c 6f61 7428 616c 6c5f  = int(float(all_
-00009c20: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-00009c30: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-00009c40: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
-00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c60: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
-00009c70: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00009c80: 5f76 616c 7565 735b 7365 6c66 2e73 7065  _values[self.spe
-00009c90: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00009cc0: 6365 6c65 7261 7469 6f6e 203d 2066 6c6f  celeration = flo
-00009cd0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009ce0: 6573 5b73 656c 662e 6163 6365 6c65 7261  es[self.accelera
-00009cf0: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
-00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009ab0: 745f 7472 6163 6b6c 6574 7320 3d20 6e70  t_tracklets = np
+00009ac0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00009ad0: 5f74 7261 636b 6c65 7473 5b73 7472 2874  _tracklets[str(t
+00009ae0: 7261 636b 5f69 6429 5d2c 2064 7479 7065  rack_id)], dtype
+00009af0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009b20: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009b30: 6572 7469 6573 203d 206e 702e 6173 6172  erties = np.asar
+00009b40: 7261 7928 6375 7272 656e 745f 7472 6163  ray(current_trac
+00009b50: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009b60: 5b73 7472 2874 7261 636b 5f69 6429 5d2c  [str(track_id)],
+00009b70: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00009b80: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009bc0: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00009bd0: 5b74 7261 636b 5f69 645d 203d 2063 7572  [track_id] = cur
+00009be0: 7265 6e74 5f74 7261 636b 6c65 7473 2020  rent_tracklets  
+00009bf0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00009c20: 636b 5f70 726f 7065 7274 6965 735b 7472  ck_properties[tr
+00009c30: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
+00009c40: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009c50: 6572 7469 6573 2020 2020 0d0a 0d0a 2020  erties    ....  
+00009c60: 2020 6465 6620 5f74 7261 636b 6c65 745f    def _tracklet_
+00009c70: 616e 645f 7072 6f70 6572 7469 6573 2873  and_properties(s
+00009c80: 656c 662c 2061 6c6c 5f64 6963 745f 7661  elf, all_dict_va
+00009c90: 6c75 6573 2c20 742c 207a 2c20 792c 2078  lues, t, z, y, x
+00009ca0: 2c20 6b2c 2063 7572 7265 6e74 5f74 7261  , k, current_tra
+00009cb0: 636b 5f69 642c 2075 6e69 7175 655f 6964  ck_id, unique_id
+00009cc0: 2c20 6375 7272 656e 745f 7472 6163 6b6c  , current_trackl
+00009cd0: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
+00009ce0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+00009cf0: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+00009d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 2066  motion_angle = f
-00009d30: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-00009d40: 6c75 6573 5b73 656c 662e 6d6f 7469 6f6e  lues[self.motion
-00009d50: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d20: 2020 2020 2020 6765 6e5f 6964 203d 2069        gen_id = i
+00009d30: 6e74 2866 6c6f 6174 2861 6c6c 5f64 6963  nt(float(all_dic
+00009d40: 745f 7661 6c75 6573 5b73 656c 662e 6765  t_values[self.ge
+00009d50: 6e65 7261 7469 6f6e 6964 5f6b 6579 5d29  nerationid_key])
+00009d60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 7261 6469 616c 5f61 6e67 6c65 203d    radial_angle =
-00009d90: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-00009da0: 7661 6c75 6573 5b73 656c 662e 7261 6469  values[self.radi
-00009db0: 616c 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  al_angle_key])..
+00009d80: 2020 2020 2020 2073 7065 6564 203d 2066         speed = f
+00009d90: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+00009da0: 6c75 6573 5b73 656c 662e 7370 6565 645f  lues[self.speed_
+00009db0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
 00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2020 2020 7261 6469 7573 203d 2066 6c6f      radius = flo
-00009df0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
-00009e00: 6573 5b73 656c 662e 7261 6469 7573 5f6b  es[self.radius_k
-00009e10: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00009dd0: 2020 2020 2020 2020 2020 2061 6363 656c             accel
+00009de0: 6572 6174 696f 6e20 3d20 666c 6f61 7428  eration = float(
+00009df0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009e00: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00009e10: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
 00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 2020 2020 2020 2020 766f 6c75 6d65            volume
-00009e40: 5f70 6978 656c 7320 3d20 696e 7428 666c  _pixels = int(fl
-00009e50: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-00009e60: 7565 735b 7365 6c66 2e71 7561 6c69 7479  ues[self.quality
-00009e70: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00009e30: 2020 2020 2020 2020 2020 2020 206d 6f74               mot
+00009e40: 696f 6e5f 616e 676c 6520 3d20 666c 6f61  ion_angle = floa
+00009e50: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+00009e60: 735b 7365 6c66 2e6d 6f74 696f 6e5f 616e  s[self.motion_an
+00009e70: 676c 655f 6b65 795d 290d 0a20 2020 2020  gle_key])..     
 00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e90: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-00009ea0: 616c 5f69 6e74 656e 7369 7479 203d 2020  al_intensity =  
-00009eb0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009ec0: 616c 7565 735b 7365 6c66 2e74 6f74 616c  alues[self.total
-00009ed0: 5f69 6e74 656e 7369 7479 5f6b 6579 5d29  _intensity_key])
-00009ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009ea0: 6164 6961 6c5f 616e 676c 6520 3d20 666c  adial_angle = fl
+00009eb0: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+00009ec0: 7565 735b 7365 6c66 2e72 6164 6961 6c5f  ues[self.radial_
+00009ed0: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-00009f30: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
-00009f40: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009f50: 616c 7565 735b 7365 6c66 2e64 6973 7461  alues[self.dista
-00009f60: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00009f70: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f90: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00009fa0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-00009fb0: 6b65 7920 696e 2061 6c6c 5f64 6963 745f  key in all_dict_
-00009fc0: 7661 6c75 6573 2e6b 6579 7328 293a 0d0a  values.keys():..
-00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ff0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00009f00: 2072 6164 6975 7320 3d20 666c 6f61 7428   radius = float(
+00009f10: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+00009f20: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+00009f30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f50: 2020 2020 2020 2076 6f6c 756d 655f 7069         volume_pi
+00009f60: 7865 6c73 203d 2069 6e74 2866 6c6f 6174  xels = int(float
+00009f70: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+00009f80: 5b73 656c 662e 7175 616c 6974 795f 6b65  [self.quality_ke
+00009f90: 795d 2929 0d0a 2020 2020 2020 2020 2020  y]))..          
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
+00009fc0: 696e 7465 6e73 6974 7920 3d20 2066 6c6f  intensity =  flo
+00009fd0: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00009fe0: 6573 5b73 656c 662e 746f 7461 6c5f 696e  es[self.total_in
+00009ff0: 7465 6e73 6974 795f 6b65 795d 290d 0a20  tensity_key]).. 
 0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a020: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-0000a030: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-0000a040: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-0000a050: 5f76 616c 7565 735b 7365 6c66 2e65 6363  _values[self.ecc
-0000a060: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-0000a070: 6972 7374 6b65 795d 290d 0a20 2020 2020  irstkey])..     
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0a0: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
-0000a0b0: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
-0000a0c0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-0000a0d0: 7661 6c75 6573 5b73 656c 662e 6563 6365  values[self.ecce
-0000a0e0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-0000a0f0: 636f 6e64 6b65 795d 290d 0a20 2020 2020  condkey])..     
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a120: 2020 2020 2020 7375 7266 6163 655f 6172        surface_ar
-0000a130: 6561 203d 2066 6c6f 6174 2861 6c6c 5f64  ea = float(all_d
-0000a140: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-0000a150: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-0000a160: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a190: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-0000a1a0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-0000a1b0: 616c 7565 735b 7365 6c66 2e63 656c 6c61  alues[self.cella
-0000a1c0: 7869 735f 6d61 736b 5f6b 6579 5d29 0d0a  xis_mask_key])..
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a020: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a040: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+0000a050: 5f63 656c 6c5f 6d61 736b 203d 2066 6c6f  _cell_mask = flo
+0000a060: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000a070: 6573 5b73 656c 662e 6469 7374 616e 6365  es[self.distance
+0000a080: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d29  _cell_mask_key])
+0000a090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0d0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+0000a0e0: 6b5f 6469 7370 6c61 6365 6d65 6e74 203d  k_displacement =
+0000a0f0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
+0000a100: 7661 6c75 6573 5b73 656c 662e 6469 7370  values[self.disp
+0000a110: 6c61 6365 6d65 6e74 5f6b 6579 5d29 0d0a  lacement_key])..
+0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a140: 2020 2020 746f 7461 6c5f 7472 6163 6b5f      total_track_
+0000a150: 6469 7374 616e 6365 203d 2066 6c6f 6174  distance = float
+0000a160: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000a170: 5b73 656c 662e 746f 7461 6c5f 7472 6163  [self.total_trac
+0000a180: 6b5f 6469 7374 616e 6365 5f6b 6579 5d29  k_distance_key])
+0000a190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 2020 2020 6d61 785f 7472 6163 6b5f        max_track_
+0000a1c0: 6469 7374 616e 6365 203d 2066 6c6f 6174  distance = float
+0000a1d0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000a1e0: 5b73 656c 662e 6d61 785f 6469 7374 616e  [self.max_distan
+0000a1f0: 6365 5f74 7261 7665 6c65 645f 6b65 795d  ce_traveled_key]
+0000a200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a220: 2020 2020 2020 2074 7261 636b 5f64 7572         track_dur
+0000a230: 6174 696f 6e20 3d20 666c 6f61 7428 616c  ation = float(al
+0000a240: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000a250: 6c66 2e74 7261 636b 5f64 7572 6174 696f  lf.track_duratio
+0000a260: 6e5f 6b65 795d 290d 0a0d 0a20 2020 2020  n_key])....     
 0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a280: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
-0000a290: 795f 636f 6d70 5f66 6972 7374 203d 202d  y_comp_first = -
-0000a2a0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a2d0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000a2e0: 5f73 6563 6f6e 6420 3d20 2d31 0d0a 2020  _second = -1..  
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2b0: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000a2c0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000a2d0: 6e20 616c 6c5f 6469 6374 5f76 616c 7565  n all_dict_value
+0000a2e0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
 0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
-0000a320: 655f 6172 6561 203d 202d 310d 0a20 2020  e_area = -1..   
+0000a310: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-0000a360: 6973 5f6d 6173 6b20 3d20 2d31 2020 2020  is_mask = -1    
-0000a370: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a390: 2020 2020 2020 2020 2066 7261 6d65 5f73           frame_s
-0000a3a0: 706f 745f 6365 6e74 726f 6964 203d 2028  pot_centroid = (
-0000a3b0: 742c 726f 756e 6428 7a29 2f73 656c 662e  t,round(z)/self.
-0000a3c0: 7a63 616c 6962 7261 7469 6f6e 2c20 726f  zcalibration, ro
-0000a3d0: 756e 6428 7929 2f73 656c 662e 7963 616c  und(y)/self.ycal
-0000a3e0: 6962 7261 7469 6f6e 2c20 726f 756e 6428  ibration, round(
-0000a3f0: 7829 2f73 656c 662e 7863 616c 6962 7261  x)/self.xcalibra
-0000a400: 7469 6f6e 2920 0d0a 2020 2020 2020 2020  tion) ..        
-0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a430: 2e75 6e69 7175 655f 7370 6f74 5f63 656e  .unique_spot_cen
-0000a440: 7472 6f69 645b 6672 616d 655f 7370 6f74  troid[frame_spot
-0000a450: 5f63 656e 7472 6f69 645d 203d 206b 0d0a  _centroid] = k..
-0000a460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a480: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-0000a490: 5f74 7261 636b 5f69 6420 696e 2063 7572  _track_id in cur
-0000a4a0: 7265 6e74 5f74 7261 636b 6c65 7473 3a0d  rent_tracklets:.
-0000a4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4d0: 2020 2020 2020 2020 2074 7261 636b 6c65           trackle
-0000a4e0: 745f 6172 7261 7920 3d20 6375 7272 656e  t_array = curren
-0000a4f0: 745f 7472 6163 6b6c 6574 735b 6375 7272  t_tracklets[curr
-0000a500: 656e 745f 7472 6163 6b5f 6964 5d0d 0a20  ent_track_id].. 
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+0000a350: 636f 6d70 5f66 6972 7374 203d 2066 6c6f  comp_first = flo
+0000a360: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000a370: 6573 5b73 656c 662e 6563 6365 6e74 7269  es[self.eccentri
+0000a380: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
+0000a390: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+0000a3d0: 6d70 5f73 6563 6f6e 6420 3d20 666c 6f61  mp_second = floa
+0000a3e0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+0000a3f0: 735b 7365 6c66 2e65 6363 656e 7472 6963  s[self.eccentric
+0000a400: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
+0000a410: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
+0000a450: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+0000a460: 616c 7565 735b 7365 6c66 2e73 7572 6661  alues[self.surfa
+0000a470: 6365 5f61 7265 615f 6b65 795d 290d 0a20  ce_area_key]).. 
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
+0000a4b0: 7869 735f 6d61 736b 203d 2066 6c6f 6174  xis_mask = float
+0000a4c0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000a4d0: 5b73 656c 662e 6365 6c6c 6178 6973 5f6d  [self.cellaxis_m
+0000a4e0: 6173 6b5f 6b65 795d 290d 0a20 2020 2020  ask_key])..     
+0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a510: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a530: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-0000a540: 7261 636b 6c65 745f 6172 7261 7920 3d20  racklet_array = 
-0000a550: 6e70 2e61 7272 6179 285b 696e 7428 666c  np.array([int(fl
-0000a560: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
-0000a570: 2074 2c20 7a2f 7365 6c66 2e7a 6361 6c69   t, z/self.zcali
-0000a580: 6272 6174 696f 6e2c 2079 2f73 656c 662e  bration, y/self.
-0000a590: 7963 616c 6962 7261 7469 6f6e 2c20 782f  ycalibration, x/
-0000a5a0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-0000a5b0: 6e5d 290d 0a20 2020 2020 2020 2020 2020  n])..           
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000a570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000a5b0: 705f 6669 7273 7420 3d20 2d31 0d0a 2020  p_first = -1..  
 0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0000a5e0: 7265 6e74 5f74 7261 636b 6c65 7473 5b63  rent_tracklets[c
-0000a5f0: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
-0000a600: 203d 206e 702e 7673 7461 636b 2828 7472   = np.vstack((tr
-0000a610: 6163 6b6c 6574 5f61 7272 6179 2c20 6375  acklet_array, cu
-0000a620: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
-0000a630: 7272 6179 2929 0d0a 0d0a 2020 2020 2020  rray))....      
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+0000a5f0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+0000a600: 6e64 203d 202d 310d 0a20 2020 2020 2020  nd = -1..       
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
+0000a640: 6120 3d20 2d31 0d0a 2020 2020 2020 2020  a = -1..        
 0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a660: 2020 7661 6c75 655f 6172 7261 7920 3d20    value_array = 
-0000a670: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-0000a680: 735f 7072 6f70 6572 7469 6573 5b63 7572  s_properties[cur
-0000a690: 7265 6e74 5f74 7261 636b 5f69 645d 0d0a  rent_track_id]..
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+0000a680: 736b 203d 202d 3120 2020 2020 0d0a 0d0a  sk = -1     ....
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0000a6d0: 7661 6c75 655f 6172 7261 7920 3d20 6e70  value_array = np
-0000a6e0: 2e61 7272 6179 285b 742c 2069 6e74 2866  .array([t, int(f
-0000a6f0: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
-0000a700: 2c20 6765 6e5f 6964 2c20 7261 6469 7573  , gen_id, radius
-0000a710: 2c20 766f 6c75 6d65 5f70 6978 656c 732c  , volume_pixels,
-0000a720: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-0000a730: 6d70 5f66 6972 7374 2c20 6563 6365 6e74  mp_first, eccent
-0000a740: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-0000a750: 6e64 2c20 7375 7266 6163 655f 6172 6561  nd, surface_area
-0000a760: 2c20 746f 7461 6c5f 696e 7465 6e73 6974  , total_intensit
-0000a770: 792c 2073 7065 6564 2c20 6d6f 7469 6f6e  y, speed, motion
-0000a780: 5f61 6e67 6c65 2c20 6163 6365 6c65 7261  _angle, accelera
-0000a790: 7469 6f6e 2c20 6469 7374 616e 6365 5f63  tion, distance_c
-0000a7a0: 656c 6c5f 6d61 736b 2c20 7261 6469 616c  ell_mask, radial
-0000a7b0: 5f61 6e67 6c65 2c20 6365 6c6c 5f61 7869  _angle, cell_axi
-0000a7c0: 735f 6d61 736b 5d29 0d0a 2020 2020 2020  s_mask])..      
+0000a6b0: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
+0000a6c0: 656e 7472 6f69 6420 3d20 2874 2c72 6f75  entroid = (t,rou
+0000a6d0: 6e64 287a 292f 7365 6c66 2e7a 6361 6c69  nd(z)/self.zcali
+0000a6e0: 6272 6174 696f 6e2c 2072 6f75 6e64 2879  bration, round(y
+0000a6f0: 292f 7365 6c66 2e79 6361 6c69 6272 6174  )/self.ycalibrat
+0000a700: 696f 6e2c 2072 6f75 6e64 2878 292f 7365  ion, round(x)/se
+0000a710: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+0000a720: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a740: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000a750: 7565 5f73 706f 745f 6365 6e74 726f 6964  ue_spot_centroid
+0000a760: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
+0000a770: 726f 6964 5d20 3d20 6b0d 0a0d 0a20 2020  roid] = k....   
+0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2069 6620 6375 7272 656e 745f 7472 6163   if current_trac
+0000a7b0: 6b5f 6964 2069 6e20 6375 7272 656e 745f  k_id in current_
+0000a7c0: 7472 6163 6b6c 6574 733a 0d0a 2020 2020  tracklets:..    
 0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-0000a820: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
-0000a830: 6f70 6572 7469 6573 5b63 7572 7265 6e74  operties[current
-0000a840: 5f74 7261 636b 5f69 645d 203d 206e 702e  _track_id] = np.
-0000a850: 7673 7461 636b 2828 7661 6c75 655f 6172  vstack((value_ar
-0000a860: 7261 792c 2063 7572 7265 6e74 5f76 616c  ray, current_val
-0000a870: 7565 5f61 7272 6179 2929 0d0a 0d0a 2020  ue_array))....  
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8a0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8d0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000a8e0: 745f 6172 7261 7920 3d20 6e70 2e61 7272  t_array = np.arr
-0000a8f0: 6179 285b 696e 7428 666c 6f61 7428 756e  ay([int(float(un
-0000a900: 6971 7565 5f69 6429 292c 2074 2c20 7a2f  ique_id)), t, z/
-0000a910: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-0000a920: 6e2c 2079 2f73 656c 662e 7963 616c 6962  n, y/self.ycalib
-0000a930: 7261 7469 6f6e 2c20 782f 7365 6c66 2e78  ration, x/self.x
-0000a940: 6361 6c69 6272 6174 696f 6e5d 290d 0a20  calibration]).. 
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 2020 2020 7472 6163 6b6c 6574 5f61 7272      tracklet_arr
+0000a800: 6179 203d 2063 7572 7265 6e74 5f74 7261  ay = current_tra
+0000a810: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
+0000a820: 7261 636b 5f69 645d 0d0a 2020 2020 2020  rack_id]..      
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a850: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+0000a860: 6574 5f61 7272 6179 203d 206e 702e 6172  et_array = np.ar
+0000a870: 7261 7928 5b69 6e74 2866 6c6f 6174 2875  ray([int(float(u
+0000a880: 6e69 7175 655f 6964 2929 2c20 742c 207a  nique_id)), t, z
+0000a890: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
+0000a8a0: 6f6e 2c20 792f 7365 6c66 2e79 6361 6c69  on, y/self.ycali
+0000a8b0: 6272 6174 696f 6e2c 2078 2f73 656c 662e  bration, x/self.
+0000a8c0: 7863 616c 6962 7261 7469 6f6e 5d29 0d0a  xcalibration])..
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0000a900: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
+0000a910: 745f 7472 6163 6b5f 6964 5d20 3d20 6e70  t_track_id] = np
+0000a920: 2e76 7374 6163 6b28 2874 7261 636b 6c65  .vstack((trackle
+0000a930: 745f 6172 7261 792c 2063 7572 7265 6e74  t_array, current
+0000a940: 5f74 7261 636b 6c65 745f 6172 7261 7929  _tracklet_array)
+0000a950: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
 0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-0000a980: 7261 636b 6c65 7473 5b63 7572 7265 6e74  racklets[current
-0000a990: 5f74 7261 636b 5f69 645d 203d 2063 7572  _track_id] = cur
-0000a9a0: 7265 6e74 5f74 7261 636b 6c65 745f 6172  rent_tracklet_ar
-0000a9b0: 7261 7920 0d0a 0d0a 2020 2020 2020 2020  ray ....        
+0000a970: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0000a980: 7565 5f61 7272 6179 203d 2063 7572 7265  ue_array = curre
+0000a990: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
+0000a9a0: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
+0000a9b0: 7472 6163 6b5f 6964 5d0d 0a20 2020 2020  track_id]..     
 0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9e0: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
-0000a9f0: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
-0000aa00: 742c 2069 6e74 2866 6c6f 6174 2875 6e69  t, int(float(uni
-0000aa10: 7175 655f 6964 2929 2c20 6765 6e5f 6964  que_id)), gen_id
-0000aa20: 2c20 7261 6469 7573 2c20 766f 6c75 6d65  , radius, volume
-0000aa30: 5f70 6978 656c 732c 2020 6563 6365 6e74  _pixels,  eccent
-0000aa40: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-0000aa50: 742c 2065 6363 656e 7472 6963 6974 795f  t, eccentricity_
-0000aa60: 636f 6d70 5f73 6563 6f6e 642c 2073 7572  comp_second, sur
-0000aa70: 6661 6365 5f61 7265 612c 2020 746f 7461  face_area,  tota
-0000aa80: 6c5f 696e 7465 6e73 6974 792c 2073 7065  l_intensity, spe
-0000aa90: 6564 2c20 6d6f 7469 6f6e 5f61 6e67 6c65  ed, motion_angle
-0000aaa0: 2c20 6163 6365 6c65 7261 7469 6f6e 2c20  , acceleration, 
-0000aab0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000aac0: 736b 2c20 7261 6469 616c 5f61 6e67 6c65  sk, radial_angle
-0000aad0: 2c20 6365 6c6c 5f61 7869 735f 6d61 736b  , cell_axis_mask
-0000aae0: 205d 290d 0a20 2020 2020 2020 2020 2020   ])..           
-0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0000ab10: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-0000ab20: 726f 7065 7274 6965 735b 6375 7272 656e  roperties[curren
-0000ab30: 745f 7472 6163 6b5f 6964 5d20 3d20 6375  t_track_id] = cu
-0000ab40: 7272 656e 745f 7661 6c75 655f 6172 7261  rrent_value_arra
-0000ab50: 790d 0a0d 0a20 2020 2020 2020 2020 2020  y....           
+0000a9e0: 2020 2063 7572 7265 6e74 5f76 616c 7565     current_value
+0000a9f0: 5f61 7272 6179 203d 206e 702e 6172 7261  _array = np.arra
+0000aa00: 7928 5b74 2c20 696e 7428 666c 6f61 7428  y([t, int(float(
+0000aa10: 756e 6971 7565 5f69 6429 292c 2067 656e  unique_id)), gen
+0000aa20: 5f69 642c 2072 6164 6975 732c 2076 6f6c  _id, radius, vol
+0000aa30: 756d 655f 7069 7865 6c73 2c20 6563 6365  ume_pixels, ecce
+0000aa40: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+0000aa50: 7273 742c 2065 6363 656e 7472 6963 6974  rst, eccentricit
+0000aa60: 795f 636f 6d70 5f73 6563 6f6e 642c 2073  y_comp_second, s
+0000aa70: 7572 6661 6365 5f61 7265 612c 2074 6f74  urface_area, tot
+0000aa80: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
+0000aa90: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
+0000aaa0: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
+0000aab0: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+0000aac0: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
+0000aad0: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
+0000aae0: 6b2c 2074 7261 636b 5f64 6973 706c 6163  k, track_displac
+0000aaf0: 656d 656e 742c 746f 7461 6c5f 7472 6163  ement,total_trac
+0000ab00: 6b5f 6469 7374 616e 6365 2c6d 6178 5f74  k_distance,max_t
+0000ab10: 7261 636b 5f64 6973 7461 6e63 652c 2074  rack_distance, t
+0000ab20: 7261 636b 5f64 7572 6174 696f 6e5d 290d  rack_duration]).
+0000ab30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000ab80: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-0000ab90: 732c 2063 7572 7265 6e74 5f74 7261 636b  s, current_track
-0000aba0: 6c65 7473 5f70 726f 7065 7274 6965 7320  lets_properties 
-0000abb0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
-0000abc0: 5f6d 6173 7465 725f 7370 6f74 5f63 6f6d  _master_spot_com
-0000abd0: 7075 7465 7228 7365 6c66 2c20 6672 616d  puter(self, fram
-0000abe0: 6529 3a0d 0a20 2020 2020 2020 2020 200d  e):..          .
-0000abf0: 0a20 2020 2020 2020 2020 2066 6f72 2053  .          for S
-0000ac00: 706f 746f 626a 6563 7420 696e 2066 7261  potobject in fra
-0000ac10: 6d65 2e66 696e 6461 6c6c 2827 5370 6f74  me.findall('Spot
-0000ac20: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000ac30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-0000ac60: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-0000ac70: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000ac80: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000ac90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 2020 6966 2073 656c 662e 756e        if self.un
-0000acc0: 6971 7565 6964 5f6b 6579 2069 6e20 5370  iqueid_key in Sp
-0000acd0: 6f74 6f62 6a65 6374 2e6b 6579 7328 293a  otobject.keys():
-0000ace0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000acf0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000ad00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad10: 2020 2020 2020 2020 2020 2020 7261 6469              radi
-0000ad20: 7573 203d 2066 6c6f 6174 2853 706f 746f  us = float(Spoto
-0000ad30: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
-0000ad40: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2020 2020 2020 2020 2020 2071 7561               qua
-0000ad70: 6c69 7479 203d 2066 6c6f 6174 2853 706f  lity = float(Spo
-0000ad80: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000ad90: 2e71 7561 6c69 7479 5f6b 6579 2929 0d0a  .quality_key))..
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adc0: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
-0000add0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
-0000ade0: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
-0000adf0: 6c5f 696e 7465 6e73 6974 795f 6b65 7929  l_intensity_key)
-0000ae00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 206d 6561 6e5f 696e 7465 6e73 6974     mean_intensit
-0000ae30: 7920 3d20 666c 6f61 7428 5370 6f74 6f62  y = float(Spotob
-0000ae40: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
-0000ae50: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000ae60: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000ae90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000aea0: 735b 6365 6c6c 5f69 645d 203d 207b 0d0a  s[cell_id] = {..
-0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 7365 6c66 2e63 656c 6c69 645f      self.cellid_
-0000aee0: 6b65 793a 2069 6e74 2866 6c6f 6174 2853  key: int(float(S
-0000aef0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000af00: 6c66 2e73 706f 7469 645f 6b65 7929 2929  lf.spotid_key)))
-0000af10: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000af40: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-0000af50: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000af60: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000af70: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000afa0: 6c66 2e7a 706f 7369 645f 6b65 7920 3a20  lf.zposid_key : 
-0000afb0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000afc0: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
-0000afd0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b000: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-0000b010: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b020: 6765 7428 7365 6c66 2e79 706f 7369 645f  get(self.yposid_
-0000b030: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b060: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
-0000b070: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b080: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
-0000b090: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b0c0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000b0d0: 6b65 7920 3a20 746f 7461 6c5f 696e 7465  key : total_inte
-0000b0e0: 6e73 6974 792c 0d0a 2020 2020 2020 2020  nsity,..        
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b110: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000b120: 6b65 7920 3a20 6d65 616e 5f69 6e74 656e  key : mean_inten
-0000b130: 7369 7479 2c0d 0a20 2020 2020 2020 2020  sity,..         
-0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b160: 7261 6469 7573 5f6b 6579 203a 2072 6164  radius_key : rad
-0000b170: 6975 732c 0d0a 2020 2020 2020 2020 2020  ius,..          
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-0000b1a0: 7561 6c69 7479 5f6b 6579 203a 2071 7561  uality_key : qua
-0000b1b0: 6c69 7479 2c0d 0a20 2020 2020 2020 2020  lity,..         
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+0000ab90: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+0000aba0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+0000abb0: 5d20 3d20 6e70 2e76 7374 6163 6b28 2876  ] = np.vstack((v
+0000abc0: 616c 7565 5f61 7272 6179 2c20 6375 7272  alue_array, curr
+0000abd0: 656e 745f 7661 6c75 655f 6172 7261 7929  ent_value_array)
+0000abe0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac30: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0000ac40: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
+0000ac50: 206e 702e 6172 7261 7928 5b69 6e74 2866   np.array([int(f
+0000ac60: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
+0000ac70: 2c20 742c 207a 2f73 656c 662e 7a63 616c  , t, z/self.zcal
+0000ac80: 6962 7261 7469 6f6e 2c20 792f 7365 6c66  ibration, y/self
+0000ac90: 2e79 6361 6c69 6272 6174 696f 6e2c 2078  .ycalibration, x
+0000aca0: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+0000acb0: 6f6e 5d29 0d0a 2020 2020 2020 2020 2020  on])..          
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000ace0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
+0000acf0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+0000ad00: 5d20 3d20 6375 7272 656e 745f 7472 6163  ] = current_trac
+0000ad10: 6b6c 6574 5f61 7272 6179 200d 0a0d 0a20  klet_array .... 
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad40: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
+0000ad50: 616c 7565 5f61 7272 6179 203d 206e 702e  alue_array = np.
+0000ad60: 6172 7261 7928 5b74 2c20 696e 7428 666c  array([t, int(fl
+0000ad70: 6f61 7428 756e 6971 7565 5f69 6429 292c  oat(unique_id)),
+0000ad80: 2067 656e 5f69 642c 2072 6164 6975 732c   gen_id, radius,
+0000ad90: 2076 6f6c 756d 655f 7069 7865 6c73 2c20   volume_pixels, 
+0000ada0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+0000adb0: 6d70 5f66 6972 7374 2c20 6563 6365 6e74  mp_first, eccent
+0000adc0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+0000add0: 6e64 2c20 7375 7266 6163 655f 6172 6561  nd, surface_area
+0000ade0: 2c20 2074 6f74 616c 5f69 6e74 656e 7369  ,  total_intensi
+0000adf0: 7479 2c20 7370 6565 642c 206d 6f74 696f  ty, speed, motio
+0000ae00: 6e5f 616e 676c 652c 2061 6363 656c 6572  n_angle, acceler
+0000ae10: 6174 696f 6e2c 2064 6973 7461 6e63 655f  ation, distance_
+0000ae20: 6365 6c6c 5f6d 6173 6b2c 2072 6164 6961  cell_mask, radia
+0000ae30: 6c5f 616e 676c 652c 2063 656c 6c5f 6178  l_angle, cell_ax
+0000ae40: 6973 5f6d 6173 6b2c 2074 7261 636b 5f64  is_mask, track_d
+0000ae50: 6973 706c 6163 656d 656e 742c 746f 7461  isplacement,tota
+0000ae60: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+0000ae70: 2c6d 6178 5f74 7261 636b 5f64 6973 7461  ,max_track_dista
+0000ae80: 6e63 652c 2074 7261 636b 5f64 7572 6174  nce, track_durat
+0000ae90: 696f 6e5d 290d 0a20 2020 2020 2020 2020  ion])..         
+0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000aec0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+0000aed0: 5f70 726f 7065 7274 6965 735b 6375 7272  _properties[curr
+0000aee0: 656e 745f 7472 6163 6b5f 6964 5d20 3d20  ent_track_id] = 
+0000aef0: 6375 7272 656e 745f 7661 6c75 655f 6172  current_value_ar
+0000af00: 7261 790d 0a0d 0a20 2020 2020 2020 2020  ray....         
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000af30: 6e20 6375 7272 656e 745f 7472 6163 6b6c  n current_trackl
+0000af40: 6574 732c 2063 7572 7265 6e74 5f74 7261  ets, current_tra
+0000af50: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+0000af60: 7320 2020 2020 0d0a 0d0a 2020 2020 6465  s     ....    de
+0000af70: 6620 5f6d 6173 7465 725f 7370 6f74 5f63  f _master_spot_c
+0000af80: 6f6d 7075 7465 7228 7365 6c66 2c20 6672  omputer(self, fr
+0000af90: 616d 6529 3a0d 0a20 2020 2020 2020 2020  ame):..         
+0000afa0: 200d 0a20 2020 2020 2020 2020 2066 6f72   ..          for
+0000afb0: 2053 706f 746f 626a 6563 7420 696e 2066   Spotobject in f
+0000afc0: 7261 6d65 2e66 696e 6461 6c6c 2827 5370  rame.findall('Sp
+0000afd0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
+0000b010: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
+0000b020: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
+0000b030: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000b040: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000b070: 756e 6971 7565 6964 5f6b 6579 2069 6e20  uniqueid_key in 
+0000b080: 5370 6f74 6f62 6a65 6374 2e6b 6579 7328  Spotobject.keys(
+0000b090: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000b0a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000b0d0: 6469 7573 203d 2066 6c6f 6174 2853 706f  dius = float(Spo
+0000b0e0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b0f0: 2e72 6164 6975 735f 6b65 7929 290d 0a20  .radius_key)).. 
+0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+0000b120: 7561 6c69 7479 203d 2066 6c6f 6174 2853  uality = float(S
+0000b130: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b140: 6c66 2e71 7561 6c69 7479 5f6b 6579 2929  lf.quality_key))
+0000b150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 746f 7461 6c5f 696e 7465 6e73 6974    total_intensit
+0000b180: 7920 3d20 666c 6f61 7428 5370 6f74 6f62  y = float(Spotob
+0000b190: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
+0000b1a0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+0000b1b0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b1e0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000b1f0: 736b 5f6b 6579 3a20 2866 6c6f 6174 2853  sk_key: (float(S
-0000b200: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b210: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-0000b220: 5f6d 6173 6b5f 6b65 7929 2929 2c0d 0a20  _mask_key))),.. 
-0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b250: 2020 2073 656c 662e 756e 6971 7565 6964     self.uniqueid
-0000b260: 5f6b 6579 203a 2073 7472 2853 706f 746f  _key : str(Spoto
-0000b270: 626a 6563 742e 6765 7428 7365 6c66 2e75  bject.get(self.u
-0000b280: 6e69 7175 6569 645f 6b65 7929 292c 0d0a  niqueid_key)),..
-0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2b0: 2020 2020 7365 6c66 2e74 7261 636b 6c65      self.trackle
-0000b2c0: 7469 645f 6b65 7920 3a20 7374 7228 5370  tid_key : str(Sp
-0000b2d0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b2e0: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
-0000b2f0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-0000b320: 6e65 7261 7469 6f6e 6964 5f6b 6579 203a  nerationid_key :
-0000b330: 2073 7472 2853 706f 746f 626a 6563 742e   str(Spotobject.
-0000b340: 6765 7428 7365 6c66 2e67 656e 6572 6174  get(self.generat
-0000b350: 696f 6e69 645f 6b65 7929 292c 0d0a 2020  ionid_key)),..  
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b380: 2020 7365 6c66 2e74 7261 636b 6964 5f6b    self.trackid_k
-0000b390: 6579 203a 2073 7472 2853 706f 746f 626a  ey : str(Spotobj
-0000b3a0: 6563 742e 6765 7428 7365 6c66 2e74 7261  ect.get(self.tra
-0000b3b0: 636b 6964 5f6b 6579 2929 2c0d 0a20 2020  ckid_key)),..   
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3e0: 2073 656c 662e 6d6f 7469 6f6e 5f61 6e67   self.motion_ang
-0000b3f0: 6c65 5f6b 6579 203a 2028 666c 6f61 7428  le_key : (float(
-0000b400: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b410: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-0000b420: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b450: 6c66 2e73 7065 6564 5f6b 6579 203a 2028  lf.speed_key : (
-0000b460: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000b470: 2e67 6574 2873 656c 662e 7370 6565 645f  .get(self.speed_
-0000b480: 6b65 7929 2929 2c0d 0a20 2020 2020 2020  key))),..       
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b4b0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-0000b4c0: 6579 203a 2028 666c 6f61 7428 5370 6f74  ey : (float(Spot
-0000b4d0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b4e0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
-0000b4f0: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
-0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000b520: 6164 6961 6c5f 616e 676c 655f 6b65 793a  adial_angle_key:
-0000b530: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000b540: 742e 6765 7428 7365 6c66 2e72 6164 6961  t.get(self.radia
-0000b550: 6c5f 616e 676c 655f 6b65 7929 292c 0d0a  l_angle_key)),..
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1d0: 2020 2020 206d 6561 6e5f 696e 7465 6e73       mean_intens
+0000b1e0: 6974 7920 3d20 666c 6f61 7428 5370 6f74  ity = float(Spot
+0000b1f0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b200: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
+0000b210: 6579 2929 0d0a 0d0a 2020 2020 2020 2020  ey))....        
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+0000b240: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+0000b250: 6965 735b 6365 6c6c 5f69 645d 203d 207b  ies[cell_id] = {
+0000b260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+0000b290: 645f 6b65 793a 2069 6e74 2866 6c6f 6174  d_key: int(float
+0000b2a0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b2b0: 7365 6c66 2e73 706f 7469 645f 6b65 7929  self.spotid_key)
+0000b2c0: 2929 2c20 0d0a 2020 2020 2020 2020 2020  )), ..          
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2e0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000b2f0: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
+0000b300: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
+0000b310: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
+0000b320: 6964 5f6b 6579 2929 292c 0d0a 2020 2020  id_key))),..    
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b350: 7365 6c66 2e7a 706f 7369 645f 6b65 7920  self.zposid_key 
+0000b360: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000b370: 6374 2e67 6574 2873 656c 662e 7a70 6f73  ct.get(self.zpos
+0000b380: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b3b0: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
+0000b3c0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000b3d0: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000b3e0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b410: 6c66 2e78 706f 7369 645f 6b65 7920 3a20  lf.xposid_key : 
+0000b420: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b430: 2e67 6574 2873 656c 662e 7870 6f73 6964  .get(self.xposid
+0000b440: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b470: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000b480: 795f 6b65 7920 3a20 746f 7461 6c5f 696e  y_key : total_in
+0000b490: 7465 6e73 6974 792c 0d0a 2020 2020 2020  tensity,..      
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b4c0: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000b4d0: 795f 6b65 7920 3a20 6d65 616e 5f69 6e74  y_key : mean_int
+0000b4e0: 656e 7369 7479 2c0d 0a20 2020 2020 2020  ensity,..       
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b510: 662e 7261 6469 7573 5f6b 6579 203a 2072  f.radius_key : r
+0000b520: 6164 6975 732c 0d0a 2020 2020 2020 2020  adius,..        
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b550: 2e71 7561 6c69 7479 5f6b 6579 203a 2071  .quality_key : q
+0000b560: 7561 6c69 7479 2c0d 0a20 2020 2020 2020  uality,..       
 0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b580: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5a0: 2020 2069 6620 7365 6c66 2e73 7572 6661     if self.surfa
-0000b5b0: 6365 5f61 7265 615f 6b65 7920 696e 2053  ce_area_key in S
-0000b5c0: 706f 746f 626a 6563 742e 6b65 7973 2829  potobject.keys()
-0000b5d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5f0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-0000b600: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-0000b610: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-0000b620: 2e75 7064 6174 6528 7b0d 0a20 2020 2020  .update({..     
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b590: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+0000b5a0: 6d61 736b 5f6b 6579 3a20 2866 6c6f 6174  mask_key: (float
+0000b5b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b5c0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+0000b5d0: 6c6c 5f6d 6173 6b5f 6b65 7929 2929 2c0d  ll_mask_key))),.
+0000b5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+0000b610: 6964 5f6b 6579 203a 2073 7472 2853 706f  id_key : str(Spo
+0000b620: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b630: 2e75 6e69 7175 6569 645f 6b65 7929 292c  .uniqueid_key)),
+0000b640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 2073 656c 662e 6563 6365 6e74 7269     self.eccentri
-0000b690: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
-0000b6a0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000b6b0: 626a 6563 742e 6765 7428 7365 6c66 2e65  bject.get(self.e
-0000b6c0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000b6d0: 5f66 6972 7374 6b65 7929 292c 0d0a 2020  _firstkey)),..  
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+0000b670: 6c65 7469 645f 6b65 7920 3a20 7374 7228  letid_key : str(
+0000b680: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b690: 656c 662e 7472 6163 6b6c 6574 6964 5f6b  elf.trackletid_k
+0000b6a0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b6d0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
+0000b6e0: 203a 2073 7472 2853 706f 746f 626a 6563   : str(Spotobjec
+0000b6f0: 742e 6765 7428 7365 6c66 2e67 656e 6572  t.get(self.gener
+0000b700: 6174 696f 6e69 645f 6b65 7929 292c 0d0a  ationid_key)),..
 0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b730: 2020 2020 2020 7365 6c66 2e65 6363 656e        self.eccen
-0000b740: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-0000b750: 6f6e 646b 6579 203a 2066 6c6f 6174 2853  ondkey : float(S
-0000b760: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b770: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-0000b780: 636f 6d70 5f73 6563 6f6e 646b 6579 2929  comp_secondkey))
-0000b790: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b7f0: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-0000b800: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000b810: 6563 742e 6765 7428 7365 6c66 2e73 7572  ect.get(self.sur
-0000b820: 6661 6365 5f61 7265 615f 6b65 7929 292c  face_area_key)),
-0000b830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b730: 2020 2020 7365 6c66 2e74 7261 636b 6964      self.trackid
+0000b740: 5f6b 6579 203a 2073 7472 2853 706f 746f  _key : str(Spoto
+0000b750: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000b760: 7261 636b 6964 5f6b 6579 2929 2c0d 0a20  rackid_key)),.. 
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b790: 2020 2073 656c 662e 6d6f 7469 6f6e 5f61     self.motion_a
+0000b7a0: 6e67 6c65 5f6b 6579 203a 2028 666c 6f61  ngle_key : (floa
+0000b7b0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000b7c0: 2873 656c 662e 6d6f 7469 6f6e 5f61 6e67  (self.motion_ang
+0000b7d0: 6c65 5f6b 6579 2929 292c 0d0a 2020 2020  le_key))),..    
+0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b800: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
+0000b810: 2028 666c 6f61 7428 5370 6f74 6f62 6a65   (float(Spotobje
+0000b820: 6374 2e67 6574 2873 656c 662e 7370 6565  ct.get(self.spee
+0000b830: 645f 6b65 7929 2929 2c0d 0a20 2020 2020  d_key))),..     
 0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000b890: 656c 6c61 7869 735f 6d61 736b 5f6b 6579  ellaxis_mask_key
-0000b8a0: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000b8b0: 6374 2e67 6574 2873 656c 662e 6365 6c6c  ct.get(self.cell
-0000b8c0: 6178 6973 5f6d 6173 6b5f 6b65 7929 290d  axis_mask_key)).
-0000b8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b920: 2020 2020 2020 2020 2020 2020 207d 290d               }).
-0000b930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b860: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+0000b870: 5f6b 6579 203a 2028 666c 6f61 7428 5370  _key : (float(Sp
+0000b880: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b890: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+0000b8a0: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
+0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b8d0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
+0000b8e0: 793a 2066 6c6f 6174 2853 706f 746f 626a  y: float(Spotobj
+0000b8f0: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
+0000b900: 6961 6c5f 616e 676c 655f 6b65 7929 292c  ial_angle_key)),
+0000b910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b930: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
 0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b950: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000b950: 2020 2020 2069 6620 7365 6c66 2e73 7572       if self.sur
+0000b960: 6661 6365 5f61 7265 615f 6b65 7920 696e  face_area_key in
+0000b970: 2053 706f 746f 626a 6563 742e 6b65 7973   Spotobject.keys
+0000b980: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
 0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b9c0: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-0000b9d0: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000b9e0: 206e 6f74 2069 6e20 5370 6f74 6f62 6a65   not in Spotobje
-0000b9f0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
+0000b9a0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000b9b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000b9c0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+0000b9d0: 295d 2e75 7064 6174 6528 7b0d 0a20 2020  )].update({..   
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba60: 2020 2020 6966 2073 656c 662e 6465 7465      if self.dete
-0000ba70: 6374 6f72 6368 616e 6e65 6c20 3d3d 2031  ctorchannel == 1
-0000ba80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ba30: 2020 2020 2073 656c 662e 6563 6365 6e74       self.eccent
+0000ba40: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+0000ba50: 746b 6579 203a 2066 6c6f 6174 2853 706f  tkey : float(Spo
+0000ba60: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000ba70: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+0000ba80: 6d70 5f66 6972 7374 6b65 7929 292c 0d0a  mp_firstkey)),..
 0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bab0: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000bac0: 454e 5349 5459 203d 2053 706f 746f 626a  ENSITY = Spotobj
-0000bad0: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
-0000bae0: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
-0000baf0: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb20: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
-0000bb30: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
-0000bb40: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000bb50: 6d65 616e 5f69 6e74 656e 7369 7479 5f63  mean_intensity_c
-0000bb60: 6832 5f6b 6579 290d 0a20 2020 2020 2020  h2_key)..       
+0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
+0000baf0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+0000bb00: 6563 6f6e 646b 6579 203a 2066 6c6f 6174  econdkey : float
+0000bb10: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000bb20: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+0000bb30: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
+0000bb40: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 2020 2065 6c73 653a 2020 2020 2020       else:      
-0000bba0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbd0: 2020 2020 2020 2020 544f 5441 4c5f 494e          TOTAL_IN
-0000bbe0: 5445 4e53 4954 5920 3d20 5370 6f74 6f62  TENSITY = Spotob
-0000bbf0: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
-0000bc00: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0000bc10: 315f 6b65 7929 0d0a 2020 2020 2020 2020  1_key)..        
+0000bb90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bba0: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+0000bbb0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000bbc0: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000bbd0: 7572 6661 6365 5f61 7265 615f 6b65 7929  urface_area_key)
+0000bbe0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
-0000bc50: 5f49 4e54 454e 5349 5459 203d 2053 706f  _INTENSITY = Spo
-0000bc60: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bc70: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000bc80: 6368 315f 6b65 7929 0d0a 2020 2020 2020  ch1_key)..      
+0000bc30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bc40: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
+0000bc50: 6579 3a20 666c 6f61 7428 5370 6f74 6f62  ey: float(Spotob
+0000bc60: 6a65 6374 2e67 6574 2873 656c 662e 6365  ject.get(self.ce
+0000bc70: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7929  llaxis_mask_key)
+0000bc80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 2020 2020 2020 5241 4449 5553 203d 2066        RADIUS = f
-0000bcc0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000bcd0: 6765 7428 7365 6c66 2e72 6164 6975 735f  get(self.radius_
-0000bce0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0000bce0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2051 5541 4c49 5459 203d 2066 6c6f     QUALITY = flo
-0000bd20: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000bd30: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
-0000bd40: 6579 2929 2020 2020 200d 0a20 2020 2020  ey))     ..     
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000bd80: 454e 5349 5459 203d 2066 6c6f 6174 2854  ENSITY = float(T
-0000bd90: 4f54 414c 5f49 4e54 454e 5349 5459 290d  OTAL_INTENSITY).
-0000bda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd60: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000bd70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000bd80: 2073 656c 662e 756e 6971 7565 6964 5f6b   self.uniqueid_k
+0000bd90: 6579 206e 6f74 2069 6e20 5370 6f74 6f62  ey not in Spotob
+0000bda0: 6a65 6374 2e6b 6579 7328 293a 0d0a 2020  ject.keys():..  
 0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
-0000bdd0: 4e5f 494e 5445 4e53 4954 5920 3d20 666c  N_INTENSITY = fl
-0000bde0: 6f61 7428 4d45 414e 5f49 4e54 454e 5349  oat(MEAN_INTENSI
-0000bdf0: 5459 290d 0a20 2020 2020 2020 2020 2020  TY)..           
+0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-0000be30: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000be40: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
+0000be10: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
+0000be20: 7465 6374 6f72 6368 616e 6e65 6c20 3d3d  tectorchannel ==
+0000be30: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be70: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
-0000be80: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
-0000be90: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
+0000be70: 4e54 454e 5349 5459 203d 2053 706f 746f  NTENSITY = Spoto
+0000be80: 626a 6563 742e 6765 7428 7365 6c66 2e74  bject.get(self.t
+0000be90: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0000bea0: 6832 5f6b 6579 290d 0a20 2020 2020 2020  h2_key)..       
 0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 2020 7365 6c66 2e66 7261 6d65 6964      self.frameid
-0000bed0: 5f6b 6579 203a 2069 6e74 2866 6c6f 6174  _key : int(float
-0000bee0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bef0: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000bf00: 2929 292c 0d0a 2020 2020 2020 2020 2020  ))),..          
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
+0000bee0: 4e5f 494e 5445 4e53 4954 5920 3d20 5370  N_INTENSITY = Sp
+0000bef0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bf00: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
+0000bf10: 5f63 6832 5f6b 6579 290d 0a20 2020 2020  _ch2_key)..     
 0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
-0000bf40: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000bf50: 6a65 6374 2e67 6574 2873 656c 662e 7a70  ject.get(self.zp
-0000bf60: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf40: 2020 2020 2020 2065 6c73 653a 2020 2020         else:    
+0000bf50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 2020 2020 2020 2020 2073 656c 662e 7970           self.yp
-0000bfa0: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
-0000bfb0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bfc0: 7365 6c66 2e79 706f 7369 645f 6b65 7929  self.yposid_key)
-0000bfd0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000bf80: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000bf90: 494e 5445 4e53 4954 5920 3d20 5370 6f74  INTENSITY = Spot
+0000bfa0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bfb0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+0000bfc0: 6368 315f 6b65 7929 0d0a 2020 2020 2020  ch1_key)..      
+0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c000: 7365 6c66 2e78 706f 7369 645f 6b65 7920  self.xposid_key 
-0000c010: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
-0000c020: 6374 2e67 6574 2873 656c 662e 7870 6f73  ct.get(self.xpos
-0000c030: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000bff0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000c000: 414e 5f49 4e54 454e 5349 5459 203d 2053  AN_INTENSITY = S
+0000c010: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000c020: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000c030: 795f 6368 315f 6b65 7929 0d0a 2020 2020  y_ch1_key)..    
 0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0000c070: 6c5f 696e 7465 6e73 6974 795f 6b65 7920  l_intensity_key 
-0000c080: 3a20 544f 5441 4c5f 494e 5445 4e53 4954  : TOTAL_INTENSIT
-0000c090: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
+0000c060: 2020 2020 2020 2020 5241 4449 5553 203d          RADIUS =
+0000c070: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c080: 742e 6765 7428 7365 6c66 2e72 6164 6975  t.get(self.radiu
+0000c090: 735f 6b65 7929 290d 0a20 2020 2020 2020  s_key))..       
 0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000c0d0: 6974 795f 6b65 7920 3a20 4d45 414e 5f49  ity_key : MEAN_I
-0000c0e0: 4e54 454e 5349 5459 2c0d 0a20 2020 2020  NTENSITY,..     
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0c0: 2020 2020 2051 5541 4c49 5459 203d 2066       QUALITY = f
+0000c0d0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000c0e0: 6765 7428 7365 6c66 2e71 7561 6c69 7479  get(self.quality
+0000c0f0: 5f6b 6579 2929 2020 2020 200d 0a20 2020  _key))     ..   
 0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-0000c120: 7573 5f6b 6579 203a 2052 4144 4955 532c  us_key : RADIUS,
-0000c130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c160: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-0000c170: 2051 5541 4c49 5459 0d0a 2020 2020 2020   QUALITY..      
-0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1a0: 2020 7d0d 0a20 2020 2020 2020 0d0a 2020    }..       ..  
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c120: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
+0000c130: 4e54 454e 5349 5459 203d 2066 6c6f 6174  NTENSITY = float
+0000c140: 2854 4f54 414c 5f49 4e54 454e 5349 5459  (TOTAL_INTENSITY
+0000c150: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000c180: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000c190: 666c 6f61 7428 4d45 414e 5f49 4e54 454e  float(MEAN_INTEN
+0000c1a0: 5349 5459 290d 0a20 2020 2020 2020 2020  SITY)..         
 0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c1d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000c1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1f0: 200d 0a0d 0a20 2020 2064 6566 205f 7370   ....    def _sp
-0000c200: 6f74 5f63 6f6d 7075 7465 7228 7365 6c66  ot_computer(self
-0000c210: 2c20 6672 616d 6529 3a0d 0a0d 0a20 2020  , frame):....   
-0000c220: 2020 2020 2020 2066 6f72 2053 706f 746f         for Spoto
-0000c230: 626a 6563 7420 696e 2066 7261 6d65 2e66  bject in frame.f
-0000c240: 696e 6461 6c6c 2827 5370 6f74 2729 3a0d  indall('Spot'):.
-0000c250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c260: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
-0000c270: 6520 6f62 6a65 6374 2077 6974 6820 756e  e object with un
-0000c280: 6971 7565 2063 656c 6c20 4944 0d0a 2020  ique cell ID..  
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-0000c2b0: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-0000c2c0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000c2d0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000c2f0: 4765 7420 7468 6520 545a 5958 206c 6f63  Get the TZYX loc
-0000c300: 6174 696f 6e20 6f66 2074 6865 2063 656c  ation of the cel
-0000c310: 6c73 2069 6e20 7468 6174 2066 7261 6d65  ls in that frame
-0000c320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c330: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000c340: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000c350: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
-0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c370: 2020 2020 2020 2020 2069 6620 5370 6f74           if Spot
-0000c380: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000c390: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000c3a0: 6368 325f 6b65 7929 2069 7320 6e6f 7420  ch2_key) is not 
-0000c3b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000c3e0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000c3f0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000c400: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000c410: 5f69 6e74 656e 7369 7479 5f63 6832 5f6b  _intensity_ch2_k
-0000c420: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c440: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000c450: 414e 5f49 4e54 454e 5349 5459 203d 2066  AN_INTENSITY = f
-0000c460: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000c470: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000c480: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
-0000c490: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1d0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+0000c1e0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000c1f0: 656c 6c5f 6964 5d20 3d20 7b0d 0a20 2020  ell_id] = {..   
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c220: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
+0000c230: 6c6c 6964 5f6b 6579 3a20 696e 7428 6365  llid_key: int(ce
+0000c240: 6c6c 5f69 6429 2c20 0d0a 2020 2020 2020  ll_id), ..      
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c270: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
+0000c280: 6964 5f6b 6579 203a 2069 6e74 2866 6c6f  id_key : int(flo
+0000c290: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000c2a0: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
+0000c2b0: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
+0000c2f0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000c300: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000c310: 7a70 6f73 6964 5f6b 6579 2929 2c0d 0a20  zposid_key)),.. 
+0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c350: 7970 6f73 6964 5f6b 6579 203a 2066 6c6f  yposid_key : flo
+0000c360: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000c370: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
+0000c380: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3b0: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
+0000c3c0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000c3d0: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
+0000c3e0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c410: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+0000c420: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+0000c430: 7920 3a20 544f 5441 4c5f 494e 5445 4e53  y : TOTAL_INTENS
+0000c440: 4954 592c 0d0a 2020 2020 2020 2020 2020  ITY,..          
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
+0000c480: 6e73 6974 795f 6b65 7920 3a20 4d45 414e  nsity_key : MEAN
+0000c490: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
 0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4e0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
-0000c4f0: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
+0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4c0: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000c4d0: 6469 7573 5f6b 6579 203a 2052 4144 4955  dius_key : RADIU
+0000c4e0: 532c 0d0a 2020 2020 2020 2020 2020 2020  S,..            
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000c520: 414e 5f49 4e54 454e 5349 5459 203d 202d  AN_INTENSITY = -
-0000c530: 3120 2020 2020 2020 0d0a 2020 2020 2020  1       ..      
+0000c510: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+0000c520: 203a 2051 5541 4c49 5459 0d0a 2020 2020   : QUALITY..    
+0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 656c 7365 3a20 2020 2020 2020 200d    else:        .
-0000c560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2069 6620 5370 6f74 6f62 6a65 6374 2e67   if Spotobject.g
-0000c590: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000c5a0: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000c5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000c5f0: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
-0000c600: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c610: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000c620: 7479 5f63 6831 5f6b 6579 2929 0d0a 2020  ty_ch1_key))..  
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c550: 2020 2020 7d0d 0a20 2020 2020 2020 0d0a      }..       ..
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000c580: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
+0000c5b0: 7370 6f74 5f63 6f6d 7075 7465 7228 7365  spot_computer(se
+0000c5c0: 6c66 2c20 6672 616d 6529 3a0d 0a0d 0a20  lf, frame):.... 
+0000c5d0: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
+0000c5e0: 746f 626a 6563 7420 696e 2066 7261 6d65  tobject in frame
+0000c5f0: 2e66 696e 6461 6c6c 2827 5370 6f74 2729  .findall('Spot')
+0000c600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c610: 2020 2020 2020 2020 2020 2023 2043 7265             # Cre
+0000c620: 6174 6520 6f62 6a65 6374 2077 6974 6820  ate object with 
+0000c630: 756e 6971 7565 2063 656c 6c20 4944 0d0a  unique cell ID..
 0000c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c650: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000c660: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000c670: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000c680: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000c690: 6368 315f 6b65 7929 290d 0a20 2020 2020  ch1_key))..     
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c6c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6e0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
-0000c6f0: 494e 5445 4e53 4954 5920 3d20 2d31 0d0a  INTENSITY = -1..
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c650: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
+0000c660: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
+0000c670: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
+0000c680: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2320 4765 7420 7468 6520 545a 5958 206c  # Get the TZYX l
+0000c6b0: 6f63 6174 696f 6e20 6f66 2074 6865 2063  ocation of the c
+0000c6c0: 656c 6c73 2069 6e20 7468 6174 2066 7261  ells in that fra
+0000c6d0: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
+0000c6e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000c6f0: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
+0000c700: 6e65 6c20 3d3d 2031 3a0d 0a20 2020 2020  nel == 1:..     
 0000c710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c720: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
-0000c730: 454e 5349 5459 203d 202d 3120 2020 2020  ENSITY = -1     
-0000c740: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c720: 2020 2020 2020 2020 2020 2069 6620 5370             if Sp
+0000c730: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c740: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000c750: 795f 6368 325f 6b65 7929 2069 7320 6e6f  y_ch2_key) is no
+0000c760: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
 0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c780: 2020 5241 4449 5553 203d 2066 6c6f 6174    RADIUS = float
-0000c790: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000c7a0: 7365 6c66 2e72 6164 6975 735f 6b65 7929  self.radius_key)
-0000c7b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000c7c0: 2020 2020 2020 2020 2020 2051 5541 4c49             QUALI
-0000c7d0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000c7e0: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000c7f0: 7561 6c69 7479 5f6b 6579 2929 0d0a 2020  uality_key))..  
-0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c810: 2020 2020 2020 7465 7374 6c6f 6361 7469        testlocati
-0000c820: 6f6e 203d 2028 666c 6f61 7428 5370 6f74  on = (float(Spot
-0000c830: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000c840: 7a70 6f73 6964 5f6b 6579 2929 2c20 666c  zposid_key)), fl
-0000c850: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000c860: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
-0000c870: 6579 2929 2c20 2066 6c6f 6174 2853 706f  ey)),  float(Spo
-0000c880: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000c890: 2e78 706f 7369 645f 6b65 7929 2929 0d0a  .xposid_key)))..
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8b0: 2020 2020 2020 2020 6672 616d 6520 3d20          frame = 
-0000c8c0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c8d0: 656c 662e 6672 616d 6569 645f 6b65 7929  elf.frameid_key)
-0000c8e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c8f0: 2020 2020 2020 2020 2020 6469 7374 616e            distan
-0000c900: 6365 5f63 656c 6c5f 6d61 736b 2c20 6d61  ce_cell_mask, ma
-0000c910: 736b 6365 6e74 726f 6964 203d 2073 656c  skcentroid = sel
-0000c920: 662e 5f67 6574 5f62 6f75 6e64 6172 795f  f._get_boundary_
-0000c930: 6469 7374 2866 7261 6d65 2c20 7465 7374  dist(frame, test
-0000c940: 6c6f 6361 7469 6f6e 290d 0a20 2020 2020  location)..     
-0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c960: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000c970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000c980: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-0000c990: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000c9a0: 5d20 3d20 7b0d 0a20 2020 2020 2020 2020  ] = {..         
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9c0: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
-0000c9d0: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
-0000c9e0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c790: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000c7a0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000c7b0: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
+0000c7c0: 616c 5f69 6e74 656e 7369 7479 5f63 6832  al_intensity_ch2
+0000c7d0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000c810: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c820: 742e 6765 7428 7365 6c66 2e6d 6561 6e5f  t.get(self.mean_
+0000c830: 696e 7465 6e73 6974 795f 6368 325f 6b65  intensity_ch2_ke
+0000c840: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 2020 2054 4f54 414c 5f49 4e54 454e 5349     TOTAL_INTENSI
+0000c8a0: 5459 203d 202d 310d 0a20 2020 2020 2020  TY = -1..       
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8d0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
+0000c8e0: 202d 3120 2020 2020 2020 0d0a 2020 2020   -1       ..    
+0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c900: 2020 2020 656c 7365 3a20 2020 2020 2020      else:       
+0000c910: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c930: 2020 2069 6620 5370 6f74 6f62 6a65 6374     if Spotobject
+0000c940: 2e67 6574 2873 656c 662e 746f 7461 6c5f  .get(self.total_
+0000c950: 696e 7465 6e73 6974 795f 6368 315f 6b65  intensity_ch1_ke
+0000c960: 7929 2069 7320 6e6f 7420 4e6f 6e65 3a0d  y) is not None:.
+0000c970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c990: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
+0000c9a0: 4e54 454e 5349 5459 203d 2066 6c6f 6174  NTENSITY = float
+0000c9b0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000c9c0: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000c9d0: 7369 7479 5f63 6831 5f6b 6579 2929 0d0a  sity_ch1_key))..
+0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca00: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000ca10: 203a 2069 6e74 2866 6c6f 6174 2853 706f   : int(float(Spo
-0000ca20: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000ca30: 2e66 7261 6d65 6964 5f6b 6579 2929 292c  .frameid_key))),
-0000ca40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ca60: 6c66 2e7a 706f 7369 645f 6b65 7920 3a20  lf.zposid_key : 
-0000ca70: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000ca80: 2e67 6574 2873 656c 662e 7a70 6f73 6964  .get(self.zposid
-0000ca90: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cab0: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-0000cac0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-0000cad0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000cae0: 2e79 706f 7369 645f 6b65 7929 292c 0d0a  .yposid_key)),..
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cb10: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
-0000cb20: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000cb30: 6574 2873 656c 662e 7870 6f73 6964 5f6b  et(self.xposid_k
-0000cb40: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb60: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-0000cb70: 7465 6e73 6974 795f 6b65 7920 3a20 544f  tensity_key : TO
-0000cb80: 5441 4c5f 494e 5445 4e53 4954 592c 0d0a  TAL_INTENSITY,..
-0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cbb0: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000cbc0: 6b65 7920 3a20 4d45 414e 5f49 4e54 454e  key : MEAN_INTEN
-0000cbd0: 5349 5459 2c0d 0a20 2020 2020 2020 2020  SITY,..         
-0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbf0: 2020 2073 656c 662e 7261 6469 7573 5f6b     self.radius_k
-0000cc00: 6579 203a 2052 4144 4955 532c 0d0a 2020  ey : RADIUS,..  
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-0000cc30: 7561 6c69 7479 5f6b 6579 203a 2051 5541  uality_key : QUA
-0000cc40: 4c49 5459 2c0d 0a20 2020 2020 2020 2020  LITY,..         
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 2020 2073 656c 662e 6469 7374 616e 6365     self.distance
-0000cc70: 5f63 656c 6c5f 6d61 736b 5f6b 6579 3a20  _cell_mask_key: 
-0000cc80: 666c 6f61 7428 6469 7374 616e 6365 5f63  float(distance_c
-0000cc90: 656c 6c5f 6d61 736b 292c 0d0a 2020 2020  ell_mask),..    
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccb0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-0000ccc0: 6b63 656e 7472 6f69 645f 7a5f 6b65 793a  kcentroid_z_key:
-0000ccd0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
-0000cce0: 6f69 645b 305d 292c 0d0a 2020 2020 2020  oid[0]),..      
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-0000cd10: 656e 7472 6f69 645f 795f 6b65 793a 2066  entroid_y_key: f
-0000cd20: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-0000cd30: 645b 315d 292c 0d0a 2020 2020 2020 2020  d[1]),..        
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd50: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
-0000cd60: 7472 6f69 645f 785f 6b65 793a 2066 6c6f  troid_x_key: flo
-0000cd70: 6174 286d 6173 6b63 656e 7472 6f69 645b  at(maskcentroid[
-0000cd80: 325d 2920 0d0a 2020 2020 2020 2020 2020  2]) ..          
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-0000cda0: 0a20 2020 2020 2020 0d0a 2020 2020 6465  .       ..    de
-0000cdb0: 6620 5f67 6574 5f6d 6173 7465 725f 786d  f _get_master_xm
-0000cdc0: 6c5f 6461 7461 2873 656c 6629 3a0d 0a20  l_data(self):.. 
-0000cdd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000cde0: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-0000cdf0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000ce00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ce10: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000ce20: 616e 6e65 6c5f 786d 6c5f 636f 6e74 656e  annel_xml_conten
-0000ce30: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
-0000ce40: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
-0000ce50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ce60: 2e78 6d6c 5f74 7265 6520 3d20 6574 2e70  .xml_tree = et.p
-0000ce70: 6172 7365 2873 656c 662e 786d 6c5f 7061  arse(self.xml_pa
-0000ce80: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000ce90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cea0: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
-0000ceb0: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
-0000cec0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000ced0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000cee0: 6861 6e6e 656c 5f78 6d6c 5f6e 616d 6520  hannel_xml_name 
-0000cef0: 3d20 2773 6563 6f6e 645f 6368 616e 6e65  = 'second_channe
-0000cf00: 6c5f 2720 2b20 6f73 2e70 6174 682e 7370  l_' + os.path.sp
-0000cf10: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
-0000cf20: 6173 656e 616d 6528 7365 6c66 2e78 6d6c  asename(self.xml
-0000cf30: 5f70 6174 6829 295b 305d 202b 2027 2e78  _path))[0] + '.x
-0000cf40: 6d6c 270d 0a20 2020 2020 2020 2020 2020  ml'..           
-0000cf50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cf60: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
-0000cf70: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-0000cf80: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000cf90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000cfa0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-0000cfb0: 7265 6174 655f 6368 616e 6e65 6c5f 7472  reate_channel_tr
-0000cfc0: 6565 2829 0d0a 0d0a 2020 2020 2020 2020  ee()....        
-0000cfd0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000cfe0: 6f62 6a65 6374 7320 3d20 7b7d 0d0a 2020  objects = {}..  
-0000cff0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000d000: 6e69 7175 655f 7072 6f70 6572 7469 6573  nique_properties
-0000d010: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-0000d020: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
-0000d030: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000d040: 2020 2020 2020 7365 6c66 2e44 6976 6964        self.Divid
-0000d050: 696e 6754 7261 636b 4964 7320 3d20 5b5d  ingTrackIds = []
-0000d060: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d070: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
-0000d080: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000d090: 2020 2020 7365 6c66 2e61 6c6c 5f74 7261      self.all_tra
-0000d0a0: 636b 5f70 726f 7065 7274 6965 7320 3d20  ck_properties = 
-0000d0b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000d0c0: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
-0000d0d0: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
-0000d0e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d0f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d100: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000d110: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000d120: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000d130: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000d140: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000d150: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000d160: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000d170: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000d180: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000d190: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000d1a0: 656c 662e 416c 6c54 7261 636b 4964 732e  elf.AllTrackIds.
-0000d1b0: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000d1c0: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000d1d0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
-0000d1e0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
-0000d1f0: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
-0000d200: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-0000d210: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000d220: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000d230: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000d240: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d250: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d260: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
-0000d270: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
-0000d280: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
-0000d290: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
-0000d2a0: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
-0000d2b0: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
-0000d2c0: 6865 2074 7261 636b 7320 6672 6f6d 2078  he tracks from x
-0000d2d0: 6d6c 0d0a 2020 2020 2020 2020 2020 2020  ml..            
-0000d2e0: 7365 6c66 2e74 7261 636b 7320 3d20 7365  self.tracks = se
-0000d2f0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000d300: 696e 6428 224d 6f64 656c 2229 2e66 696e  ind("Model").fin
-0000d310: 6428 2241 6c6c 5472 6163 6b73 2229 0d0a  d("AllTracks")..
-0000d320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d330: 2e73 6574 7469 6e67 7320 3d20 7365 6c66  .settings = self
-0000d340: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000d350: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000d360: 6e64 2822 496d 6167 6544 6174 6122 290d  nd("ImageData").
-0000d370: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d380: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
-0000d390: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000d3a0: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
-0000d3b0: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
-0000d3c0: 2020 2020 2073 656c 662e 7963 616c 6962       self.ycalib
-0000d3d0: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000d3e0: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000d3f0: 2822 7069 7865 6c68 6569 6768 7422 2929  ("pixelheight"))
-0000d400: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d410: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
-0000d420: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
-0000d430: 7469 6e67 732e 6765 7428 2276 6f78 656c  tings.get("voxel
-0000d440: 6465 7074 6822 2929 0d0a 2020 2020 2020  depth"))..      
-0000d450: 2020 2020 2020 7365 6c66 2e74 6361 6c69        self.tcali
-0000d460: 6272 6174 696f 6e20 3d20 696e 7428 666c  bration = int(fl
-0000d470: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000d480: 732e 6765 7428 2274 696d 6569 6e74 6572  s.get("timeinter
-0000d490: 7661 6c22 2929 290d 0a20 2020 2020 2020  val")))..       
-0000d4a0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000d4b0: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
-0000d4c0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000d4d0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
-0000d4e0: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
-0000d4f0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
-0000d500: 2020 2020 2073 656c 662e 6261 7369 6373       self.basics
-0000d510: 6574 7469 6e67 7320 3d20 7365 6c66 2e78  ettings = self.x
-0000d520: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
-0000d530: 2253 6574 7469 6e67 7322 292e 6669 6e64  "Settings").find
-0000d540: 2822 4261 7369 6353 6574 7469 6e67 7322  ("BasicSettings"
-0000d550: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0000d560: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000d570: 6e65 6c20 3d20 696e 7428 666c 6f61 7428  nel = int(float(
-0000d580: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
-0000d590: 7469 6e67 732e 6765 7428 2254 4152 4745  tings.get("TARGE
-0000d5a0: 545f 4348 414e 4e45 4c22 2929 290d 0a20  T_CHANNEL"))).. 
-0000d5b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d5c0: 7473 7461 7274 203d 2069 6e74 2866 6c6f  tstart = int(flo
-0000d5d0: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
-0000d5e0: 7469 6e67 732e 6765 7428 2274 7374 6172  tings.get("tstar
-0000d5f0: 7422 2929 290d 0a20 2020 2020 2020 2020  t")))..         
-0000d600: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
-0000d610: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
-0000d620: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
-0000d630: 2274 656e 6422 2929 2920 2020 2020 200d  "tend")))      .
-0000d640: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-0000d650: 7269 6e74 2827 4974 6572 6174 696e 6720  rint('Iterating 
-0000d660: 6f76 6572 2073 706f 7473 2069 6e20 6672  over spots in fr
-0000d670: 616d 6527 290d 0a20 2020 2020 2020 2020  ame')..         
-0000d680: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000d690: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
-0000d6a0: 7574 7572 6573 203d 205b 5d0d 0a0d 0a20  utures = [].... 
-0000d6b0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000d6c0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-0000d6d0: 6573 2e54 6872 6561 6450 6f6f 6c45 7865  es.ThreadPoolExe
-0000d6e0: 6375 746f 7228 6d61 785f 776f 726b 6572  cutor(max_worker
-0000d6f0: 7320 3d20 6f73 2e63 7075 5f63 6f75 6e74  s = os.cpu_count
-0000d700: 2829 2920 6173 2065 7865 6375 746f 723a  ()) as executor:
-0000d710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d720: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d730: 2020 2020 666f 7220 6672 616d 6520 696e      for frame in
-0000d740: 2073 656c 662e 5370 6f74 6f62 6a65 6374   self.Spotobject
-0000d750: 732e 6669 6e64 616c 6c28 2753 706f 7473  s.findall('Spots
-0000d760: 496e 4672 616d 6527 293a 0d0a 2020 2020  InFrame'):..    
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
-0000d790: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
-0000d7a0: 7375 626d 6974 2873 656c 662e 5f6d 6173  submit(self._mas
-0000d7b0: 7465 725f 7370 6f74 5f63 6f6d 7075 7465  ter_spot_compute
-0000d7c0: 722c 2066 7261 6d65 2929 0d0a 2020 2020  r, frame))..    
-0000d7d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000d7e0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d7f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000d820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d840: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000d850: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
-0000d860: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d890: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000d8a0: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8d0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
-0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8f0: 2020 2020 2020 2020 6c65 6e28 6675 7475          len(futu
-0000d900: 7265 7329 2c0d 0a20 2020 2020 2020 2020  res),..         
-0000d910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d920: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0000d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d940: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000d950: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-0000d960: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-0000d970: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
-0000d980: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-0000d990: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-0000d9a0: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d9d0: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000d9e0: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000da10: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000da20: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000da30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da50: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000da60: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
-0000da70: 6520 3d20 2073 656c 662e 636f 756e 740d  e =  self.count.
-0000da80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 2020 2020 2072 2e72 6573 756c 7428 2920       r.result() 
-0000dab0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
-0000dac0: 2020 2070 7269 6e74 2866 2749 7465 7261     print(f'Itera
-0000dad0: 7469 6e67 206f 7665 7220 7472 6163 6b73  ting over tracks
-0000dae0: 207b 6c65 6e28 7365 6c66 2e66 696c 7465   {len(self.filte
-0000daf0: 7265 645f 7472 6163 6b5f 6964 7329 7d27  red_track_ids)}'
-0000db00: 2920 200d 0a20 2020 2020 2020 2020 2020  )  ..           
-0000db10: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
-0000db20: 0a20 2020 2020 2020 2020 2020 2066 7574  .            fut
-0000db30: 7572 6573 203d 205b 5d0d 0a20 2020 2020  ures = []..     
-0000db40: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000db50: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000db60: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000db70: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000db80: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-0000db90: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-0000dba0: 5472 6163 6b73 220d 0a20 2020 2020 2020  Tracks"..       
-0000dbb0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000dbc0: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-0000dbd0: 203d 2028 302c 206c 656e 2873 656c 662e   = (0, len(self.
-0000dbe0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000dbf0: 6473 2929 0d0a 2020 2020 2020 2020 2020  ds))..          
-0000dc00: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000dc10: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
-0000dc20: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000dc30: 7220 7472 6163 6b20 696e 2073 656c 662e  r track in self.
-0000dc40: 7472 6163 6b73 2e66 696e 6461 6c6c 2827  tracks.findall('
-0000dc50: 5472 6163 6b27 293a 0d0a 2020 2020 2020  Track'):..      
-0000dc60: 2020 2020 2020 2020 2020 7472 6163 6b5f            track_
-0000dc70: 6964 203d 2069 6e74 2874 7261 636b 2e67  id = int(track.g
-0000dc80: 6574 2873 656c 662e 7472 6163 6b69 645f  et(self.trackid_
-0000dc90: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-0000dca0: 2020 2020 2020 2069 6620 7472 6163 6b5f         if track_
-0000dcb0: 6964 2069 6e20 7365 6c66 2e66 696c 7465  id in self.filte
-0000dcc0: 7265 645f 7472 6163 6b5f 6964 733a 0d0a  red_track_ids:..
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dce0: 2020 2020 7365 6c66 2e5f 6d61 7374 6572      self._master
-0000dcf0: 5f74 7261 636b 5f63 6f6d 7075 7465 7228  _track_computer(
-0000dd00: 7472 6163 6b2c 2074 7261 636b 5f69 6429  track, track_id)
-0000dd10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dd20: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000dd30: 202b 3d20 310d 0a20 2020 2020 2020 2020   += 1..         
-0000dd40: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000dd50: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
-0000dd60: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000ca00: 2020 2020 2020 2020 4d45 414e 5f49 4e54          MEAN_INT
+0000ca10: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
+0000ca20: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ca30: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000ca40: 795f 6368 315f 6b65 7929 290d 0a20 2020  y_ch1_key))..   
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000ca70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
+0000caa0: 4c5f 494e 5445 4e53 4954 5920 3d20 2d31  L_INTENSITY = -1
+0000cab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 2020 2020 2020 2020 2020 4d45 414e 5f49            MEAN_I
+0000cae0: 4e54 454e 5349 5459 203d 202d 3120 2020  NTENSITY = -1   
+0000caf0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 2020 2020 5241 4449 5553 203d 2066 6c6f      RADIUS = flo
+0000cb40: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000cb50: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
+0000cb60: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000cb70: 2020 2020 2020 2020 2020 2020 2051 5541               QUA
+0000cb80: 4c49 5459 203d 2066 6c6f 6174 2853 706f  LITY = float(Spo
+0000cb90: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000cba0: 2e71 7561 6c69 7479 5f6b 6579 2929 0d0a  .quality_key))..
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 2020 2020 2020 7465 7374 6c6f 6361          testloca
+0000cbd0: 7469 6f6e 203d 2028 666c 6f61 7428 5370  tion = (float(Sp
+0000cbe0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000cbf0: 662e 7a70 6f73 6964 5f6b 6579 2929 2c20  f.zposid_key)), 
+0000cc00: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000cc10: 2e67 6574 2873 656c 662e 7970 6f73 6964  .get(self.yposid
+0000cc20: 5f6b 6579 2929 2c20 2066 6c6f 6174 2853  _key)),  float(S
+0000cc30: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000cc40: 6c66 2e78 706f 7369 645f 6b65 7929 2929  lf.xposid_key)))
+0000cc50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cc60: 2020 2020 2020 2020 2020 6672 616d 6520            frame 
+0000cc70: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
+0000cc80: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
+0000cc90: 7929 0d0a 2020 2020 2020 2020 2020 2020  y)..            
+0000cca0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+0000ccb0: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+0000ccc0: 6d61 736b 6365 6e74 726f 6964 203d 2073  maskcentroid = s
+0000ccd0: 656c 662e 5f67 6574 5f62 6f75 6e64 6172  elf._get_boundar
+0000cce0: 795f 6469 7374 2866 7261 6d65 2c20 7465  y_dist(frame, te
+0000ccf0: 7374 6c6f 6361 7469 6f6e 290d 0a20 2020  stlocation)..   
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cd20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cd30: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+0000cd40: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000cd50: 6964 5d20 3d20 7b0d 0a20 2020 2020 2020  id] = {..       
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2073 656c 662e 6365 6c6c 6964       self.cellid
+0000cd80: 5f6b 6579 3a20 696e 7428 6365 6c6c 5f69  _key: int(cell_i
+0000cd90: 6429 2c20 0d0a 2020 2020 2020 2020 2020  d), ..          
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 7365 6c66 2e66 7261 6d65 6964 5f6b    self.frameid_k
+0000cdc0: 6579 203a 2069 6e74 2866 6c6f 6174 2853  ey : int(float(S
+0000cdd0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000cde0: 6c66 2e66 7261 6d65 6964 5f6b 6579 2929  lf.frameid_key))
+0000cdf0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce10: 7365 6c66 2e7a 706f 7369 645f 6b65 7920  self.zposid_key 
+0000ce20: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000ce30: 6374 2e67 6574 2873 656c 662e 7a70 6f73  ct.get(self.zpos
+0000ce40: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2020 2020 2020 2073 656c 662e 7970 6f73         self.ypos
+0000ce70: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
+0000ce80: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ce90: 6c66 2e79 706f 7369 645f 6b65 7929 292c  lf.yposid_key)),
+0000cea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cec0: 6c66 2e78 706f 7369 645f 6b65 7920 3a20  lf.xposid_key : 
+0000ced0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000cee0: 2e67 6574 2873 656c 662e 7870 6f73 6964  .get(self.xposid
+0000cef0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+0000cf20: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+0000cf30: 544f 5441 4c5f 494e 5445 4e53 4954 592c  TOTAL_INTENSITY,
+0000cf40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cf60: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
+0000cf70: 795f 6b65 7920 3a20 4d45 414e 5f49 4e54  y_key : MEAN_INT
+0000cf80: 454e 5349 5459 2c0d 0a20 2020 2020 2020  ENSITY,..       
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2073 656c 662e 7261 6469 7573       self.radius
+0000cfb0: 5f6b 6579 203a 2052 4144 4955 532c 0d0a  _key : RADIUS,..
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cfe0: 2e71 7561 6c69 7479 5f6b 6579 203a 2051  .quality_key : Q
+0000cff0: 5541 4c49 5459 2c0d 0a20 2020 2020 2020  UALITY,..       
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2073 656c 662e 6469 7374 616e       self.distan
+0000d020: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+0000d030: 3a20 666c 6f61 7428 6469 7374 616e 6365  : float(distance
+0000d040: 5f63 656c 6c5f 6d61 736b 292c 0d0a 2020  _cell_mask),..  
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000d070: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+0000d080: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
+0000d090: 7472 6f69 645b 305d 292c 0d0a 2020 2020  troid[0]),..    
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000d0c0: 6b63 656e 7472 6f69 645f 795f 6b65 793a  kcentroid_y_key:
+0000d0d0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
+0000d0e0: 6f69 645b 315d 292c 0d0a 2020 2020 2020  oid[1]),..      
+0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d100: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
+0000d110: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
+0000d120: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
+0000d130: 645b 325d 2920 0d0a 2020 2020 2020 2020  d[2]) ..        
+0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d150: 7d0d 0a20 2020 2020 2020 0d0a 2020 2020  }..       ..    
+0000d160: 6465 6620 5f67 6574 5f6d 6173 7465 725f  def _get_master_
+0000d170: 786d 6c5f 6461 7461 2873 656c 6629 3a0d  xml_data(self):.
+0000d180: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d190: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
+0000d1a0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+0000d1b0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000d1c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d1d0: 6368 616e 6e65 6c5f 786d 6c5f 636f 6e74  channel_xml_cont
+0000d1e0: 656e 7420 3d20 7365 6c66 2e78 6d6c 5f63  ent = self.xml_c
+0000d1f0: 6f6e 7465 6e74 0d0a 2020 2020 2020 2020  ontent..        
+0000d200: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d210: 6c66 2e78 6d6c 5f74 7265 6520 3d20 6574  lf.xml_tree = et
+0000d220: 2e70 6172 7365 2873 656c 662e 786d 6c5f  .parse(self.xml_
+0000d230: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
+0000d240: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d250: 662e 786d 6c5f 726f 6f74 203d 2073 656c  f.xml_root = sel
+0000d260: 662e 786d 6c5f 7472 6565 2e67 6574 726f  f.xml_tree.getro
+0000d270: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
+0000d280: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d290: 2e63 6861 6e6e 656c 5f78 6d6c 5f6e 616d  .channel_xml_nam
+0000d2a0: 6520 3d20 2773 6563 6f6e 645f 6368 616e  e = 'second_chan
+0000d2b0: 6e65 6c5f 2720 2b20 6f73 2e70 6174 682e  nel_' + os.path.
+0000d2c0: 7370 6c69 7465 7874 286f 732e 7061 7468  splitext(os.path
+0000d2d0: 2e62 6173 656e 616d 6528 7365 6c66 2e78  .basename(self.x
+0000d2e0: 6d6c 5f70 6174 6829 295b 305d 202b 2027  ml_path))[0] + '
+0000d2f0: 2e78 6d6c 270d 0a20 2020 2020 2020 2020  .xml'..         
+0000d300: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d310: 662e 6368 616e 6e65 6c5f 786d 6c5f 7061  f.channel_xml_pa
+0000d320: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+0000d330: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
+0000d340: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
+0000d350: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d360: 5f63 7265 6174 655f 6368 616e 6e65 6c5f  _create_channel_
+0000d370: 7472 6565 2829 0d0a 0d0a 2020 2020 2020  tree()....      
+0000d380: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000d390: 655f 6f62 6a65 6374 7320 3d20 7b7d 0d0a  e_objects = {}..
+0000d3a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d3b0: 2e75 6e69 7175 655f 7072 6f70 6572 7469  .unique_properti
+0000d3c0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
+0000d3d0: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000d3e0: 636b 4964 7320 3d20 5b5d 0d0a 2020 2020  ckIds = []..    
+0000d3f0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
+0000d400: 6964 696e 6754 7261 636b 4964 7320 3d20  idingTrackIds = 
+0000d410: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000d420: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+0000d430: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000d440: 2020 2020 2020 7365 6c66 2e61 6c6c 5f74        self.all_t
+0000d450: 7261 636b 5f70 726f 7065 7274 6965 7320  rack_properties 
+0000d460: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+0000d470: 2020 7365 6c66 2e73 706c 6974 5f70 6f69    self.split_poi
+0000d480: 6e74 735f 7469 6d65 7320 3d20 5b5d 0d0a  nts_times = []..
+0000d490: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000d4a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d4b0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000d4c0: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
+0000d4d0: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+0000d4e0: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+0000d4f0: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+0000d500: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+0000d510: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
+0000d520: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000d530: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
+0000d540: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d550: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+0000d560: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
+0000d570: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
+0000d580: 2020 2020 2020 2073 656c 662e 4469 7669         self.Divi
+0000d590: 6469 6e67 5472 6163 6b49 6473 2e61 7070  dingTrackIds.app
+0000d5a0: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
+0000d5b0: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
+0000d5c0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
+0000d5d0: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000d5e0: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000d5f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000d600: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000d610: 2020 2020 2020 2073 656c 662e 5370 6f74         self.Spot
+0000d620: 6f62 6a65 6374 7320 3d20 7365 6c66 2e78  objects = self.x
+0000d630: 6d6c 5f63 6f6e 7465 6e74 2e66 696e 6428  ml_content.find(
+0000d640: 274d 6f64 656c 2729 2e66 696e 6428 2741  'Model').find('A
+0000d650: 6c6c 5370 6f74 7327 290d 0a20 2020 2020  llSpots')..     
+0000d660: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+0000d670: 2074 6865 2074 7261 636b 7320 6672 6f6d   the tracks from
+0000d680: 2078 6d6c 0d0a 2020 2020 2020 2020 2020   xml..          
+0000d690: 2020 7365 6c66 2e74 7261 636b 7320 3d20    self.tracks = 
+0000d6a0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000d6b0: 2e66 696e 6428 224d 6f64 656c 2229 2e66  .find("Model").f
+0000d6c0: 696e 6428 2241 6c6c 5472 6163 6b73 2229  ind("AllTracks")
+0000d6d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d6e0: 6c66 2e73 6574 7469 6e67 7320 3d20 7365  lf.settings = se
+0000d6f0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000d700: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000d710: 6669 6e64 2822 496d 6167 6544 6174 6122  find("ImageData"
+0000d720: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000d730: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
+0000d740: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
+0000d750: 7474 696e 6773 2e67 6574 2822 7069 7865  ttings.get("pixe
+0000d760: 6c77 6964 7468 2229 290d 0a20 2020 2020  lwidth"))..     
+0000d770: 2020 2020 2020 2073 656c 662e 7963 616c         self.ycal
+0000d780: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000d790: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000d7a0: 6574 2822 7069 7865 6c68 6569 6768 7422  et("pixelheight"
+0000d7b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000d7c0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+0000d7d0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000d7e0: 6574 7469 6e67 732e 6765 7428 2276 6f78  ettings.get("vox
+0000d7f0: 656c 6465 7074 6822 2929 0d0a 2020 2020  eldepth"))..    
+0000d800: 2020 2020 2020 2020 7365 6c66 2e74 6361          self.tca
+0000d810: 6c69 6272 6174 696f 6e20 3d20 696e 7428  libration = int(
+0000d820: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
+0000d830: 6e67 732e 6765 7428 2274 696d 6569 6e74  ngs.get("timeint
+0000d840: 6572 7661 6c22 2929 290d 0a20 2020 2020  erval")))..     
+0000d850: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+0000d860: 6374 6f72 7365 7474 696e 6773 203d 2073  ctorsettings = s
+0000d870: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000d880: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000d890: 2e66 696e 6428 2244 6574 6563 746f 7253  .find("DetectorS
+0000d8a0: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
+0000d8b0: 2020 2020 2020 2073 656c 662e 6261 7369         self.basi
+0000d8c0: 6373 6574 7469 6e67 7320 3d20 7365 6c66  csettings = self
+0000d8d0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
+0000d8e0: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
+0000d8f0: 6e64 2822 4261 7369 6353 6574 7469 6e67  nd("BasicSetting
+0000d900: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+0000d910: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
+0000d920: 616e 6e65 6c20 3d20 696e 7428 666c 6f61  annel = int(floa
+0000d930: 7428 7365 6c66 2e64 6574 6563 746f 7273  t(self.detectors
+0000d940: 6574 7469 6e67 732e 6765 7428 2254 4152  ettings.get("TAR
+0000d950: 4745 545f 4348 414e 4e45 4c22 2929 290d  GET_CHANNEL"))).
+0000d960: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d970: 662e 7473 7461 7274 203d 2069 6e74 2866  f.tstart = int(f
+0000d980: 6c6f 6174 2873 656c 662e 6261 7369 6373  loat(self.basics
+0000d990: 6574 7469 6e67 732e 6765 7428 2274 7374  ettings.get("tst
+0000d9a0: 6172 7422 2929 290d 0a20 2020 2020 2020  art")))..       
+0000d9b0: 2020 2020 2073 656c 662e 7465 6e64 203d       self.tend =
+0000d9c0: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
+0000d9d0: 6261 7369 6373 6574 7469 6e67 732e 6765  basicsettings.ge
+0000d9e0: 7428 2274 656e 6422 2929 2920 2020 2020  t("tend")))     
+0000d9f0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000da00: 2070 7269 6e74 2827 4974 6572 6174 696e   print('Iteratin
+0000da10: 6720 6f76 6572 2073 706f 7473 2069 6e20  g over spots in 
+0000da20: 6672 616d 6527 290d 0a20 2020 2020 2020  frame')..       
+0000da30: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000da40: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000da50: 2066 7574 7572 6573 203d 205b 5d0d 0a0d   futures = []...
+0000da60: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000da70: 6820 636f 6e63 7572 7265 6e74 2e66 7574  h concurrent.fut
+0000da80: 7572 6573 2e54 6872 6561 6450 6f6f 6c45  ures.ThreadPoolE
+0000da90: 7865 6375 746f 7228 6d61 785f 776f 726b  xecutor(max_work
+0000daa0: 6572 7320 3d20 6f73 2e63 7075 5f63 6f75  ers = os.cpu_cou
+0000dab0: 6e74 2829 2920 6173 2065 7865 6375 746f  nt()) as executo
+0000dac0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+0000dad0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000dae0: 2020 2020 2020 666f 7220 6672 616d 6520        for frame 
+0000daf0: 696e 2073 656c 662e 5370 6f74 6f62 6a65  in self.Spotobje
+0000db00: 6374 732e 6669 6e64 616c 6c28 2753 706f  cts.findall('Spo
+0000db10: 7473 496e 4672 616d 6527 293a 0d0a 2020  tsInFrame'):..  
+0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db30: 2020 2020 2020 2020 2020 6675 7475 7265            future
+0000db40: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
+0000db50: 722e 7375 626d 6974 2873 656c 662e 5f6d  r.submit(self._m
+0000db60: 6173 7465 725f 7370 6f74 5f63 6f6d 7075  aster_spot_compu
+0000db70: 7465 722c 2066 7261 6d65 2929 0d0a 2020  ter, frame))..  
+0000db80: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000db90: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000dba0: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+0000dbb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbd0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000dc00: 5f62 6172 2e6c 6162 656c 203d 2022 436f  _bar.label = "Co
+0000dc10: 6c6c 6563 7469 6e67 2053 706f 7473 220d  llecting Spots".
+0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+0000dc50: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc80: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dca0: 2020 2020 2020 2020 2020 6c65 6e28 6675            len(fu
+0000dcb0: 7475 7265 7329 2c0d 0a20 2020 2020 2020  tures),..       
+0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcd0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000dd00: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+0000dd10: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
+0000dd20: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+0000dd30: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+0000dd40: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+0000dd50: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
+0000dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd80: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000dd90: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
-0000dda0: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
-0000ddb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ddc0: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-0000ddd0: 6520 6973 206e 6f74 204e 6f6e 653a 2020  e is not None:  
-0000dde0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ddf0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 7365 6c66 2e5f 6372 6561 7465 5f73    self._create_s
-0000de20: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-0000de30: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
-0000de40: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000de50: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-0000de60: 6f72 2028 6b2c 7629 2069 6e20 7365 6c66  or (k,v) in self
-0000de70: 2e67 7261 7068 5f73 706c 6974 2e69 7465  .graph_split.ite
-0000de80: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dea0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
-0000ded0: 6420 3d20 2069 6e74 2866 6c6f 6174 2873  d =  int(float(s
-0000dee0: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-0000def0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000df00: 6e74 2866 6c6f 6174 286b 2929 5d5b 7365  nt(float(k))][se
-0000df10: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
-0000df20: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
-0000df50: 203d 2069 6e74 2866 6c6f 6174 2873 7472   = int(float(str
-0000df60: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-0000df70: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-0000df80: 2866 6c6f 6174 2876 2929 5d5b 7365 6c66  (float(v))][self
-0000df90: 2e75 6e69 7175 6569 645f 6b65 795d 2929  .uniqueid_key]))
-0000dfa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000dfc0: 656c 662e 6772 6170 685f 7472 6163 6b73  elf.graph_tracks
-0000dfd0: 5b64 6175 6768 7465 725f 7472 6163 6b5f  [daughter_track_
-0000dfe0: 6964 5d20 3d20 7061 7265 6e74 5f74 7261  id] = parent_tra
-0000dff0: 636b 5f69 640d 0a0d 0a20 2020 2020 2020  ck_id....       
-0000e000: 2020 2020 2070 7269 6e74 2827 6765 7474       print('gett
-0000e010: 696e 6720 6174 7472 6962 7574 6573 2729  ing attributes')
-0000e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e030: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000e040: 6c66 2e5f 6765 745f 6174 7472 6962 7574  lf._get_attribut
-0000e050: 6573 2829 0d0a 2020 2020 2020 2020 2020  es()..          
-0000e060: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-0000e070: 656c 662e 636f 756e 7420 3d20 300d 0a20  elf.count = 0.. 
-0000e080: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-0000e090: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
-0000e0a0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000e0b0: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000e0e0: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-0000e0f0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e120: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e130: 735f 6261 722e 6c61 6265 6c20 3d20 224a  s_bar.label = "J
-0000e140: 7573 7420 6f6e 6520 6d6f 7265 2074 6869  ust one more thi
-0000e150: 6e67 220d 0a20 2020 2020 2020 2020 2020  ng"..           
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e180: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-0000e190: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd80: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
+0000dd90: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddc0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000ddd0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000dde0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000de10: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+0000de20: 6c75 6520 3d20 2073 656c 662e 636f 756e  lue =  self.coun
+0000de30: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de50: 2020 2020 2020 2072 2e72 6573 756c 7428         r.result(
+0000de60: 2920 2020 200d 0a0d 0a20 2020 2020 2020  )    ....       
+0000de70: 2020 2020 2070 7269 6e74 2866 2749 7465       print(f'Ite
+0000de80: 7261 7469 6e67 206f 7665 7220 7472 6163  rating over trac
+0000de90: 6b73 207b 6c65 6e28 7365 6c66 2e66 696c  ks {len(self.fil
+0000dea0: 7465 7265 645f 7472 6163 6b5f 6964 7329  tered_track_ids)
+0000deb0: 7d27 2920 200d 0a20 2020 2020 2020 2020  }')  ..         
+0000dec0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+0000ded0: 300d 0a20 2020 2020 2020 2020 2020 2066  0..            f
+0000dee0: 7574 7572 6573 203d 205b 5d0d 0a20 2020  utures = []..   
+0000def0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000df00: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+0000df10: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000df20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000df30: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+0000df40: 6265 6c20 3d20 2243 6f6c 6c65 6374 696e  bel = "Collectin
+0000df50: 6720 5472 6163 6b73 220d 0a20 2020 2020  g Tracks"..     
+0000df60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000df70: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+0000df80: 6765 203d 2028 302c 206c 656e 2873 656c  ge = (0, len(sel
+0000df90: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+0000dfa0: 5f69 6473 2929 0d0a 2020 2020 2020 2020  _ids))..        
+0000dfb0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000dfc0: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
+0000dfd0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000dfe0: 666f 7220 7472 6163 6b20 696e 2073 656c  for track in sel
+0000dff0: 662e 7472 6163 6b73 2e66 696e 6461 6c6c  f.tracks.findall
+0000e000: 2827 5472 6163 6b27 293a 0d0a 2020 2020  ('Track'):..    
+0000e010: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+0000e020: 6b5f 6964 203d 2069 6e74 2874 7261 636b  k_id = int(track
+0000e030: 2e67 6574 2873 656c 662e 7472 6163 6b69  .get(self.tracki
+0000e040: 645f 6b65 7929 290d 0a20 2020 2020 2020  d_key))..       
+0000e050: 2020 2020 2020 2020 2069 6620 7472 6163           if trac
+0000e060: 6b5f 6964 2069 6e20 7365 6c66 2e66 696c  k_id in self.fil
+0000e070: 7465 7265 645f 7472 6163 6b5f 6964 733a  tered_track_ids:
+0000e080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e090: 2020 2020 2020 7365 6c66 2e5f 6d61 7374        self._mast
+0000e0a0: 6572 5f74 7261 636b 5f63 6f6d 7075 7465  er_track_compute
+0000e0b0: 7228 7472 6163 6b2c 2074 7261 636b 5f69  r(track, track_i
+0000e0c0: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+0000e0d0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+0000e0e0: 6e74 202b 3d20 310d 0a20 2020 2020 2020  nt += 1..       
+0000e0f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e100: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000e110: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000e140: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+0000e150: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
+0000e160: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000e170: 662e 6368 616e 6e65 6c5f 7365 675f 696d  f.channel_seg_im
+0000e180: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+0000e190: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e1a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1c0: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
-0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-0000e200: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
-0000e210: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
-0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e240: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 2020 2020 7365 6c66 2e5f 6372 6561 7465      self._create
+0000e1d0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
+0000e1e0: 786d 6c28 290d 0a20 2020 2020 2020 2020  xml()..         
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0000e210: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+0000e220: 6c66 2e67 7261 7068 5f73 706c 6974 2e69  lf.graph_split.i
+0000e230: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e250: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e270: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e280: 735f 6261 722e 7368 6f77 2829 0d0a 2020  s_bar.show()..  
-0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000e2c0: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000e2d0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
+0000e270: 2020 6461 7567 6874 6572 5f74 7261 636b    daughter_track
+0000e280: 5f69 6420 3d20 2069 6e74 2866 6c6f 6174  _id =  int(float
+0000e290: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
+0000e2a0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000e2b0: 5b69 6e74 2866 6c6f 6174 286b 2929 5d5b  [int(float(k))][
+0000e2c0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+0000e2d0: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
 0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e300: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-0000e310: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-0000e320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 2020 2020 2073 656c 662e 5f66 696e 616c       self._final
-0000e350: 5f74 7261 636b 7328 7472 6163 6b5f 6964  _tracks(track_id
-0000e360: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-0000e370: 2020 6966 2073 656c 662e 666f 7572 6965    if self.fourie
-0000e380: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-0000e390: 2020 2020 2020 2070 7269 6e74 2827 636f         print('co
-0000e3a0: 6d70 7574 696e 6720 466f 7572 6965 7227  mputing Fourier'
-0000e3b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e3c0: 2020 2020 2020 7365 6c66 2e5f 636f 6d70        self._comp
-0000e3d0: 7574 655f 7068 656e 6f74 7970 6573 2829  ute_phenotypes()
-0000e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e400: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-0000e410: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-0000e420: 6d61 7465 2829 2020 2020 2020 2020 0d0a  mate()        ..
-0000e430: 0d0a 0d0a 2020 2020 6465 6620 5f63 7265  ....    def _cre
-0000e440: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
-0000e450: 656c 5f78 6d6c 2873 656c 6629 3a0d 0a20  el_xml(self):.. 
-0000e460: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000e2f0: 2020 2070 6172 656e 745f 7472 6163 6b5f     parent_track_
+0000e300: 6964 203d 2069 6e74 2866 6c6f 6174 2873  id = int(float(s
+0000e310: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
+0000e320: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+0000e330: 6e74 2866 6c6f 6174 2876 2929 5d5b 7365  nt(float(v))][se
+0000e340: 6c66 2e75 6e69 7175 6569 645f 6b65 795d  lf.uniqueid_key]
+0000e350: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 2073 656c 662e 6772 6170 685f 7472 6163   self.graph_trac
+0000e380: 6b73 5b64 6175 6768 7465 725f 7472 6163  ks[daughter_trac
+0000e390: 6b5f 6964 5d20 3d20 7061 7265 6e74 5f74  k_id] = parent_t
+0000e3a0: 7261 636b 5f69 640d 0a0d 0a20 2020 2020  rack_id....     
+0000e3b0: 2020 2020 2020 2070 7269 6e74 2827 6765         print('ge
+0000e3c0: 7474 696e 6720 6174 7472 6962 7574 6573  tting attributes
+0000e3d0: 2729 2020 2020 2020 2020 2020 2020 2020  ')              
+0000e3e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e3f0: 7365 6c66 2e5f 6765 745f 6174 7472 6962  self._get_attrib
+0000e400: 7574 6573 2829 0d0a 2020 2020 2020 2020  utes()..        
+0000e410: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e420: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
+0000e430: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000e440: 2074 7261 636b 5f69 6420 696e 2073 656c   track_id in sel
+0000e450: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+0000e460: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
 0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e480: 7072 696e 7428 2754 7261 6e73 6665 7272  print('Transferr
-0000e490: 696e 6720 584d 4c27 2920 2020 0d0a 2020  ing XML')   ..  
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4b0: 2020 6368 616e 6e65 6c5f 6669 6c74 6572    channel_filter
-0000e4c0: 6564 5f74 7261 636b 7320 3d20 5b5d 2020  ed_tracks = []  
-0000e4d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
-0000e500: 6e20 7365 6c66 2e78 6d6c 5f72 6f6f 742e  n self.xml_root.
-0000e510: 6974 6572 2827 5370 6f74 2729 3a0d 0a20  iter('Spot'):.. 
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e530: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-0000e540: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
-0000e550: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
-0000e560: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
-0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-0000e590: 6420 696e 2073 656c 662e 6368 616e 6e65  d in self.channe
-0000e5a0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000e5b0: 6f70 6572 7469 6573 2e6b 6579 7328 293a  operties.keys():
-0000e5c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000e480: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e490: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+0000e4a0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000e4e0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
+0000e4f0: 224a 7573 7420 6f6e 6520 6d6f 7265 2074  "Just one more t
+0000e500: 6869 6e67 220d 0a20 2020 2020 2020 2020  hing"..         
+0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e530: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000e540: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
+0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5b0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
+0000e5c0: 645f 7472 6163 6b5f 6964 7329 2c0d 0a20  d_track_ids),.. 
 0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000e610: 706f 7369 7469 6f6e 7820 3d20 2073 656c  positionx =  sel
-0000e620: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e630: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e640: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e78  [cell_id][self.x
-0000e650: 706f 7369 645f 6b65 795d 0d0a 2020 2020  posid_key]..    
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e680: 6e65 775f 706f 7369 7469 6f6e 7920 3d20  new_positiony = 
-0000e690: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e6a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e6b0: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e6c0: 6c66 2e79 706f 7369 645f 6b65 795d 0d0a  lf.yposid_key]..
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000e630: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+0000e670: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
+0000e680: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e6b0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+0000e6c0: 616c 7565 203d 2073 656c 662e 636f 756e  alue = self.coun
+0000e6d0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
 0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6f0: 2020 2020 6e65 775f 706f 7369 7469 6f6e      new_position
-0000e700: 7a20 3d20 2073 656c 662e 6368 616e 6e65  z =  self.channe
-0000e710: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000e720: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000e730: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-0000e740: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
-0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e760: 2020 2020 2020 2020 2020 6e65 775f 746f            new_to
-0000e770: 7461 6c5f 696e 7465 6e73 6974 7920 3d20  tal_intensity = 
-0000e780: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000e790: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e7a0: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
-0000e7b0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000e7c0: 795f 6b65 795d 0d0a 2020 2020 2020 2020  y_key]..        
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7e0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000e7f0: 6d65 616e 5f69 6e74 656e 7369 7479 203d  mean_intensity =
-0000e800: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000e810: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e820: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000e830: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000e840: 795f 6b65 795d 0d0a 0d0a 2020 2020 2020  y_key]....      
+0000e6f0: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
+0000e700: 616c 5f74 7261 636b 7328 7472 6163 6b5f  al_tracks(track_
+0000e710: 6964 2920 0d0a 0d0a 2020 2020 2020 2020  id) ....        
+0000e720: 2020 2020 6966 2073 656c 662e 666f 7572      if self.four
+0000e730: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
+0000e740: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000e750: 636f 6d70 7574 696e 6720 466f 7572 6965  computing Fourie
+0000e760: 7227 290d 0a20 2020 2020 2020 2020 2020  r')..           
+0000e770: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+0000e780: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
+0000e790: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
+0000e7a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000e7b0: 2020 2020 2020 2020 7365 6c66 2e5f 7465          self._te
+0000e7c0: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
+0000e7d0: 636b 6d61 7465 2829 2020 2020 2020 2020  ckmate()        
+0000e7e0: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f63  ......    def _c
+0000e7f0: 7265 6174 655f 7365 636f 6e64 5f63 6861  reate_second_cha
+0000e800: 6e6e 656c 5f78 6d6c 2873 656c 6629 3a0d  nnel_xml(self):.
+0000e810: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e830: 2020 7072 696e 7428 2754 7261 6e73 6665    print('Transfe
+0000e840: 7272 696e 6720 584d 4c27 2920 2020 0d0a  rring XML')   ..
 0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e870: 775f 7261 6469 7573 203d 2073 656c 662e  w_radius = self.
-0000e880: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000e890: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000e8a0: 656c 6c5f 6964 5d5b 7365 6c66 2e72 6164  ell_id][self.rad
-0000e8b0: 6975 735f 6b65 795d 0d0a 2020 2020 2020  ius_key]..      
-0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8d0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-0000e8e0: 775f 7175 616c 6974 7920 3d20 7365 6c66  w_quality = self
-0000e8f0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000e900: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000e910: 6365 6c6c 5f69 645d 5b73 656c 662e 7175  cell_id][self.qu
-0000e920: 616c 6974 795f 6b65 795d 0d0a 2020 2020  ality_key]..    
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 6e65 775f 6469 7374 616e 6365 5f63 656c  new_distance_cel
-0000e960: 6c5f 6d61 736b 203d 2073 656c 662e 6368  l_mask = self.ch
-0000e970: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000e980: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000e990: 6c5f 6964 5d5b 7365 6c66 2e64 6973 7461  l_id][self.dista
-0000e9a0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-0000e9b0: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000e9e0: 6a65 6374 2e73 6574 2873 656c 662e 7870  ject.set(self.xp
-0000e9f0: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
-0000ea00: 775f 706f 7369 7469 6f6e 7829 2920 2020  w_positionx))   
-0000ea10: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e860: 2020 2020 6368 616e 6e65 6c5f 6669 6c74      channel_filt
+0000e870: 6572 6564 5f74 7261 636b 7320 3d20 5b5d  ered_tracks = []
+0000e880: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8a0: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
+0000e8b0: 2069 6e20 7365 6c66 2e78 6d6c 5f72 6f6f   in self.xml_roo
+0000e8c0: 742e 6974 6572 2827 5370 6f74 2729 3a0d  t.iter('Spot'):.
+0000e8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e8e0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000e8f0: 6c5f 6964 203d 2069 6e74 2853 706f 746f  l_id = int(Spoto
+0000e900: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
+0000e910: 706f 7469 645f 6b65 7929 290d 0a20 2020  potid_key))..   
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e930: 2020 2020 2020 2020 2069 6620 6365 6c6c           if cell
+0000e940: 5f69 6420 696e 2073 656c 662e 6368 616e  _id in self.chan
+0000e950: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000e960: 7072 6f70 6572 7469 6573 2e6b 6579 7328  properties.keys(
+0000e970: 293a 2020 2020 2020 2020 0d0a 2020 2020  ):        ..    
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000e9c0: 775f 706f 7369 7469 6f6e 7820 3d20 2073  w_positionx =  s
+0000e9d0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000e9e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000e9f0: 6573 5b63 656c 6c5f 6964 5d5b 7365 6c66  es[cell_id][self
+0000ea00: 2e78 706f 7369 645f 6b65 795d 0d0a 2020  .xposid_key]..  
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
-0000ea40: 6374 2e73 6574 2873 656c 662e 7970 6f73  ct.set(self.ypos
-0000ea50: 6964 5f6b 6579 2c20 7374 7228 6e65 775f  id_key, str(new_
-0000ea60: 706f 7369 7469 6f6e 7929 290d 0a20 2020  positiony))..   
-0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea90: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000eaa0: 7365 6c66 2e7a 706f 7369 645f 6b65 792c  self.zposid_key,
-0000eab0: 2073 7472 286e 6577 5f70 6f73 6974 696f   str(new_positio
-0000eac0: 6e7a 2929 0d0a 0d0a 2020 2020 2020 2020  nz))....        
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000eaf0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000eb00: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000eb10: 6b65 792c 2073 7472 286e 6577 5f74 6f74  key, str(new_tot
-0000eb20: 616c 5f69 6e74 656e 7369 7479 2929 2020  al_intensity))  
-0000eb30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000eb60: 6563 742e 7365 7428 7365 6c66 2e6d 6561  ect.set(self.mea
-0000eb70: 6e5f 696e 7465 6e73 6974 795f 6b65 792c  n_intensity_key,
-0000eb80: 2073 7472 286e 6577 5f6d 6561 6e5f 696e   str(new_mean_in
-0000eb90: 7465 6e73 6974 7929 290d 0a20 2020 2020  tensity))..     
-0000eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000ebc0: 706f 746f 626a 6563 742e 7365 7428 7365  potobject.set(se
-0000ebd0: 6c66 2e72 6164 6975 735f 6b65 792c 2073  lf.radius_key, s
-0000ebe0: 7472 286e 6577 5f72 6164 6975 7329 2920  tr(new_radius)) 
-0000ebf0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ea30: 2020 6e65 775f 706f 7369 7469 6f6e 7920    new_positiony 
+0000ea40: 3d20 2073 656c 662e 6368 616e 6e65 6c5f  =  self.channel_
+0000ea50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000ea60: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000ea70: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+0000ea80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 2020 2020 2020 6e65 775f 706f 7369 7469        new_positi
+0000eab0: 6f6e 7a20 3d20 2073 656c 662e 6368 616e  onz =  self.chan
+0000eac0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000ead0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000eae0: 6964 5d5b 7365 6c66 2e7a 706f 7369 645f  id][self.zposid_
+0000eaf0: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000eb20: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
+0000eb30: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
+0000eb40: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000eb50: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000eb60: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000eb70: 6974 795f 6b65 795d 0d0a 2020 2020 2020  ity_key]..      
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000eba0: 775f 6d65 616e 5f69 6e74 656e 7369 7479  w_mean_intensity
+0000ebb0: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
+0000ebc0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+0000ebd0: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
+0000ebe0: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+0000ebf0: 6974 795f 6b65 795d 0d0a 0d0a 2020 2020  ity_key]....    
 0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec10: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000ec20: 6a65 6374 2e73 6574 2873 656c 662e 7175  ject.set(self.qu
-0000ec30: 616c 6974 795f 6b65 792c 2073 7472 286e  ality_key, str(n
-0000ec40: 6577 5f71 7561 6c69 7479 2929 0d0a 2020  ew_quality))..  
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000ec80: 2873 656c 662e 6469 7374 616e 6365 5f63  (self.distance_c
-0000ec90: 656c 6c5f 6d61 736b 5f6b 6579 2c20 7374  ell_mask_key, st
-0000eca0: 7228 6e65 775f 6469 7374 616e 6365 5f63  r(new_distance_c
-0000ecb0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 7472 6163 6b5f 6964 203d 2073 656c 662e  track_id = self.
-0000ecf0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000ed00: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-0000ed10: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-0000ed20: 662e 7472 6163 6b69 645f 6b65 795d 0d0a  f.trackid_key]..
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed50: 2020 2020 6368 616e 6e65 6c5f 6669 6c74      channel_filt
-0000ed60: 6572 6564 5f74 7261 636b 732e 6170 7065  ered_tracks.appe
-0000ed70: 6e64 2874 7261 636b 5f69 6429 0d0a 2020  nd(track_id)..  
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eda0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000edb0: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
-0000edc0: 5f74 7265 652e 7772 6974 6528 6f73 2e70  _tree.write(os.p
-0000edd0: 6174 682e 6a6f 696e 2873 656c 662e 6368  ath.join(self.ch
-0000ede0: 616e 6e65 6c5f 786d 6c5f 7061 7468 2c20  annel_xml_path, 
-0000edf0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000ee00: 5f6e 616d 6529 2920 0d0a 0d0a 2020 2020  _name)) ....    
-0000ee10: 6465 6620 5f67 6574 5f78 6d6c 5f64 6174  def _get_xml_dat
-0000ee20: 6128 7365 6c66 293a 0d0a 0d0a 2020 2020  a(self):....    
-0000ee30: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-0000ee60: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000ee70: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000ee80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ee90: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f63  lf.channel_xml_c
-0000eea0: 6f6e 7465 6e74 203d 2073 656c 662e 786d  ontent = self.xm
-0000eeb0: 6c5f 636f 6e74 656e 740d 0a20 2020 2020  l_content..     
-0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eed0: 2073 656c 662e 786d 6c5f 7472 6565 203d   self.xml_tree =
-0000eee0: 2065 742e 7061 7273 6528 7365 6c66 2e78   et.parse(self.x
-0000eef0: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef10: 7365 6c66 2e78 6d6c 5f72 6f6f 7420 3d20  self.xml_root = 
-0000ef20: 7365 6c66 2e78 6d6c 5f74 7265 652e 6765  self.xml_tree.ge
-0000ef30: 7472 6f6f 7428 290d 0a20 2020 2020 2020  troot()..       
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ef50: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000ef60: 6e61 6d65 203d 2027 7365 636f 6e64 5f63  name = 'second_c
-0000ef70: 6861 6e6e 656c 5f27 202b 206f 732e 7061  hannel_' + os.pa
-0000ef80: 7468 2e73 706c 6974 6578 7428 6f73 2e70  th.splitext(os.p
-0000ef90: 6174 682e 6261 7365 6e61 6d65 2873 656c  ath.basename(sel
-0000efa0: 662e 786d 6c5f 7061 7468 2929 5b30 5d20  f.xml_path))[0] 
-0000efb0: 2b20 272e 786d 6c27 0d0a 2020 2020 2020  + '.xml'..      
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000efe0: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0000eff0: 6469 726e 616d 6528 7365 6c66 2e78 6d6c  dirname(self.xml
-0000f000: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000f010: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f020: 6c66 2e5f 6372 6561 7465 5f63 6861 6e6e  lf._create_chann
-0000f030: 656c 5f74 7265 6528 290d 0a20 2020 2020  el_tree()..     
-0000f040: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f050: 6c66 2e61 7574 6f65 6e63 6f64 6572 5f6d  lf.autoencoder_m
-0000f060: 6f64 656c 2069 7320 6e6f 7420 4e6f 6e65  odel is not None
-0000f070: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
-0000f080: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
-0000f090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f0a0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000f0b0: 7374 6572 5f78 6d6c 5f63 6f6e 7465 6e74  ster_xml_content
-0000f0c0: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000f0d0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-0000f0e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f0f0: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
-0000f100: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
-0000f110: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
-0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f130: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
-0000f140: 6d6c 5f72 6f6f 7420 3d20 7365 6c66 2e6d  ml_root = self.m
-0000f150: 6173 7465 725f 786d 6c5f 7472 6565 2e67  aster_xml_tree.g
-0000f160: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-0000f190: 5f6e 616d 6520 3d20 276d 6173 7465 725f  _name = 'master_
-0000f1a0: 2720 2b20 7365 6c66 2e6d 6173 7465 725f  ' + self.master_
-0000f1b0: 6578 7472 615f 6e61 6d65 2020 2b20 6f73  extra_name  + os
-0000f1c0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
-0000f1d0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000f1e0: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
-0000f1f0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
-0000f200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f210: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000f220: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
-0000f230: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
-0000f240: 786d 6c5f 7061 7468 2920 2020 2020 200d  xml_path)      .
-0000f250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f260: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000f270: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0000f280: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
-0000f290: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-0000f2a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000f2b0: 7072 6f70 6572 7469 6573 203d 207b 7d0d  properties = {}.
-0000f2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f2d0: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000f2e0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000f2f0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
-0000f300: 6964 696e 6754 7261 636b 4964 7320 3d20  idingTrackIds = 
-0000f310: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-0000f320: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
-0000f330: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
-0000f340: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f350: 6c66 2e61 6c6c 5f74 7261 636b 5f70 726f  lf.all_track_pro
-0000f360: 7065 7274 6965 7320 3d20 5b5d 0d0a 2020  perties = []..  
-0000f370: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f380: 6c66 2e73 706c 6974 5f70 6f69 6e74 735f  lf.split_points_
-0000f390: 7469 6d65 7320 3d20 5b5d 0d0a 0d0a 2020  times = []....  
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f3d0: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
-0000f3e0: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
-0000f3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f400: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
-0000f410: 6163 6b49 6473 2e61 7070 656e 6428 4e6f  ackIds.append(No
-0000f420: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000f430: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000f440: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000f450: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
-0000f460: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000f470: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000f480: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
-0000f490: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
-0000f4a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f4b0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000f4c0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000f4d0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000f4e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f4f0: 2020 7365 6c66 2e4e 6f72 6d61 6c54 7261    self.NormalTra
-0000f500: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
-0000f510: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
-0000f520: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f540: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000f550: 2020 2073 656c 662e 5370 6f74 6f62 6a65     self.Spotobje
-0000f560: 6374 7320 3d20 7365 6c66 2e78 6d6c 5f63  cts = self.xml_c
-0000f570: 6f6e 7465 6e74 2e66 696e 6428 274d 6f64  ontent.find('Mod
-0000f580: 656c 2729 2e66 696e 6428 2741 6c6c 5370  el').find('AllSp
-0000f590: 6f74 7327 290d 0a20 2020 2020 2020 2020  ots')..         
-0000f5a0: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
-0000f5b0: 2074 6865 2074 7261 636b 7320 6672 6f6d   the tracks from
-0000f5c0: 2078 6d6c 0d0a 2020 2020 2020 2020 2020   xml..          
-0000f5d0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
-0000f5e0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000f5f0: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
-0000f600: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
-0000f610: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
-0000f620: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000f630: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-0000f640: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-0000f650: 7469 6e67 7322 292e 6669 6e64 2822 496d  tings").find("Im
-0000f660: 6167 6544 6174 6122 290d 0a20 2020 2020  ageData")..     
-0000f670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f680: 696d 6167 6573 697a 6520 3d20 2869 6e74  imagesize = (int
-0000f690: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
-0000f6a0: 696e 6773 2e67 6574 2822 6e66 7261 6d65  ings.get("nframe
-0000f6b0: 7322 2929 292c 696e 7428 666c 6f61 7428  s"))),int(float(
-0000f6c0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000f6d0: 7428 226e 736c 6963 6573 2229 2929 2c69  t("nslices"))),i
-0000f6e0: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
-0000f6f0: 7474 696e 6773 2e67 6574 2822 6865 6967  ttings.get("heig
-0000f700: 6874 2229 2929 2c20 2069 6e74 2866 6c6f  ht"))),  int(flo
-0000f710: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
-0000f720: 2e67 6574 2822 7769 6474 6822 2929 2929  .get("width"))))
-0000f730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f740: 2020 7072 696e 7428 6627 584d 4c20 6669    print(f'XML fi
-0000f750: 6c65 206d 6164 6520 7573 696e 6720 696d  le made using im
-0000f760: 6167 6520 6f66 207b 7365 6c66 2e69 6d61  age of {self.ima
-0000f770: 6765 7369 7a65 7d27 290d 0a20 2020 2020  gesize}')..     
-0000f780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f790: 7863 616c 6962 7261 7469 6f6e 203d 2066  xcalibration = f
-0000f7a0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
-0000f7b0: 6773 2e67 6574 2822 7069 7865 6c77 6964  gs.get("pixelwid
-0000f7c0: 7468 2229 290d 0a20 2020 2020 2020 2020  th"))..         
-0000f7d0: 2020 2020 2020 2073 656c 662e 7963 616c         self.ycal
-0000f7e0: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
-0000f7f0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000f800: 6574 2822 7069 7865 6c68 6569 6768 7422  et("pixelheight"
-0000f810: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000f820: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
-0000f830: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
-0000f840: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000f850: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
-0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f870: 7365 6c66 2e74 6361 6c69 6272 6174 696f  self.tcalibratio
-0000f880: 6e20 3d20 696e 7428 666c 6f61 7428 7365  n = int(float(se
-0000f890: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000f8a0: 2274 696d 6569 6e74 6572 7661 6c22 2929  "timeinterval"))
-0000f8b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f8c0: 2020 2073 656c 662e 6465 7465 6374 6f72     self.detector
-0000f8d0: 7365 7474 696e 6773 203d 2073 656c 662e  settings = self.
-0000f8e0: 786d 6c5f 636f 6e74 656e 742e 6669 6e64  xml_content.find
-0000f8f0: 2822 5365 7474 696e 6773 2229 2e66 696e  ("Settings").fin
-0000f900: 6428 2244 6574 6563 746f 7253 6574 7469  d("DetectorSetti
-0000f910: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
-0000f920: 2020 2020 2020 2073 656c 662e 6261 7369         self.basi
-0000f930: 6373 6574 7469 6e67 7320 3d20 7365 6c66  csettings = self
-0000f940: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f950: 6428 2253 6574 7469 6e67 7322 292e 6669  d("Settings").fi
-0000f960: 6e64 2822 4261 7369 6353 6574 7469 6e67  nd("BasicSetting
-0000f970: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000f980: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
-0000f990: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
-0000f9a0: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
-0000f9b0: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
-0000f9c0: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
-0000f9d0: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000f9e0: 2020 2020 2073 656c 662e 7473 7461 7274       self.tstart
-0000f9f0: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
-0000fa00: 662e 6261 7369 6373 6574 7469 6e67 732e  f.basicsettings.
-0000fa10: 6765 7428 2274 7374 6172 7422 2929 290d  get("tstart"))).
-0000fa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa30: 2073 656c 662e 7465 6e64 203d 2069 6e74   self.tend = int
-0000fa40: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
-0000fa50: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
-0000fa60: 656e 6422 2929 290d 0a20 2020 2020 2020  end")))..       
-0000fa70: 2020 2020 2020 2020 2073 656c 662e 5f67           self._g
-0000fa80: 6574 5f62 6f75 6e64 6172 795f 706f 696e  et_boundary_poin
-0000fa90: 7473 2829 0d0a 2020 2020 2020 2020 2020  ts()..          
-0000faa0: 2020 2020 2020 7072 696e 7428 2749 7465        print('Ite
-0000fab0: 7261 7469 6e67 206f 7665 7220 7370 6f74  rating over spot
-0000fac0: 7320 696e 2066 7261 6d65 2729 0d0a 2020  s in frame')..  
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fae0: 6c66 2e63 6f75 6e74 203d 2030 0d0a 2020  lf.count = 0..  
-0000faf0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-0000fb00: 7475 7265 7320 3d20 5b5d 0d0a 0d0a 2020  tures = []....  
-0000fb10: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-0000fb20: 7468 2063 6f6e 6375 7272 656e 742e 6675  th concurrent.fu
-0000fb30: 7475 7265 732e 5468 7265 6164 506f 6f6c  tures.ThreadPool
-0000fb40: 4578 6563 7574 6f72 286d 6178 5f77 6f72  Executor(max_wor
-0000fb50: 6b65 7273 203d 206f 732e 6370 755f 636f  kers = os.cpu_co
-0000fb60: 756e 7428 2929 2061 7320 6578 6563 7574  unt()) as execut
-0000fb70: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-0000fb80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000fb90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000fba0: 6f72 2066 7261 6d65 2069 6e20 7365 6c66  or frame in self
-0000fbb0: 2e53 706f 746f 626a 6563 7473 2e66 696e  .Spotobjects.fin
-0000fbc0: 6461 6c6c 2827 5370 6f74 7349 6e46 7261  dall('SpotsInFra
-0000fbd0: 6d65 2729 3a0d 0a20 2020 2020 2020 2020  me'):..         
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2020 2020 6675 7475 7265 732e 6170 7065      futures.appe
-0000fc00: 6e64 2865 7865 6375 746f 722e 7375 626d  nd(executor.subm
-0000fc10: 6974 2873 656c 662e 5f73 706f 745f 636f  it(self._spot_co
-0000fc20: 6d70 7574 6572 2c20 6672 616d 6529 290d  mputer, frame)).
-0000fc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc40: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-0000fc50: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-0000fc60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fca0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fcb0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000fcc0: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-0000fcd0: 7469 6e67 2053 706f 7473 220d 0a20 2020  ting Spots"..   
-0000fce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd00: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000fd10: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd40: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 2020 6c65 6e28 6675 7475 7265 7329 2c0d    len(futures),.
-0000fd80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fdd0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000fde0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
-0000fdf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000fe00: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
-0000fe10: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
-0000fe20: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe50: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000fe60: 6e74 203d 2073 656c 662e 636f 756e 7420  nt = self.count 
-0000fe70: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 6e65 775f 7261 6469 7573 203d 2073 656c  new_radius = sel
+0000ec30: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000ec40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000ec50: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e72  [cell_id][self.r
+0000ec60: 6164 6975 735f 6b65 795d 0d0a 2020 2020  adius_key]..    
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec90: 6e65 775f 7175 616c 6974 7920 3d20 7365  new_quality = se
+0000eca0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000ecb0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000ecc0: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000ecd0: 7175 616c 6974 795f 6b65 795d 0d0a 2020  quality_key]..  
+0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed00: 2020 6e65 775f 6469 7374 616e 6365 5f63    new_distance_c
+0000ed10: 656c 6c5f 6d61 736b 203d 2073 656c 662e  ell_mask = self.
+0000ed20: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+0000ed30: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000ed40: 656c 6c5f 6964 5d5b 7365 6c66 2e64 6973  ell_id][self.dis
+0000ed50: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
+0000ed60: 6b65 795d 0d0a 0d0a 2020 2020 2020 2020  key]....        
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed80: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000ed90: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000eda0: 7870 6f73 6964 5f6b 6579 2c20 7374 7228  xposid_key, str(
+0000edb0: 6e65 775f 706f 7369 7469 6f6e 7829 2920  new_positionx)) 
+0000edc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
+0000edf0: 6a65 6374 2e73 6574 2873 656c 662e 7970  ject.set(self.yp
+0000ee00: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
+0000ee10: 775f 706f 7369 7469 6f6e 7929 290d 0a20  w_positiony)).. 
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee40: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000ee50: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
+0000ee60: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
+0000ee70: 696f 6e7a 2929 0d0a 0d0a 2020 2020 2020  ionz))....      
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+0000eea0: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
+0000eeb0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000eec0: 795f 6b65 792c 2073 7472 286e 6577 5f74  y_key, str(new_t
+0000eed0: 6f74 616c 5f69 6e74 656e 7369 7479 2929  otal_intensity))
+0000eee0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef00: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000ef10: 626a 6563 742e 7365 7428 7365 6c66 2e6d  bject.set(self.m
+0000ef20: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+0000ef30: 792c 2073 7472 286e 6577 5f6d 6561 6e5f  y, str(new_mean_
+0000ef40: 696e 7465 6e73 6974 7929 290d 0a20 2020  intensity))..   
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef70: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
+0000ef80: 7365 6c66 2e72 6164 6975 735f 6b65 792c  self.radius_key,
+0000ef90: 2073 7472 286e 6577 5f72 6164 6975 7329   str(new_radius)
+0000efa0: 2920 2020 2020 0d0a 2020 2020 2020 2020  )     ..        
+0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efc0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
+0000efd0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
+0000efe0: 7175 616c 6974 795f 6b65 792c 2073 7472  quality_key, str
+0000eff0: 286e 6577 5f71 7561 6c69 7479 2929 0d0a  (new_quality))..
+0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f020: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000f030: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
+0000f040: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2c20  _cell_mask_key, 
+0000f050: 7374 7228 6e65 775f 6469 7374 616e 6365  str(new_distance
+0000f060: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f090: 2020 7472 6163 6b5f 6964 203d 2073 656c    track_id = sel
+0000f0a0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000f0b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000f0c0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+0000f0d0: 656c 662e 7472 6163 6b69 645f 6b65 795d  elf.trackid_key]
+0000f0e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2020 2020 6368 616e 6e65 6c5f 6669        channel_fi
+0000f110: 6c74 6572 6564 5f74 7261 636b 732e 6170  ltered_tracks.ap
+0000f120: 7065 6e64 2874 7261 636b 5f69 6429 0d0a  pend(track_id)..
+0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f150: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f160: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+0000f170: 6d6c 5f74 7265 652e 7772 6974 6528 6f73  ml_tree.write(os
+0000f180: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+0000f190: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
+0000f1a0: 2c20 7365 6c66 2e63 6861 6e6e 656c 5f78  , self.channel_x
+0000f1b0: 6d6c 5f6e 616d 6529 2920 0d0a 0d0a 2020  ml_name)) ....  
+0000f1c0: 2020 6465 6620 5f67 6574 5f78 6d6c 5f64    def _get_xml_d
+0000f1d0: 6174 6128 7365 6c66 293a 0d0a 0d0a 2020  ata(self):....  
+0000f1e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000f1f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f200: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+0000f210: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+0000f220: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f240: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
+0000f250: 5f63 6f6e 7465 6e74 203d 2073 656c 662e  _content = self.
+0000f260: 786d 6c5f 636f 6e74 656e 740d 0a20 2020  xml_content..   
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 2020 2073 656c 662e 786d 6c5f 7472 6565     self.xml_tree
+0000f290: 203d 2065 742e 7061 7273 6528 7365 6c66   = et.parse(self
+0000f2a0: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2020 7365 6c66 2e78 6d6c 5f72 6f6f 7420    self.xml_root 
+0000f2d0: 3d20 7365 6c66 2e78 6d6c 5f74 7265 652e  = self.xml_tree.
+0000f2e0: 6765 7472 6f6f 7428 290d 0a20 2020 2020  getroot()..     
+0000f2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f300: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000f310: 6c5f 6e61 6d65 203d 2027 7365 636f 6e64  l_name = 'second
+0000f320: 5f63 6861 6e6e 656c 5f27 202b 206f 732e  _channel_' + os.
+0000f330: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
+0000f340: 2e70 6174 682e 6261 7365 6e61 6d65 2873  .path.basename(s
+0000f350: 656c 662e 786d 6c5f 7061 7468 2929 5b30  elf.xml_path))[0
+0000f360: 5d20 2b20 272e 786d 6c27 0d0a 2020 2020  ] + '.xml'..    
+0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f380: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000f390: 6d6c 5f70 6174 6820 3d20 6f73 2e70 6174  ml_path = os.pat
+0000f3a0: 682e 6469 726e 616d 6528 7365 6c66 2e78  h.dirname(self.x
+0000f3b0: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3d0: 7365 6c66 2e5f 6372 6561 7465 5f63 6861  self._create_cha
+0000f3e0: 6e6e 656c 5f74 7265 6528 290d 0a20 2020  nnel_tree()..   
+0000f3f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f400: 7365 6c66 2e61 7574 6f65 6e63 6f64 6572  self.autoencoder
+0000f410: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
+0000f420: 6e65 2061 6e64 2073 656c 662e 7365 675f  ne and self.seg_
+0000f430: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000f440: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f460: 6d61 7374 6572 5f78 6d6c 5f63 6f6e 7465  master_xml_conte
+0000f470: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000f480: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000f490: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f4a0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7472  lf.master_xml_tr
+0000f4b0: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
+0000f4c0: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4e0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000f4f0: 5f78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  _xml_root = self
+0000f500: 2e6d 6173 7465 725f 786d 6c5f 7472 6565  .master_xml_tree
+0000f510: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
+0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f530: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+0000f540: 6d6c 5f6e 616d 6520 3d20 276d 6173 7465  ml_name = 'maste
+0000f550: 725f 2720 2b20 7365 6c66 2e6d 6173 7465  r_' + self.maste
+0000f560: 725f 6578 7472 615f 6e61 6d65 2020 2b20  r_extra_name  + 
+0000f570: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+0000f580: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
+0000f590: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
+0000f5a0: 295b 305d 202b 2027 2e78 6d6c 270d 0a20  )[0] + '.xml'.. 
+0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5c0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000f5d0: 725f 786d 6c5f 7061 7468 203d 206f 732e  r_xml_path = os.
+0000f5e0: 7061 7468 2e64 6972 6e61 6d65 2873 656c  path.dirname(sel
+0000f5f0: 662e 786d 6c5f 7061 7468 2920 2020 2020  f.xml_path)     
+0000f600: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f610: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f630: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
+0000f640: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0000f650: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000f660: 655f 7072 6f70 6572 7469 6573 203d 207b  e_properties = {
+0000f670: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+0000f680: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000f690: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000f6a0: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+0000f6b0: 6976 6964 696e 6754 7261 636b 4964 7320  ividingTrackIds 
+0000f6c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+0000f6d0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000f6e0: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
+0000f6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f700: 7365 6c66 2e61 6c6c 5f74 7261 636b 5f70  self.all_track_p
+0000f710: 726f 7065 7274 6965 7320 3d20 5b5d 0d0a  roperties = []..
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 7365 6c66 2e73 706c 6974 5f70 6f69 6e74  self.split_point
+0000f740: 735f 7469 6d65 7320 3d20 5b5d 0d0a 0d0a  s_times = []....
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f770: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f780: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
+0000f790: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
+0000f7a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f7b0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
+0000f7c0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000f7d0: 4e6f 6e65 290d 0a20 2020 2020 2020 2020  None)..         
+0000f7e0: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000f7f0: 616c 5472 6163 6b49 6473 2e61 7070 656e  alTrackIds.appen
+0000f800: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
+0000f810: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000f820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f830: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000f840: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
+0000f850: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
+0000f860: 2020 2020 2073 656c 662e 4469 7669 6469       self.Dividi
+0000f870: 6e67 5472 6163 6b49 6473 2e61 7070 656e  ngTrackIds.appen
+0000f880: 6428 7365 6c66 2e54 7261 636b 6964 426f  d(self.TrackidBo
+0000f890: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000f8a0: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000f8b0: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
+0000f8c0: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
+0000f8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f8f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f900: 2020 2020 2073 656c 662e 5370 6f74 6f62       self.Spotob
+0000f910: 6a65 6374 7320 3d20 7365 6c66 2e78 6d6c  jects = self.xml
+0000f920: 5f63 6f6e 7465 6e74 2e66 696e 6428 274d  _content.find('M
+0000f930: 6f64 656c 2729 2e66 696e 6428 2741 6c6c  odel').find('All
+0000f940: 5370 6f74 7327 290d 0a20 2020 2020 2020  Spots')..       
+0000f950: 2020 2020 2020 2020 2023 2045 7874 7261           # Extra
+0000f960: 6374 2074 6865 2074 7261 636b 7320 6672  ct the tracks fr
+0000f970: 6f6d 2078 6d6c 0d0a 2020 2020 2020 2020  om xml..        
+0000f980: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000f990: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
+0000f9a0: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
+0000f9b0: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
+0000f9c0: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
+0000f9d0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000f9e0: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+0000f9f0: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+0000fa00: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+0000fa10: 496d 6167 6544 6174 6122 290d 0a20 2020  ImageData")..   
+0000fa20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fa30: 662e 696d 6167 6573 697a 6520 3d20 2869  f.imagesize = (i
+0000fa40: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
+0000fa50: 7474 696e 6773 2e67 6574 2822 6e66 7261  ttings.get("nfra
+0000fa60: 6d65 7322 2929 292c 696e 7428 666c 6f61  mes"))),int(floa
+0000fa70: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000fa80: 6765 7428 226e 736c 6963 6573 2229 2929  get("nslices")))
+0000fa90: 2c69 6e74 2866 6c6f 6174 2873 656c 662e  ,int(float(self.
+0000faa0: 7365 7474 696e 6773 2e67 6574 2822 6865  settings.get("he
+0000fab0: 6967 6874 2229 2929 2c20 2069 6e74 2866  ight"))),  int(f
+0000fac0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000fad0: 6773 2e67 6574 2822 7769 6474 6822 2929  gs.get("width"))
+0000fae0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000faf0: 2020 2020 7072 696e 7428 6627 584d 4c20      print(f'XML 
+0000fb00: 6669 6c65 206d 6164 6520 7573 696e 6720  file made using 
+0000fb10: 696d 6167 6520 6f66 207b 7365 6c66 2e69  image of {self.i
+0000fb20: 6d61 6765 7369 7a65 7d27 290d 0a20 2020  magesize}')..   
+0000fb30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fb40: 662e 7863 616c 6962 7261 7469 6f6e 203d  f.xcalibration =
+0000fb50: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+0000fb60: 696e 6773 2e67 6574 2822 7069 7865 6c77  ings.get("pixelw
+0000fb70: 6964 7468 2229 290d 0a20 2020 2020 2020  idth"))..       
+0000fb80: 2020 2020 2020 2020 2073 656c 662e 7963           self.yc
+0000fb90: 616c 6962 7261 7469 6f6e 203d 2066 6c6f  alibration = flo
+0000fba0: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000fbb0: 2e67 6574 2822 7069 7865 6c68 6569 6768  .get("pixelheigh
+0000fbc0: 7422 2929 0d0a 2020 2020 2020 2020 2020  t"))..          
+0000fbd0: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
+0000fbe0: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000fbf0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000fc00: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
+0000fc10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fc20: 2020 7365 6c66 2e74 6361 6c69 6272 6174    self.tcalibrat
+0000fc30: 696f 6e20 3d20 696e 7428 666c 6f61 7428  ion = int(float(
+0000fc40: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000fc50: 7428 2274 696d 6569 6e74 6572 7661 6c22  t("timeinterval"
+0000fc60: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000fc70: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+0000fc80: 6f72 7365 7474 696e 6773 203d 2073 656c  orsettings = sel
+0000fc90: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000fca0: 6e64 2822 5365 7474 696e 6773 2229 2e66  nd("Settings").f
+0000fcb0: 696e 6428 2244 6574 6563 746f 7253 6574  ind("DetectorSet
+0000fcc0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+0000fcd0: 2020 2020 2020 2020 2073 656c 662e 6261           self.ba
+0000fce0: 7369 6373 6574 7469 6e67 7320 3d20 7365  sicsettings = se
+0000fcf0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000fd00: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
+0000fd10: 6669 6e64 2822 4261 7369 6353 6574 7469  find("BasicSetti
+0000fd20: 6e67 7322 290d 0a20 2020 2020 2020 2020  ngs")..         
+0000fd30: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
+0000fd40: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
+0000fd50: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
+0000fd60: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
+0000fd70: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
+0000fd80: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
+0000fd90: 2020 2020 2020 2073 656c 662e 7473 7461         self.tsta
+0000fda0: 7274 203d 2069 6e74 2866 6c6f 6174 2873  rt = int(float(s
+0000fdb0: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
+0000fdc0: 732e 6765 7428 2274 7374 6172 7422 2929  s.get("tstart"))
+0000fdd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fde0: 2020 2073 656c 662e 7465 6e64 203d 2069     self.tend = i
+0000fdf0: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+0000fe00: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+0000fe10: 2274 656e 6422 2929 290d 0a20 2020 2020  "tend")))..     
+0000fe20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fe30: 5f67 6574 5f62 6f75 6e64 6172 795f 706f  _get_boundary_po
+0000fe40: 696e 7473 2829 0d0a 2020 2020 2020 2020  ints()..        
+0000fe50: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
+0000fe60: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
+0000fe70: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
 0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000fea0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-0000feb0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000fe90: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000feb0: 6675 7475 7265 7320 3d20 5b5d 0d0a 0d0a  futures = []....
 0000fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fef0: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-0000ff00: 7565 203d 2020 7365 6c66 2e63 6f75 6e74  ue =  self.count
-0000ff10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff30: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
-0000ff40: 6c74 2829 0d0a 2020 2020 2020 2020 2020  lt()..          
-0000ff50: 2020 2020 2020 7072 696e 7428 6627 4974        print(f'It
-0000ff60: 6572 6174 696e 6720 6f76 6572 2074 7261  erating over tra
-0000ff70: 636b 7320 7b6c 656e 2873 656c 662e 6669  cks {len(self.fi
-0000ff80: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000ff90: 297d 2729 2020 0d0a 2020 2020 2020 2020  )}')  ..        
-0000ffa0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000ffb0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-0000ffc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ffd0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-0000ffe0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000fff0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010000: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00010010: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-00010020: 7469 6e67 2054 7261 636b 7322 0d0a 2020  ting Tracks"..  
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010050: 6261 722e 7261 6e67 6520 3d20 2830 2c20  bar.range = (0, 
-00010060: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-00010070: 645f 7472 6163 6b5f 6964 7329 290d 0a20  d_track_ids)).. 
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000100a0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
-000100b0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000100c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000100d0: 206d 6178 5f6c 656e 6774 6820 3d20 3020   max_length = 0 
-000100e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000100f0: 2020 2020 2066 6f72 2074 7261 636b 2069       for track i
-00010100: 6e20 7365 6c66 2e74 7261 636b 732e 6669  n self.tracks.fi
-00010110: 6e64 616c 6c28 2754 7261 636b 2729 3a0d  ndall('Track'):.
-00010120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010130: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-00010140: 696e 7428 7472 6163 6b2e 6765 7428 7365  int(track.get(se
-00010150: 6c66 2e74 7261 636b 6964 5f6b 6579 2929  lf.trackid_key))
-00010160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010170: 2020 2020 2020 6966 2074 7261 636b 5f69        if track_i
-00010180: 6420 696e 2073 656c 662e 6669 6c74 6572  d in self.filter
-00010190: 6564 5f74 7261 636b 5f69 6473 3a0d 0a20  ed_track_ids:.. 
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 2020 2020 2020 2020 2020 2064 6967 6974             digit
-000101c0: 5f6c 656e 6774 6820 3d20 6c65 6e28 7374  _length = len(st
-000101d0: 7228 7472 6163 6b5f 6964 2929 0d0a 2020  r(track_id))..  
-000101e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101f0: 2020 2020 2020 2020 2020 6966 2064 6967            if dig
-00010200: 6974 5f6c 656e 6774 6820 3e20 6d61 785f  it_length > max_
-00010210: 6c65 6e67 7468 3a0d 0a20 2020 2020 2020  length:..       
-00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 2020 2020 2020 2020 206d 6178 5f6c 656e           max_len
-00010240: 6774 6820 3d20 6469 6769 745f 6c65 6e67  gth = digit_leng
-00010250: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
-00010260: 2020 2020 7365 6c66 2e6d 6178 5f74 7261      self.max_tra
-00010270: 636b 5f64 6967 6974 203d 206d 6178 5f6c  ck_digit = max_l
-00010280: 656e 6774 6820 2020 2020 2020 2020 2020  ength           
-00010290: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000102a0: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
-000102b0: 2069 6e20 7365 6c66 2e74 7261 636b 732e   in self.tracks.
-000102c0: 6669 6e64 616c 6c28 2754 7261 636b 2729  findall('Track')
-000102d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000102e0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-000102f0: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
-00010300: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-00010310: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00010320: 2020 2020 2020 2020 6966 2074 7261 636b          if track
-00010330: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
-00010340: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
-00010350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010360: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
-00010370: 7261 636b 5f63 6f6d 7075 7465 7228 7472  rack_computer(tr
-00010380: 6163 6b2c 2074 7261 636b 5f69 6429 0d0a  ack, track_id)..
-00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-000103b0: 6e74 202b 3d20 310d 0a20 2020 2020 2020  nt += 1..       
-000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103d0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-000103e0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-000103f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010420: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
-00010430: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-00010440: 2020 2020 2020 6966 2073 656c 662e 6368        if self.ch
-00010450: 616e 6e65 6c5f 7365 675f 696d 6167 6520  annel_seg_image 
-00010460: 6973 206e 6f74 204e 6f6e 653a 2020 0d0a  is not None:  ..
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-00010490: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
-000104a0: 656c 5f78 6d6c 2829 0d0a 2020 2020 2020  el_xml()..      
-000104b0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-000104c0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000104d0: 7220 286b 2c76 2920 696e 2073 656c 662e  r (k,v) in self.
-000104e0: 6772 6170 685f 7370 6c69 742e 6974 656d  graph_split.item
-000104f0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010520: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00010530: 6175 6768 7465 725f 7472 6163 6b5f 6964  aughter_track_id
-00010540: 203d 2020 696e 7428 666c 6f61 7428 7374   =  int(float(st
-00010550: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
-00010560: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00010570: 7428 666c 6f61 7428 6b29 295d 5b73 656c  t(float(k))][sel
-00010580: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
-00010590: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 7061 7265 6e74 5f74 7261 636b 5f69 6420  parent_track_id 
-000105c0: 3d20 696e 7428 666c 6f61 7428 7374 7228  = int(float(str(
-000105d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000105e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000105f0: 666c 6f61 7428 7629 295d 5b73 656c 662e  float(v))][self.
-00010600: 756e 6971 7565 6964 5f6b 6579 5d29 2929  uniqueid_key])))
-00010610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010620: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010630: 6c66 2e67 7261 7068 5f74 7261 636b 735b  lf.graph_tracks[
-00010640: 6461 7567 6874 6572 5f74 7261 636b 5f69  daughter_track_i
-00010650: 645d 203d 2070 6172 656e 745f 7472 6163  d] = parent_trac
-00010660: 6b5f 6964 0d0a 2020 2020 2020 2020 2020  k_id..          
-00010670: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-00010680: 6174 7472 6962 7574 6573 2829 0d0a 2020  attributes()..  
-00010690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000106a0: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
-000106b0: 725f 6d6f 6465 6c20 616e 6420 7365 6c66  r_model and self
-000106c0: 2e73 6567 5f69 6d61 6765 2069 7320 6e6f  .seg_image is no
-000106d0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106f0: 7072 696e 7428 2747 6574 7469 6e67 2061  print('Getting a
-00010700: 7574 6f65 6e63 6f64 6572 2063 6c6f 7564  utoencoder cloud
-00010710: 7327 290d 0a20 2020 2020 2020 2020 2020  s')..           
-00010720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010730: 2e5f 6173 7369 676e 5f63 6c75 7374 6572  ._assign_cluster
-00010740: 5f63 6c61 7373 2829 0d0a 2020 2020 2020  _class()..      
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 2070 7269 6e74 2827 4372 6561 7469 6e67   print('Creating
-00010770: 206d 6173 7465 7220 786d 6c27 290d 0a20   master xml').. 
-00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
-000107a0: 7465 5f6d 6173 7465 725f 786d 6c28 290d  te_master_xml().
-000107b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000107c0: 2073 656c 662e 636f 756e 7420 3d20 3020   self.count = 0 
-000107d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000107e0: 2020 666f 7220 7472 6163 6b5f 6964 2069    for track_id i
-000107f0: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
-00010800: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010830: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00010840: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00010850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010880: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-00010890: 656c 203d 2022 4a75 7374 206f 6e65 206d  el = "Just one m
-000108a0: 6f72 6520 7468 696e 6722 0d0a 2020 2020  ore thing"..    
+0000fed0: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
+0000fee0: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
+0000fef0: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
+0000ff00: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
+0000ff10: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
+0000ff20: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
+0000ff30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff50: 2066 6f72 2066 7261 6d65 2069 6e20 7365   for frame in se
+0000ff60: 6c66 2e53 706f 746f 626a 6563 7473 2e66  lf.Spotobjects.f
+0000ff70: 696e 6461 6c6c 2827 5370 6f74 7349 6e46  indall('SpotsInF
+0000ff80: 7261 6d65 2729 3a0d 0a20 2020 2020 2020  rame'):..       
+0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ffa0: 2020 2020 2020 6675 7475 7265 732e 6170        futures.ap
+0000ffb0: 7065 6e64 2865 7865 6375 746f 722e 7375  pend(executor.su
+0000ffc0: 626d 6974 2873 656c 662e 5f73 706f 745f  bmit(self._spot_
+0000ffd0: 636f 6d70 7574 6572 2c20 6672 616d 6529  computer, frame)
+0000ffe0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fff0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00010000: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
+00010010: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010030: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010060: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00010070: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+00010080: 6563 7469 6e67 2053 706f 7473 220d 0a20  ecting Spots".. 
+00010090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100b0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+000100c0: 5f62 6172 2e72 616e 6765 203d 2028 0d0a  _bar.range = (..
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
+00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 6c65 6e28 6675 7475 7265 7329      len(futures)
+00010130: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010150: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010170: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010180: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010190: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
+000101a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000101b0: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
+000101c0: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
+000101d0: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
+000101e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010210: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
+00010220: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
+00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010240: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010250: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+00010260: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+00010270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000102a0: 662e 7072 6f67 7265 7373 5f62 6172 2e76  f.progress_bar.v
+000102b0: 616c 7565 203d 2020 7365 6c66 2e63 6f75  alue =  self.cou
+000102c0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102e0: 2020 2020 2020 2020 2020 2020 722e 7265              r.re
+000102f0: 7375 6c74 2829 0d0a 2020 2020 2020 2020  sult()..        
+00010300: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00010310: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
+00010320: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
+00010330: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+00010340: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
+00010350: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010360: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+00010370: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010380: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+00010390: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+000103a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103b0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+000103c0: 6172 2e6c 6162 656c 203d 2022 436f 6c6c  ar.label = "Coll
+000103d0: 6563 7469 6e67 2054 7261 636b 7322 0d0a  ecting Tracks"..
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010400: 735f 6261 722e 7261 6e67 6520 3d20 2830  s_bar.range = (0
+00010410: 2c20 6c65 6e28 7365 6c66 2e66 696c 7465  , len(self.filte
+00010420: 7265 645f 7472 6163 6b5f 6964 7329 290d  red_track_ids)).
+00010430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010440: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010450: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+00010460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010470: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00010480: 2020 206d 6178 5f6c 656e 6774 6820 3d20     max_length = 
+00010490: 3020 2020 200d 0a20 2020 2020 2020 2020  0    ..         
+000104a0: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
+000104b0: 2069 6e20 7365 6c66 2e74 7261 636b 732e   in self.tracks.
+000104c0: 6669 6e64 616c 6c28 2754 7261 636b 2729  findall('Track')
+000104d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000104e0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+000104f0: 3d20 696e 7428 7472 6163 6b2e 6765 7428  = int(track.get(
+00010500: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+00010510: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00010520: 2020 2020 2020 2020 6966 2074 7261 636b          if track
+00010530: 5f69 6420 696e 2073 656c 662e 6669 6c74  _id in self.filt
+00010540: 6572 6564 5f74 7261 636b 5f69 6473 3a0d  ered_track_ids:.
+00010550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010560: 2020 2020 2020 2020 2020 2020 2064 6967               dig
+00010570: 6974 5f6c 656e 6774 6820 3d20 6c65 6e28  it_length = len(
+00010580: 7374 7228 7472 6163 6b5f 6964 2929 0d0a  str(track_id))..
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+000105b0: 6967 6974 5f6c 656e 6774 6820 3e20 6d61  igit_length > ma
+000105c0: 785f 6c65 6e67 7468 3a0d 0a20 2020 2020  x_length:..     
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 2020 2020 2020 2020 2020 206d 6178 5f6c             max_l
+000105f0: 656e 6774 6820 3d20 6469 6769 745f 6c65  ength = digit_le
+00010600: 6e67 7468 0d0a 2020 2020 2020 2020 2020  ngth..          
+00010610: 2020 2020 2020 7365 6c66 2e6d 6178 5f74        self.max_t
+00010620: 7261 636b 5f64 6967 6974 203d 206d 6178  rack_digit = max
+00010630: 5f6c 656e 6774 6820 2020 2020 2020 2020  _length         
+00010640: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010650: 2020 2020 2020 2020 2066 6f72 2074 7261           for tra
+00010660: 636b 2069 6e20 7365 6c66 2e74 7261 636b  ck in self.track
+00010670: 732e 6669 6e64 616c 6c28 2754 7261 636b  s.findall('Track
+00010680: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00010690: 2020 2020 2020 2020 2074 7261 636b 5f69           track_i
+000106a0: 6420 3d20 696e 7428 7472 6163 6b2e 6765  d = int(track.ge
+000106b0: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
+000106c0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+000106d0: 2020 2020 2020 2020 2020 6966 2074 7261            if tra
+000106e0: 636b 5f69 6420 696e 2073 656c 662e 6669  ck_id in self.fi
+000106f0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00010700: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010720: 5f74 7261 636b 5f63 6f6d 7075 7465 7228  _track_computer(
+00010730: 7472 6163 6b2c 2074 7261 636b 5f69 6429  track, track_id)
+00010740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010750: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010760: 6f75 6e74 202b 3d20 310d 0a20 2020 2020  ount += 1..     
+00010770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010780: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
+00010790: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
+000107a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107c0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000107d0: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
+000107e0: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
+000107f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010800: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
+00010810: 6520 6973 206e 6f74 204e 6f6e 653a 2020  e is not None:  
+00010820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010830: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+00010840: 7265 6174 655f 7365 636f 6e64 5f63 6861  reate_second_cha
+00010850: 6e6e 656c 5f78 6d6c 2829 0d0a 2020 2020  nnel_xml()..    
+00010860: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00010870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010880: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
+00010890: 662e 6772 6170 685f 7370 6c69 742e 6974  f.graph_split.it
+000108a0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
 000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-000108e0: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-000108f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-00010930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
-00010960: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-00010970: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00010980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000109b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000109d0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-000109e0: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010a10: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
-00010a20: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108e0: 2064 6175 6768 7465 725f 7472 6163 6b5f   daughter_track_
+000108f0: 6964 203d 2020 696e 7428 666c 6f61 7428  id =  int(float(
+00010900: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
+00010910: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00010920: 696e 7428 666c 6f61 7428 6b29 295d 5b73  int(float(k))][s
+00010930: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+00010940: 5d29 2929 0d0a 2020 2020 2020 2020 2020  ])))..          
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 2020 7061 7265 6e74 5f74 7261 636b 5f69    parent_track_i
+00010970: 6420 3d20 696e 7428 666c 6f61 7428 7374  d = int(float(st
+00010980: 7228 7365 6c66 2e75 6e69 7175 655f 7370  r(self.unique_sp
+00010990: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000109a0: 7428 666c 6f61 7428 7629 295d 5b73 656c  t(float(v))][sel
+000109b0: 662e 756e 6971 7565 6964 5f6b 6579 5d29  f.uniqueid_key])
+000109c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 7365 6c66 2e67 7261 7068 5f74 7261 636b  self.graph_track
+000109f0: 735b 6461 7567 6874 6572 5f74 7261 636b  s[daughter_track
+00010a00: 5f69 645d 203d 2070 6172 656e 745f 7472  _id] = parent_tr
+00010a10: 6163 6b5f 6964 0d0a 2020 2020 2020 2020  ack_id..        
+00010a20: 2020 2020 2020 2020 7365 6c66 2e5f 6765          self._ge
+00010a30: 745f 6174 7472 6962 7574 6573 2829 0d0a  t_attributes()..
 00010a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a50: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00010a60: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
-00010a70: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
-00010a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010aa0: 2e5f 6669 6e61 6c5f 7472 6163 6b73 2874  ._final_tracks(t
-00010ab0: 7261 636b 5f69 6429 200d 0a0d 0a20 2020  rack_id) ....   
-00010ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010ad0: 7365 6c66 2e66 6f75 7269 6572 3a0d 0a20  self.fourier:.. 
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2020 7072 696e 7428 2763 6f6d 7075 7469    print('computi
-00010b00: 6e67 2046 6f75 7269 6572 2729 0d0a 2020  ng Fourier')..  
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b20: 2073 656c 662e 5f63 6f6d 7075 7465 5f70   self._compute_p
-00010b30: 6865 6e6f 7479 7065 7328 2920 2020 2020  henotypes()     
-00010b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010b60: 2020 2020 2073 656c 662e 5f74 656d 706f       self._tempo
-00010b70: 7261 6c5f 706c 6f74 735f 7472 6163 6b6d  ral_plots_trackm
-00010b80: 6174 6528 290d 0a20 2020 2020 2020 2020  ate()..         
-00010b90: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
-00010ba0: 6566 205f 6372 6561 7465 5f6d 6173 7465  ef _create_maste
-00010bb0: 725f 786d 6c28 7365 6c66 293a 0d0a 2020  r_xml(self):..  
-00010bc0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010bd0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010be0: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
-00010bf0: 6e20 7365 6c66 2e6d 6173 7465 725f 786d  n self.master_xm
-00010c00: 6c5f 726f 6f74 2e69 7465 7228 2753 706f  l_root.iter('Spo
-00010c10: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
-00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c30: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-00010c40: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-00010c50: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-00010c60: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+00010a50: 6966 2073 656c 662e 6175 746f 656e 636f  if self.autoenco
+00010a60: 6465 725f 6d6f 6465 6c20 616e 6420 7365  der_model and se
+00010a70: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
+00010a80: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010aa0: 2020 7072 696e 7428 2747 6574 7469 6e67    print('Getting
+00010ab0: 2061 7574 6f65 6e63 6f64 6572 2063 6c6f   autoencoder clo
+00010ac0: 7564 7327 290d 0a20 2020 2020 2020 2020  uds')..         
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010ae0: 6c66 2e5f 6173 7369 676e 5f63 6c75 7374  lf._assign_clust
+00010af0: 6572 5f63 6c61 7373 2829 0d0a 2020 2020  er_class()..    
+00010b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b10: 2020 2070 7269 6e74 2827 4372 6561 7469     print('Creati
+00010b20: 6e67 206d 6173 7465 7220 786d 6c27 290d  ng master xml').
+00010b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b40: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+00010b50: 6561 7465 5f6d 6173 7465 725f 786d 6c28  eate_master_xml(
+00010b60: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010b70: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+00010b80: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
+00010b90: 2020 2020 666f 7220 7472 6163 6b5f 6964      for track_id
+00010ba0: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
+00010bb0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
+00010bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010be0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+00010bf0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+00010c00: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010c30: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+00010c40: 6162 656c 203d 2022 4a75 7374 206f 6e65  abel = "Just one
+00010c50: 206d 6f72 6520 7468 696e 6722 0d0a 2020   more thing"..  
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 2020 6966 2063 656c 6c5f 6964        if cell_id
-00010c90: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-00010ca0: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
-00010cb0: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+00010c80: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+00010c90: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
+00010ca0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010cd0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
+00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-00010d10: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
-00010d20: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-00010d30: 6c6c 5f69 645d 2e6b 6579 7328 293a 0d0a  ll_id].keys():..
-00010d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-00010d70: 746f 626a 6563 742e 7365 7428 6b2c 2073  tobject.set(k, s
-00010d80: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
-00010d90: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00010da0: 656c 6c5f 6964 5d5b 6b5d 2929 2020 200d  ell_id][k]))   .
-00010db0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-00010de0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
-00010df0: 7465 725f 786d 6c5f 7472 6565 2e77 7269  ter_xml_tree.wri
-00010e00: 7465 286f 732e 7061 7468 2e6a 6f69 6e28  te(os.path.join(
-00010e10: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-00010e20: 7061 7468 2c20 7365 6c66 2e6d 6173 7465  path, self.maste
-00010e30: 725f 786d 6c5f 6e61 6d65 2929 0d0a 2020  r_xml_name))..  
-00010e40: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e70: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e90: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-00010ea0: 2020 2064 6566 205f 6173 7369 676e 5f63     def _assign_c
-00010eb0: 6c75 7374 6572 5f63 6c61 7373 2873 656c  luster_class(sel
-00010ec0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
-00010ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010ee0: 2020 2020 2020 7365 6c66 2e61 7865 7320        self.axes 
-00010ef0: 3d20 7365 6c66 2e61 7865 732e 7265 706c  = self.axes.repl
-00010f00: 6163 6528 2254 222c 2022 2229 0d0a 2020  ace("T", "")..  
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010f30: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
-00010f40: 742c 2074 696d 655f 6b65 7920 696e 2065  t, time_key in e
-00010f50: 6e75 6d65 7261 7465 2873 656c 662e 5f74  numerate(self._t
-00010f60: 696d 6564 5f63 656e 7472 6f69 642e 6b65  imed_centroid.ke
-00010f70: 7973 2829 293a 0d0a 2020 2020 2020 2020  ys()):..        
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fb0: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
-00010fc0: 6f69 6473 203d 2073 656c 662e 5f74 696d  oids = self._tim
-00010fd0: 6564 5f63 656e 7472 6f69 645b 7469 6d65  ed_centroid[time
-00010fe0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
-00011010: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
-00011020: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00011050: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
-00011060: 4175 746f 656e 636f 6465 7220 666f 7220  Autoencoder for 
-00011070: 7265 6669 6e69 6e67 2070 6f69 6e74 2063  refining point c
-00011080: 6c6f 7564 7322 0d0a 2020 2020 2020 2020  louds"..        
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-000110b0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
-000110c0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011100: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011140: 2020 2020 2020 2020 206c 656e 2873 656c           len(sel
-00011150: 662e 5f74 696d 6564 5f63 656e 7472 6f69  f._timed_centroi
-00011160: 642e 6b65 7973 2829 2920 2b20 312c 0d0a  d.keys()) + 1,..
+00010d00: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+00010d10: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+00010d20: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d50: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010d80: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+00010d90: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010dc0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
+00010dd0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010e10: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
+00010e20: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010e50: 6c66 2e5f 6669 6e61 6c5f 7472 6163 6b73  lf._final_tracks
+00010e60: 2874 7261 636b 5f69 6429 200d 0a0d 0a20  (track_id) .... 
+00010e70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010e80: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
+00010e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ea0: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
+00010eb0: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
+00010ee0: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00010f10: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
+00010f20: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
+00010f30: 6b6d 6174 6528 290d 0a20 2020 2020 2020  kmate()..       
+00010f40: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00010f50: 2064 6566 205f 6372 6561 7465 5f6d 6173   def _create_mas
+00010f60: 7465 725f 786d 6c28 7365 6c66 293a 0d0a  ter_xml(self):..
+00010f70: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00010f80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00010f90: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
+00010fa0: 2069 6e20 7365 6c66 2e6d 6173 7465 725f   in self.master_
+00010fb0: 786d 6c5f 726f 6f74 2e69 7465 7228 2753  xml_root.iter('S
+00010fc0: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
+00010ff0: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
+00011000: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
+00011010: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
+00011040: 6964 2069 6e20 7365 6c66 2e75 6e69 7175  id in self.uniqu
+00011050: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011060: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110b0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+000110c0: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
+000110d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000110e0: 6365 6c6c 5f69 645d 2e6b 6579 7328 293a  cell_id].keys():
+000110f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011110: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00011120: 706f 746f 626a 6563 742e 7365 7428 6b2c  potobject.set(k,
+00011130: 2073 7472 2873 656c 662e 756e 6971 7565   str(self.unique
+00011140: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011150: 5b63 656c 6c5f 6964 5d5b 6b5d 2929 2020  [cell_id][k]))  
+00011160: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
 00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000111d0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000111e0: 2e76 616c 7565 203d 2020 636f 756e 7420  .value =  count 
-000111f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011180: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00011190: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000111a0: 6173 7465 725f 786d 6c5f 7472 6565 2e77  aster_xml_tree.w
+000111b0: 7269 7465 286f 732e 7061 7468 2e6a 6f69  rite(os.path.joi
+000111c0: 6e28 7365 6c66 2e6d 6173 7465 725f 786d  n(self.master_xm
+000111d0: 6c5f 7061 7468 2c20 7365 6c66 2e6d 6173  l_path, self.mas
+000111e0: 7465 725f 786d 6c5f 6e61 6d65 2929 0d0a  ter_xml_name))..
+000111f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-00011220: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
+00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011220: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 2020 2020 2020 2063 6c75 7374 6572           cluster
-00011250: 5f65 7661 6c20 3d20 436c 7573 7465 7269  _eval = Clusteri
-00011260: 6e67 2873 656c 662e 6163 6365 6c65 7261  ng(self.accelera
-00011270: 746f 722c 2073 656c 662e 6465 7669 6365  tor, self.device
-00011280: 732c 2073 656c 662e 7365 675f 696d 6167  s, self.seg_imag
-00011290: 655b 696e 7428 7469 6d65 5f6b 6579 292c  e[int(time_key),
-000112a0: 3a5d 2c20 2073 656c 662e 6178 6573 2c20  :],  self.axes, 
-000112b0: 7365 6c66 2e6e 756d 5f70 6f69 6e74 732c  self.num_points,
-000112c0: 2073 656c 662e 6175 746f 656e 636f 6465   self.autoencode
-000112d0: 725f 6d6f 6465 6c2c 206b 6579 203d 2074  r_model, key = t
-000112e0: 696d 655f 6b65 792c 2070 726f 6772 6573  ime_key, progres
-000112f0: 735f 6261 723d 7365 6c66 2e70 726f 6772  s_bar=self.progr
-00011300: 6573 735f 6261 722c 2062 6174 6368 5f73  ess_bar, batch_s
-00011310: 697a 6520 3d20 7365 6c66 2e62 6174 6368  ize = self.batch
-00011320: 5f73 697a 652c 2073 6361 6c65 5f7a 3d73  _size, scale_z=s
-00011330: 656c 662e 7363 616c 655f 7a2c 2073 6361  elf.scale_z, sca
-00011340: 6c65 5f78 793d 2073 656c 662e 7363 616c  le_xy= self.scal
-00011350: 655f 7879 2c20 6365 6e74 6572 203d 2073  e_xy, center = s
-00011360: 656c 662e 6365 6e74 6572 2920 2020 2020  elf.center)     
-00011370: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00011380: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011390: 6c75 7374 6572 5f65 7661 6c2e 5f63 7265  luster_eval._cre
-000113a0: 6174 655f 636c 7573 7465 725f 6c61 6265  ate_cluster_labe
-000113b0: 6c73 2829 0d0a 2020 2020 2020 2020 2020  ls()..          
-000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
-000113e0: 6162 656c 203d 2063 6c75 7374 6572 5f65  abel = cluster_e
-000113f0: 7661 6c2e 7469 6d65 645f 636c 7573 7465  val.timed_cluste
-00011400: 725f 6c61 6265 6c20 0d0a 2020 2020 2020  r_label ..      
-00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011420: 2020 2020 206f 7574 7075 745f 6c61 6265       output_labe
-00011430: 6c73 2c20 206f 7574 7075 745f 636c 7573  ls,  output_clus
-00011440: 7465 725f 6365 6e74 726f 6964 2c20 6f75  ter_centroid, ou
-00011450: 7470 7574 5f63 6c6f 7564 5f65 6363 656e  tput_cloud_eccen
-00011460: 7472 6963 6974 792c 206f 7574 7075 745f  tricity, output_
-00011470: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00011480: 746f 722c 206f 7574 7075 745f 6c61 7267  tor, output_larg
-00011490: 6573 745f 6569 6765 6e76 616c 7565 2c20  est_eigenvalue, 
-000114a0: 6f75 7470 7574 5f64 696d 656e 7369 6f6e  output_dimension
-000114b0: 732c 206f 7574 7075 745f 636c 6f75 645f  s, output_cloud_
-000114c0: 7375 7266 6163 655f 6172 6561 203d 2074  surface_area = t
-000114d0: 696d 6564 5f63 6c75 7374 6572 5f6c 6162  imed_cluster_lab
-000114e0: 656c 5b74 696d 655f 6b65 795d 0d0a 2020  el[time_key]..  
-000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00011510: 203d 2031 0d0a 2020 2020 2020 2020 2020   = 1..          
-00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011530: 2073 6361 6c65 5f32 203d 2031 0d0a 2020   scale_2 = 1..  
+00011240: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00011250: 0a20 2020 2064 6566 205f 6173 7369 676e  .    def _assign
+00011260: 5f63 6c75 7374 6572 5f63 6c61 7373 2873  _cluster_class(s
+00011270: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+00011280: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00011290: 2020 2020 2020 2020 7365 6c66 2e61 7865          self.axe
+000112a0: 7320 3d20 7365 6c66 2e61 7865 732e 7265  s = self.axes.re
+000112b0: 706c 6163 6528 2254 222c 2022 2229 0d0a  place("T", "")..
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000112e0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
+000112f0: 756e 742c 2074 696d 655f 6b65 7920 696e  unt, time_key in
+00011300: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
+00011310: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
+00011320: 6b65 7973 2829 293a 0d0a 2020 2020 2020  keys()):..      
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011360: 2020 7472 6565 2c20 7370 6f74 5f63 656e    tree, spot_cen
+00011370: 7472 6f69 6473 203d 2073 656c 662e 5f74  troids = self._t
+00011380: 696d 6564 5f63 656e 7472 6f69 645b 7469  imed_centroid[ti
+00011390: 6d65 5f6b 6579 5d0d 0a20 2020 2020 2020  me_key]..       
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+000113c0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+000113d0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113f0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+00011400: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+00011410: 2022 4175 746f 656e 636f 6465 7220 666f   "Autoencoder fo
+00011420: 7220 7265 6669 6e69 6e67 2070 6f69 6e74  r refining point
+00011430: 2063 6c6f 7564 7322 0d0a 2020 2020 2020   clouds"..      
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00011460: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+00011470: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114b0: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114f0: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+00011500: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+00011510: 6f69 642e 6b65 7973 2829 2920 2b20 312c  oid.keys()) + 1,
+00011520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00011560: 6e20 7261 6e67 6528 6c65 6e28 6f75 7470  n range(len(outp
-00011570: 7574 5f63 6c75 7374 6572 5f63 656e 7472  ut_cluster_centr
-00011580: 6f69 6429 293a 0d0a 2020 2020 2020 2020  oid)):..        
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-000115b0: 726f 6964 203d 206f 7574 7075 745f 636c  roid = output_cl
-000115c0: 7573 7465 725f 6365 6e74 726f 6964 5b69  uster_centroid[i
-000115d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00011550: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00011560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011580: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00011590: 6172 2e76 616c 7565 203d 2020 636f 756e  ar.value =  coun
+000115a0: 7420 0d0a 2020 2020 2020 2020 2020 2020  t ..            
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115c0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+000115d0: 735f 6261 722e 7368 6f77 2829 0d0a 0d0a  s_bar.show()....
 000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 2020 2020 2020 2071 7561 6c69 7479 203d         quality =
-00011600: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
-00011610: 6569 6765 6e76 616c 7565 5b69 5d0d 0a20  eigenvalue[i].. 
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011640: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
-00011650: 636f 6d70 5f66 6972 7374 797a 203d 206f  comp_firstyz = o
-00011660: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
-00011670: 6e74 7269 6369 7479 5b69 5d0d 0a20 2020  ntricity[i]..   
-00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116a0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
-000116b0: 6d65 6e73 696f 6e20 3d20 6f75 7470 7574  mension = output
-000116c0: 5f64 696d 656e 7369 6f6e 735b 695d 200d  _dimensions[i] .
-000116d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116f0: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00011700: 6369 7479 5f64 696d 656e 7369 6f6e 5b30  city_dimension[0
-00011710: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115f0: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+00011600: 6572 5f65 7661 6c20 3d20 436c 7573 7465  er_eval = Cluste
+00011610: 7269 6e67 2873 656c 662e 6163 6365 6c65  ring(self.accele
+00011620: 7261 746f 722c 2073 656c 662e 6465 7669  rator, self.devi
+00011630: 6365 732c 2073 656c 662e 7365 675f 696d  ces, self.seg_im
+00011640: 6167 655b 696e 7428 7469 6d65 5f6b 6579  age[int(time_key
+00011650: 292c 3a5d 2c20 2073 656c 662e 6178 6573  ),:],  self.axes
+00011660: 2c20 7365 6c66 2e6e 756d 5f70 6f69 6e74  , self.num_point
+00011670: 732c 2073 656c 662e 6175 746f 656e 636f  s, self.autoenco
+00011680: 6465 725f 6d6f 6465 6c2c 206b 6579 203d  der_model, key =
+00011690: 2074 696d 655f 6b65 792c 2070 726f 6772   time_key, progr
+000116a0: 6573 735f 6261 723d 7365 6c66 2e70 726f  ess_bar=self.pro
+000116b0: 6772 6573 735f 6261 722c 2062 6174 6368  gress_bar, batch
+000116c0: 5f73 697a 6520 3d20 7365 6c66 2e62 6174  _size = self.bat
+000116d0: 6368 5f73 697a 652c 2073 6361 6c65 5f7a  ch_size, scale_z
+000116e0: 3d73 656c 662e 7363 616c 655f 7a2c 2073  =self.scale_z, s
+000116f0: 6361 6c65 5f78 793d 2073 656c 662e 7363  cale_xy= self.sc
+00011700: 616c 655f 7879 2c20 6365 6e74 6572 203d  ale_xy, center =
+00011710: 2073 656c 662e 6365 6e74 6572 2920 2020   self.center)   
+00011720: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011740: 2020 2020 7363 616c 655f 3120 3d20 7365      scale_1 = se
-00011750: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
-00011760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011740: 2063 6c75 7374 6572 5f65 7661 6c2e 5f63   cluster_eval._c
+00011750: 7265 6174 655f 636c 7573 7465 725f 6c61  reate_cluster_la
+00011760: 6265 6c73 2829 0d0a 2020 2020 2020 2020  bels()..        
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00011790: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
-000117a0: 6e73 696f 6e5b 315d 203d 3d20 313a 0d0a  nsion[1] == 1:..
-000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011780: 2020 2074 696d 6564 5f63 6c75 7374 6572     timed_cluster
+00011790: 5f6c 6162 656c 203d 2063 6c75 7374 6572  _label = cluster
+000117a0: 5f65 7661 6c2e 7469 6d65 645f 636c 7573  _eval.timed_clus
+000117b0: 7465 725f 6c61 6265 6c20 0d0a 2020 2020  ter_label ..    
 000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117e0: 2020 7363 616c 655f 3220 3d20 7365 6c66    scale_2 = self
-000117f0: 2e79 6361 6c69 6272 6174 696f 6e0d 0a0d  .ycalibration...
-00011800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
-00011830: 6369 7479 5f64 696d 656e 7369 6f6e 5b30  city_dimension[0
-00011840: 5d20 3d3d 2032 3a0d 0a20 2020 2020 2020  ] == 2:..       
-00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011870: 2020 2020 7363 616c 655f 3120 3d20 7365      scale_1 = se
-00011880: 6c66 2e7a 6361 6c69 6272 6174 696f 6e0d  lf.zcalibration.
-00011890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000117d0: 2020 2020 2020 206f 7574 7075 745f 6c61         output_la
+000117e0: 6265 6c73 2c20 206f 7574 7075 745f 636c  bels,  output_cl
+000117f0: 7573 7465 725f 6365 6e74 726f 6964 2c20  uster_centroid, 
+00011800: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
+00011810: 656e 7472 6963 6974 792c 206f 7574 7075  entricity, outpu
+00011820: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
+00011830: 6563 746f 722c 206f 7574 7075 745f 6c61  ector, output_la
+00011840: 7267 6573 745f 6569 6765 6e76 616c 7565  rgest_eigenvalue
+00011850: 2c20 6f75 7470 7574 5f64 696d 656e 7369  , output_dimensi
+00011860: 6f6e 732c 206f 7574 7075 745f 636c 6f75  ons, output_clou
+00011870: 645f 7375 7266 6163 655f 6172 6561 203d  d_surface_area =
+00011880: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
+00011890: 6162 656c 5b74 696d 655f 6b65 795d 0d0a  abel[time_key]..
 000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118b0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-000118c0: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
-000118d0: 6e73 696f 6e5b 315d 203d 3d20 303a 0d0a  nsion[1] == 0:..
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118b0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000118c0: 5f31 203d 2031 0d0a 2020 2020 2020 2020  _1 = 1..        
+000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118e0: 2020 2073 6361 6c65 5f32 203d 2031 0d0a     scale_2 = 1..
 000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 7363 616c 655f 3220 3d20 7365 6c66    scale_2 = self
-00011920: 2e78 6361 6c69 6272 6174 696f 6e20 2020  .xcalibration   
-00011930: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011900: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00011910: 2069 6e20 7261 6e67 6528 6c65 6e28 6f75   in range(len(ou
+00011920: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+00011930: 7472 6f69 6429 293a 0d0a 2020 2020 2020  troid)):..      
 00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
-00011960: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
-00011970: 6e5b 305d 203d 3d20 313a 0d0a 2020 2020  n[0] == 1:..    
-00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00011960: 6e74 726f 6964 203d 206f 7574 7075 745f  ntroid = output_
+00011970: 636c 7573 7465 725f 6365 6e74 726f 6964  cluster_centroid
+00011980: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
 00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 2020 2020 2020 2073 6361 6c65 5f31 203d         scale_1 =
-000119b0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-000119c0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000119f0: 6620 6573 7365 6e74 7269 6369 7479 5f64  f essentricity_d
-00011a00: 696d 656e 7369 6f6e 5b31 5d20 3d3d 2030  imension[1] == 0
-00011a10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119a0: 2020 2020 2020 2020 2071 7561 6c69 7479           quality
+000119b0: 203d 206f 7574 7075 745f 6c61 7267 6573   = output_larges
+000119c0: 745f 6569 6765 6e76 616c 7565 5b69 5d0d  t_eigenvalue[i].
+000119d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119f0: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
+00011a00: 795f 636f 6d70 5f66 6972 7374 797a 203d  y_comp_firstyz =
+00011a10: 206f 7574 7075 745f 636c 6f75 645f 6563   output_cloud_ec
+00011a20: 6365 6e74 7269 6369 7479 5b69 5d0d 0a20  centricity[i].. 
 00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a40: 2020 2020 2073 6361 6c65 5f32 203d 2073       scale_2 = s
-00011a50: 656c 662e 7863 616c 6962 7261 7469 6f6e  elf.xcalibration
-00011a60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00011a90: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00011aa0: 696f 6e5b 305d 203d 3d20 313a 0d0a 2020  ion[0] == 1:..  
-00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ad0: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-00011ae0: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
-00011af0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00011b30: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00011b40: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00011b80: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00011b90: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
-00011ba0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00011bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bc0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-00011bd0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-00011be0: 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20 2020  on[0] == 0:..   
-00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2020 2065 7373 656e 7472 6963 6974 795f     essentricity_
+00011a60: 6469 6d65 6e73 696f 6e20 3d20 6f75 7470  dimension = outp
+00011a70: 7574 5f64 696d 656e 7369 6f6e 735b 695d  ut_dimensions[i]
+00011a80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011aa0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011ab0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011ac0: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
+00011b00: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00011b10: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011b40: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011b50: 6d65 6e73 696f 6e5b 315d 203d 3d20 313a  mension[1] == 1:
+00011b60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b90: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
+00011ba0: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
+00011bb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011be0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011bf0: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
 00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c10: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
-00011c20: 3d20 7365 6c66 2e78 6361 6c69 6272 6174  = self.xcalibrat
-00011c30: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
+00011c30: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00011c40: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
 00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-00011c70: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
-00011c80: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011c70: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011c80: 6d65 6e73 696f 6e5b 315d 203d 3d20 303a  mension[1] == 0:
+00011c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-00011cc0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
-00011cd0: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
-00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cf0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-00011d00: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-00011d10: 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20 2020  on[0] == 0:..   
-00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cc0: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
+00011cd0: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+00011ce0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00011d10: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00011d20: 696f 6e5b 305d 203d 3d20 313a 0d0a 2020  ion[0] == 1:..  
 00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d40: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
-00011d50: 3d20 7365 6c66 2e78 6361 6c69 6272 6174  = self.xcalibrat
-00011d60: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d50: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00011d60: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
+00011d70: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
 00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d90: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-00011da0: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
-00011db0: 323a 0d0a 2020 2020 2020 2020 2020 2020  2:..            
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011da0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00011db0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+00011dc0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
 00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-00011df0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-00011e00: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011df0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+00011e00: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+00011e10: 6f6e 2020 0d0a 0d0a 2020 2020 2020 2020  on  ....        
 00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e60: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00011e30: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00011e40: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00011e50: 6e73 696f 6e5b 305d 203d 3d20 313a 0d0a  nsion[0] == 1:..
+00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00011ec0: 5f61 7869 7320 3d20 6f75 7470 7574 5f6c  _axis = output_l
-00011ed0: 6172 6765 7374 5f65 6967 656e 7665 6374  argest_eigenvect
-00011ee0: 6f72 5b69 5d0d 0a20 2020 2020 2020 2020  or[i]..         
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
-00011f10: 6365 5f61 7265 6120 3d20 6f75 7470 7574  ce_area = output
-00011f20: 5f63 6c6f 7564 5f73 7572 6661 6365 5f61  _cloud_surface_a
-00011f30: 7265 615b 695d 202a 2073 656c 662e 7a63  rea[i] * self.zc
-00011f40: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
-00011f50: 662e 7963 616c 6962 7261 7469 6f6e 202a  f.ycalibration *
-00011f60: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-00011f70: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f90: 2020 2020 2020 2020 6469 7374 2c20 696e          dist, in
-00011fa0: 6465 7820 3d20 7472 6565 2e71 7565 7279  dex = tree.query
-00011fb0: 2863 656e 7472 6f69 6429 0d0a 2020 2020  (centroid)..    
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fe0: 7261 6469 7573 203d 2071 7561 6c69 7479  radius = quality
-00011ff0: 202a 206d 6174 682e 706f 7728 7365 6c66   * math.pow(self
-00012000: 2e7a 6361 6c69 6272 6174 696f 6e20 2a20  .zcalibration * 
-00012010: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-00012020: 6e20 2a20 7365 6c66 2e79 6361 6c69 6272  n * self.ycalibr
-00012030: 6174 696f 6e2c 2031 2e30 2f33 2e30 290d  ation, 1.0/3.0).
-00012040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e80: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011e90: 5f31 203d 2073 656c 662e 7963 616c 6962  _1 = self.ycalib
+00011ea0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+00011ee0: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+00011ef0: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f20: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+00011f30: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
+00011f40: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
+00011f50: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f70: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00011f80: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00011f90: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011fd0: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
+00011fe0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012010: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00012020: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+00012030: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012060: 2020 2020 2069 6620 6469 7374 203c 2071       if dist < q
-00012070: 7561 6c69 7479 3a0d 0a20 2020 2020 2020  uality:..       
-00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00012070: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
+00012080: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
 00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120a0: 2020 2020 2063 6c6f 7365 7374 5f63 656e       closest_cen
-000120b0: 7472 6f69 6420 3d20 7370 6f74 5f63 656e  troid = spot_cen
-000120c0: 7472 6f69 6473 5b69 6e64 6578 5d0d 0a20  troids[index].. 
+000120a0: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+000120b0: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+000120c0: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
 000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120f0: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
-00012100: 5f73 706f 745f 6365 6e74 726f 6964 203d  _spot_centroid =
-00012110: 2028 696e 7428 7469 6d65 5f6b 6579 292c   (int(time_key),
-00012120: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
-00012130: 5b30 5d2c 2063 6c6f 7365 7374 5f63 656e  [0], closest_cen
-00012140: 7472 6f69 645b 315d 2c20 636c 6f73 6573  troid[1], closes
-00012150: 745f 6365 6e74 726f 6964 5b32 5d29 0d0a  t_centroid[2])..
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00012100: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
+00012110: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012140: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00012150: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+00012160: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
 00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012180: 2020 2020 2020 2020 2020 2020 636c 6f73              clos
-00012190: 6573 745f 6365 6c6c 5f69 6420 3d20 7365  est_cell_id = se
-000121a0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f63  lf.unique_spot_c
-000121b0: 656e 7472 6f69 645b 6672 616d 655f 7370  entroid[frame_sp
-000121c0: 6f74 5f63 656e 7472 6f69 645d 0d0a 2020  ot_centroid]..  
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+000121a0: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
+000121b0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 2020 2020 2020 6d61 736b 5f76            mask_v
-00012200: 6563 746f 7220 3d20 5b20 666c 6f61 7428  ector = [ float(
-00012210: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012220: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00012230: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012240: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
-00012250: 6f69 645f 785f 6b65 795d 292c 2066 6c6f  oid_x_key]), flo
-00012260: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00012270: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00012280: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00012290: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
-000122a0: 6e74 726f 6964 5f79 5f6b 6579 5d29 2c20  ntroid_y_key]), 
-000122b0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000122c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000122d0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-000122e0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-000122f0: 6b63 656e 7472 6f69 645f 7a5f 6b65 795d  kcentroid_z_key]
-00012300: 2920 5d0d 0a20 2020 2020 2020 2020 2020  ) ]..           
-00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012330: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
-00012340: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-00012350: 2863 656c 6c5f 6178 6973 2c20 6d61 736b  (cell_axis, mask
-00012360: 5f76 6563 746f 7229 0d0a 2020 2020 2020  _vector)..      
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012210: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012240: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012260: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00012270: 6c6c 5f61 7869 7320 3d20 6f75 7470 7574  ll_axis = output
+00012280: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
+00012290: 6374 6f72 5b69 5d0d 0a20 2020 2020 2020  ctor[i]..       
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122b0: 2020 2020 2020 2020 2020 2020 2073 7572               sur
+000122c0: 6661 6365 5f61 7265 6120 3d20 6f75 7470  face_area = outp
+000122d0: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
+000122e0: 5f61 7265 615b 695d 202a 2073 656c 662e  _area[i] * self.
+000122f0: 7a63 616c 6962 7261 7469 6f6e 202a 2073  zcalibration * s
+00012300: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00012310: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
+00012320: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012340: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
+00012350: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+00012360: 7279 2863 656e 7472 6f69 6429 0d0a 2020  ry(centroid)..  
 00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000123d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000123e0: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-000123f0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00012400: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
-00012410: 5f6b 6579 203a 2063 656c 6c5f 6178 6973  _key : cell_axis
-00012420: 5f6d 6173 6b7d 290d 0a20 2020 2020 2020  _mask})..       
+00012390: 2020 7261 6469 7573 203d 2071 7561 6c69    radius = quali
+000123a0: 7479 202a 206d 6174 682e 706f 7728 7365  ty * math.pow(se
+000123b0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
+000123c0: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
+000123d0: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
+000123e0: 6272 6174 696f 6e2c 2031 2e30 2f33 2e30  bration, 1.0/3.0
+000123f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012410: 2020 2020 2020 2069 6620 6469 7374 203c         if dist <
+00012420: 2071 7561 6c69 7479 3a0d 0a20 2020 2020   quality:..     
 00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2020 2020 2069 6620 7365 6c66 2e75 6e69       if self.uni
-00012460: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012470: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012480: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e72  cell_id)][self.r
-00012490: 6164 6975 735f 6b65 795d 203e 2030 3a0d  adius_key] > 0:.
-000124a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000124e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000124f0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00012500: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00012510: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00012520: 5f63 6f6d 705f 6669 7273 746b 6579 203a  _comp_firstkey :
-00012530: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
-00012540: 6d70 5f66 6972 7374 797a 5b30 5d20 2a20  mp_firstyz[0] * 
-00012550: 7363 616c 655f 317d 290d 0a20 2020 2020  scale_1})..     
-00012560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012590: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000125a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000125b0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-000125c0: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
-000125d0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000125e0: 7365 636f 6e64 6b65 7920 3a20 6563 6365  secondkey : ecce
-000125f0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00012600: 7273 7479 7a5b 315d 202a 2073 6361 6c65  rstyz[1] * scale
-00012610: 5f32 7d29 0d0a 2020 2020 2020 2020 2020  _2})..          
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00012650: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00012660: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
-00012670: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
-00012680: 7465 287b 7365 6c66 2e73 7572 6661 6365  te({self.surface
-00012690: 5f61 7265 615f 6b65 7920 3a20 7375 7266  _area_key : surf
-000126a0: 6163 655f 6172 6561 7d29 0d0a 2020 2020  ace_area})..    
-000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012450: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
+00012460: 656e 7472 6f69 6420 3d20 7370 6f74 5f63  entroid = spot_c
+00012470: 656e 7472 6f69 6473 5b69 6e64 6578 5d0d  entroids[index].
+00012480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+000124b0: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+000124c0: 203d 2028 696e 7428 7469 6d65 5f6b 6579   = (int(time_key
+000124d0: 292c 636c 6f73 6573 745f 6365 6e74 726f  ),closest_centro
+000124e0: 6964 5b30 5d2c 2063 6c6f 7365 7374 5f63  id[0], closest_c
+000124f0: 656e 7472 6f69 645b 315d 2c20 636c 6f73  entroid[1], clos
+00012500: 6573 745f 6365 6e74 726f 6964 5b32 5d29  est_centroid[2])
+00012510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00012540: 6f73 6573 745f 6365 6c6c 5f69 6420 3d20  osest_cell_id = 
+00012550: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00012560: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+00012570: 7370 6f74 5f63 656e 7472 6f69 645d 0d0a  spot_centroid]..
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125a0: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+000125b0: 5f76 6563 746f 7220 3d20 5b20 666c 6f61  _vector = [ floa
+000125c0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+000125d0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000125e0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+000125f0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00012600: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00012610: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00012620: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00012630: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00012640: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
+00012650: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
+00012660: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
+00012670: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012680: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012690: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+000126a0: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+000126b0: 795d 2920 5d0d 0a20 2020 2020 2020 2020  y]) ]..         
 000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000126f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00012700: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012710: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
-00012720: 7561 6c69 7479 5f6b 6579 203a 2071 7561  uality_key : qua
-00012730: 6c69 7479 7d29 0d0a 2020 2020 2020 2020  lity})..        
-00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
+000126f0: 6b20 3d20 616e 6775 6c61 725f 6368 616e  k = angular_chan
+00012700: 6765 2863 656c 6c5f 6178 6973 2c20 6d61  ge(cell_axis, ma
+00012710: 736b 5f76 6563 746f 7229 0d0a 2020 2020  sk_vector)..    
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012740: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012770: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00012780: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-00012790: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-000127a0: 6461 7465 287b 7365 6c66 2e72 6164 6975  date({self.radiu
-000127b0: 735f 6b65 7920 3a20 7261 6469 7573 207d  s_key : radius }
-000127c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000127f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012860: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00012870: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00012880: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00012890: 2e75 7064 6174 6528 7b73 656c 662e 6563  .update({self.ec
-000128a0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-000128b0: 6669 7273 746b 6579 203a 202d 317d 290d  firstkey : -1}).
-000128c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128f0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00012900: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00012910: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00012920: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00012930: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-00012940: 5f63 6f6d 705f 7365 636f 6e64 6b65 7920  _comp_secondkey 
-00012950: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012990: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000129a0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-000129b0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-000129c0: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
-000129d0: 6365 5f61 7265 615f 6b65 7920 3a20 2d31  ce_area_key : -1
-000129e0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a10: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012a20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012a30: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012a40: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00012a50: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
-00012a60: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00012780: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00012790: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+000127a0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000127b0: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
+000127c0: 736b 5f6b 6579 203a 2063 656c 6c5f 6178  sk_key : cell_ax
+000127d0: 6973 5f6d 6173 6b7d 290d 0a20 2020 2020  is_mask})..     
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012800: 2020 2020 2020 2069 6620 7365 6c66 2e75         if self.u
+00012810: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00012820: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00012830: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
+00012840: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
+00012850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012880: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012890: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000128a0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+000128b0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+000128c0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+000128d0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+000128e0: 203a 2065 6363 656e 7472 6963 6974 795f   : eccentricity_
+000128f0: 636f 6d70 5f66 6972 7374 797a 5b30 5d20  comp_firstyz[0] 
+00012900: 2a20 7363 616c 655f 317d 290d 0a20 2020  * scale_1})..   
+00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012940: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012950: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012960: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012970: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00012980: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00012990: 705f 7365 636f 6e64 6b65 7920 3a20 6563  p_secondkey : ec
+000129a0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+000129b0: 6669 7273 7479 7a5b 315d 202a 2073 6361  firstyz[1] * sca
+000129c0: 6c65 5f32 7d29 0d0a 2020 2020 2020 2020  le_2})..        
+000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012a00: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00012a10: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00012a20: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00012a30: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
+00012a40: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
+00012a50: 7266 6163 655f 6172 6561 7d29 0d0a 2020  rface_area})..  
+00012a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012aa0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00012ab0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00012ac0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00012ad0: 2e75 7064 6174 6528 7b73 656c 662e 7261  .update({self.ra
-00012ae0: 6469 7573 5f6b 6579 203a 202d 3120 7d29  dius_key : -1 })
-00012af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012a90: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00012aa0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012ab0: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00012ac0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012ad0: 2e71 7561 6c69 7479 5f6b 6579 203a 2071  .quality_key : q
+00012ae0: 7561 6c69 7479 7d29 0d0a 2020 2020 2020  uality})..      
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2020 2020 200d 0a0d 0a0d 0a0d 0a0d 0a20       .......... 
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b70: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
-00012b80: 662e 726f 6f74 5f73 706f 7473 2e69 7465  f.root_spots.ite
-00012b90: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bb0: 2020 2020 2020 2020 2073 656c 662e 726f           self.ro
-00012bc0: 6f74 5f73 706f 7473 5b6b 5d20 3d20 7365  ot_spots[k] = se
-00012bd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012be0: 726f 7065 7274 6965 735b 6b5d 2020 2020  roperties[k]    
-00012bf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00012c00: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00012c10: 205f 636f 6d70 7574 655f 7068 656e 6f74   _compute_phenot
-00012c20: 7970 6573 2873 656c 6629 3a0d 0a0d 0a20  ypes(self):.... 
-00012c30: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-00012c40: 7629 2069 6e20 7365 6c66 2e75 6e69 7175  v) in self.uniqu
-00012c50: 655f 7472 6163 6b73 2e69 7465 6d73 2829  e_tracks.items()
-00012c60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012c70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012c80: 2020 2020 2074 7261 636b 5f69 6420 3d20       track_id = 
-00012c90: 6b0d 0a20 2020 2020 2020 2020 2020 2020  k..             
-00012ca0: 2020 2074 7261 636b 6c65 745f 7072 6f70     tracklet_prop
-00012cb0: 6572 7469 6573 203d 2073 656c 662e 756e  erties = self.un
-00012cc0: 6971 7565 5f74 7261 636b 5f70 726f 7065  ique_track_prope
-00012cd0: 7274 6965 735b 6b5d 0d0a 2020 2020 2020  rties[k]..      
-00012ce0: 2020 2020 2020 2020 2020 7472 6163 6b73            tracks
-00012cf0: 203d 2073 656c 662e 756e 6971 7565 5f74   = self.unique_t
-00012d00: 7261 636b 735b 6b5d 0d0a 2020 2020 2020  racks[k]..      
-00012d10: 2020 2020 2020 2020 2020 5a20 3d20 7472            Z = tr
-00012d20: 6163 6b73 5b3a 2c32 5d0d 0a20 2020 2020  acks[:,2]..     
-00012d30: 2020 2020 2020 2020 2020 2059 203d 2074             Y = t
-00012d40: 7261 636b 735b 3a2c 335d 0d0a 2020 2020  racks[:,3]..    
-00012d50: 2020 2020 2020 2020 2020 2020 5820 3d20              X = 
-00012d60: 7472 6163 6b73 5b3a 2c34 5d0d 0a20 2020  tracks[:,4]..   
-00012d70: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00012d80: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
-00012d90: 7065 7274 6965 735b 3a2c 305d 0d0a 2020  perties[:,0]..  
-00012da0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00012db0: 6971 7565 5f69 6473 203d 2074 7261 636b  ique_ids = track
-00012dc0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012dd0: 2c31 5d0d 0a20 2020 2020 2020 2020 2020  ,1]..           
-00012de0: 2020 2020 2075 6e69 7175 655f 6964 735f       unique_ids_
-00012df0: 7365 7420 3d20 7365 7428 756e 6971 7565  set = set(unique
-00012e00: 5f69 6473 290d 0a20 2020 2020 2020 2020  _ids)..         
-00012e10: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-00012e20: 6e5f 6964 7320 3d20 7472 6163 6b6c 6574  n_ids = tracklet
-00012e30: 5f70 726f 7065 7274 6965 735b 3a2c 325d  _properties[:,2]
-00012e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012e50: 2020 7261 6469 7573 203d 2074 7261 636b    radius = track
-00012e60: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
-00012e70: 2c33 5d0d 0a20 2020 2020 2020 2020 2020  ,3]..           
-00012e80: 2020 2020 2076 6f6c 756d 6520 3d20 7472       volume = tr
-00012e90: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00012ea0: 735b 3a2c 345d 0d0a 2020 2020 2020 2020  s[:,4]..        
-00012eb0: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-00012ec0: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-00012ed0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00012ee0: 7274 6965 735b 3a2c 355d 0d0a 2020 2020  rties[:,5]..    
-00012ef0: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
-00012f00: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00012f10: 636f 6e64 203d 2074 7261 636b 6c65 745f  cond = tracklet_
-00012f20: 7072 6f70 6572 7469 6573 5b3a 2c36 5d0d  properties[:,6].
-00012f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012f40: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
-00012f50: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012f60: 6965 735b 3a2c 375d 0d0a 2020 2020 2020  ies[:,7]..      
-00012f70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00012f80: 2020 2020 2020 2020 2020 2069 6e74 656e             inten
-00012f90: 7369 7479 203d 2074 7261 636b 6c65 745f  sity = tracklet_
-00012fa0: 7072 6f70 6572 7469 6573 5b3a 2c38 5d0d  properties[:,8].
-00012fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012fc0: 2073 7065 6564 203d 2074 7261 636b 6c65   speed = trackle
-00012fd0: 745f 7072 6f70 6572 7469 6573 5b3a 2c39  t_properties[:,9
-00012fe0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012ff0: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
-00013000: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00013010: 7274 6965 735b 3a2c 3130 5d0d 0a20 2020  rties[:,10]..   
-00013020: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-00013030: 656c 6572 6174 696f 6e20 3d20 7472 6163  eleration = trac
-00013040: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00013050: 3a2c 3131 5d0d 0a20 2020 2020 2020 2020  :,11]..         
-00013060: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
-00013070: 6365 6c6c 5f6d 6173 6b20 3d20 7472 6163  cell_mask = trac
-00013080: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00013090: 3a2c 3132 5d0d 0a20 2020 2020 2020 2020  :,12]..         
-000130a0: 2020 2020 2020 2072 6164 6961 6c5f 616e         radial_an
-000130b0: 676c 6520 3d20 7472 6163 6b6c 6574 5f70  gle = tracklet_p
-000130c0: 726f 7065 7274 6965 735b 3a2c 3133 5d0d  roperties[:,13].
-000130d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000130e0: 2063 656c 6c5f 6178 6973 5f6d 6173 6b20   cell_axis_mask 
-000130f0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
-00013100: 7274 6965 735b 3a2c 3134 5d0d 0a0d 0a0d  rties[:,14].....
-00013110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013120: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013130: 2020 2075 6e69 7175 655f 6666 745f 7072     unique_fft_pr
-00013140: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-00013150: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
-00013160: 2020 2020 2020 2020 756e 6971 7565 5f63          unique_c
-00013170: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
-00013180: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
-00013190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000131a0: 2073 656c 662e 756e 6971 7565 5f66 6674   self.unique_fft
-000131b0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-000131c0: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
-000131d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000131e0: 2e75 6e69 7175 655f 636c 7573 7465 725f  .unique_cluster_
-000131f0: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
-00013200: 5f69 645d 203d 207b 7d0d 0a0d 0a20 2020  _id] = {}....   
-00013210: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-00013220: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
-00013230: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
-00013240: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00013250: 2020 2020 756e 6971 7565 5f64 796e 616d      unique_dynam
-00013260: 6963 5f70 726f 7065 7274 6965 735f 7472  ic_properties_tr
-00013270: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
-00013280: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013290: 662e 756e 6971 7565 5f73 6861 7065 5f70  f.unique_shape_p
-000132a0: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
-000132b0: 6964 5d20 3d20 7b7d 0d0a 2020 2020 2020  id] = {}..      
-000132c0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000132d0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-000132e0: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-000132f0: 645d 203d 207b 7d0d 0a20 2020 2020 2020  d] = {}..       
-00013300: 2020 2020 2020 2020 2065 7870 616e 6465           expande
-00013310: 645f 7469 6d65 203d 206e 702e 7a65 726f  d_time = np.zero
-00013320: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
-00013330: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 706f 696e 745f 7361 6d70 6c65 203d 2065  point_sample = e
-00013360: 7870 616e 6465 645f 7469 6d65 2e73 6861  xpanded_time.sha
-00013370: 7065 5b30 5d0d 0a20 2020 2020 2020 2020  pe[0]..         
-00013380: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00013390: 7261 6e67 6528 6c65 6e28 6578 7061 6e64  range(len(expand
-000133a0: 6564 5f74 696d 6529 293a 0d0a 2020 2020  ed_time)):..    
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2065 7870 616e 6465 645f 7469 6d65     expanded_time
-000133d0: 5b69 5d20 3d20 6920 0d0a 2020 2020 2020  [i] = i ..      
-000133e0: 2020 2020 2020 2020 2020 666f 7220 6375            for cu
-000133f0: 7272 656e 745f 756e 6971 7565 5f69 6420  rrent_unique_id 
-00013400: 696e 2075 6e69 7175 655f 6964 735f 7365  in unique_ids_se
-00013410: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00013420: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013430: 2020 2020 2020 2020 2020 2020 6578 7061              expa
-00013440: 6e64 6564 5f69 6e74 656e 7369 7479 203d  nded_intensity =
-00013450: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
-00013460: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
-00013470: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
-00013480: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000134b0: 2020 2020 2063 7572 7265 6e74 5f74 696d       current_tim
-000134c0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000134d0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-000134e0: 6e74 5f7a 203d 205b 5d0d 0a20 2020 2020  nt_z = []..     
-000134f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013500: 7272 656e 745f 7920 3d20 5b5d 0d0a 2020  rrent_y = []..  
-00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013520: 2063 7572 7265 6e74 5f78 203d 205b 5d0d   current_x = [].
-00013530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013540: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
-00013550: 6e73 6974 7920 3d20 5b5d 0d0a 2020 2020  nsity = []..    
-00013560: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013570: 7572 7265 6e74 5f72 6164 6975 7320 3d20  urrent_radius = 
-00013580: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013590: 2020 2020 2020 2063 7572 7265 6e74 5f76         current_v
-000135a0: 6f6c 756d 6520 3d20 5b5d 0d0a 2020 2020  olume = []..    
-000135b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000135c0: 7572 7265 6e74 5f73 7065 6564 203d 205b  urrent_speed = [
-000135d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000135e0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-000135f0: 7469 6f6e 5f61 6e67 6c65 203d 205b 5d0d  tion_angle = [].
-00013600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013610: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00013620: 6c65 7261 7469 6f6e 203d 205b 5d0d 0a20  leration = [].. 
-00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013640: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
-00013650: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00013660: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00013670: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
-00013680: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013690: 6669 7273 7420 3d20 5b5d 0d0a 2020 2020  first = []..    
-000136a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000136b0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-000136c0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
-000136d0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000136e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000136f0: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-00013700: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00013710: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013720: 5f72 6164 6961 6c5f 616e 676c 6520 3d20  _radial_angle = 
-00013730: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013740: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00013750: 656c 6c5f 6178 6973 5f6d 6173 6b20 3d20  ell_axis_mask = 
-00013760: 5b5d 200d 0a20 2020 2020 2020 2020 2020  [] ..           
-00013770: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013780: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00013790: 206a 2069 6e20 7261 6e67 6528 7469 6d65   j in range(time
-000137a0: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
-000137b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137c0: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
-000137d0: 745f 756e 6971 7565 5f69 6420 3d3d 2075  t_unique_id == u
-000137e0: 6e69 7175 655f 6964 735b 6a5d 3a0d 0a20  nique_ids[j]:.. 
-000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013810: 6375 7272 656e 745f 7469 6d65 2e61 7070  current_time.app
-00013820: 656e 6428 7469 6d65 5b6a 5d29 0d0a 2020  end(time[j])..  
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013850: 7572 7265 6e74 5f7a 2e61 7070 656e 6428  urrent_z.append(
-00013860: 5a5b 6a5d 290d 0a20 2020 2020 2020 2020  Z[j])..         
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013890: 792e 6170 7065 6e64 2859 5b6a 5d29 0d0a  y.append(Y[j])..
+00012b10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012b20: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00012b30: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012b40: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00012b50: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00012b60: 6975 735f 6b65 7920 3a20 7261 6469 7573  ius_key : radius
+00012b70: 207d 290d 0a20 2020 2020 2020 2020 2020   })..           
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ba0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012c20: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012c30: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012c40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00012c50: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00012c60: 705f 6669 7273 746b 6579 203a 202d 317d  p_firstkey : -1}
+00012c70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ca0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012cb0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012cc0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00012cd0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00012ce0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+00012cf0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+00012d00: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
+00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012d40: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00012d50: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012d60: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00012d70: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
+00012d80: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
+00012d90: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dc0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00012dd0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00012de0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00012df0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+00012e00: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
+00012e10: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012e60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012e70: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012e80: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00012e90: 7261 6469 7573 5f6b 6579 203a 202d 3120  radius_key : -1 
+00012ea0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 2020 2020 2020 200d 0a0d 0a0d 0a0d 0a0d         .........
+00012ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f00: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f20: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+00012f30: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
+00012f40: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012f70: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
+00012f80: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00012f90: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
+00012fa0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00012fb0: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00012fc0: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
+00012fd0: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
+00012fe0: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
+00012ff0: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
+00013000: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
+00013010: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00013020: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00013030: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+00013040: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
+00013050: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
+00013060: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
+00013070: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
+00013080: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
+00013090: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+000130a0: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
+000130b0: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
+000130c0: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
+000130d0: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
+000130e0: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
+000130f0: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
+00013100: 2020 2020 2020 2020 2020 2020 2020 5820                X 
+00013110: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
+00013120: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00013130: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
+00013140: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
+00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013160: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
+00013170: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00013180: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
+00013190: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
+000131a0: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
+000131b0: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
+000131c0: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+000131d0: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
+000131e0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000131f0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
+00013200: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
+00013210: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00013220: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
+00013230: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
+00013240: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00013250: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
+00013260: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+00013270: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00013280: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
+00013290: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
+000132a0: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+000132b0: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+000132c0: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
+000132d0: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
+000132e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000132f0: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
+00013300: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00013310: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
+00013320: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00013330: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+00013340: 656e 7369 7479 203d 2074 7261 636b 6c65  ensity = trackle
+00013350: 745f 7072 6f70 6572 7469 6573 5b3a 2c38  t_properties[:,8
+00013360: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013370: 2020 2073 7065 6564 203d 2074 7261 636b     speed = track
+00013380: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00013390: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
+000133a0: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
+000133b0: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+000133c0: 7065 7274 6965 735b 3a2c 3130 5d0d 0a20  perties[:,10].. 
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000133e0: 6363 656c 6572 6174 696f 6e20 3d20 7472  cceleration = tr
+000133f0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00013400: 735b 3a2c 3131 5d0d 0a20 2020 2020 2020  s[:,11]..       
+00013410: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+00013420: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7472  e_cell_mask = tr
+00013430: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00013440: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
+00013450: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
+00013460: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
+00013470: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
+00013480: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013490: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
+000134a0: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
+000134b0: 7065 7274 6965 735b 3a2c 3134 5d0d 0a0d  perties[:,14]...
+000134c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000134d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000134e0: 2020 2020 2075 6e69 7175 655f 6666 745f       unique_fft_
+000134f0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00013500: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
+00013510: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013520: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+00013530: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
+00013540: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00013550: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
+00013560: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
+00013570: 6163 6b5f 6964 5d20 3d20 7b7d 0d0a 2020  ack_id] = {}..  
+00013580: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013590: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
+000135a0: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
+000135b0: 636b 5f69 645d 203d 207b 7d0d 0a0d 0a20  ck_id] = {}.... 
+000135c0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000135d0: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
+000135e0: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
+000135f0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00013600: 2020 2020 2020 756e 6971 7565 5f64 796e        unique_dyn
+00013610: 616d 6963 5f70 726f 7065 7274 6965 735f  amic_properties_
+00013620: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
+00013630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013640: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
+00013650: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
+00013660: 6b5f 6964 5d20 3d20 7b7d 0d0a 2020 2020  k_id] = {}..    
+00013670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013680: 2e75 6e69 7175 655f 6479 6e61 6d69 635f  .unique_dynamic_
+00013690: 7072 6f70 6572 7469 6573 5b74 7261 636b  properties[track
+000136a0: 5f69 645d 203d 207b 7d0d 0a20 2020 2020  _id] = {}..     
+000136b0: 2020 2020 2020 2020 2020 2065 7870 616e             expan
+000136c0: 6465 645f 7469 6d65 203d 206e 702e 7a65  ded_time = np.ze
+000136d0: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
+000136e0: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
+000136f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013700: 2020 706f 696e 745f 7361 6d70 6c65 203d    point_sample =
+00013710: 2065 7870 616e 6465 645f 7469 6d65 2e73   expanded_time.s
+00013720: 6861 7065 5b30 5d0d 0a20 2020 2020 2020  hape[0]..       
+00013730: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00013740: 6e20 7261 6e67 6528 6c65 6e28 6578 7061  n range(len(expa
+00013750: 6e64 6564 5f74 696d 6529 293a 0d0a 2020  nded_time)):..  
+00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013770: 2020 2020 2065 7870 616e 6465 645f 7469       expanded_ti
+00013780: 6d65 5b69 5d20 3d20 6920 0d0a 2020 2020  me[i] = i ..    
+00013790: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000137a0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+000137b0: 6420 696e 2075 6e69 7175 655f 6964 735f  d in unique_ids_
+000137c0: 7365 743a 0d0a 2020 2020 2020 2020 2020  set:..          
+000137d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000137e0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000137f0: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
+00013800: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
+00013810: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
+00013820: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
+00013830: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013850: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00013860: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00013870: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
+00013880: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013890: 7265 6e74 5f7a 203d 205b 5d0d 0a20 2020  rent_z = []..   
 000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138c0: 2063 7572 7265 6e74 5f78 2e61 7070 656e   current_x.appen
-000138d0: 6428 585b 6a5d 290d 0a20 2020 2020 2020  d(X[j])..       
-000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
-00013900: 6564 5f69 6e74 656e 7369 7479 5b69 6e74  ed_intensity[int
-00013910: 2874 696d 655b 6a5d 295d 203d 2069 6e74  (time[j])] = int
-00013920: 656e 7369 7479 5b6a 5d0d 0a20 2020 2020  ensity[j]..     
-00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013940: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013950: 656e 745f 696e 7465 6e73 6974 792e 6170  ent_intensity.ap
-00013960: 7065 6e64 2869 6e74 656e 7369 7479 5b6a  pend(intensity[j
-00013970: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013990: 2020 2020 2063 7572 7265 6e74 5f72 6164       current_rad
-000139a0: 6975 732e 6170 7065 6e64 2872 6164 6975  ius.append(radiu
-000139b0: 735b 6a5d 290d 0a20 2020 2020 2020 2020  s[j])..         
-000139c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139d0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000139e0: 766f 6c75 6d65 2e61 7070 656e 6428 766f  volume.append(vo
-000139f0: 6c75 6d65 5b6a 5d29 0d0a 2020 2020 2020  lume[j])..      
-00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a10: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013a20: 6e74 5f73 7065 6564 2e61 7070 656e 6428  nt_speed.append(
-00013a30: 7370 6565 645b 6a5d 290d 0a20 2020 2020  speed[j])..     
-00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013a60: 656e 745f 6d6f 7469 6f6e 5f61 6e67 6c65  ent_motion_angle
-00013a70: 2e61 7070 656e 6428 6d6f 7469 6f6e 5f61  .append(motion_a
-00013a80: 6e67 6c65 5b6a 5d29 0d0a 2020 2020 2020  ngle[j])..      
-00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013aa0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013ab0: 6e74 5f61 6363 656c 6572 6174 696f 6e2e  nt_acceleration.
-00013ac0: 6170 7065 6e64 2861 6363 656c 6572 6174  append(accelerat
-00013ad0: 696f 6e5b 6a5d 290d 0a20 2020 2020 2020  ion[j])..       
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013af0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013b00: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-00013b10: 6d61 736b 2e61 7070 656e 6428 6469 7374  mask.append(dist
-00013b20: 616e 6365 5f63 656c 6c5f 6d61 736b 5b6a  ance_cell_mask[j
-00013b30: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b50: 2020 2020 2063 7572 7265 6e74 5f65 6363       current_ecc
-00013b60: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00013b70: 6972 7374 2e61 7070 656e 6428 6563 6365  irst.append(ecce
-00013b80: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00013b90: 7273 745b 6a5d 290d 0a20 2020 2020 2020  rst[j])..       
-00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bb0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013bc0: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00013bd0: 6f6d 705f 7365 636f 6e64 2e61 7070 656e  omp_second.appen
-00013be0: 6428 6563 6365 6e74 7269 6369 7479 5f63  d(eccentricity_c
-00013bf0: 6f6d 705f 7365 636f 6e64 5b6a 5d29 0d0a  omp_second[j])..
-00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c20: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
-00013c30: 5f61 7265 612e 6170 7065 6e64 2873 7572  _area.append(sur
-00013c40: 6661 6365 5f61 7265 615b 6a5d 290d 0a20  face_area[j]).. 
-00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138b0: 6375 7272 656e 745f 7920 3d20 5b5d 0d0a  current_y = []..
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138d0: 2020 2063 7572 7265 6e74 5f78 203d 205b     current_x = [
+000138e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000138f0: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
+00013900: 7465 6e73 6974 7920 3d20 5b5d 0d0a 2020  tensity = []..  
+00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013920: 2063 7572 7265 6e74 5f72 6164 6975 7320   current_radius 
+00013930: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00013940: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013950: 5f76 6f6c 756d 6520 3d20 5b5d 0d0a 2020  _volume = []..  
+00013960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013970: 2063 7572 7265 6e74 5f73 7065 6564 203d   current_speed =
+00013980: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00013990: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000139a0: 6d6f 7469 6f6e 5f61 6e67 6c65 203d 205b  motion_angle = [
+000139b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000139c0: 2020 2020 2020 6375 7272 656e 745f 6163        current_ac
+000139d0: 6365 6c65 7261 7469 6f6e 203d 205b 5d0d  celeration = [].
+000139e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000139f0: 2020 2020 6375 7272 656e 745f 6469 7374      current_dist
+00013a00: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
+00013a10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00013a20: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013a30: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013a40: 705f 6669 7273 7420 3d20 5b5d 0d0a 2020  p_first = []..  
+00013a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a60: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+00013a70: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00013a80: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+00013a90: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013aa0: 6e74 5f73 7572 6661 6365 5f61 7265 6120  nt_surface_area 
+00013ab0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00013ac0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013ad0: 6e74 5f72 6164 6961 6c5f 616e 676c 6520  nt_radial_angle 
+00013ae0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00013af0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013b00: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b20  _cell_axis_mask 
+00013b10: 3d20 5b5d 200d 0a20 2020 2020 2020 2020  = [] ..         
+00013b20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013b30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00013b40: 6f72 206a 2069 6e20 7261 6e67 6528 7469  or j in range(ti
+00013b50: 6d65 2e73 6861 7065 5b30 5d29 3a0d 0a20  me.shape[0]):.. 
+00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b70: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
+00013b80: 656e 745f 756e 6971 7565 5f69 6420 3d3d  ent_unique_id ==
+00013b90: 2075 6e69 7175 655f 6964 735b 6a5d 3a0d   unique_ids[j]:.
+00013ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bc0: 2020 6375 7272 656e 745f 7469 6d65 2e61    current_time.a
+00013bd0: 7070 656e 6428 7469 6d65 5b6a 5d29 0d0a  ppend(time[j])..
+00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2063 7572 7265 6e74 5f7a 2e61 7070 656e   current_z.appen
+00013c10: 6428 5a5b 6a5d 290d 0a20 2020 2020 2020  d(Z[j])..       
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013c40: 745f 792e 6170 7065 6e64 2859 5b6a 5d29  t_y.append(Y[j])
+00013c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 6375 7272 656e 745f 7261 6469 616c 5f61  current_radial_a
-00013c80: 6e67 6c65 2e61 7070 656e 6428 7261 6469  ngle.append(radi
-00013c90: 616c 5f61 6e67 6c65 5b6a 5d29 0d0a 2020  al_angle[j])..  
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013cc0: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-00013cd0: 5f6d 6173 6b2e 6170 7065 6e64 2863 656c  _mask.append(cel
-00013ce0: 6c5f 6178 6973 5f6d 6173 6b5b 6a5d 290d  l_axis_mask[j]).
-00013cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013d00: 2020 2020 6375 7272 656e 745f 7469 6d65      current_time
-00013d10: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013d20: 7272 656e 745f 7469 6d65 2c20 6474 7970  rrent_time, dtyp
-00013d30: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d50: 2020 6375 7272 656e 745f 696e 7465 6e73    current_intens
-00013d60: 6974 7920 3d20 6e70 2e61 7361 7272 6179  ity = np.asarray
-00013d70: 2863 7572 7265 6e74 5f69 6e74 656e 7369  (current_intensi
-00013d80: 7479 2c20 6474 7970 653d 6e70 2e66 6c6f  ty, dtype=np.flo
-00013d90: 6174 3332 290d 0a0d 0a0d 0a0d 0a20 2020  at32)........   
-00013da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013db0: 6375 7272 656e 745f 7261 6469 7573 203d  current_radius =
-00013dc0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00013dd0: 656e 745f 7261 6469 7573 2c20 6474 7970  ent_radius, dtyp
-00013de0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+00013c70: 2020 2063 7572 7265 6e74 5f78 2e61 7070     current_x.app
+00013c80: 656e 6428 585b 6a5d 290d 0a20 2020 2020  end(X[j])..     
+00013c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ca0: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+00013cb0: 6e64 6564 5f69 6e74 656e 7369 7479 5b69  nded_intensity[i
+00013cc0: 6e74 2874 696d 655b 6a5d 295d 203d 2069  nt(time[j])] = i
+00013cd0: 6e74 656e 7369 7479 5b6a 5d0d 0a20 2020  ntensity[j]..   
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cf0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013d00: 7272 656e 745f 696e 7465 6e73 6974 792e  rrent_intensity.
+00013d10: 6170 7065 6e64 2869 6e74 656e 7369 7479  append(intensity
+00013d20: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d40: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+00013d50: 6164 6975 732e 6170 7065 6e64 2872 6164  adius.append(rad
+00013d60: 6975 735b 6a5d 290d 0a20 2020 2020 2020  ius[j])..       
+00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d80: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013d90: 745f 766f 6c75 6d65 2e61 7070 656e 6428  t_volume.append(
+00013da0: 766f 6c75 6d65 5b6a 5d29 0d0a 2020 2020  volume[j])..    
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dc0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013dd0: 7265 6e74 5f73 7065 6564 2e61 7070 656e  rent_speed.appen
+00013de0: 6428 7370 6565 645b 6a5d 290d 0a20 2020  d(speed[j])..   
 00013df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e00: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
-00013e10: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00013e20: 7272 656e 745f 766f 6c75 6d65 2c20 6474  rrent_volume, dt
-00013e30: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00013e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013e50: 2020 2020 6375 7272 656e 745f 6563 6365      current_ecce
-00013e60: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-00013e70: 7273 7420 3d20 6e70 2e61 7361 7272 6179  rst = np.asarray
-00013e80: 2863 7572 7265 6e74 5f65 6363 656e 7472  (current_eccentr
-00013e90: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013ea0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00013eb0: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00013ec0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013ed0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013ee0: 705f 7365 636f 6e64 203d 206e 702e 6173  p_second = np.as
-00013ef0: 6172 7261 7928 6375 7272 656e 745f 6563  array(current_ec
-00013f00: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-00013f10: 7365 636f 6e64 2c20 6474 7970 653d 6e70  second, dtype=np
-00013f20: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00013f30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013f40: 7272 656e 745f 7375 7266 6163 655f 6172  rrent_surface_ar
-00013f50: 6561 203d 206e 702e 6173 6172 7261 7928  ea = np.asarray(
-00013f60: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
-00013f70: 6172 6561 2c20 6474 7970 653d 6e70 2e66  area, dtype=np.f
-00013f80: 6c6f 6174 3332 290d 0a0d 0a20 2020 2020  loat32)....     
-00013f90: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013fa0: 7272 656e 745f 7370 6565 6420 3d20 6e70  rrent_speed = np
-00013fb0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00013fc0: 5f73 7065 6564 2c20 6474 7970 653d 6e70  _speed, dtype=np
-00013fd0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013ff0: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
-00014000: 6c65 203d 206e 702e 6173 6172 7261 7928  le = np.asarray(
-00014010: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
-00014020: 6e67 6c65 2c20 6474 7970 653d 6e70 2e66  ngle, dtype=np.f
-00014030: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00014040: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00014050: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
-00014060: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00014070: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
-00014080: 6f6e 2c20 6474 7970 653d 6e70 2e66 6c6f  on, dtype=np.flo
-00014090: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-000140a0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000140b0: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-000140c0: 6d61 736b 203d 206e 702e 6173 6172 7261  mask = np.asarra
-000140d0: 7928 6375 7272 656e 745f 6469 7374 616e  y(current_distan
-000140e0: 6365 5f63 656c 6c5f 6d61 736b 2c20 6474  ce_cell_mask, dt
-000140f0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00014100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014110: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00014120: 616c 5f61 6e67 6c65 203d 206e 702e 6173  al_angle = np.as
-00014130: 6172 7261 7928 6375 7272 656e 745f 7261  array(current_ra
-00014140: 6469 616c 5f61 6e67 6c65 2c20 6474 7970  dial_angle, dtyp
-00014150: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014170: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
-00014180: 7869 735f 6d61 736b 203d 206e 702e 6173  xis_mask = np.as
-00014190: 6172 7261 7928 6375 7272 656e 745f 6365  array(current_ce
-000141a0: 6c6c 5f61 7869 735f 6d61 736b 2c20 6474  ll_axis_mask, dt
-000141b0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-000141c0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-000141d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000141e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014200: 2020 6966 2070 6f69 6e74 5f73 616d 706c    if point_sampl
-00014210: 6520 3e20 303a 0d0a 2020 2020 2020 2020  e > 0:..        
-00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014230: 2020 2020 2020 2020 7866 5f73 616d 706c          xf_sampl
-00014240: 6520 3d20 6666 7466 7265 7128 706f 696e  e = fftfreq(poin
-00014250: 745f 7361 6d70 6c65 2c20 7365 6c66 2e74  t_sample, self.t
-00014260: 6361 6c69 6272 6174 696f 6e29 0d0a 2020  calibration)..  
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 2020 2020 2020 2020 2020 2020 2020 6666                ff
-00014290: 7473 7472 6970 5f73 616d 706c 6520 3d20  tstrip_sample = 
-000142a0: 6666 7428 6578 7061 6e64 6564 5f69 6e74  fft(expanded_int
-000142b0: 656e 7369 7479 290d 0a20 2020 2020 2020  ensity)..       
-000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142d0: 2020 2020 2020 2020 2066 6674 746f 7461           ffttota
-000142e0: 6c5f 7361 6d70 6c65 203d 206e 702e 6162  l_sample = np.ab
-000142f0: 7328 6666 7473 7472 6970 5f73 616d 706c  s(fftstrip_sampl
-00014300: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2020 2020 7866 5f73 616d 706c 6520 3d20      xf_sample = 
-00014330: 7866 5f73 616d 706c 655b 3020 3a20 6c65  xf_sample[0 : le
-00014340: 6e28 7866 5f73 616d 706c 6529 202f 2f20  n(xf_sample) // 
-00014350: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014370: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
-00014380: 706c 6520 3d20 6666 7474 6f74 616c 5f73  ple = ffttotal_s
-00014390: 616d 706c 655b 3020 3a20 6c65 6e28 6666  ample[0 : len(ff
-000143a0: 7474 6f74 616c 5f73 616d 706c 6529 202f  ttotal_sample) /
-000143b0: 2f20 325d 0d0a 0d0a 2020 2020 2020 2020  / 2]....        
-000143c0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-000143d0: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-000143e0: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-000143f0: 745f 756e 6971 7565 5f69 645d 203d 2065  t_unique_id] = e
-00014400: 7870 616e 6465 645f 7469 6d65 2c20 6578  xpanded_time, ex
-00014410: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-00014420: 2c20 7866 5f73 616d 706c 652c 2066 6674  , xf_sample, fft
-00014430: 746f 7461 6c5f 7361 6d70 6c65 0d0a 2020  total_sample..  
-00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014450: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
-00014460: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00014470: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00014480: 7565 5f69 645d 203d 2020 6375 7272 656e  ue_id] =  curren
-00014490: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
-000144a0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-000144b0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-000144c0: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-000144d0: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
-000144e0: 2063 7572 7265 6e74 5f74 696d 652c 2063   current_time, c
-000144f0: 7572 7265 6e74 5f7a 2c20 6375 7272 656e  urrent_z, curren
-00014500: 745f 792c 2063 7572 7265 6e74 5f78 2c20  t_y, current_x, 
-00014510: 6375 7272 656e 745f 7261 6469 7573 2c20  current_radius, 
-00014520: 6375 7272 656e 745f 766f 6c75 6d65 2c20  current_volume, 
-00014530: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00014540: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
-00014550: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00014560: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-00014570: 642c 2063 7572 7265 6e74 5f73 7572 6661  d, current_surfa
-00014580: 6365 5f61 7265 610d 0a20 2020 2020 2020  ce_area..       
-00014590: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-000145a0: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-000145b0: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-000145c0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-000145d0: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
-000145e0: 2c20 6375 7272 656e 745f 7370 6565 642c  , current_speed,
-000145f0: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
-00014600: 616e 676c 652c 2063 7572 7265 6e74 5f61  angle, current_a
-00014610: 6363 656c 6572 6174 696f 6e2c 2063 7572  cceleration, cur
-00014620: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
-00014630: 6c6c 5f6d 6173 6b2c 2063 7572 7265 6e74  ll_mask, current
-00014640: 5f72 6164 6961 6c5f 616e 676c 652c 2063  _radial_angle, c
-00014650: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-00014660: 5f6d 6173 6b0d 0a20 2020 2020 2020 2020  _mask..         
-00014670: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00014680: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
-00014690: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
-000146a0: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
-000146b0: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
-000146c0: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
-000146d0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
-000146e0: 756e 6971 7565 5f69 645d 7d29 0d0a 2020  unique_id]})..  
-000146f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014700: 2073 656c 662e 756e 6971 7565 5f63 6c75   self.unique_clu
-00014710: 7374 6572 5f70 726f 7065 7274 6965 735b  ster_properties[
-00014720: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
-00014730: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
-00014740: 5f69 643a 756e 6971 7565 5f63 6c75 7374  _id:unique_clust
-00014750: 6572 5f70 726f 7065 7274 6965 735f 7472  er_properties_tr
-00014760: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
-00014770: 6e69 7175 655f 6964 5d7d 290d 0a0d 0a20  nique_id]}).... 
-00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014790: 2020 7365 6c66 2e75 6e69 7175 655f 7368    self.unique_sh
-000147a0: 6170 655f 7072 6f70 6572 7469 6573 5b74  ape_properties[t
-000147b0: 7261 636b 5f69 645d 2e75 7064 6174 6528  rack_id].update(
-000147c0: 7b63 7572 7265 6e74 5f75 6e69 7175 655f  {current_unique_
-000147d0: 6964 3a75 6e69 7175 655f 7368 6170 655f  id:unique_shape_
-000147e0: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-000147f0: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00014800: 7565 5f69 645d 7d29 0d0a 2020 2020 2020  ue_id]})..      
-00014810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00014820: 662e 756e 6971 7565 5f64 796e 616d 6963  f.unique_dynamic
-00014830: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-00014840: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
-00014850: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
-00014860: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
-00014870: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00014880: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00014890: 655f 6964 5d7d 290d 0a0d 0a20 2020 2064  e_id]})....    d
-000148a0: 6566 205f 7365 636f 6e64 5f63 6861 6e6e  ef _second_chann
-000148b0: 656c 5f73 706f 7473 2873 656c 662c 2066  el_spots(self, f
-000148c0: 7261 6d65 2c20 7a2c 2079 2c20 782c 2063  rame, z, y, x, c
-000148d0: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
-000148e0: 293a 0d0a 2020 2020 2020 2020 2020 200d  ):..           .
-000148f0: 0a20 2020 2020 2020 2020 2020 2074 7265  .            tre
-00014900: 652c 2063 656e 7472 6f69 6473 2c20 6c61  e, centroids, la
-00014910: 6265 6c73 2c20 766f 6c75 6d65 2c20 696e  bels, volume, in
-00014920: 7465 6e73 6974 795f 6d65 616e 2c20 696e  tensity_mean, in
-00014930: 7465 6e73 6974 795f 746f 7461 6c2c 2062  tensity_total, b
-00014940: 6f75 6e64 696e 675f 626f 7865 7320 3d20  ounding_boxes = 
-00014950: 7365 6c66 2e5f 7469 6d65 645f 6368 616e  self._timed_chan
-00014960: 6e65 6c5f 7365 675f 696d 6167 655b 7374  nel_seg_image[st
-00014970: 7228 696e 7428 666c 6f61 7428 6672 616d  r(int(float(fram
-00014980: 6529 2929 5d0d 0a20 2020 2020 2020 2020  e)))]..         
-00014990: 2020 2070 6978 656c 7465 7374 6c6f 6361     pixeltestloca
-000149a0: 7469 6f6e 203d 2028 7a2c 792c 7829 0d0a  tion = (z,y,x)..
-000149b0: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-000149c0: 2c20 696e 6465 7820 3d20 7472 6565 2e71  , index = tree.q
-000149d0: 7565 7279 2870 6978 656c 7465 7374 6c6f  uery(pixeltestlo
-000149e0: 6361 7469 6f6e 290d 0a0d 0a0d 0a20 2020  cation)......   
-000149f0: 2020 2020 2020 2020 2062 626f 7820 3d20           bbox = 
-00014a00: 626f 756e 6469 6e67 5f62 6f78 6573 5b69  bounding_boxes[i
-00014a10: 6e64 6578 5d0d 0a20 2020 2020 2020 2020  ndex]..         
-00014a20: 2020 2073 697a 657a 203d 2061 6273 2862     sizez = abs(b
-00014a30: 626f 785b 305d 202d 2062 626f 785b 335d  box[0] - bbox[3]
-00014a40: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00014a50: 697a 6579 203d 2061 6273 2862 626f 785b  izey = abs(bbox[
-00014a60: 315d 202d 2062 626f 785b 345d 290d 0a20  1] - bbox[4]).. 
-00014a70: 2020 2020 2020 2020 2020 2073 697a 6578             sizex
-00014a80: 203d 2061 6273 2862 626f 785b 325d 202d   = abs(bbox[2] -
-00014a90: 2062 626f 785b 355d 2920 0d0a 2020 2020   bbox[5]) ..    
-00014aa0: 2020 2020 2020 2020 7665 746f 5f76 6f6c          veto_vol
-00014ab0: 756d 6520 3d20 7369 7a65 7820 2a20 7369  ume = sizex * si
-00014ac0: 7a65 7920 2a20 7369 7a65 7a0d 0a20 2020  zey * sizez..   
-00014ad0: 2020 2020 2020 2020 2076 6574 6f5f 7261           veto_ra
-00014ae0: 6469 7573 203d 206d 6174 682e 706f 7728  dius = math.pow(
-00014af0: 3320 2a20 7665 746f 5f76 6f6c 756d 6520  3 * veto_volume 
-00014b00: 2f20 2834 202a 206d 6174 682e 7069 292c  / (4 * math.pi),
-00014b10: 2031 2e30 202f 2033 2e30 290d 0a0d 0a20   1.0 / 3.0).... 
-00014b20: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-00014b30: 696f 6e20 3d20 2863 656e 7472 6f69 6473  ion = (centroids
-00014b40: 5b69 6e64 6578 5d5b 305d 202a 2073 656c  [index][0] * sel
-00014b50: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
-00014b60: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-00014b70: 5b31 5d2a 7365 6c66 2e79 6361 6c69 6272  [1]*self.ycalibr
-00014b80: 6174 696f 6e2c 2063 656e 7472 6f69 6473  ation, centroids
-00014b90: 5b69 6e64 6578 5d5b 325d 2a73 656c 662e  [index][2]*self.
-00014ba0: 7863 616c 6962 7261 7469 6f6e 290d 0a20  xcalibration).. 
-00014bb0: 2020 2020 2020 2020 2020 2051 5541 4c49             QUALI
-00014bc0: 5459 203d 206d 6174 682e 706f 7728 766f  TY = math.pow(vo
-00014bd0: 6c75 6d65 5b69 6e64 6578 5d2c 2031 2e30  lume[index], 1.0
-00014be0: 2f33 2e30 290d 0a20 2020 2020 2020 2020  /3.0)..         
-00014bf0: 2020 2052 4144 4955 5320 3d20 6d61 7468     RADIUS = math
-00014c00: 2e70 6f77 2876 6f6c 756d 655b 696e 6465  .pow(volume[inde
-00014c10: 785d 202a 2073 656c 662e 7863 616c 6962  x] * self.xcalib
-00014c20: 7261 7469 6f6e 202a 2073 656c 662e 7963  ration * self.yc
-00014c30: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
-00014c40: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
-00014c50: 312e 302f 332e 3029 200d 0a0d 0a20 2020  1.0/3.0) ....   
-00014c60: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
-00014c70: 655f 6365 6c6c 5f6d 6173 6b2c 206d 6173  e_cell_mask, mas
-00014c80: 6b63 656e 7472 6f69 6420 3d20 7365 6c66  kcentroid = self
-00014c90: 2e5f 6765 745f 626f 756e 6461 7279 5f64  ._get_boundary_d
-00014ca0: 6973 7428 6672 616d 652c 206c 6f63 6174  ist(frame, locat
-00014cb0: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
-00014cc0: 2020 6966 2064 6973 7420 3c3d 2032 202a    if dist <= 2 *
-00014cd0: 2076 6574 6f5f 7261 6469 7573 3a0d 0a20   veto_radius:.. 
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014cf0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-00014d00: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00014d10: 6573 5b63 656c 6c5f 6964 5d20 3d20 7b0d  es[cell_id] = {.
-00014d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014d30: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
-00014d40: 6c6c 6964 5f6b 6579 3a20 696e 7428 6365  llid_key: int(ce
-00014d50: 6c6c 5f69 6429 2c20 0d0a 2020 2020 2020  ll_id), ..      
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d70: 2020 7365 6c66 2e66 7261 6d65 6964 5f6b    self.frameid_k
-00014d80: 6579 203a 2069 6e74 2866 7261 6d65 292c  ey : int(frame),
-00014d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014da0: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-00014db0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-00014dc0: 7428 6365 6e74 726f 6964 735b 696e 6465  t(centroids[inde
-00014dd0: 785d 5b30 5d2a 2073 656c 662e 7a63 616c  x][0]* self.zcal
-00014de0: 6962 7261 7469 6f6e 292c 0d0a 2020 2020  ibration),..    
-00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e00: 2020 2020 7365 6c66 2e79 706f 7369 645f      self.yposid_
-00014e10: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
-00014e20: 726f 6964 735b 696e 6465 785d 5b31 5d2a  roids[index][1]*
-00014e30: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00014e40: 6f6e 292c 0d0a 2020 2020 2020 2020 2020  on),..          
-00014e50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014e60: 6c66 2e78 706f 7369 645f 6b65 7920 3a20  lf.xposid_key : 
-00014e70: 666c 6f61 7428 6365 6e74 726f 6964 735b  float(centroids[
-00014e80: 696e 6465 785d 5b32 5d2a 2073 656c 662e  index][2]* self.
-00014e90: 7863 616c 6962 7261 7469 6f6e 292c 0d0a  xcalibration),..
-00014ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014eb0: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-00014ec0: 636b 6964 5f6b 6579 3a20 696e 7428 7472  ckid_key: int(tr
-00014ed0: 6163 6b5f 6964 292c 0d0a 2020 2020 2020  ack_id),..      
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ef0: 2020 7365 6c66 2e74 6f74 616c 5f69 6e74    self.total_int
-00014f00: 656e 7369 7479 5f6b 6579 203a 2028 666c  ensity_key : (fl
-00014f10: 6f61 7428 696e 7465 6e73 6974 795f 746f  oat(intensity_to
-00014f20: 7461 6c5b 696e 6465 785d 2929 2c0d 0a20  tal[index])),.. 
-00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f40: 2020 2020 2020 2073 656c 662e 6d65 616e         self.mean
-00014f50: 5f69 6e74 656e 7369 7479 5f6b 6579 203a  _intensity_key :
-00014f60: 2028 666c 6f61 7428 696e 7465 6e73 6974   (float(intensit
-00014f70: 795f 6d65 616e 5b69 6e64 6578 5d29 292c  y_mean[index])),
-00014f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014f90: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00014fa0: 6164 6975 735f 6b65 7920 3a20 2866 6c6f  adius_key : (flo
-00014fb0: 6174 2852 4144 4955 5329 292c 0d0a 2020  at(RADIUS)),..  
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-00014fe0: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
-00014ff0: 5155 414c 4954 5929 292c 0d0a 2020 2020  QUALITY)),..    
-00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015010: 2020 2020 7365 6c66 2e64 6973 7461 6e63      self.distanc
-00015020: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 793a  e_cell_mask_key:
-00015030: 2066 6c6f 6174 2864 6973 7461 6e63 655f   float(distance_
-00015040: 6365 6c6c 5f6d 6173 6b29 2c0d 0a20 2020  cell_mask),..   
-00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015060: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-00015070: 6e74 726f 6964 5f7a 5f6b 6579 3a20 666c  ntroid_z_key: fl
-00015080: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-00015090: 5b30 5d29 2c0d 0a20 2020 2020 2020 2020  [0]),..         
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000150b0: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-000150c0: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
-000150d0: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
-000150e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000150f0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00015100: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-00015110: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-00015120: 726f 6964 5b32 5d29 200d 0a0d 0a20 2020  roid[2]) ....   
-00015130: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-00015140: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00015150: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015160: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00015170: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-00015180: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-00015190: 6964 5d20 3d20 7365 6c66 2e75 6e69 7175  id] = self.uniqu
-000151a0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000151b0: 735b 6365 6c6c 5f69 645d 0d0a 2020 2020  s[cell_id]..    
-000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151d0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-000151e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000151f0: 6965 735b 6365 6c6c 5f69 645d 2e75 7064  ies[cell_id].upd
-00015200: 6174 6528 7b73 656c 662e 746f 7461 6c5f  ate({self.total_
-00015210: 696e 7465 6e73 6974 795f 6b65 793a 202d  intensity_key: -
-00015220: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-00015230: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00015240: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-00015250: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-00015260: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
-00015270: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-00015280: 795f 6b65 793a 202d 317d 290d 0a20 2020  y_key: -1})..   
+00013e00: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013e10: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
+00013e20: 6c65 2e61 7070 656e 6428 6d6f 7469 6f6e  le.append(motion
+00013e30: 5f61 6e67 6c65 5b6a 5d29 0d0a 2020 2020  _angle[j])..    
+00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e50: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013e60: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
+00013e70: 6e2e 6170 7065 6e64 2861 6363 656c 6572  n.append(acceler
+00013e80: 6174 696f 6e5b 6a5d 290d 0a20 2020 2020  ation[j])..     
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013eb0: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00013ec0: 6c5f 6d61 736b 2e61 7070 656e 6428 6469  l_mask.append(di
+00013ed0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00013ee0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
+00013f10: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00013f20: 5f66 6972 7374 2e61 7070 656e 6428 6563  _first.append(ec
+00013f30: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013f40: 6669 7273 745b 6a5d 290d 0a20 2020 2020  first[j])..     
+00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f60: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013f70: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013f80: 5f63 6f6d 705f 7365 636f 6e64 2e61 7070  _comp_second.app
+00013f90: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
+00013fa0: 5f63 6f6d 705f 7365 636f 6e64 5b6a 5d29  _comp_second[j])
+00013fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00013fe0: 6365 5f61 7265 612e 6170 7065 6e64 2873  ce_area.append(s
+00013ff0: 7572 6661 6365 5f61 7265 615b 6a5d 290d  urface_area[j]).
+00014000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014020: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
+00014030: 5f61 6e67 6c65 2e61 7070 656e 6428 7261  _angle.append(ra
+00014040: 6469 616c 5f61 6e67 6c65 5b6a 5d29 0d0a  dial_angle[j])..
+00014050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014070: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00014080: 6973 5f6d 6173 6b2e 6170 7065 6e64 2863  is_mask.append(c
+00014090: 656c 6c5f 6178 6973 5f6d 6173 6b5b 6a5d  ell_axis_mask[j]
+000140a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000140b0: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
+000140c0: 6d65 203d 206e 702e 6173 6172 7261 7928  me = np.asarray(
+000140d0: 6375 7272 656e 745f 7469 6d65 2c20 6474  current_time, dt
+000140e0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+000140f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014100: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
+00014110: 6e73 6974 7920 3d20 6e70 2e61 7361 7272  nsity = np.asarr
+00014120: 6179 2863 7572 7265 6e74 5f69 6e74 656e  ay(current_inten
+00014130: 7369 7479 2c20 6474 7970 653d 6e70 2e66  sity, dtype=np.f
+00014140: 6c6f 6174 3332 290d 0a0d 0a0d 0a0d 0a20  loat32)........ 
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 6375 7272 656e 745f 7261 6469 7573    current_radius
+00014170: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00014180: 7272 656e 745f 7261 6469 7573 2c20 6474  rrent_radius, dt
+00014190: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+000141a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000141b0: 2020 2020 6375 7272 656e 745f 766f 6c75      current_volu
+000141c0: 6d65 203d 206e 702e 6173 6172 7261 7928  me = np.asarray(
+000141d0: 6375 7272 656e 745f 766f 6c75 6d65 2c20  current_volume, 
+000141e0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000141f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014200: 2020 2020 2020 6375 7272 656e 745f 6563        current_ec
+00014210: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00014220: 6669 7273 7420 3d20 6e70 2e61 7361 7272  first = np.asarr
+00014230: 6179 2863 7572 7265 6e74 5f65 6363 656e  ay(current_eccen
+00014240: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+00014250: 7374 2c20 6474 7970 653d 6e70 2e66 6c6f  st, dtype=np.flo
+00014260: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00014270: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00014280: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00014290: 6f6d 705f 7365 636f 6e64 203d 206e 702e  omp_second = np.
+000142a0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+000142b0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+000142c0: 705f 7365 636f 6e64 2c20 6474 7970 653d  p_second, dtype=
+000142d0: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
+000142e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142f0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
+00014300: 6172 6561 203d 206e 702e 6173 6172 7261  area = np.asarra
+00014310: 7928 6375 7272 656e 745f 7375 7266 6163  y(current_surfac
+00014320: 655f 6172 6561 2c20 6474 7970 653d 6e70  e_area, dtype=np
+00014330: 2e66 6c6f 6174 3332 290d 0a0d 0a20 2020  .float32)....   
+00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014350: 6375 7272 656e 745f 7370 6565 6420 3d20  current_speed = 
+00014360: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00014370: 6e74 5f73 7065 6564 2c20 6474 7970 653d  nt_speed, dtype=
+00014380: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
+00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143a0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+000143b0: 6e67 6c65 203d 206e 702e 6173 6172 7261  ngle = np.asarra
+000143c0: 7928 6375 7272 656e 745f 6d6f 7469 6f6e  y(current_motion
+000143d0: 5f61 6e67 6c65 2c20 6474 7970 653d 6e70  _angle, dtype=np
+000143e0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
+000143f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00014400: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00014410: 6f6e 203d 206e 702e 6173 6172 7261 7928  on = np.asarray(
+00014420: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00014430: 7469 6f6e 2c20 6474 7970 653d 6e70 2e66  tion, dtype=np.f
+00014440: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00014450: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00014460: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00014470: 6c5f 6d61 736b 203d 206e 702e 6173 6172  l_mask = np.asar
+00014480: 7261 7928 6375 7272 656e 745f 6469 7374  ray(current_dist
+00014490: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+000144a0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+000144b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000144c0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
+000144d0: 6469 616c 5f61 6e67 6c65 203d 206e 702e  dial_angle = np.
+000144e0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+000144f0: 7261 6469 616c 5f61 6e67 6c65 2c20 6474  radial_angle, dt
+00014500: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00014510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014520: 2020 2020 6375 7272 656e 745f 6365 6c6c      current_cell
+00014530: 5f61 7869 735f 6d61 736b 203d 206e 702e  _axis_mask = np.
+00014540: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00014550: 6365 6c6c 5f61 7869 735f 6d61 736b 2c20  cell_axis_mask, 
+00014560: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00014570: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
+00014580: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00014590: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000145a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145b0: 2020 2020 6966 2070 6f69 6e74 5f73 616d      if point_sam
+000145c0: 706c 6520 3e20 303a 0d0a 2020 2020 2020  ple > 0:..      
+000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145e0: 2020 2020 2020 2020 2020 7866 5f73 616d            xf_sam
+000145f0: 706c 6520 3d20 6666 7466 7265 7128 706f  ple = fftfreq(po
+00014600: 696e 745f 7361 6d70 6c65 2c20 7365 6c66  int_sample, self
+00014610: 2e74 6361 6c69 6272 6174 696f 6e29 0d0a  .tcalibration)..
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014640: 6666 7473 7472 6970 5f73 616d 706c 6520  fftstrip_sample 
+00014650: 3d20 6666 7428 6578 7061 6e64 6564 5f69  = fft(expanded_i
+00014660: 6e74 656e 7369 7479 290d 0a20 2020 2020  ntensity)..     
+00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014680: 2020 2020 2020 2020 2020 2066 6674 746f             fftto
+00014690: 7461 6c5f 7361 6d70 6c65 203d 206e 702e  tal_sample = np.
+000146a0: 6162 7328 6666 7473 7472 6970 5f73 616d  abs(fftstrip_sam
+000146b0: 706c 6529 0d0a 2020 2020 2020 2020 2020  ple)..          
+000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146d0: 2020 2020 2020 7866 5f73 616d 706c 6520        xf_sample 
+000146e0: 3d20 7866 5f73 616d 706c 655b 3020 3a20  = xf_sample[0 : 
+000146f0: 6c65 6e28 7866 5f73 616d 706c 6529 202f  len(xf_sample) /
+00014700: 2f20 325d 0d0a 2020 2020 2020 2020 2020  / 2]..          
+00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014720: 2020 2020 2020 6666 7474 6f74 616c 5f73        ffttotal_s
+00014730: 616d 706c 6520 3d20 6666 7474 6f74 616c  ample = ffttotal
+00014740: 5f73 616d 706c 655b 3020 3a20 6c65 6e28  _sample[0 : len(
+00014750: 6666 7474 6f74 616c 5f73 616d 706c 6529  ffttotal_sample)
+00014760: 202f 2f20 325d 0d0a 0d0a 2020 2020 2020   // 2]....      
+00014770: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00014780: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+00014790: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+000147a0: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
+000147b0: 2065 7870 616e 6465 645f 7469 6d65 2c20   expanded_time, 
+000147c0: 6578 7061 6e64 6564 5f69 6e74 656e 7369  expanded_intensi
+000147d0: 7479 2c20 7866 5f73 616d 706c 652c 2066  ty, xf_sample, f
+000147e0: 6674 746f 7461 6c5f 7361 6d70 6c65 0d0a  fttotal_sample..
+000147f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014800: 2020 2075 6e69 7175 655f 636c 7573 7465     unique_cluste
+00014810: 725f 7072 6f70 6572 7469 6573 5f74 7261  r_properties_tra
+00014820: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00014830: 6971 7565 5f69 645d 203d 2020 6375 7272  ique_id] =  curr
+00014840: 656e 745f 7469 6d65 0d0a 2020 2020 2020  ent_time..      
+00014850: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00014860: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
+00014870: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
+00014880: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
+00014890: 203d 2063 7572 7265 6e74 5f74 696d 652c   = current_time,
+000148a0: 2063 7572 7265 6e74 5f7a 2c20 6375 7272   current_z, curr
+000148b0: 656e 745f 792c 2063 7572 7265 6e74 5f78  ent_y, current_x
+000148c0: 2c20 6375 7272 656e 745f 7261 6469 7573  , current_radius
+000148d0: 2c20 6375 7272 656e 745f 766f 6c75 6d65  , current_volume
+000148e0: 2c20 6375 7272 656e 745f 6563 6365 6e74  , current_eccent
+000148f0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00014900: 742c 2063 7572 7265 6e74 5f65 6363 656e  t, current_eccen
+00014910: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00014920: 6f6e 642c 2063 7572 7265 6e74 5f73 7572  ond, current_sur
+00014930: 6661 6365 5f61 7265 610d 0a20 2020 2020  face_area..     
+00014940: 2020 2020 2020 2020 2020 2020 2020 756e                un
+00014950: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+00014960: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00014970: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+00014980: 6964 5d20 3d20 6375 7272 656e 745f 7469  id] = current_ti
+00014990: 6d65 2c20 6375 7272 656e 745f 7370 6565  me, current_spee
+000149a0: 642c 2063 7572 7265 6e74 5f6d 6f74 696f  d, current_motio
+000149b0: 6e5f 616e 676c 652c 2063 7572 7265 6e74  n_angle, current
+000149c0: 5f61 6363 656c 6572 6174 696f 6e2c 2063  _acceleration, c
+000149d0: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
+000149e0: 6365 6c6c 5f6d 6173 6b2c 2063 7572 7265  cell_mask, curre
+000149f0: 6e74 5f72 6164 6961 6c5f 616e 676c 652c  nt_radial_angle,
+00014a00: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00014a10: 6973 5f6d 6173 6b0d 0a20 2020 2020 2020  is_mask..       
+00014a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014a30: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
+00014a40: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00014a50: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
+00014a60: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
+00014a70: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00014a80: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00014a90: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ab0: 2020 2073 656c 662e 756e 6971 7565 5f63     self.unique_c
+00014ac0: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
+00014ad0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
+00014ae0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
+00014af0: 7565 5f69 643a 756e 6971 7565 5f63 6c75  ue_id:unique_clu
+00014b00: 7374 6572 5f70 726f 7065 7274 6965 735f  ster_properties_
+00014b10: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00014b20: 5f75 6e69 7175 655f 6964 5d7d 290d 0a0d  _unique_id]})...
+00014b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00014b50: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
+00014b60: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
+00014b70: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
+00014b80: 655f 6964 3a75 6e69 7175 655f 7368 6170  e_id:unique_shap
+00014b90: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
+00014ba0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+00014bb0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
+00014bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014bd0: 656c 662e 756e 6971 7565 5f64 796e 616d  elf.unique_dynam
+00014be0: 6963 5f70 726f 7065 7274 6965 735b 7472  ic_properties[tr
+00014bf0: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+00014c00: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00014c10: 643a 756e 6971 7565 5f64 796e 616d 6963  d:unique_dynamic
+00014c20: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00014c30: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00014c40: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
+00014c50: 2064 6566 205f 7365 636f 6e64 5f63 6861   def _second_cha
+00014c60: 6e6e 656c 5f73 706f 7473 2873 656c 662c  nnel_spots(self,
+00014c70: 2066 7261 6d65 2c20 7a2c 2079 2c20 782c   frame, z, y, x,
+00014c80: 2063 656c 6c5f 6964 2c20 7472 6163 6b5f   cell_id, track_
+00014c90: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
+00014ca0: 200d 0a20 2020 2020 2020 2020 2020 2074   ..            t
+00014cb0: 7265 652c 2063 656e 7472 6f69 6473 2c20  ree, centroids, 
+00014cc0: 6c61 6265 6c73 2c20 766f 6c75 6d65 2c20  labels, volume, 
+00014cd0: 696e 7465 6e73 6974 795f 6d65 616e 2c20  intensity_mean, 
+00014ce0: 696e 7465 6e73 6974 795f 746f 7461 6c2c  intensity_total,
+00014cf0: 2062 6f75 6e64 696e 675f 626f 7865 7320   bounding_boxes 
+00014d00: 3d20 7365 6c66 2e5f 7469 6d65 645f 6368  = self._timed_ch
+00014d10: 616e 6e65 6c5f 7365 675f 696d 6167 655b  annel_seg_image[
+00014d20: 7374 7228 696e 7428 666c 6f61 7428 6672  str(int(float(fr
+00014d30: 616d 6529 2929 5d0d 0a20 2020 2020 2020  ame)))]..       
+00014d40: 2020 2020 2070 6978 656c 7465 7374 6c6f       pixeltestlo
+00014d50: 6361 7469 6f6e 203d 2028 7a2c 792c 7829  cation = (z,y,x)
+00014d60: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+00014d70: 7374 2c20 696e 6465 7820 3d20 7472 6565  st, index = tree
+00014d80: 2e71 7565 7279 2870 6978 656c 7465 7374  .query(pixeltest
+00014d90: 6c6f 6361 7469 6f6e 290d 0a0d 0a0d 0a20  location)...... 
+00014da0: 2020 2020 2020 2020 2020 2062 626f 7820             bbox 
+00014db0: 3d20 626f 756e 6469 6e67 5f62 6f78 6573  = bounding_boxes
+00014dc0: 5b69 6e64 6578 5d0d 0a20 2020 2020 2020  [index]..       
+00014dd0: 2020 2020 2073 697a 657a 203d 2061 6273       sizez = abs
+00014de0: 2862 626f 785b 305d 202d 2062 626f 785b  (bbox[0] - bbox[
+00014df0: 335d 290d 0a20 2020 2020 2020 2020 2020  3])..           
+00014e00: 2073 697a 6579 203d 2061 6273 2862 626f   sizey = abs(bbo
+00014e10: 785b 315d 202d 2062 626f 785b 345d 290d  x[1] - bbox[4]).
+00014e20: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00014e30: 6578 203d 2061 6273 2862 626f 785b 325d  ex = abs(bbox[2]
+00014e40: 202d 2062 626f 785b 355d 2920 0d0a 2020   - bbox[5]) ..  
+00014e50: 2020 2020 2020 2020 2020 7665 746f 5f76            veto_v
+00014e60: 6f6c 756d 6520 3d20 7369 7a65 7820 2a20  olume = sizex * 
+00014e70: 7369 7a65 7920 2a20 7369 7a65 7a0d 0a20  sizey * sizez.. 
+00014e80: 2020 2020 2020 2020 2020 2076 6574 6f5f             veto_
+00014e90: 7261 6469 7573 203d 206d 6174 682e 706f  radius = math.po
+00014ea0: 7728 3320 2a20 7665 746f 5f76 6f6c 756d  w(3 * veto_volum
+00014eb0: 6520 2f20 2834 202a 206d 6174 682e 7069  e / (4 * math.pi
+00014ec0: 292c 2031 2e30 202f 2033 2e30 290d 0a0d  ), 1.0 / 3.0)...
+00014ed0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+00014ee0: 6174 696f 6e20 3d20 2863 656e 7472 6f69  ation = (centroi
+00014ef0: 6473 5b69 6e64 6578 5d5b 305d 202a 2073  ds[index][0] * s
+00014f00: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00014f10: 2c20 6365 6e74 726f 6964 735b 696e 6465  , centroids[inde
+00014f20: 785d 5b31 5d2a 7365 6c66 2e79 6361 6c69  x][1]*self.ycali
+00014f30: 6272 6174 696f 6e2c 2063 656e 7472 6f69  bration, centroi
+00014f40: 6473 5b69 6e64 6578 5d5b 325d 2a73 656c  ds[index][2]*sel
+00014f50: 662e 7863 616c 6962 7261 7469 6f6e 290d  f.xcalibration).
+00014f60: 0a20 2020 2020 2020 2020 2020 2051 5541  .            QUA
+00014f70: 4c49 5459 203d 206d 6174 682e 706f 7728  LITY = math.pow(
+00014f80: 766f 6c75 6d65 5b69 6e64 6578 5d2c 2031  volume[index], 1
+00014f90: 2e30 2f33 2e30 290d 0a20 2020 2020 2020  .0/3.0)..       
+00014fa0: 2020 2020 2052 4144 4955 5320 3d20 6d61       RADIUS = ma
+00014fb0: 7468 2e70 6f77 2876 6f6c 756d 655b 696e  th.pow(volume[in
+00014fc0: 6465 785d 202a 2073 656c 662e 7863 616c  dex] * self.xcal
+00014fd0: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+00014fe0: 7963 616c 6962 7261 7469 6f6e 202a 2073  ycalibration * s
+00014ff0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+00015000: 2c20 312e 302f 332e 3029 200d 0a0d 0a20  , 1.0/3.0) .... 
+00015010: 2020 2020 2020 2020 2020 2064 6973 7461             dista
+00015020: 6e63 655f 6365 6c6c 5f6d 6173 6b2c 206d  nce_cell_mask, m
+00015030: 6173 6b63 656e 7472 6f69 6420 3d20 7365  askcentroid = se
+00015040: 6c66 2e5f 6765 745f 626f 756e 6461 7279  lf._get_boundary
+00015050: 5f64 6973 7428 6672 616d 652c 206c 6f63  _dist(frame, loc
+00015060: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00015070: 2020 2020 6966 2064 6973 7420 3c3d 2032      if dist <= 2
+00015080: 202a 2076 6574 6f5f 7261 6469 7573 3a0d   * veto_radius:.
+00015090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150a0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+000150b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000150c0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
+000150d0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+000150e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000150f0: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
+00015100: 6365 6c6c 5f69 6429 2c20 0d0a 2020 2020  cell_id), ..    
+00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015120: 2020 2020 7365 6c66 2e66 7261 6d65 6964      self.frameid
+00015130: 5f6b 6579 203a 2069 6e74 2866 7261 6d65  _key : int(frame
+00015140: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00015150: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015160: 2e7a 706f 7369 645f 6b65 7920 3a20 666c  .zposid_key : fl
+00015170: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
+00015180: 6465 785d 5b30 5d2a 2073 656c 662e 7a63  dex][0]* self.zc
+00015190: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
+000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151b0: 2020 2020 2020 7365 6c66 2e79 706f 7369        self.yposi
+000151c0: 645f 6b65 7920 3a20 666c 6f61 7428 6365  d_key : float(ce
+000151d0: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
+000151e0: 5d2a 2073 656c 662e 7963 616c 6962 7261  ]* self.ycalibra
+000151f0: 7469 6f6e 292c 0d0a 2020 2020 2020 2020  tion),..        
+00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015210: 7365 6c66 2e78 706f 7369 645f 6b65 7920  self.xposid_key 
+00015220: 3a20 666c 6f61 7428 6365 6e74 726f 6964  : float(centroid
+00015230: 735b 696e 6465 785d 5b32 5d2a 2073 656c  s[index][2]* sel
+00015240: 662e 7863 616c 6962 7261 7469 6f6e 292c  f.xcalibration),
+00015250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015260: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00015270: 7261 636b 6964 5f6b 6579 3a20 696e 7428  rackid_key: int(
+00015280: 7472 6163 6b5f 6964 292c 0d0a 2020 2020  track_id),..    
 00015290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152a0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-000152b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000152c0: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-000152d0: 6461 7465 287b 7365 6c66 2e72 6164 6975  date({self.radiu
-000152e0: 735f 6b65 793a 202d 317d 290d 0a20 2020  s_key: -1})..   
-000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015300: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00015310: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015320: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00015330: 6461 7465 287b 7365 6c66 2e71 7561 6c69  date({self.quali
-00015340: 7479 5f6b 6579 3a20 2d31 7d29 0d0a 0d0a  ty_key: -1})....
-00015350: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015370: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
-00015380: 6469 6374 5f75 7064 6174 6528 7365 6c66  dict_update(self
-00015390: 2c20 756e 6971 7565 5f74 7261 636b 6c65  , unique_trackle
-000153a0: 745f 6964 733a 204c 6973 742c 2020 6365  t_ids: List,  ce
-000153b0: 6c6c 5f69 643a 2069 6e74 2c20 7472 6163  ll_id: int, trac
-000153c0: 6b5f 6964 3a20 696e 742c 2073 6f75 7263  k_id: int, sourc
-000153d0: 655f 6964 3a20 696e 742c 2074 6172 6765  e_id: int, targe
-000153e0: 745f 6964 3a20 696e 7429 3a0d 0a0d 0a20  t_id: int):.... 
-000153f0: 0d0a 2020 2020 2020 2020 6765 6e65 7261  ..        genera
-00015400: 7469 6f6e 5f69 6420 3d20 7365 6c66 2e67  tion_id = self.g
-00015410: 656e 6572 6174 696f 6e5f 6469 6374 5b63  eneration_dict[c
-00015420: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
-00015430: 2074 7261 636b 6c65 745f 6964 203d 2073   tracklet_id = s
-00015440: 656c 662e 7472 6163 6b6c 6574 5f64 6963  elf.tracklet_dic
-00015450: 745b 6365 6c6c 5f69 645d 0d0a 2020 2020  t[cell_id]..    
-00015460: 2020 200d 0a0d 0a20 2020 2020 2020 2075     ....        u
-00015470: 6e69 7175 655f 6964 203d 2073 7472 2874  nique_id = str(t
-00015480: 7261 636b 5f69 6429 202b 2020 7374 7228  rack_id) +  str(
-00015490: 6765 6e65 7261 7469 6f6e 5f69 6429 202b  generation_id) +
-000154a0: 2073 7472 2874 7261 636b 6c65 745f 6964   str(tracklet_id
-000154b0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000154c0: 2020 2020 2076 6563 5f6d 6173 6b20 3d20       vec_mask = 
-000154d0: 5b66 6c6f 6174 2873 656c 662e 756e 6971  [float(self.uniq
-000154e0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000154f0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015500: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
-00015510: 6964 5f78 5f6b 6579 5d29 2c20 666c 6f61  id_x_key]), floa
-00015520: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015530: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015540: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00015550: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00015560: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
-00015570: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015580: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015590: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
-000155a0: 6365 6e74 726f 6964 5f7a 5f6b 6579 5d29  centroid_z_key])
-000155b0: 205d 0d0a 0d0a 2020 2020 2020 2020 7665   ]....        ve
-000155c0: 635f 6365 6c6c 203d 205b 666c 6f61 7428  c_cell = [float(
-000155d0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000155e0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000155f0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00015600: 706f 7369 645f 6b65 795d 2920 2c20 0d0a  posid_key]) , ..
-00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015620: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00015630: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00015640: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015650: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00015660: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
-00015670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015680: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00015690: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000156a0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000156b0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-000156c0: 662e 7a70 6f73 6964 5f6b 6579 5d29 5d0d  f.zposid_key])].
-000156d0: 0a0d 0a20 2020 2020 2020 2061 6e67 6c65  ...        angle
-000156e0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-000156f0: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
-00015700: 6365 6c6c 290d 0a0d 0a20 2020 2020 2020  cell)....       
-00015710: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00015720: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00015730: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00015740: 6528 7b73 656c 662e 7261 6469 616c 5f61  e({self.radial_a
-00015750: 6e67 6c65 5f6b 6579 203a 2061 6e67 6c65  ngle_key : angle
-00015760: 7d29 2020 2020 2020 2020 2020 2020 2020  })              
-00015770: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
-00015780: 2020 756e 6971 7565 5f74 7261 636b 6c65    unique_trackle
-00015790: 745f 6964 732e 6170 7065 6e64 2873 7472  t_ids.append(str
-000157a0: 2875 6e69 7175 655f 6964 2929 0d0a 2020  (unique_id))..  
-000157b0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-000157c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000157d0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-000157e0: 7570 6461 7465 287b 7365 6c66 2e75 6e69  update({self.uni
-000157f0: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
-00015800: 756e 6971 7565 5f69 6429 7d29 0d0a 2020  unique_id)})..  
-00015810: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015820: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015830: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015840: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
-00015850: 636b 6c65 7469 645f 6b65 7920 3a20 7374  ckletid_key : st
-00015860: 7228 7472 6163 6b6c 6574 5f69 6429 7d29  r(tracklet_id)})
-00015870: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00015880: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015890: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000158a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000158b0: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
-000158c0: 6579 203a 2073 7472 2867 656e 6572 6174  ey : str(generat
-000158d0: 696f 6e5f 6964 297d 2920 0d0a 2020 2020  ion_id)}) ..    
-000158e0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000158f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015900: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015910: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
-00015920: 6964 5f6b 6579 203a 2073 7472 2874 7261  id_key : str(tra
-00015930: 636b 5f69 6429 7d29 0d0a 2020 2020 2020  ck_id)})..      
-00015940: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00015950: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015960: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00015970: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
-00015980: 616e 676c 655f 6b65 7920 3a20 302e 307d  angle_key : 0.0}
-00015990: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000159a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000159b0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000159c0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000159d0: 662e 7370 6565 645f 6b65 7920 3a20 302e  f.speed_key : 0.
-000159e0: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
-000159f0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015a00: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015a10: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015a20: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00015a30: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-00015a40: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015a50: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015a60: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015a70: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
-00015a80: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00015a90: 6972 7374 6b65 7920 3a20 2d31 7d29 0d0a  irstkey : -1})..
-00015aa0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015ab0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015ac0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015ad0: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00015ae0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00015af0: 5f73 6563 6f6e 646b 6579 203a 202d 317d  _secondkey : -1}
-00015b00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00015b10: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015b20: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015b30: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015b40: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
-00015b50: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
-00015b60: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015b70: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015b80: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015b90: 6174 6528 7b73 656c 662e 6365 6c6c 6178  ate({self.cellax
-00015ba0: 6973 5f6d 6173 6b5f 6b65 7920 3a20 2d31  is_mask_key : -1
-00015bb0: 7d29 0d0a 0d0a 2020 2020 2020 2020 6966  })....        if
-00015bc0: 2073 6f75 7263 655f 6964 2069 7320 6e6f   source_id is no
-00015bd0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-00015be0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015bf0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015c00: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015c10: 7064 6174 6528 7b73 656c 662e 6265 666f  pdate({self.befo
-00015c20: 7265 6964 5f6b 6579 203a 2069 6e74 2873  reid_key : int(s
-00015c30: 6f75 7263 655f 6964 297d 290d 0a20 2020  ource_id)})..   
-00015c40: 2020 2020 2020 2020 2076 6563 5f31 203d           vec_1 =
-00015c50: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00015c60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015c70: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015c80: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00015c90: 795d 2920 2d20 666c 6f61 7428 7365 6c66  y]) - float(self
-00015ca0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015cb0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-00015cc0: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
-00015cd0: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00015d00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015d10: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00015d20: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
-00015d30: 6f73 6964 5f6b 6579 5d29 202d 2066 6c6f  osid_key]) - flo
-00015d40: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015d50: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015d60: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00015d70: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00015d80: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00015d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015da0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00015db0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015dc0: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
-00015dd0: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
-00015de0: 2920 2d20 2066 6c6f 6174 2873 656c 662e  ) -  float(self.
-00015df0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015e00: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00015e10: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
-00015e20: 6964 5f6b 6579 5d29 5d0d 0a20 2020 2020  id_key])]..     
-00015e30: 2020 2020 2020 2073 7065 6564 203d 206e         speed = n
-00015e40: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
-00015e50: 635f 312c 2076 6563 5f31 2929 2f73 656c  c_1, vec_1))/sel
-00015e60: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
-00015e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015e80: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015e90: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015ea0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015eb0: 6c66 2e73 7065 6564 5f6b 6579 203a 2073  lf.speed_key : s
-00015ec0: 7065 6564 7d29 0d0a 0d0a 2020 2020 2020  peed})....      
-00015ed0: 2020 2020 2020 6d6f 7469 6f6e 5f61 6e67        motion_ang
-00015ee0: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
-00015ef0: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
-00015f00: 635f 3129 0d0a 0d0a 2020 2020 2020 2020  c_1)....        
-00015f10: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00015f20: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015f30: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015f40: 6461 7465 287b 7365 6c66 2e6d 6f74 696f  date({self.motio
-00015f50: 6e5f 616e 676c 655f 6b65 7920 3a20 6d6f  n_angle_key : mo
-00015f60: 7469 6f6e 5f61 6e67 6c65 7d29 200d 0a0d  tion_angle}) ...
-00015f70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015f80: 736f 7572 6365 5f69 6420 696e 2073 656c  source_id in sel
-00015f90: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
-00015fa0: 6f6b 7570 3a0d 0a20 2020 2020 2020 2020  okup:..         
-00015fb0: 2020 2020 2020 2020 2020 2070 7265 5f73             pre_s
-00015fc0: 6f75 7263 655f 6964 203d 2073 656c 662e  ource_id = self.
-00015fd0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
-00015fe0: 7570 5b73 6f75 7263 655f 6964 5d0d 0a20  up[source_id].. 
-00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016000: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016010: 2020 2020 2020 2020 2076 6563 5f32 203d           vec_2 =
-00016020: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00016030: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016040: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00016050: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00016060: 795d 2920 2d20 3220 2a20 666c 6f61 7428  y]) - 2 * float(
-00016070: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016080: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016090: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-000160a0: 2e78 706f 7369 645f 6b65 795d 2920 2b20  .xposid_key]) + 
-000160b0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000160c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000160d0: 735b 696e 7428 7072 655f 736f 7572 6365  s[int(pre_source
-000160e0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
-000160f0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
-00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016110: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-00016120: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016130: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00016140: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
-00016150: 6964 5f6b 6579 5d29 202d 2032 202a 2066  id_key]) - 2 * f
-00016160: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00016170: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00016180: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
-00016190: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-000161a0: 5d29 202b 2066 6c6f 6174 2873 656c 662e  ]) + float(self.
-000161b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000161c0: 6572 7469 6573 5b69 6e74 2870 7265 5f73  erties[int(pre_s
-000161d0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
-000161e0: 7970 6f73 6964 5f6b 6579 5d29 2c20 0d0a  yposid_key]), ..
-000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016200: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00016210: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00016220: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016230: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
-00016240: 2e7a 706f 7369 645f 6b65 795d 2920 2d20  .zposid_key]) - 
-00016250: 2032 202a 2066 6c6f 6174 2873 656c 662e   2 * float(self.
-00016260: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016270: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00016280: 655f 6964 295d 5b73 656c 662e 7a70 6f73  e_id)][self.zpos
-00016290: 6964 5f6b 6579 5d29 202b 2066 6c6f 6174  id_key]) + float
-000162a0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000162b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000162c0: 2870 7265 5f73 6f75 7263 655f 6964 295d  (pre_source_id)]
-000162d0: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-000162e0: 5d29 5d0d 0a20 2020 2020 2020 2020 2020  ])]..           
-000162f0: 2020 2020 2020 2020 2061 6363 203d 206e           acc = n
-00016300: 702e 7371 7274 286e 702e 646f 7428 7665  p.sqrt(np.dot(ve
-00016310: 635f 322c 2076 6563 5f32 2929 2f73 656c  c_2, vec_2))/sel
-00016320: 662e 7463 616c 6962 7261 7469 6f6e 0d0a  f.tcalibration..
-00016330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016340: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00016350: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00016360: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00016370: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00016380: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00016390: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-000163a0: 7920 3a20 6163 637d 290d 0a20 2020 2020  y : acc})..     
-000163b0: 2020 2065 6c69 6620 736f 7572 6365 5f69     elif source_i
-000163c0: 6420 6973 204e 6f6e 653a 0d0a 2020 2020  d is None:..    
-000163d0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000163e0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000163f0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00016400: 5d2e 7570 6461 7465 287b 7365 6c66 2e62  ].update({self.b
-00016410: 6566 6f72 6569 645f 6b65 7920 3a20 4e6f  eforeid_key : No
-00016420: 6e65 7d29 200d 0a20 2020 2020 2020 2020  ne}) ..         
-00016430: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
-00016440: 6620 7461 7267 6574 5f69 6420 6973 206e  f target_id is n
-00016450: 6f74 204e 6f6e 653a 2020 2020 2020 200d  ot None:       .
-00016460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016470: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016480: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00016490: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000164a0: 656c 662e 6166 7465 7269 645f 6b65 7920  elf.afterid_key 
-000164b0: 3a20 696e 7428 7461 7267 6574 5f69 6429  : int(target_id)
-000164c0: 7d29 200d 0a20 2020 2020 2020 2065 6c69  }) ..        eli
-000164d0: 6620 7461 7267 6574 5f69 6420 6973 204e  f target_id is N
-000164e0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000164f0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016500: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016510: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016520: 7465 287b 7365 6c66 2e61 6674 6572 6964  te({self.afterid
-00016530: 5f6b 6579 203a 204e 6f6e 657d 290d 0a20  _key : None}).. 
-00016540: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00016550: 2020 2020 2073 656c 662e 5f73 6563 6f6e       self._secon
-00016560: 645f 6368 616e 6e65 6c5f 7570 6461 7465  d_channel_update
-00016570: 2863 656c 6c5f 6964 2c20 7472 6163 6b5f  (cell_id, track_
-00016580: 6964 2920 2020 200d 0a0d 0a0d 0a20 2020  id)    ......   
-00016590: 2064 6566 205f 7465 6d70 6f72 616c 5f70   def _temporal_p
-000165a0: 6c6f 7473 5f74 7261 636b 6d61 7465 2873  lots_trackmate(s
-000165b0: 656c 6629 3a0d 0a20 2020 200d 0a20 2020  elf):..    ..   
-000165c0: 200d 0a20 2020 200d 0a20 2020 2020 2020   ..    ..       
-000165d0: 2020 2020 2020 2020 2073 656c 662e 4174           self.At
-000165e0: 7472 203d 207b 7d0d 0a20 2020 2020 2020  tr = {}..       
-000165f0: 2020 2020 2020 2020 2073 7461 7274 7469           startti
-00016600: 6d65 203d 2069 6e74 286d 696e 2873 656c  me = int(min(sel
-00016610: 662e 416c 6c56 616c 7565 735b 7365 6c66  f.AllValues[self
-00016620: 2e66 7261 6d65 6964 5f6b 6579 5d29 290d  .frameid_key])).
-00016630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016640: 2065 6e64 7469 6d65 203d 2069 6e74 286d   endtime = int(m
-00016650: 6178 2873 656c 662e 416c 6c56 616c 7565  ax(self.AllValue
-00016660: 735b 7365 6c66 2e66 7261 6d65 6964 5f6b  s[self.frameid_k
-00016670: 6579 5d29 290d 0a20 2020 2020 2020 2020  ey]))..         
-00016680: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00016690: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000166a0: 696d 6520 3d20 5b5d 0d0a 2020 2020 2020  ime = []..      
-000166b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000166c0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-000166d0: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
-000166e0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000166f0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
-00016700: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016710: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00016720: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00016730: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-00016740: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00016750: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
-00016760: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016770: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00016780: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f78  otic_mean_disp_x
-00016790: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000167a0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000167b0: 7469 635f 7661 725f 6469 7370 5f78 203d  tic_var_disp_x =
-000167c0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000167d0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000167e0: 7469 635f 6d65 616e 5f72 6164 6975 7320  tic_mean_radius 
-000167f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016800: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016810: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
-00016820: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016830: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016840: 6963 5f6d 6561 6e5f 7370 6565 6420 3d20  ic_mean_speed = 
-00016850: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016860: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016870: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-00016880: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016890: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-000168a0: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000168c0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-000168d0: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-000168e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000168f0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00016900: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00016910: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016920: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016930: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00016940: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00016950: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016960: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00016970: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
-00016980: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
-00016990: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000169a0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-000169b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000169c0: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
-000169d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000169e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000169f0: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
-00016a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016a10: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00016a20: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-00016a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016a40: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00016a50: 635f 6d65 616e 5f64 6973 705f 7920 3d20  c_mean_disp_y = 
-00016a60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016a70: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00016a80: 6f74 6963 5f76 6172 5f64 6973 705f 7920  otic_var_disp_y 
-00016a90: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016aa0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00016ab0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00016ac0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
-00016ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016ae0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016af0: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-00016b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016b10: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00016b20: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
-00016b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016b40: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00016b50: 6963 5f76 6172 5f72 6164 6975 7320 3d20  ic_var_radius = 
-00016b60: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016b70: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00016b80: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-00016b90: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-00016ba0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00016bb0: 5f6d 6974 6f74 6963 5f76 6172 5f73 7065  _mitotic_var_spe
-00016bc0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-00016bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016be0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016bf0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00016c00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016c10: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016c20: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-00016c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016c40: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00016c50: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00016c60: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
-00016c70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016c80: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016c90: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016ca0: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00016cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016cc0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016cd0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00016ce0: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
-00016cf0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016d00: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00016d10: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00016d20: 6b20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  k = []....      
-00016d30: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016d40: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 203d  ll_mean_disp_z =
-00016d50: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016d60: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00016d70: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-00016d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d90: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-00016da0: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
-00016db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016dc0: 2e61 6c6c 5f76 6172 5f64 6973 705f 7920  .all_var_disp_y 
-00016dd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00016de0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00016df0: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
-00016e00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016e10: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016e20: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016e40: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
-00016e50: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-00016e60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00016e70: 6c6c 5f76 6172 5f72 6164 6975 7320 3d20  ll_var_radius = 
-00016e80: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00016e90: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00016ea0: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
-00016eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ec0: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
-00016ed0: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-00016ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016ef0: 616c 6c5f 6d65 616e 5f61 6363 203d 205b  all_mean_acc = [
-00016f00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016f10: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016f20: 6163 6320 3d20 5b5d 0d0a 0d0a 2020 2020  acc = []....    
-00016f30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016f40: 2e61 6c6c 5f6d 6561 6e5f 6469 7265 6374  .all_mean_direct
-00016f50: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
-00016f60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016f70: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016f80: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016f90: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00016fa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016fb0: 616c 6c5f 6d65 616e 5f64 6973 7461 6e63  all_mean_distanc
-00016fc0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
-00016fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016fe0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00016ff0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00017000: 6b20 3d20 5b5d 0d0a 0d0a 0d0a 2020 2020  k = []......    
-00017010: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017020: 7370 6f74 735f 7472 6163 6b73 203d 207b  spots_tracks = {
-00017030: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00017040: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-00017050: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00017060: 5f70 726f 7065 7274 6965 732e 6974 656d  _properties.item
-00017070: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00017080: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 2020 616c 6c5f 7370 6f74 7320 3d20      all_spots = 
-000170b0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000170c0: 5f70 726f 7065 7274 6965 735b 6b5d 0d0a  _properties[k]..
-000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170e0: 2020 2020 2020 6966 2073 656c 662e 7472        if self.tr
-000170f0: 6163 6b69 645f 6b65 7920 696e 2061 6c6c  ackid_key in all
-00017100: 5f73 706f 7473 3a0d 0a20 2020 2020 2020  _spots:..       
-00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 2020 2061 6c6c 5f73 706f 7473 5f74 7261     all_spots_tra
-00017130: 636b 735b 6b5d 203d 2061 6c6c 5f73 706f  cks[k] = all_spo
-00017140: 7473 0d0a 2020 2020 2020 2020 2020 2020  ts..            
-00017150: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00017160: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00017170: 2020 2020 2020 2020 2020 6675 7475 7265            future
-00017180: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00017190: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
-000171a0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-000171b0: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
-000171c0: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
-000171d0: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
-000171e0: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
-000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017200: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017210: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00017220: 2069 6e20 7471 646d 2872 616e 6765 2873   in tqdm(range(s
-00017230: 7461 7274 7469 6d65 2c20 656e 6474 696d  tarttime, endtim
-00017240: 6529 2c20 746f 7461 6c3d 656e 6474 696d  e), total=endtim
-00017250: 6520 2d20 7374 6172 7474 696d 6529 3a0d  e - starttime):.
-00017260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017270: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00017280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017290: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
-000172a0: 6578 6563 7574 6f72 2e73 7562 6d69 7428  executor.submit(
-000172b0: 7365 6c66 2e5f 636f 6d70 7574 655f 7465  self._compute_te
-000172c0: 6d70 6f72 616c 2c20 692c 2061 6c6c 5f73  mporal, i, all_s
-000172d0: 706f 7473 5f74 7261 636b 7329 290d 0a20  pots_tracks)).. 
-000172e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000172f0: 2020 2020 2020 5b72 2e72 6573 756c 7428        [r.result(
-00017300: 2920 666f 7220 7220 696e 2063 6f6e 6375  ) for r in concu
-00017310: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
-00017320: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
-00017330: 6573 295d 0d0a 0d0a 0d0a 2020 2020 6465  es)]......    de
-00017340: 6620 5f63 6f6d 7075 7465 5f74 656d 706f  f _compute_tempo
-00017350: 7261 6c28 7365 6c66 2c20 692c 2061 6c6c  ral(self, i, all
-00017360: 5f73 706f 7473 5f74 7261 636b 7329 3a20  _spots_tracks): 
-00017370: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00017380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017390: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-000173a0: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-000173b0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000173c0: 746f 7469 635f 6469 7370 5f79 203d 205b  totic_disp_y = [
-000173d0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000173e0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-000173f0: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017410: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
-00017420: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017430: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017440: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017460: 206d 6974 6f74 6963 5f61 6363 203d 205b   mitotic_acc = [
-00017470: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017480: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017490: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000174a0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000174b0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-000174c0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-000174d0: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a20  l_mask = [].... 
-000174e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174f0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00017500: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
-00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017520: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00017530: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00017540: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017550: 5f6d 6974 6f74 6963 5f64 6973 705f 7820  _mitotic_disp_x 
-00017560: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00017570: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00017580: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
-00017590: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000175a0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000175b0: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f61     non_mitotic_a
-000175e0: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
-000175f0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017600: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00017610: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00017620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017630: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017640: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00017650: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-00017660: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00017670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017680: 2020 2020 2061 6c6c 5f64 6973 705f 7a20       all_disp_z 
-00017690: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000176a0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
-000176b0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-000176c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000176d0: 6c6c 5f64 6973 705f 7820 3d20 5b5d 0d0a  ll_disp_x = []..
-000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 616c 6c5f 7261 6469 7573 203d      all_radius =
-00017700: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017710: 2020 2020 2020 2020 2061 6c6c 5f73 7065           all_spe
-00017720: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-00017730: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017740: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00017750: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017760: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00017770: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-000177a0: 6c5f 6d61 736b 203d 205b 5d0d 0a0d 0a0d  l_mask = [].....
-000177b0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-000177c0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-000177d0: 7629 2069 6e20 616c 6c5f 7370 6f74 735f  v) in all_spots_
-000177e0: 7472 6163 6b73 2e69 7465 6d73 2829 3a0d  tracks.items():.
-000177f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017800: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017820: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00017830: 6e74 5f74 696d 6520 3d20 616c 6c5f 7370  nt_time = all_sp
-00017840: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017850: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d0d  lf.frameid_key].
-00017860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017870: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017880: 6f74 6963 203d 2061 6c6c 5f73 706f 7473  otic = all_spots
-00017890: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000178a0: 6469 7669 6469 6e67 5f6b 6579 5d0d 0a20  dividing_key].. 
-000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178e0: 2020 2020 2020 2020 6966 2069 203d 3d20          if i == 
-000178f0: 696e 7428 6375 7272 656e 745f 7469 6d65  int(current_time
-00017900: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00017910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017920: 2020 2020 2020 6966 206d 6974 6f74 6963        if mitotic
-00017930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017950: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017960: 6963 5f64 6973 705f 7a2e 6170 7065 6e64  ic_disp_z.append
-00017970: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017980: 735b 6b5d 5b73 656c 662e 7a70 6f73 6964  s[k][self.zposid
-00017990: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 6d69 746f 7469 635f 6469 7370 5f79 2e61  mitotic_disp_y.a
-000179d0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-000179e0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
-000179f0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152a0: 2020 2020 7365 6c66 2e74 6f74 616c 5f69      self.total_i
+000152b0: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
+000152c0: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
+000152d0: 746f 7461 6c5b 696e 6465 785d 2929 2c0d  total[index])),.
+000152e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000152f0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
+00015300: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+00015310: 203a 2028 666c 6f61 7428 696e 7465 6e73   : (float(intens
+00015320: 6974 795f 6d65 616e 5b69 6e64 6578 5d29  ity_mean[index])
+00015330: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00015340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015350: 2e72 6164 6975 735f 6b65 7920 3a20 2866  .radius_key : (f
+00015360: 6c6f 6174 2852 4144 4955 5329 292c 0d0a  loat(RADIUS)),..
+00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015380: 2020 2020 2020 2020 7365 6c66 2e71 7561          self.qua
+00015390: 6c69 7479 5f6b 6579 203a 2028 666c 6f61  lity_key : (floa
+000153a0: 7428 5155 414c 4954 5929 292c 0d0a 2020  t(QUALITY)),..  
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153c0: 2020 2020 2020 7365 6c66 2e64 6973 7461        self.dista
+000153d0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+000153e0: 793a 2066 6c6f 6174 2864 6973 7461 6e63  y: float(distanc
+000153f0: 655f 6365 6c6c 5f6d 6173 6b29 2c0d 0a20  e_cell_mask),.. 
+00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015410: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+00015420: 6365 6e74 726f 6964 5f7a 5f6b 6579 3a20  centroid_z_key: 
+00015430: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+00015440: 6964 5b30 5d29 2c0d 0a20 2020 2020 2020  id[0]),..       
+00015450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015460: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+00015470: 6964 5f79 5f6b 6579 3a20 666c 6f61 7428  id_y_key: float(
+00015480: 6d61 736b 6365 6e74 726f 6964 5b31 5d29  maskcentroid[1])
+00015490: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000154a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000154b0: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
+000154c0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
+000154d0: 6e74 726f 6964 5b32 5d29 200d 0a0d 0a20  ntroid[2]) .... 
+000154e0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000154f0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00015500: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00015510: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+00015520: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+00015530: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00015540: 6c5f 6964 5d20 3d20 7365 6c66 2e75 6e69  l_id] = self.uni
+00015550: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015560: 6965 735b 6365 6c6c 5f69 645d 0d0a 2020  ies[cell_id]..  
+00015570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015580: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00015590: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000155a0: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
+000155b0: 7064 6174 6528 7b73 656c 662e 746f 7461  pdate({self.tota
+000155c0: 6c5f 696e 7465 6e73 6974 795f 6b65 793a  l_intensity_key:
+000155d0: 202d 317d 290d 0a20 2020 2020 2020 2020   -1})..         
+000155e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000155f0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
+00015600: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00015610: 656c 6c5f 6964 5d2e 7570 6461 7465 287b  ell_id].update({
+00015620: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+00015630: 6974 795f 6b65 793a 202d 317d 290d 0a20  ity_key: -1}).. 
+00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015650: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+00015660: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015670: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00015680: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00015690: 6975 735f 6b65 793a 202d 317d 290d 0a20  ius_key: -1}).. 
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156b0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+000156c0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+000156d0: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+000156e0: 7570 6461 7465 287b 7365 6c66 2e71 7561  update({self.qua
+000156f0: 6c69 7479 5f6b 6579 3a20 2d31 7d29 0d0a  lity_key: -1})..
+00015700: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015720: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00015730: 205f 6469 6374 5f75 7064 6174 6528 7365   _dict_update(se
+00015740: 6c66 2c20 756e 6971 7565 5f74 7261 636b  lf, unique_track
+00015750: 6c65 745f 6964 733a 204c 6973 742c 2020  let_ids: List,  
+00015760: 6365 6c6c 5f69 643a 2069 6e74 2c20 7472  cell_id: int, tr
+00015770: 6163 6b5f 6964 3a20 696e 742c 2073 6f75  ack_id: int, sou
+00015780: 7263 655f 6964 3a20 696e 742c 2074 6172  rce_id: int, tar
+00015790: 6765 745f 6964 3a20 696e 7429 3a0d 0a0d  get_id: int):...
+000157a0: 0a20 0d0a 2020 2020 2020 2020 6765 6e65  . ..        gene
+000157b0: 7261 7469 6f6e 5f69 6420 3d20 7365 6c66  ration_id = self
+000157c0: 2e67 656e 6572 6174 696f 6e5f 6469 6374  .generation_dict
+000157d0: 5b63 656c 6c5f 6964 5d0d 0a20 2020 2020  [cell_id]..     
+000157e0: 2020 2074 7261 636b 6c65 745f 6964 203d     tracklet_id =
+000157f0: 2073 656c 662e 7472 6163 6b6c 6574 5f64   self.tracklet_d
+00015800: 6963 745b 6365 6c6c 5f69 645d 0d0a 2020  ict[cell_id]..  
+00015810: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+00015820: 2075 6e69 7175 655f 6964 203d 2073 7472   unique_id = str
+00015830: 2874 7261 636b 5f69 6429 202b 2020 7374  (track_id) +  st
+00015840: 7228 6765 6e65 7261 7469 6f6e 5f69 6429  r(generation_id)
+00015850: 202b 2073 7472 2874 7261 636b 6c65 745f   + str(tracklet_
+00015860: 6964 290d 0a20 2020 2020 2020 200d 0a20  id)..        .. 
+00015870: 2020 2020 2020 2076 6563 5f6d 6173 6b20         vec_mask 
+00015880: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+00015890: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000158a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000158b0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
+000158c0: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
+000158d0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000158e0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000158f0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00015900: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00015910: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
+00015920: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015930: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015940: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
+00015950: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
+00015960: 5d29 205d 0d0a 0d0a 2020 2020 2020 2020  ]) ]....        
+00015970: 7665 635f 6365 6c6c 203d 205b 666c 6f61  vec_cell = [floa
+00015980: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00015990: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000159a0: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+000159b0: 2e78 706f 7369 645f 6b65 795d 2920 2c20  .xposid_key]) , 
+000159c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000159d0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+000159e0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000159f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015a00: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00015a10: 6c66 2e79 706f 7369 645f 6b65 795d 292c  lf.yposid_key]),
+00015a20: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015a40: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00015a50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015a60: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00015a70: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00015a80: 5d0d 0a0d 0a20 2020 2020 2020 2061 6e67  ]....        ang
+00015a90: 6c65 203d 2061 6e67 756c 6172 5f63 6861  le = angular_cha
+00015aa0: 6e67 6528 7665 635f 6d61 736b 2c20 7665  nge(vec_mask, ve
+00015ab0: 635f 6365 6c6c 290d 0a0d 0a20 2020 2020  c_cell)....     
+00015ac0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00015ad0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015ae0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00015af0: 6174 6528 7b73 656c 662e 7261 6469 616c  ate({self.radial
+00015b00: 5f61 6e67 6c65 5f6b 6579 203a 2061 6e67  _angle_key : ang
+00015b10: 6c65 7d29 2020 2020 2020 2020 2020 2020  le})            
+00015b20: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00015b30: 2020 2020 756e 6971 7565 5f74 7261 636b      unique_track
+00015b40: 6c65 745f 6964 732e 6170 7065 6e64 2873  let_ids.append(s
+00015b50: 7472 2875 6e69 7175 655f 6964 2929 0d0a  tr(unique_id))..
+00015b60: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015b70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015b80: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015b90: 5d2e 7570 6461 7465 287b 7365 6c66 2e75  ].update({self.u
+00015ba0: 6e69 7175 6569 645f 6b65 7920 3a20 7374  niqueid_key : st
+00015bb0: 7228 756e 6971 7565 5f69 6429 7d29 0d0a  r(unique_id)})..
+00015bc0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015bd0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015be0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015bf0: 5d2e 7570 6461 7465 287b 7365 6c66 2e74  ].update({self.t
+00015c00: 7261 636b 6c65 7469 645f 6b65 7920 3a20  rackletid_key : 
+00015c10: 7374 7228 7472 6163 6b6c 6574 5f69 6429  str(tracklet_id)
+00015c20: 7d29 200d 0a20 2020 2020 2020 2073 656c  }) ..        sel
+00015c30: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015c40: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015c50: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015c60: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
+00015c70: 5f6b 6579 203a 2073 7472 2867 656e 6572  _key : str(gener
+00015c80: 6174 696f 6e5f 6964 297d 2920 0d0a 2020  ation_id)}) ..  
+00015c90: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015ca0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015cb0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015cc0: 7570 6461 7465 287b 7365 6c66 2e74 7261  update({self.tra
+00015cd0: 636b 6964 5f6b 6579 203a 2073 7472 2874  ckid_key : str(t
+00015ce0: 7261 636b 5f69 6429 7d29 0d0a 2020 2020  rack_id)})..    
+00015cf0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015d00: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015d10: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015d20: 6461 7465 287b 7365 6c66 2e6d 6f74 696f  date({self.motio
+00015d30: 6e5f 616e 676c 655f 6b65 7920 3a20 302e  n_angle_key : 0.
+00015d40: 307d 290d 0a20 2020 2020 2020 2073 656c  0})..        sel
+00015d50: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015d60: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015d70: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015d80: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
+00015d90: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+00015da0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015db0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015dc0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015dd0: 7b73 656c 662e 6163 6365 6c65 7261 7469  {self.accelerati
+00015de0: 6f6e 5f6b 6579 203a 2030 2e30 7d29 0d0a  on_key : 0.0})..
+00015df0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015e00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015e10: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015e20: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
+00015e30: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+00015e40: 5f66 6972 7374 6b65 7920 3a20 2d31 7d29  _firstkey : -1})
+00015e50: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00015e60: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015e70: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015e80: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015e90: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+00015ea0: 6d70 5f73 6563 6f6e 646b 6579 203a 202d  mp_secondkey : -
+00015eb0: 317d 290d 0a20 2020 2020 2020 2073 656c  1})..        sel
+00015ec0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015ed0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015ee0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015ef0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+00015f00: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+00015f10: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00015f20: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015f30: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+00015f40: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
+00015f50: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
+00015f60: 2d31 7d29 0d0a 0d0a 2020 2020 2020 2020  -1})....        
+00015f70: 6966 2073 6f75 7263 655f 6964 2069 7320  if source_id is 
+00015f80: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00015f90: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00015fa0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015fb0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015fc0: 2e75 7064 6174 6528 7b73 656c 662e 6265  .update({self.be
+00015fd0: 666f 7265 6964 5f6b 6579 203a 2069 6e74  foreid_key : int
+00015fe0: 2873 6f75 7263 655f 6964 297d 290d 0a20  (source_id)}).. 
+00015ff0: 2020 2020 2020 2020 2020 2076 6563 5f31             vec_1
+00016000: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+00016010: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00016020: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00016030: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00016040: 6b65 795d 2920 2d20 666c 6f61 7428 7365  key]) - float(se
+00016050: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016060: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00016070: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
+00016080: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
+00016090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160a0: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+000160b0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000160c0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000160d0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000160e0: 7970 6f73 6964 5f6b 6579 5d29 202d 2066  yposid_key]) - f
+000160f0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00016100: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016110: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
+00016120: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00016130: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
+00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016150: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
+00016160: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00016170: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00016180: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
+00016190: 795d 2920 2d20 2066 6c6f 6174 2873 656c  y]) -  float(sel
+000161a0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000161b0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+000161c0: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
+000161d0: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
+000161e0: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
+000161f0: 206e 702e 7371 7274 286e 702e 646f 7428   np.sqrt(np.dot(
+00016200: 7665 635f 312c 2076 6563 5f31 2929 2f73  vec_1, vec_1))/s
+00016210: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+00016220: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00016230: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016240: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00016250: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00016260: 7365 6c66 2e73 7065 6564 5f6b 6579 203a  self.speed_key :
+00016270: 2073 7065 6564 7d29 0d0a 0d0a 2020 2020   speed})....    
+00016280: 2020 2020 2020 2020 6d6f 7469 6f6e 5f61          motion_a
+00016290: 6e67 6c65 203d 2061 6e67 756c 6172 5f63  ngle = angular_c
+000162a0: 6861 6e67 6528 7665 635f 6d61 736b 2c20  hange(vec_mask, 
+000162b0: 7665 635f 3129 0d0a 0d0a 2020 2020 2020  vec_1)....      
+000162c0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000162d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000162e0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000162f0: 7570 6461 7465 287b 7365 6c66 2e6d 6f74  update({self.mot
+00016300: 696f 6e5f 616e 676c 655f 6b65 7920 3a20  ion_angle_key : 
+00016310: 6d6f 7469 6f6e 5f61 6e67 6c65 7d29 200d  motion_angle}) .
+00016320: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00016330: 6620 736f 7572 6365 5f69 6420 696e 2073  f source_id in s
+00016340: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00016350: 6c6f 6f6b 7570 3a0d 0a20 2020 2020 2020  lookup:..       
+00016360: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00016370: 5f73 6f75 7263 655f 6964 203d 2073 656c  _source_id = sel
+00016380: 662e 6564 6765 5f73 6f75 7263 655f 6c6f  f.edge_source_lo
+00016390: 6f6b 7570 5b73 6f75 7263 655f 6964 5d0d  okup[source_id].
+000163a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000163c0: 2020 2020 2020 2020 2020 2076 6563 5f32             vec_2
+000163d0: 203d 205b 666c 6f61 7428 7365 6c66 2e75   = [float(self.u
+000163e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000163f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00016400: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00016410: 6b65 795d 2920 2d20 3220 2a20 666c 6f61  key]) - 2 * floa
+00016420: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00016430: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00016440: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
+00016450: 6c66 2e78 706f 7369 645f 6b65 795d 2920  lf.xposid_key]) 
+00016460: 2b20 666c 6f61 7428 7365 6c66 2e75 6e69  + float(self.uni
+00016470: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00016480: 6965 735b 696e 7428 7072 655f 736f 7572  ies[int(pre_sour
+00016490: 6365 5f69 6429 5d5b 7365 6c66 2e78 706f  ce_id)][self.xpo
+000164a0: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000164c0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+000164d0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000164e0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000164f0: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
+00016500: 6f73 6964 5f6b 6579 5d29 202d 2032 202a  osid_key]) - 2 *
+00016510: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00016520: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00016530: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+00016540: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+00016550: 6579 5d29 202b 2066 6c6f 6174 2873 656c  ey]) + float(sel
+00016560: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00016570: 6f70 6572 7469 6573 5b69 6e74 2870 7265  operties[int(pre
+00016580: 5f73 6f75 7263 655f 6964 295d 5b73 656c  _source_id)][sel
+00016590: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+000165a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000165b0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+000165c0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000165d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000165e0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+000165f0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
+00016600: 2d20 2032 202a 2066 6c6f 6174 2873 656c  -  2 * float(sel
+00016610: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00016620: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
+00016630: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
+00016640: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
+00016650: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00016660: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00016670: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
+00016680: 295d 5b73 656c 662e 7a70 6f73 6964 5f6b  )][self.zposid_k
+00016690: 6579 5d29 5d0d 0a20 2020 2020 2020 2020  ey])]..         
+000166a0: 2020 2020 2020 2020 2020 2061 6363 203d             acc =
+000166b0: 206e 702e 7371 7274 286e 702e 646f 7428   np.sqrt(np.dot(
+000166c0: 7665 635f 322c 2076 6563 5f32 2929 2f73  vec_2, vec_2))/s
+000166d0: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+000166e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000166f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016710: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00016720: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00016730: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00016740: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+00016750: 6b65 7920 3a20 6163 637d 290d 0a20 2020  key : acc})..   
+00016760: 2020 2020 2065 6c69 6620 736f 7572 6365       elif source
+00016770: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
+00016780: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00016790: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000167a0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+000167b0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+000167c0: 2e62 6566 6f72 6569 645f 6b65 7920 3a20  .beforeid_key : 
+000167d0: 4e6f 6e65 7d29 200d 0a20 2020 2020 2020  None}) ..       
+000167e0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+000167f0: 2069 6620 7461 7267 6574 5f69 6420 6973   if target_id is
+00016800: 206e 6f74 204e 6f6e 653a 2020 2020 2020   not None:      
+00016810: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+00016820: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016830: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00016840: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00016850: 7b73 656c 662e 6166 7465 7269 645f 6b65  {self.afterid_ke
+00016860: 7920 3a20 696e 7428 7461 7267 6574 5f69  y : int(target_i
+00016870: 6429 7d29 200d 0a20 2020 2020 2020 2065  d)}) ..        e
+00016880: 6c69 6620 7461 7267 6574 5f69 6420 6973  lif target_id is
+00016890: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000168a0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000168b0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000168c0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000168d0: 6461 7465 287b 7365 6c66 2e61 6674 6572  date({self.after
+000168e0: 6964 5f6b 6579 203a 204e 6f6e 657d 290d  id_key : None}).
+000168f0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00016900: 2020 2020 2020 2073 656c 662e 5f73 6563         self._sec
+00016910: 6f6e 645f 6368 616e 6e65 6c5f 7570 6461  ond_channel_upda
+00016920: 7465 2863 656c 6c5f 6964 2c20 7472 6163  te(cell_id, trac
+00016930: 6b5f 6964 2920 2020 200d 0a0d 0a0d 0a20  k_id)    ...... 
+00016940: 2020 2064 6566 205f 7465 6d70 6f72 616c     def _temporal
+00016950: 5f70 6c6f 7473 5f74 7261 636b 6d61 7465  _plots_trackmate
+00016960: 2873 656c 6629 3a0d 0a20 2020 200d 0a20  (self):..    .. 
+00016970: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+00016980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016990: 4174 7472 203d 207b 7d0d 0a20 2020 2020  Attr = {}..     
+000169a0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000169b0: 7469 6d65 203d 2069 6e74 286d 696e 2873  time = int(min(s
+000169c0: 656c 662e 416c 6c56 616c 7565 735b 7365  elf.AllValues[se
+000169d0: 6c66 2e66 7261 6d65 6964 5f6b 6579 5d29  lf.frameid_key])
+000169e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000169f0: 2020 2065 6e64 7469 6d65 203d 2069 6e74     endtime = int
+00016a00: 286d 6178 2873 656c 662e 416c 6c56 616c  (max(self.AllVal
+00016a10: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
+00016a20: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
+00016a30: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00016a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016a50: 2e74 696d 6520 3d20 5b5d 0d0a 2020 2020  .time = []..    
+00016a60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016a70: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00016a80: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00016a90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016aa0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00016ab0: 5f7a 203d 205b 5d0d 0a0d 0a20 2020 2020  _z = []....     
+00016ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016ad0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00016ae0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00016af0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016b00: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00016b10: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00016b20: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00016b30: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00016b40: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00016b50: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016b60: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00016b70: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00016b80: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016b90: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
+00016ba0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00016bb0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00016bc0: 6f74 6963 5f76 6172 5f72 6164 6975 7320  otic_var_radius 
+00016bd0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016be0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00016bf0: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
+00016c00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016c10: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00016c20: 6963 5f76 6172 5f73 7065 6564 203d 205b  ic_var_speed = [
+00016c30: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016c40: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016c50: 635f 6d65 616e 5f61 6363 203d 205b 5d0d  c_mean_acc = [].
+00016c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c70: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00016c80: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
+00016c90: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016ca0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00016cb0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00016cc0: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00016cd0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00016ce0: 746f 7469 635f 7661 725f 6469 7265 6374  totic_var_direct
+00016cf0: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
+00016d00: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016d10: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016d20: 635f 6d65 616e 5f64 6973 7461 6e63 655f  c_mean_distance_
+00016d30: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d50: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00016d60: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00016d70: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
+00016d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016d90: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00016da0: 6e5f 6469 7370 5f7a 203d 205b 5d0d 0a20  n_disp_z = [].. 
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016dc0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016dd0: 7661 725f 6469 7370 5f7a 203d 205b 5d0d  var_disp_z = [].
+00016de0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016df0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00016e00: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
+00016e10: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016e20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00016e30: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00016e40: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00016e50: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016e60: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00016e70: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00016e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016e90: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016ea0: 725f 6469 7370 5f78 203d 205b 5d0d 0a0d  r_disp_x = []...
+00016eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ec0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016ed0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
+00016ee0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016ef0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016f00: 6f74 6963 5f76 6172 5f72 6164 6975 7320  otic_var_radius 
+00016f10: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016f20: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00016f30: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7370  _mitotic_mean_sp
+00016f40: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
+00016f50: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016f60: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f73  on_mitotic_var_s
+00016f70: 7065 6564 203d 205b 5d0d 0a0d 0a20 2020  peed = []....   
+00016f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016f90: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00016fa0: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
+00016fb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016fc0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016fd0: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
+00016fe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016ff0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00017000: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
+00017010: 6368 616e 6765 203d 205b 5d0d 0a20 2020  change = []..   
+00017020: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017030: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00017040: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00017050: 616e 6765 203d 205b 5d0d 0a0d 0a20 2020  ange = []....   
+00017060: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017070: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00017080: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00017090: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+000170a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000170b0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+000170c0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000170d0: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
+000170e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000170f0: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f7a  .all_mean_disp_z
+00017100: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00017110: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00017120: 7661 725f 6469 7370 5f7a 203d 205b 5d0d  var_disp_z = [].
+00017130: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017140: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00017150: 5f64 6973 705f 7920 3d20 5b5d 0d0a 2020  _disp_y = []..  
+00017160: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017170: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
+00017180: 7920 3d20 5b5d 0d0a 0d0a 2020 2020 2020  y = []....      
+00017190: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000171a0: 6c6c 5f6d 6561 6e5f 6469 7370 5f78 203d  ll_mean_disp_x =
+000171b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000171c0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000171d0: 725f 6469 7370 5f78 203d 205b 5d0d 0a0d  r_disp_x = []...
+000171e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000171f0: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
+00017200: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+00017210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017220: 2e61 6c6c 5f76 6172 5f72 6164 6975 7320  .all_var_radius 
+00017230: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00017240: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00017250: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
+00017260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017270: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
+00017280: 7065 6564 203d 205b 5d0d 0a0d 0a20 2020  peed = []....   
+00017290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000172a0: 662e 616c 6c5f 6d65 616e 5f61 6363 203d  f.all_mean_acc =
+000172b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000172c0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000172d0: 725f 6163 6320 3d20 5b5d 0d0a 0d0a 2020  r_acc = []....  
+000172e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000172f0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7265  lf.all_mean_dire
+00017300: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00017310: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017320: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00017330: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00017340: 616e 6765 203d 205b 5d0d 0a0d 0a20 2020  ange = []....   
+00017350: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017360: 662e 616c 6c5f 6d65 616e 5f64 6973 7461  f.all_mean_dista
+00017370: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00017380: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017390: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000173a0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000173b0: 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a 2020  ask = []......  
+000173c0: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000173d0: 6c5f 7370 6f74 735f 7472 6163 6b73 203d  l_spots_tracks =
+000173e0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+000173f0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
+00017400: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
+00017410: 6f74 5f70 726f 7065 7274 6965 732e 6974  ot_properties.it
+00017420: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+00017430: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017450: 2020 2020 2020 616c 6c5f 7370 6f74 7320        all_spots 
+00017460: 3d20 7365 6c66 2e75 6e69 7175 655f 7370  = self.unique_sp
+00017470: 6f74 5f70 726f 7065 7274 6965 735b 6b5d  ot_properties[k]
+00017480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017490: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000174a0: 7472 6163 6b69 645f 6b65 7920 696e 2061  trackid_key in a
+000174b0: 6c6c 5f73 706f 7473 3a0d 0a20 2020 2020  ll_spots:..     
+000174c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000174d0: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
+000174e0: 7261 636b 735b 6b5d 203d 2061 6c6c 5f73  racks[k] = all_s
+000174f0: 706f 7473 0d0a 2020 2020 2020 2020 2020  pots..          
+00017500: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00017510: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00017520: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+00017530: 7265 7320 3d20 5b5d 0d0a 2020 2020 2020  res = []..      
+00017540: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+00017550: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+00017560: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+00017570: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
+00017580: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+00017590: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+000175a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000175c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000175d0: 2069 2069 6e20 7471 646d 2872 616e 6765   i in tqdm(range
+000175e0: 2873 7461 7274 7469 6d65 2c20 656e 6474  (starttime, endt
+000175f0: 696d 6529 2c20 746f 7461 6c3d 656e 6474  ime), total=endt
+00017600: 696d 6520 2d20 7374 6172 7474 696d 6529  ime - starttime)
+00017610: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017620: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2066 7574 7572 6573 2e61 7070 656e     futures.appen
+00017650: 6428 6578 6563 7574 6f72 2e73 7562 6d69  d(executor.submi
+00017660: 7428 7365 6c66 2e5f 636f 6d70 7574 655f  t(self._compute_
+00017670: 7465 6d70 6f72 616c 2c20 692c 2061 6c6c  temporal, i, all
+00017680: 5f73 706f 7473 5f74 7261 636b 7329 290d  _spots_tracks)).
+00017690: 0a20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
+000176a0: 2020 2020 2020 2020 5b72 2e72 6573 756c          [r.resul
+000176b0: 7428 2920 666f 7220 7220 696e 2063 6f6e  t() for r in con
+000176c0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+000176d0: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
+000176e0: 7572 6573 295d 0d0a 0d0a 0d0a 2020 2020  ures)]......    
+000176f0: 6465 6620 5f63 6f6d 7075 7465 5f74 656d  def _compute_tem
+00017700: 706f 7261 6c28 7365 6c66 2c20 692c 2061  poral(self, i, a
+00017710: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
+00017720: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+00017730: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017740: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017750: 6973 705f 7a20 3d20 5b5d 0d0a 2020 2020  isp_z = []..    
+00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017770: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
+00017780: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017790: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+000177a0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+000177b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177c0: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
+000177d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000177e0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+000177f0: 6963 5f73 7065 6564 203d 205b 5d0d 0a20  ic_speed = [].. 
+00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017810: 2020 206d 6974 6f74 6963 5f61 6363 203d     mitotic_acc =
+00017820: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017830: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017840: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00017850: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+00017860: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017870: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
+00017880: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00017890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178a0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000178b0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178d0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
+000178e0: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
+000178f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00017900: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00017910: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
+00017920: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017930: 6d69 746f 7469 635f 7261 6469 7573 203d  mitotic_radius =
+00017940: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017950: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017960: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
+00017970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017980: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00017990: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
+000179a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000179b0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
+000179c0: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+000179d0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000179e0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+000179f0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+00017a00: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
 00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00017a30: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
-00017a40: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017a50: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-00017a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017a20: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017a30: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
+00017a40: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+00017a50: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017a60: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
 00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-00017a90: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00017aa0: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
-00017ab0: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ae0: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
-00017af0: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00017b00: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017b10: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a80: 2061 6c6c 5f64 6973 705f 7820 3d20 5b5d   all_disp_x = []
+00017a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017aa0: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
+00017ab0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00017ac0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00017ad0: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+00017ae0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00017af0: 6c6c 5f61 6363 203d 205b 5d0d 0a20 2020  ll_acc = []..   
+00017b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b10: 2061 6c6c 5f64 6972 6563 7469 6f6e 616c   all_directional
+00017b20: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 2020  _change = []..  
 00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-00017b80: 635f 7261 6469 7573 2e61 7070 656e 6428  c_radius.append(
-00017b90: 4e6f 6e65 2920 2020 2020 2020 0d0a 2020  None)       ..  
-00017ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bc0: 2020 2020 2020 6d69 746f 7469 635f 7370        mitotic_sp
-00017bd0: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00017be0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017bf0: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00017c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c20: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017c30: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
-00017c40: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017c50: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-00017c60: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
-00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b40: 2020 616c 6c5f 6469 7374 616e 6365 5f63    all_distance_c
+00017b50: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a0d  ell_mask = []...
+00017b60: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
+00017b70: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+00017b80: 6b2c 7629 2069 6e20 616c 6c5f 7370 6f74  k,v) in all_spot
+00017b90: 735f 7472 6163 6b73 2e69 7465 6d73 2829  s_tracks.items()
+00017ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00017bb0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00017bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017bd0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00017be0: 7265 6e74 5f74 696d 6520 3d20 616c 6c5f  rent_time = all_
+00017bf0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017c00: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00017c10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017c20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017c30: 6974 6f74 6963 203d 2061 6c6c 5f73 706f  itotic = all_spo
+00017c40: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017c50: 662e 6469 7669 6469 6e67 5f6b 6579 5d0d  f.dividing_key].
+00017c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00017c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c90: 206d 6974 6f74 6963 5f64 6972 6563 7469   mitotic_directi
-00017ca0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00017cb0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017cc0: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
-00017cd0: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c90: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
+00017ca0: 3d20 696e 7428 6375 7272 656e 745f 7469  = int(current_ti
+00017cb0: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cd0: 2020 2020 2020 2020 6966 206d 6974 6f74          if mitot
+00017ce0: 6963 3a0d 0a20 2020 2020 2020 2020 2020  ic:..           
 00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017d10: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00017d20: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
-00017d30: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017d40: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-00017d50: 5f6d 6173 6b5f 6b65 795d 290d 0a0d 0a0d  _mask_key]).....
-00017d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d80: 2020 2069 6620 6e6f 7420 6d69 746f 7469     if not mitoti
-00017d90: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
-00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017db0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-00017dc0: 6d69 746f 7469 635f 6469 7370 5f7a 2e61  mitotic_disp_z.a
-00017dd0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017de0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
-00017df0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
-00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e20: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017e30: 5f64 6973 705f 792e 6170 7065 6e64 2861  _disp_y.append(a
+00017d00: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00017d10: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
+00017d20: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017d30: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
+00017d40: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
+00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d70: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
+00017d80: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017d90: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017da0: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00017db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dd0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017de0: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
+00017df0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017e00: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+00017e10: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e30: 2020 2020 2020 2020 2020 2020 6966 2061              if a
 00017e40: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017e50: 6b5d 5b73 656c 662e 7970 6f73 6964 5f6b  k][self.yposid_k
-00017e60: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017e50: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
+00017e60: 6579 5d20 3e20 303a 0d0a 2020 2020 2020  ey] > 0:..      
 00017e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e80: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00017e90: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-00017ea0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017eb0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017ec0: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
-00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e90: 2020 2020 206d 6974 6f74 6963 5f72 6164       mitotic_rad
+00017ea0: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+00017eb0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017ec0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+00017ed0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ef0: 2020 2020 2020 2069 6620 616c 6c5f 7370         if all_sp
-00017f00: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017f10: 6c66 2e72 6164 6975 735f 6b65 795d 203e  lf.radius_key] >
-00017f20: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f50: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
-00017f60: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
-00017f70: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017f80: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
-00017f90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fb0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00017fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017ff0: 5f6d 6974 6f74 6963 5f72 6164 6975 732e  _mitotic_radius.
-00018000: 6170 7065 6e64 284e 6f6e 6529 2020 2020  append(None)    
-00018010: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00017ef0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00017f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f20: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017f30: 7469 635f 7261 6469 7573 2e61 7070 656e  tic_radius.appen
+00017f40: 6428 4e6f 6e65 2920 2020 2020 2020 0d0a  d(None)       ..
+00017f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f70: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00017f80: 7370 6565 642e 6170 7065 6e64 2861 6c6c  speed.append(all
+00017f90: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017fa0: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
+00017fb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fd0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00017fe0: 6963 5f61 6363 2e61 7070 656e 6428 616c  ic_acc.append(al
+00017ff0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00018000: 5d5b 7365 6c66 2e61 6363 656c 6572 6174  ][self.accelerat
+00018010: 696f 6e5f 6b65 795d 290d 0a20 2020 2020  ion_key])..     
 00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018040: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00018050: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
-00018060: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018070: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
-00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180a0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000180b0: 6963 5f61 6363 2e61 7070 656e 6428 616c  ic_acc.append(al
-000180c0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000180d0: 5d5b 7365 6c66 2e61 6363 656c 6572 6174  ][self.accelerat
-000180e0: 696f 6e5f 6b65 795d 290d 0a20 2020 2020  ion_key])..     
-000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018110: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00018120: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018130: 652e 6170 7065 6e64 2861 6c6c 5f73 706f  e.append(all_spo
-00018140: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018150: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-00018160: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018190: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-000181a0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-000181b0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-000181c0: 6163 6b73 5b6b 5d5b 7365 6c66 2e64 6973  acks[k][self.dis
-000181d0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-000181e0: 6b65 795d 290d 0a0d 0a20 2020 2020 2020  key])....       
-000181f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018200: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
-00018210: 6973 705f 7a2e 6170 7065 6e64 2861 6c6c  isp_z.append(all
-00018220: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
-00018230: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-00018240: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-00018250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018260: 2020 2020 2020 616c 6c5f 6469 7370 5f79        all_disp_y
-00018270: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018280: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018290: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
-000182a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182c0: 2061 6c6c 5f64 6973 705f 782e 6170 7065   all_disp_x.appe
-000182d0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-000182e0: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-000182f0: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018310: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00018320: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00018330: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
-00018340: 6579 5d20 3e20 303a 0d0a 2020 2020 2020  ey] > 0:..      
+00018040: 2020 206d 6974 6f74 6963 5f64 6972 6563     mitotic_direc
+00018050: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
+00018060: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00018070: 7261 636b 735b 6b5d 5b73 656c 662e 6d6f  racks[k][self.mo
+00018080: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 5d29  tion_angle_key])
+00018090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180b0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000180c0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
+000180d0: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
+000180e0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000180f0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
+00018100: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a0d  ll_mask_key])...
+00018110: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018130: 2020 2020 2069 6620 6e6f 7420 6d69 746f       if not mito
+00018140: 7469 633a 0d0a 2020 2020 2020 2020 2020  tic:..          
+00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018160: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018170: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00018180: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00018190: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000181a0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
+000181b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181d0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+000181e0: 6963 5f64 6973 705f 792e 6170 7065 6e64  ic_disp_y.append
+000181f0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00018200: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
+00018210: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018240: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018250: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
+00018260: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00018270: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
+00018280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182a0: 2020 2020 2020 2020 2069 6620 616c 6c5f           if all_
+000182b0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000182c0: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+000182d0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
+000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018300: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f72     non_mitotic_r
+00018310: 6164 6975 732e 6170 7065 6e64 2861 6c6c  adius.append(all
+00018320: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00018330: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
+00018340: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018370: 616c 6c5f 7261 6469 7573 2e61 7070 656e  all_radius.appen
-00018380: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-00018390: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-000183a0: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000183d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018360: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00018370: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018390: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000183a0: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+000183b0: 732e 6170 7065 6e64 284e 6f6e 6529 2020  s.append(None)  
+000183c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000183d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 2020 2020 2020 2020 616c 6c5f 7261 6469          all_radi
-00018400: 7573 2e61 7070 656e 6428 4e6f 6e65 2920  us.append(None) 
-00018410: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00018420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018430: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
-00018440: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
-00018450: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00018460: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
-00018470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 2020 2061 6c6c 5f61 6363 2e61 7070 656e     all_acc.appen
-000184a0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000184b0: 6b73 5b6b 5d5b 7365 6c66 2e61 6363 656c  ks[k][self.accel
-000184c0: 6572 6174 696f 6e5f 6b65 795d 290d 0a20  eration_key]).. 
-000184d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184f0: 2061 6c6c 5f64 6972 6563 7469 6f6e 616c   all_directional
-00018500: 5f63 6861 6e67 652e 6170 7065 6e64 2861  _change.append(a
-00018510: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00018520: 6b5d 5b73 656c 662e 6d6f 7469 6f6e 5f61  k][self.motion_a
-00018530: 6e67 6c65 5f6b 6579 5d29 2020 200d 0a20  ngle_key])   .. 
-00018540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018560: 2061 6c6c 5f64 6973 7461 6e63 655f 6365   all_distance_ce
-00018570: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 2861  ll_mask.append(a
-00018580: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00018590: 6b5d 5b73 656c 662e 6469 7374 616e 6365  k][self.distance
-000185a0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d29  _cell_mask_key])
-000185b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000185f0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00018600: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
-00018610: 6e70 2e64 6966 6628 6d69 746f 7469 635f  np.diff(mitotic_
-00018620: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018630: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00018640: 746f 7469 635f 6469 7370 5f79 203d 206e  totic_disp_y = n
-00018650: 702e 6162 7328 6e70 2e64 6966 6628 6d69  p.abs(np.diff(mi
-00018660: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
-00018670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018680: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00018690: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
-000186a0: 6966 6628 6d69 746f 7469 635f 6469 7370  iff(mitotic_disp
-000186b0: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-000186c0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
-000186d0: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-000186e0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-000186f0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018700: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
-00018710: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018720: 746f 7469 635f 6469 7370 5f79 203d 206e  totic_disp_y = n
-00018730: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
-00018740: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
-00018750: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018760: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00018770: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
-00018780: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
-00018790: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-000187a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000187b0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-000187c0: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
-000187d0: 6966 6628 616c 6c5f 6469 7370 5f7a 2929  iff(all_disp_z))
-000187e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000187f0: 2020 2020 2020 616c 6c5f 6469 7370 5f79        all_disp_y
-00018800: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
-00018810: 6628 616c 6c5f 6469 7370 5f79 2929 0d0a  f(all_disp_y))..
-00018820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018830: 2020 2020 616c 6c5f 6469 7370 5f78 203d      all_disp_x =
-00018840: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-00018850: 616c 6c5f 6469 7370 5f78 2929 0d0a 0d0a  all_disp_x))....
-00018860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018880: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000183f0: 2020 6e6f 6e5f 6d69 746f 7469 635f 7370    non_mitotic_sp
+00018400: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
+00018410: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00018420: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
+00018430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018450: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00018460: 6f74 6963 5f61 6363 2e61 7070 656e 6428  otic_acc.append(
+00018470: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00018480: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
+00018490: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000184d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+000184e0: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
+000184f0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00018500: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00018510: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018540: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00018550: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018560: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00018570: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+00018580: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018590: 6b5f 6b65 795d 290d 0a0d 0a20 2020 2020  k_key])....     
+000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000185c0: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
+000185d0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+000185e0: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
+000185f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018610: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00018620: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
+00018630: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00018640: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+00018650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018670: 2020 2061 6c6c 5f64 6973 705f 782e 6170     all_disp_x.ap
+00018680: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00018690: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
+000186a0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000186d0: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+000186e0: 735b 6b5d 5b73 656c 662e 7261 6469 7573  s[k][self.radius
+000186f0: 5f6b 6579 5d20 3e20 303a 0d0a 2020 2020  _key] > 0:..    
+00018700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018720: 2020 616c 6c5f 7261 6469 7573 2e61 7070    all_radius.app
+00018730: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00018740: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+00018750: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018770: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00018780: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187a0: 2020 2020 2020 2020 2020 616c 6c5f 7261            all_ra
+000187b0: 6469 7573 2e61 7070 656e 6428 4e6f 6e65  dius.append(None
+000187c0: 2920 2020 2020 2020 0d0a 2020 2020 2020  )       ..      
+000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187e0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000187f0: 7370 6565 642e 6170 7065 6e64 2861 6c6c  speed.append(all
+00018800: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00018810: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
+00018820: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018840: 2020 2020 2061 6c6c 5f61 6363 2e61 7070       all_acc.app
+00018850: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00018860: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
+00018870: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
+00018880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 7365 6c66 2e74 696d 652e 6170 7065 6e64  self.time.append
-000188b0: 2869 202a 2073 656c 662e 7463 616c 6962  (i * self.tcalib
-000188c0: 7261 7469 6f6e 290d 0a0d 0a0d 0a20 2020  ration)......   
-000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-000188f0: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
-00018900: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00018910: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00018920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018930: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00018940: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018950: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
-00018960: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
-00018970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018980: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00018990: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-000189a0: 6d65 616e 286d 6974 6f74 6963 5f64 6973  mean(mitotic_dis
-000189b0: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
-000189c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000189d0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-000189e0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-000189f0: 286d 6974 6f74 6963 5f64 6973 705f 7929  (mitotic_disp_y)
-00018a00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018a10: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018a20: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00018a30: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
-00018a40: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
-00018a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018a60: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018a70: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-00018a80: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00018a90: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-00018aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ab0: 2020 2020 2066 696c 7465 7265 645f 7661       filtered_va
-00018ac0: 6c75 6573 203d 205b 7661 6c20 666f 7220  lues = [val for 
-00018ad0: 7661 6c20 696e 206d 6974 6f74 6963 5f72  val in mitotic_r
-00018ae0: 6164 6975 7320 6966 2076 616c 2069 7320  adius if val is 
-00018af0: 6e6f 7420 4e6f 6e65 5d0d 0a20 2020 2020  not None]..     
-00018b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018b10: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00018b20: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
-00018b30: 702e 6d65 616e 2866 696c 7465 7265 645f  p.mean(filtered_
-00018b40: 7661 6c75 6573 2929 0d0a 2020 2020 2020  values))..      
-00018b50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b70: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018b80: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-00018b90: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
-00018ba0: 6564 5f76 616c 7565 7329 290d 0a20 2020  ed_values))..   
-00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bc0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00018bd0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018be0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
-00018bf0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00018c00: 746f 7469 635f 7370 6565 6429 290d 0a20  totic_speed)).. 
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c20: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018c30: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
-00018c40: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00018c50: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
-00018c60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018c70: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00018c80: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-00018c90: 6561 6e28 6d69 746f 7469 635f 6163 6329  ean(mitotic_acc)
-00018ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018cb0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018cc0: 7469 635f 7661 725f 6163 632e 6170 7065  tic_var_acc.appe
-00018cd0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00018ce0: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018d00: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00018d10: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018d20: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-00018d30: 616e 286d 6974 6f74 6963 5f64 6972 6563  an(mitotic_direc
-00018d40: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
-00018d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d60: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018d70: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
-00018d80: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00018d90: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
-00018da0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018db0: 6529 290d 0a0d 0a20 2020 2020 2020 2020  e))....         
+000188a0: 2020 2061 6c6c 5f64 6972 6563 7469 6f6e     all_direction
+000188b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+000188c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+000188d0: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
+000188e0: 5f61 6e67 6c65 5f6b 6579 5d29 2020 200d  _angle_key])   .
+000188f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018910: 2020 2061 6c6c 5f64 6973 7461 6e63 655f     all_distance_
+00018920: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
+00018930: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00018940: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
+00018950: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
+00018960: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000189a0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000189b0: 635f 6469 7370 5f7a 203d 206e 702e 6162  c_disp_z = np.ab
+000189c0: 7328 6e70 2e64 6966 6628 6d69 746f 7469  s(np.diff(mitoti
+000189d0: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
+000189e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189f0: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
+00018a00: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00018a10: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+00018a20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018a30: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00018a40: 7370 5f78 203d 206e 702e 6162 7328 6e70  sp_x = np.abs(np
+00018a50: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
+00018a60: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00018a70: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018a80: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00018a90: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+00018aa0: 6628 6e6f 6e5f 6d69 746f 7469 635f 6469  f(non_mitotic_di
+00018ab0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+00018ac0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00018ad0: 6d69 746f 7469 635f 6469 7370 5f79 203d  mitotic_disp_y =
+00018ae0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00018af0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00018b00: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00018b10: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00018b20: 746f 7469 635f 6469 7370 5f78 203d 206e  totic_disp_x = n
+00018b30: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
+00018b40: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00018b50: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018b60: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00018b70: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
+00018b80: 2e64 6966 6628 616c 6c5f 6469 7370 5f7a  .diff(all_disp_z
+00018b90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018ba0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00018bb0: 5f79 203d 206e 702e 6162 7328 6e70 2e64  _y = np.abs(np.d
+00018bc0: 6966 6628 616c 6c5f 6469 7370 5f79 2929  iff(all_disp_y))
+00018bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018be0: 2020 2020 2020 616c 6c5f 6469 7370 5f78        all_disp_x
+00018bf0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+00018c00: 6628 616c 6c5f 6469 7370 5f78 2929 0d0a  f(all_disp_x))..
+00018c10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00018c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c50: 2020 7365 6c66 2e74 696d 652e 6170 7065    self.time.appe
+00018c60: 6e64 2869 202a 2073 656c 662e 7463 616c  nd(i * self.tcal
+00018c70: 6962 7261 7469 6f6e 290d 0a0d 0a0d 0a20  ibration)...... 
+00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c90: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018ca0: 6d65 616e 5f64 6973 705f 7a2e 6170 7065  mean_disp_z.appe
+00018cb0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+00018cc0: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ce0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00018cf0: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
+00018d00: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00018d10: 6973 705f 7a29 290d 0a0d 0a20 2020 2020  isp_z))....     
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018d30: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00018d40: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
+00018d50: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+00018d60: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+00018d70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018d80: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00018d90: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
+00018da0: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
+00018db0: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
 00018dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
 00018dd0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00018de0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00018df0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00018e00: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-00018e10: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00018e40: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
-00018e50: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
-00018e60: 7464 286d 6974 6f74 6963 5f64 6973 7461  td(mitotic_dista
-00018e70: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-00018e80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018e90: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00018ea0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00018eb0: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
-00018ec0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00018ed0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
-00018ee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018ef0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00018f00: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
-00018f10: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00018f20: 6963 5f64 6973 705f 7a29 290d 0a0d 0a20  ic_disp_z)).... 
-00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f40: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018f50: 7469 635f 6d65 616e 5f64 6973 705f 792e  tic_mean_disp_y.
-00018f60: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
-00018f70: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00018f80: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00018f90: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00018fa0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-00018fb0: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
-00018fc0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
-00018fd0: 6973 705f 7929 290d 0a0d 0a20 2020 2020  isp_y))....     
-00018fe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018ff0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00019000: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
-00019010: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
-00019020: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
-00019030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019040: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00019050: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
-00019060: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00019070: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-00019080: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
-00019090: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-000190a0: 7265 645f 7661 6c75 6573 203d 205b 7661  red_values = [va
-000190b0: 6c20 666f 7220 7661 6c20 696e 206e 6f6e  l for val in non
-000190c0: 5f6d 6974 6f74 6963 5f72 6164 6975 7320  _mitotic_radius 
-000190d0: 6966 2076 616c 2069 7320 6e6f 7420 4e6f  if val is not No
-000190e0: 6e65 5d0d 0a20 2020 2020 2020 2020 2020  ne]..           
-000190f0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00019100: 6e5f 6d69 746f 7469 635f 6d65 616e 5f72  n_mitotic_mean_r
-00019110: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00019120: 6d65 616e 2866 696c 7465 7265 645f 7661  mean(filtered_va
-00019130: 6c75 6573 2929 0d0a 2020 2020 2020 2020  lues))..        
-00019140: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019160: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00019170: 6963 5f76 6172 5f72 6164 6975 732e 6170  ic_var_radius.ap
-00019180: 7065 6e64 286e 702e 7374 6428 6669 6c74  pend(np.std(filt
-00019190: 6572 6564 5f76 616c 7565 7329 290d 0a0d  ered_values))...
-000191a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000191b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000191c0: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-000191d0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-000191e0: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-000191f0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00019200: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00019210: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-00019220: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-00019230: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
-00019240: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00019250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019260: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019270: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-00019280: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00019290: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
-000192a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000192b0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-000192c0: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-000192d0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-000192e0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-000192f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019300: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019310: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00019320: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00019330: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00019340: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00019350: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
-00019360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019370: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00019380: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00019390: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-000193a0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
-000193b0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-000193c0: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-000193d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000193e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-000193f0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00019400: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00019410: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00019420: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00019430: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019440: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00019450: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00019460: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00019470: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-00019480: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00019490: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-000194a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000194b0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000194c0: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
-000194d0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-000194e0: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-000194f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019500: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00019510: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
-00019520: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
-00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019540: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00019550: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
-00019560: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
-00019570: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00019580: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00019590: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
-000195a0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-000195b0: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
-000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195d0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-000195e0: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
-000195f0: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
-00019600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019610: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00019620: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
-00019630: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-00019640: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00019650: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
-00019660: 6572 6564 5f76 616c 7565 7320 3d20 5b76  ered_values = [v
-00019670: 616c 2066 6f72 2076 616c 2069 6e20 616c  al for val in al
-00019680: 6c5f 7261 6469 7573 2069 6620 7661 6c20  l_radius if val 
-00019690: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-000196c0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-000196d0: 2e6d 6561 6e28 6669 6c74 6572 6564 5f76  .mean(filtered_v
-000196e0: 616c 7565 7329 290d 0a20 2020 2020 2020  alues))..       
-000196f0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00019720: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
-00019730: 2e73 7464 2866 696c 7465 7265 645f 7661  .std(filtered_va
-00019740: 6c75 6573 2929 0d0a 0d0a 2020 2020 2020  lues))....      
-00019750: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019760: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
-00019770: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-00019780: 2861 6c6c 5f73 7065 6564 2929 0d0a 2020  (all_speed))..  
-00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197a0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
-000197b0: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
-000197c0: 7464 2861 6c6c 5f73 7065 6564 2929 0d0a  td(all_speed))..
-000197d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000197e0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-000197f0: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00019800: 702e 6d65 616e 2861 6c6c 5f61 6363 2929  p.mean(all_acc))
-00019810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019820: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00019830: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
-00019840: 2e73 7464 2861 6c6c 5f61 6363 2929 0d0a  .std(all_acc))..
+00018de0: 705f 782e 6170 7065 6e64 286e 702e 6d65  p_x.append(np.me
+00018df0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+00018e00: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+00018e10: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018e20: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00018e30: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00018e40: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00018e50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018e60: 2020 2020 2020 2066 696c 7465 7265 645f         filtered_
+00018e70: 7661 6c75 6573 203d 205b 7661 6c20 666f  values = [val fo
+00018e80: 7220 7661 6c20 696e 206d 6974 6f74 6963  r val in mitotic
+00018e90: 5f72 6164 6975 7320 6966 2076 616c 2069  _radius if val i
+00018ea0: 7320 6e6f 7420 4e6f 6e65 5d0d 0a20 2020  s not None]..   
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ec0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00018ed0: 616e 5f72 6164 6975 732e 6170 7065 6e64  an_radius.append
+00018ee0: 286e 702e 6d65 616e 2866 696c 7465 7265  (np.mean(filtere
+00018ef0: 645f 7661 6c75 6573 2929 0d0a 2020 2020  d_values))..    
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018f20: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018f30: 6963 5f76 6172 5f72 6164 6975 732e 6170  ic_var_radius.ap
+00018f40: 7065 6e64 286e 702e 7374 6428 6669 6c74  pend(np.std(filt
+00018f50: 6572 6564 5f76 616c 7565 7329 290d 0a20  ered_values)).. 
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f70: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00018f80: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018f90: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+00018fa0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018fb0: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
+00018fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018fd0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018fe0: 635f 7661 725f 7370 6565 642e 6170 7065  c_var_speed.appe
+00018ff0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00019000: 635f 7370 6565 6429 290d 0a0d 0a20 2020  c_speed))....   
+00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019020: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00019030: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
+00019040: 2e6d 6561 6e28 6d69 746f 7469 635f 6163  .mean(mitotic_ac
+00019050: 6329 290d 0a20 2020 2020 2020 2020 2020  c))..           
+00019060: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00019070: 746f 7469 635f 7661 725f 6163 632e 6170  totic_var_acc.ap
+00019080: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00019090: 7469 635f 6163 6329 290d 0a0d 0a20 2020  tic_acc))....   
+000190a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190b0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+000190c0: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+000190d0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+000190e0: 6d65 616e 286d 6974 6f74 6963 5f64 6972  mean(mitotic_dir
+000190f0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00019100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019110: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00019120: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
+00019130: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00019140: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+00019150: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019160: 6e67 6529 290d 0a0d 0a20 2020 2020 2020  nge))....       
+00019170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019180: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00019190: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000191a0: 6b2e 6170 7065 6e64 286e 702e 6d65 616e  k.append(np.mean
+000191b0: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
+000191c0: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a20  e_cell_mask)).. 
+000191d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191e0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000191f0: 7661 725f 6469 7374 616e 6365 5f63 656c  var_distance_cel
+00019200: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00019210: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
+00019220: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
+00019230: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019240: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00019250: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+00019260: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+00019270: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+00019280: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00019290: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000192a0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000192b0: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
+000192c0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
+000192d0: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
+000192e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000192f0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00019300: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00019310: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
+00019320: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00019330: 705f 7929 290d 0a20 2020 2020 2020 2020  p_y))..         
+00019340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019350: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019360: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+00019370: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+00019380: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000193b0: 635f 6d65 616e 5f64 6973 705f 782e 6170  c_mean_disp_x.ap
+000193c0: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+000193d0: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
+000193e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000193f0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00019400: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00019410: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
+00019420: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00019430: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
+00019440: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00019450: 7465 7265 645f 7661 6c75 6573 203d 205b  tered_values = [
+00019460: 7661 6c20 666f 7220 7661 6c20 696e 206e  val for val in n
+00019470: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+00019480: 7320 6966 2076 616c 2069 7320 6e6f 7420  s if val is not 
+00019490: 4e6f 6e65 5d0d 0a20 2020 2020 2020 2020  None]..         
+000194a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000194b0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000194c0: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+000194d0: 702e 6d65 616e 2866 696c 7465 7265 645f  p.mean(filtered_
+000194e0: 7661 6c75 6573 2929 0d0a 2020 2020 2020  values))..      
+000194f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019510: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00019520: 6f74 6963 5f76 6172 5f72 6164 6975 732e  otic_var_radius.
+00019530: 6170 7065 6e64 286e 702e 7374 6428 6669  append(np.std(fi
+00019540: 6c74 6572 6564 5f76 616c 7565 7329 290d  ltered_values)).
+00019550: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019560: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00019570: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+00019580: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
+00019590: 6e28 6e6f 6e5f 6d69 746f 7469 635f 7370  n(non_mitotic_sp
+000195a0: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+000195b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000195c0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+000195d0: 7370 6565 642e 6170 7065 6e64 286e 702e  speed.append(np.
+000195e0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+000195f0: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00019600: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019610: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00019620: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
+00019630: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00019640: 7469 635f 6163 6329 290d 0a20 2020 2020  tic_acc))..     
+00019650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019660: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00019670: 7661 725f 6163 632e 6170 7065 6e64 286e  var_acc.append(n
+00019680: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00019690: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
+000196a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000196b0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000196c0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+000196d0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+000196e0: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+000196f0: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00019700: 6861 6e67 6529 290d 0a20 2020 2020 2020  hange))..       
+00019710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019720: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00019730: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00019740: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+00019750: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00019760: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00019770: 6529 2920 0d0a 0d0a 2020 2020 2020 2020  e)) ....        
+00019780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019790: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+000197a0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+000197b0: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
+000197c0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+000197d0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000197e0: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+000197f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00019800: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
+00019810: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00019820: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+00019830: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+00019840: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
 00019850: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
 00019860: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00019870: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
-00019880: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00019890: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-000198a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000198b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000198c0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000198d0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-000198e0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-000198f0: 702e 7374 6428 616c 6c5f 6469 7265 6374  p.std(all_direct
-00019900: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
-00019910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019920: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00019930: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
-00019940: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
-00019950: 2e6d 6561 6e28 616c 6c5f 6469 7374 616e  .mean(all_distan
-00019960: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00019870: 6c6c 5f6d 6561 6e5f 6469 7370 5f7a 2e61  ll_mean_disp_z.a
+00019880: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00019890: 6c5f 6469 7370 5f7a 2929 0d0a 2020 2020  l_disp_z))..    
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+000198c0: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
+000198d0: 6428 616c 6c5f 6469 7370 5f7a 2929 0d0a  d(all_disp_z))..
+000198e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000198f0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00019900: 6561 6e5f 6469 7370 5f79 2e61 7070 656e  ean_disp_y.appen
+00019910: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+00019920: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
+00019930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019940: 2e61 6c6c 5f76 6172 5f64 6973 705f 792e  .all_var_disp_y.
+00019950: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00019960: 6c5f 6469 7370 5f79 2929 0d0a 0d0a 2020  l_disp_y))....  
 00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019980: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00019990: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000199a0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
-000199b0: 6428 616c 6c5f 6469 7374 616e 6365 5f63  d(all_distance_c
-000199c0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000199f0: 2020 0d0a 6465 6620 626f 756e 6461 7279    ..def boundary
-00019a00: 5f70 6f69 6e74 7328 6d61 736b 2c20 7863  _points(mask, xc
-00019a10: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
-00019a20: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
-00019a30: 7261 7469 6f6e 293a 0d0a 0d0a 2020 2020  ration):....    
-00019a40: 6e64 696d 203d 206c 656e 286d 6173 6b2e  ndim = len(mask.
-00019a50: 7368 6170 6529 0d0a 2020 2020 7469 6d65  shape)..    time
-00019a60: 645f 6d61 736b 203d 207b 7d0d 0a20 2020  d_mask = {}..   
-00019a70: 206d 6173 6b20 3d20 6d61 736b 203e 2030   mask = mask > 0
-00019a80: 0d0a 2020 2020 6d61 736b 203d 206d 6173  ..    mask = mas
-00019a90: 6b2e 6173 7479 7065 2827 7569 6e74 3827  k.astype('uint8'
-00019aa0: 290d 0a20 2020 2023 2059 5820 7368 6170  )..    # YX shap
-00019ab0: 6564 206f 626a 6563 740d 0a20 2020 2069  ed object..    i
-00019ac0: 6620 6e64 696d 203d 3d20 323a 0d0a 2020  f ndim == 2:..  
-00019ad0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00019ae0: 626f 756e 6461 7279 203d 2066 696e 645f  boundary = find_
-00019af0: 626f 756e 6461 7269 6573 286d 6173 6b29  boundaries(mask)
-00019b00: 0d0a 2020 2020 2020 2020 7265 6769 6f6e  ..        region
-00019b10: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
-00019b20: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
-00019b30: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
-00019b40: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-00019b50: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
-00019b60: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
-00019b70: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
-00019b80: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
-00019b90: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
-00019ba0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00019bb0: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
-00019bc0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00019bd0: 616e 6765 2830 2c20 6c65 6e28 7265 616c  ange(0, len(real
-00019be0: 5f69 6e64 6963 6573 2929 3a0d 0a0d 0a20  _indices)):.... 
-00019bf0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-00019c00: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
-00019c10: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-00019c20: 305d 202a 2079 6361 6c69 6272 6174 696f  0] * ycalibratio
-00019c30: 6e0d 0a20 2020 2020 2020 2020 2020 2072  n..            r
-00019c40: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019c50: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-00019c60: 5b6a 5d5b 315d 202a 2078 6361 6c69 6272  [j][1] * xcalibr
-00019c70: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
-00019c80: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
-00019c90: 634b 4454 7265 6528 7265 616c 5f69 6e64  cKDTree(real_ind
-00019ca0: 6963 6573 290d 0a20 2020 2020 2020 2023  ices)..        #
-00019cb0: 2054 6869 7320 6f62 6a65 6374 2063 6f6e   This object con
-00019cc0: 7461 696e 7320 6c69 7374 206f 6620 616c  tains list of al
-00019cd0: 6c20 7468 6520 706f 696e 7473 2066 6f72  l the points for
-00019ce0: 2061 6c6c 2074 6865 206c 6162 656c 7320   all the labels 
-00019cf0: 696e 2074 6865 204d 6173 6b20 696d 6167  in the Mask imag
-00019d00: 6520 7769 7468 2074 6865 206c 6162 656c  e with the label
-00019d10: 2069 6420 616e 6420 766f 6c75 6d65 206f   id and volume o
-00019d20: 6620 6561 6368 206c 6162 656c 0d0a 2020  f each label..  
-00019d30: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
-00019d40: 5b73 7472 2830 295d 203d 205b 7472 6565  [str(0)] = [tree
-00019d50: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
-00019d60: 6e63 656e 7472 6f69 645d 0d0a 0d0a 2020  ncentroid]....  
-00019d70: 2020 2320 5459 5820 7368 6170 6564 206f    # TYX shaped o
-00019d80: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
-00019d90: 696d 203d 3d20 333a 0d0a 0d0a 0d0a 2020  im == 3:......  
-00019da0: 2020 2020 2020 666f 7220 6920 696e 2074        for i in t
-00019db0: 7164 6d28 7261 6e67 6528 302c 206d 6173  qdm(range(0, mas
-00019dc0: 6b2e 7368 6170 655b 305d 2929 3a0d 0a20  k.shape[0])):.. 
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00019de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019df0: 2062 6f75 6e64 6172 7920 3d20 6669 6e64   boundary = find
-00019e00: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
-00019e10: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
-00019e20: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
-00019e30: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
-00019e40: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-00019e50: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
-00019e60: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-00019e70: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
-00019e80: 626f 756e 6461 7279 203e 2030 290d 0a20  boundary > 0).. 
-00019e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019ea0: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
-00019eb0: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
-00019ec0: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
-00019ed0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00019ee0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
-00019ef0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019f00: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
-00019f10: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
-00019f20: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-00019f30: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019f40: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
-00019f50: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-00019f60: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-00019f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019f80: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019f90: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
-00019fa0: 6e64 6963 6573 5b6a 5d5b 315d 202a 2078  ndices[j][1] * x
-00019fb0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
-00019fc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00019fd0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
-00019fe0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
-00019ff0: 6573 290d 0a0d 0a20 2020 2020 2020 2020  es)....         
-0001a000: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
-0001a010: 6b5b 7374 7228 6929 5d20 3d20 5b74 7265  k[str(i)] = [tre
-0001a020: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
-0001a030: 6f6e 6365 6e74 726f 6964 5d0d 0a20 2020  oncentroid]..   
-0001a040: 2020 2020 2020 2020 200d 0a20 2020 2023           ..    #
-0001a050: 2054 5a59 5820 7368 6170 6564 206f 626a   TZYX shaped obj
-0001a060: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-0001a070: 203d 3d20 343a 0d0a 2020 2020 2020 2020   == 4:..        
-0001a080: 7072 696e 7428 274d 616b 696e 6720 6d61  print('Making ma
-0001a090: 736b 2069 6e20 3444 2729 0d0a 2020 2020  sk in 4D')..    
-0001a0a0: 2020 2020 626f 756e 6461 7279 203d 206e      boundary = n
-0001a0b0: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
-0001a0c0: 2020 2020 2020 5b6d 6173 6b2e 7368 6170        [mask.shap
-0001a0d0: 655b 305d 2c20 6d61 736b 2e73 6861 7065  e[0], mask.shape
-0001a0e0: 5b31 5d2c 206d 6173 6b2e 7368 6170 655b  [1], mask.shape[
-0001a0f0: 325d 2c20 6d61 736b 2e73 6861 7065 5b33  2], mask.shape[3
-0001a100: 5d5d 2c20 6474 7970 653d 6e70 2e75 696e  ]], dtype=np.uin
-0001a110: 7438 0d0a 2020 2020 2020 2020 290d 0a20  t8..        ).. 
-0001a120: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0001a130: 7261 6e67 6528 302c 206d 6173 6b2e 7368  range(0, mask.sh
-0001a140: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
-0001a150: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001a160: 2020 2020 626f 756e 6461 7279 5b69 2c3a      boundary[i,:
-0001a170: 5d20 3d20 6669 6e64 5f62 6f75 6e64 6172  ] = find_boundar
-0001a180: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
-0001a190: 2020 2020 2020 2020 2020 2020 7265 6769              regi
-0001a1a0: 6f6e 6365 6e74 726f 6964 203d 2063 6f6d  oncentroid = com
-0001a1b0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-0001a1c0: 756e 6461 7279 5b69 2c3a 5d29 200d 0a20  undary[i,:]) .. 
-0001a1d0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
-0001a1e0: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
-0001a1f0: 756e 6461 7279 5b69 2c3a 5d20 3e20 3029  undary[i,:] > 0)
-0001a200: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001a210: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
-0001a220: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
-0001a230: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
-0001a240: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
-0001a250: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
-0001a260: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0001a270: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
-0001a280: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
-0001a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2a0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-0001a2b0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-0001a2c0: 6469 6365 735b 6a5d 5b30 5d20 2a20 7a63  dices[j][0] * zc
-0001a2d0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2f0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-0001a300: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
-0001a310: 735b 6a5d 5b31 5d20 2a20 7963 616c 6962  s[j][1] * ycalib
-0001a320: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a330: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001a340: 5f69 6e64 6963 6573 5b6a 5d5b 325d 203d  _indices[j][2] =
-0001a350: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-0001a360: 5b32 5d20 2a20 7863 616c 6962 7261 7469  [2] * xcalibrati
-0001a370: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-0001a380: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
-0001a390: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
-0001a3a0: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
-0001a3b0: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-0001a3c0: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
-0001a3d0: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-0001a3e0: 656e 7472 6f69 645d 0d0a 2020 2020 7072  entroid]..    pr
-0001a3f0: 696e 7428 2743 6f6d 7075 7465 6420 7468  int('Computed th
-0001a400: 6520 626f 756e 6461 7279 2070 6f69 6e74  e boundary point
-0001a410: 7327 290d 0a0d 0a20 2020 2072 6574 7572  s')....    retur
-0001a420: 6e20 7469 6d65 645f 6d61 736b 2c20 626f  n timed_mask, bo
-0001a430: 756e 6461 7279 2020 2020 2020 2020 0d0a  undary        ..
-0001a440: 0d0a 6465 6620 636f 6d70 7574 655f 6365  ..def compute_ce
-0001a450: 6e74 726f 6964 2862 696e 6172 795f 696d  ntroid(binary_im
-0001a460: 6167 6529 3a0d 0a20 2020 2023 2045 6e73  age):..    # Ens
-0001a470: 7572 6520 6269 6e61 7279 2069 6d61 6765  ure binary image
-0001a480: 2069 7320 6120 4e75 6d50 7920 6172 7261   is a NumPy arra
-0001a490: 790d 0a20 2020 2062 696e 6172 795f 696d  y..    binary_im
-0001a4a0: 6167 6520 3d20 6e70 2e61 7272 6179 2862  age = np.array(b
-0001a4b0: 696e 6172 795f 696d 6167 6529 0d0a 0d0a  inary_image)....
-0001a4c0: 2020 2020 7768 6974 655f 7069 7865 6c73      white_pixels
-0001a4d0: 203d 206e 702e 7768 6572 6528 6269 6e61   = np.where(bina
-0001a4e0: 7279 5f69 6d61 6765 203d 3d20 3129 0d0a  ry_image == 1)..
-0001a4f0: 2020 2020 6e75 6d5f 7069 7865 6c73 203d      num_pixels =
-0001a500: 206c 656e 2877 6869 7465 5f70 6978 656c   len(white_pixel
-0001a510: 735b 305d 290d 0a0d 0a20 2020 2023 2043  s[0])....    # C
-0001a520: 6f6d 7075 7465 2074 6865 2063 656e 7472  ompute the centr
-0001a530: 6f69 6420 6f66 2074 6865 2077 6869 7465  oid of the white
-0001a540: 2070 6978 656c 7320 696e 2074 6865 2062   pixels in the b
-0001a550: 6f75 6e64 6172 7920 696d 6167 650d 0a20  oundary image.. 
-0001a560: 2020 2063 656e 7472 6f69 6420 3d20 6e70     centroid = np
-0001a570: 2e7a 6572 6f73 2862 696e 6172 795f 696d  .zeros(binary_im
-0001a580: 6167 652e 6e64 696d 290d 0a20 2020 2066  age.ndim)..    f
-0001a590: 6f72 2064 696d 2069 6e20 7261 6e67 6528  or dim in range(
-0001a5a0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
-0001a5b0: 6d29 3a0d 0a20 2020 2020 2020 2063 656e  m):..        cen
-0001a5c0: 7472 6f69 645b 6469 6d5d 203d 2077 6869  troid[dim] = whi
-0001a5d0: 7465 5f70 6978 656c 735b 6469 6d5d 2e73  te_pixels[dim].s
-0001a5e0: 756d 2829 202f 206e 756d 5f70 6978 656c  um() / num_pixel
-0001a5f0: 730d 0a0d 0a20 2020 2072 6574 7572 6e20  s....    return 
-0001a600: 6365 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a  centroid........
-0001a610: 200d 0a0d 0a64 6566 2067 6574 5f63 7376   ....def get_csv
-0001a620: 5f64 6174 6128 6373 7629 3a0d 0a0d 0a20  _data(csv):.... 
-0001a630: 2020 2020 2020 2064 6174 6173 6574 203d         dataset =
-0001a640: 2070 642e 7265 6164 5f63 7376 280d 0a20   pd.read_csv(.. 
-0001a650: 2020 2020 2020 2020 2020 2063 7376 2c20             csv, 
-0001a660: 6465 6c69 6d69 7465 723d 222c 222c 2065  delimiter=",", e
-0001a670: 6e63 6f64 696e 673d 2275 6e69 636f 6465  ncoding="unicode
-0001a680: 5f65 7363 6170 6522 2c20 6c6f 775f 6d65  _escape", low_me
-0001a690: 6d6f 7279 3d46 616c 7365 0d0a 2020 2020  mory=False..    
-0001a6a0: 2020 2020 295b 333a 5d0d 0a20 2020 2020      )[3:]..     
-0001a6b0: 2020 2064 6174 6173 6574 5f69 6e64 6578     dataset_index
-0001a6c0: 203d 2064 6174 6173 6574 2e69 6e64 6578   = dataset.index
-0001a6d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001a6e0: 2064 6174 6173 6574 2c20 6461 7461 7365   dataset, datase
-0001a6f0: 745f 696e 6465 780d 0a20 2020 200d 0a64  t_index..    ..d
-0001a700: 6566 2067 6574 5f73 706f 745f 6461 7461  ef get_spot_data
-0001a710: 7365 7428 7370 6f74 5f64 6174 6173 6574  set(spot_dataset
-0001a720: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-0001a730: 5f73 706f 745f 6b65 7973 2c20 7863 616c  _spot_keys, xcal
-0001a740: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
-0001a750: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
-0001a760: 7469 6f6e 2c20 4174 7472 6962 7574 6542  tion, AttributeB
-0001a770: 6f78 6e61 6d65 2c20 6465 7465 6374 696f  oxname, detectio
-0001a780: 6e63 6861 6e6e 656c 293a 0d0a 2020 2020  nchannel):..    
-0001a790: 2020 2020 416c 6c56 616c 7565 7320 3d20      AllValues = 
-0001a7a0: 7b7d 0d0a 2020 2020 2020 2020 706f 7369  {}..        posi
-0001a7b0: 7820 3d20 7472 6163 6b5f 616e 616c 7973  x = track_analys
-0001a7c0: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-0001a7d0: 7369 7822 5d0d 0a20 2020 2020 2020 2070  six"]..        p
-0001a7e0: 6f73 6979 203d 2074 7261 636b 5f61 6e61  osiy = track_ana
-0001a7f0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001a800: 2270 6f73 6979 225d 0d0a 2020 2020 2020  "posiy"]..      
-0001a810: 2020 706f 7369 7a20 3d20 7472 6163 6b5f    posiz = track_
-0001a820: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a830: 7973 5b22 706f 7369 7a22 5d0d 0a20 2020  ys["posiz"]..   
-0001a840: 2020 2020 2066 7261 6d65 203d 2074 7261       frame = tra
-0001a850: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a860: 5f6b 6579 735b 2266 7261 6d65 225d 0d0a  _keys["frame"]..
-0001a870: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001a880: 2020 4c6f 6361 7469 6f6e 5820 3d20 280d    LocationX = (.
-0001a890: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-0001a8a0: 745f 6461 7461 7365 745b 706f 7369 785d  t_dataset[posix]
-0001a8b0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a8c0: 202f 2078 6361 6c69 6272 6174 696f 6e0d   / xcalibration.
-0001a8d0: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-0001a8e0: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-0001a8f0: 2020 4c6f 6361 7469 6f6e 5920 3d20 280d    LocationY = (.
-0001a900: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-0001a910: 745f 6461 7461 7365 745b 706f 7369 795d  t_dataset[posiy]
-0001a920: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a930: 202f 2079 6361 6c69 6272 6174 696f 6e0d   / ycalibration.
-0001a940: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-0001a950: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-0001a960: 2020 4c6f 6361 7469 6f6e 5a20 3d20 280d    LocationZ = (.
-0001a970: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
-0001a980: 745f 6461 7461 7365 745b 706f 7369 7a5d  t_dataset[posiz]
-0001a990: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001a9a0: 202f 207a 6361 6c69 6272 6174 696f 6e0d   / zcalibration.
-0001a9b0: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
-0001a9c0: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-0001a9d0: 2020 4c6f 6361 7469 6f6e 5420 3d20 2873    LocationT = (s
-0001a9e0: 706f 745f 6461 7461 7365 745b 6672 616d  pot_dataset[fram
-0001a9f0: 655d 2e61 7374 7970 6528 2266 6c6f 6174  e].astype("float
-0001aa00: 2229 292e 6173 7479 7065 2822 696e 7422  ")).astype("int"
-0001aa10: 290d 0a20 2020 2020 2020 200d 0a0d 0a20  )..        .... 
-0001aa20: 2020 2020 2020 2069 676e 6f72 655f 7661         ignore_va
-0001aa30: 6c75 6573 203d 205b 7472 6163 6b5f 616e  lues = [track_an
-0001aa40: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001aa50: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
-0001aa60: 225d 2c74 7261 636b 5f61 6e61 6c79 7369  "],track_analysi
-0001aa70: 735f 7370 6f74 5f6b 6579 735b 2274 6f74  s_spot_keys["tot
-0001aa80: 616c 5f69 6e74 656e 7369 7479 225d 5d0d  al_intensity"]].
-0001aa90: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
-0001aaa0: 7629 2069 6e20 7472 6163 6b5f 616e 616c  v) in track_anal
-0001aab0: 7973 6973 5f73 706f 745f 6b65 7973 2e69  ysis_spot_keys.i
-0001aac0: 7465 6d73 2829 3a0d 0a0d 0a20 2020 2020  tems():....     
-0001aad0: 2020 2020 2020 2020 2020 2069 6620 6465             if de
-0001aae0: 7465 6374 696f 6e63 6861 6e6e 656c 203d  tectionchannel =
-0001aaf0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
-0001ab00: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
-0001ab10: 3d3d 2022 6d65 616e 5f69 6e74 656e 7369  == "mean_intensi
-0001ab20: 7479 5f63 6832 223a 0d0a 2020 2020 2020  ty_ch2":..      
-0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab40: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
-0001ab50: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001ab60: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
-0001ab70: 6e73 6974 7922 5d0d 0a20 2020 2020 2020  nsity"]..       
-0001ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab90: 2020 2020 416c 6c56 616c 7565 735b 7661      AllValues[va
-0001aba0: 6c75 655d 203d 2073 706f 745f 6461 7461  lue] = spot_data
-0001abb0: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
-0001abc0: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
-0001abd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001abe0: 6b20 3d3d 2022 746f 7461 6c5f 696e 7465  k == "total_inte
-0001abf0: 6e73 6974 795f 6368 3222 3a0d 0a20 2020  nsity_ch2":..   
-0001ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac10: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-0001ac20: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001ac30: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
-0001ac40: 696e 7465 6e73 6974 7922 5d0d 0a20 2020  intensity"]..   
-0001ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac60: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001ac70: 735b 7661 6c75 655d 203d 2073 706f 745f  s[value] = spot_
-0001ac80: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
-0001ac90: 6528 2266 6c6f 6174 2229 2020 2020 2020  e("float")      
-0001aca0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0001acb0: 2020 2020 2069 6620 7620 6e6f 7420 696e       if v not in
-0001acc0: 2069 676e 6f72 655f 7661 6c75 6573 3a0d   ignore_values:.
-0001acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ace0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad00: 2041 6c6c 5661 6c75 6573 5b76 5d20 3d20   AllValues[v] = 
-0001ad10: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
-0001ad20: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001ad30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ad40: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0001ad50: 416c 6c56 616c 7565 735b 706f 7369 785d  AllValues[posix]
-0001ad60: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001ad70: 6e58 2c33 290d 0a20 2020 2020 2020 2041  nX,3)..        A
-0001ad80: 6c6c 5661 6c75 6573 5b70 6f73 6979 5d20  llValues[posiy] 
-0001ad90: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
-0001ada0: 592c 3329 0d0a 2020 2020 2020 2020 416c  Y,3)..        Al
-0001adb0: 6c56 616c 7565 735b 706f 7369 7a5d 203d  lValues[posiz] =
-0001adc0: 2072 6f75 6e64 284c 6f63 6174 696f 6e5a   round(LocationZ
-0001add0: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
-0001ade0: 5661 6c75 6573 5b66 7261 6d65 5d20 3d20  Values[frame] = 
-0001adf0: 726f 756e 6428 4c6f 6361 7469 6f6e 542c  round(LocationT,
-0001ae00: 3329 0d0a 2020 2020 2020 2020 4174 7472  3)..        Attr
-0001ae10: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
-0001ae20: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
-0001ae30: 6964 732e 6170 7065 6e64 2841 7474 7269  ids.append(Attri
-0001ae40: 6275 7465 426f 786e 616d 6529 0d0a 2020  buteBoxname)..  
-0001ae50: 2020 2020 2020 666f 7220 6174 7472 6962        for attrib
-0001ae60: 7574 656e 616d 6520 696e 2041 6c6c 5661  utename in AllVa
-0001ae70: 6c75 6573 2e6b 6579 7328 293a 0d0a 2020  lues.keys():..  
-0001ae80: 2020 2020 2020 2020 2020 2020 4174 7472              Attr
-0001ae90: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
-0001aea0: 6174 7472 6962 7574 656e 616d 6529 2020  attributename)  
-0001aeb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0001aec0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0001aed0: 2020 2020 7265 7475 726e 2041 7474 7269      return Attri
-0001aee0: 6275 7465 6964 732c 2041 6c6c 5661 6c75  buteids, AllValu
-0001aef0: 6573 2020 2020 200d 0a20 2020 200d 0a64  es     ..    ..d
-0001af00: 6566 2067 6574 5f74 7261 636b 5f64 6174  ef get_track_dat
-0001af10: 6173 6574 2874 7261 636b 5f64 6174 6173  aset(track_datas
-0001af20: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
-0001af30: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
-0001af40: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
-0001af50: 636b 5f6b 6579 732c 2054 7261 636b 4174  ck_keys, TrackAt
-0001af60: 7472 6962 7574 6542 6f78 6e61 6d65 293a  tributeBoxname):
-0001af70: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
-0001af80: 7261 636b 5661 6c75 6573 203d 207b 7d0d  rackValues = {}.
-0001af90: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
-0001afa0: 6420 3d20 7472 6163 6b5f 616e 616c 7973  d = track_analys
-0001afb0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
-0001afc0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
-0001afd0: 2020 5469 6420 3d20 7472 6163 6b5f 6461    Tid = track_da
-0001afe0: 7461 7365 745b 7472 6163 6b5f 6964 5d2e  taset[track_id].
-0001aff0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001b000: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-0001b010: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
-0001b020: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
-0001b030: 0d0a 2020 2020 2020 0d0a 2020 2020 2020  ..      ..      
-0001b040: 2020 666f 7220 286b 2c20 7629 2069 6e20    for (k, v) in 
-0001b050: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
-0001b060: 7261 636b 5f6b 6579 732e 6974 656d 7328  rack_keys.items(
-0001b070: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
-0001b080: 2020 2020 2020 7820 3d20 7472 6163 6b5f        x = track_
-0001b090: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
-0001b0a0: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
-0001b0b0: 2020 2020 2020 2020 2020 2020 6d69 6e76              minv
-0001b0c0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
-0001b0d0: 2020 2020 2020 2020 2020 2020 206d 6178               max
-0001b0e0: 7661 6c20 3d20 6d61 7828 7829 0d0a 0d0a  val = max(x)....
-0001b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b100: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
-0001b110: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
-0001b120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b130: 2020 2020 2020 7820 3d20 7820 2b20 310d        x = x + 1.
-0001b140: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001b150: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
-0001b160: 735b 6b5d 203d 2072 6f75 6e64 2878 2c20  s[k] = round(x, 
-0001b170: 3329 0d0a 0d0a 2020 2020 2020 2020 5472  3)....        Tr
-0001b180: 6163 6b41 7474 7269 6275 7465 6964 7320  ackAttributeids 
-0001b190: 3d20 5b5d 0d0a 2020 2020 2020 2020 5472  = []..        Tr
-0001b1a0: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
-0001b1b0: 6170 7065 6e64 2854 7261 636b 4174 7472  append(TrackAttr
-0001b1c0: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
-0001b1d0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
-0001b1e0: 6275 7465 6e61 6d65 2069 6e20 7472 6163  butename in trac
-0001b1f0: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
-0001b200: 5f6b 6579 732e 6b65 7973 2829 3a0d 0a20  _keys.keys():.. 
-0001b210: 2020 2020 2020 2020 2020 2054 7261 636b             Track
-0001b220: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001b230: 656e 6428 6174 7472 6962 7574 656e 616d  end(attributenam
-0001b240: 6529 2020 2020 0d0a 2020 2020 0d0a 2020  e)    ..    ..  
-0001b250: 2020 2020 2020 7265 7475 726e 2054 7261        return Tra
-0001b260: 636b 4174 7472 6962 7574 6569 6473 2c20  ckAttributeids, 
-0001b270: 416c 6c54 7261 636b 5661 6c75 6573 0d0a  AllTrackValues..
-0001b280: 2020 2020 0d0a 6465 6620 6765 745f 6564      ..def get_ed
-0001b290: 6765 735f 6461 7461 7365 7428 6564 6765  ges_dataset(edge
-0001b2a0: 735f 6461 7461 7365 742c 2065 6467 6573  s_dataset, edges
-0001b2b0: 5f64 6174 6173 6574 5f69 6e64 6578 2c20  _dataset_index, 
-0001b2c0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001b2d0: 706f 745f 6b65 7973 2c20 7472 6163 6b5f  pot_keys, track_
-0001b2e0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
-0001b2f0: 6579 7329 3a0d 0a0d 0a20 2020 2020 2020  eys):....       
-0001b300: 2041 6c6c 4564 6765 7356 616c 7565 7320   AllEdgesValues 
-0001b310: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
-0001b320: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
-0001b330: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001b340: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
-0001b350: 2020 2020 2020 2054 6964 203d 2065 6467         Tid = edg
-0001b360: 6573 5f64 6174 6173 6574 5b74 7261 636b  es_dataset[track
-0001b370: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
-0001b380: 6174 2229 0d0a 2020 2020 2020 2020 696e  at")..        in
-0001b390: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
-0001b3a0: 2854 6964 203d 3d20 3029 0d0a 2020 2020  (Tid == 0)..    
-0001b3b0: 2020 2020 6d61 7874 7261 636b 5f69 6420      maxtrack_id 
-0001b3c0: 3d20 6d61 7828 5469 6429 0d0a 2020 2020  = max(Tid)..    
-0001b3d0: 2020 2020 636f 6e64 6974 696f 6e5f 696e      condition_in
-0001b3e0: 6469 6365 7320 3d20 6564 6765 735f 6461  dices = edges_da
-0001b3f0: 7461 7365 745f 696e 6465 785b 696e 6469  taset_index[indi
-0001b400: 6365 735d 0d0a 2020 2020 2020 2020 5469  ces]..        Ti
-0001b410: 645b 636f 6e64 6974 696f 6e5f 696e 6469  d[condition_indi
-0001b420: 6365 735d 203d 206d 6178 7472 6163 6b5f  ces] = maxtrack_
-0001b430: 6964 202b 2031 0d0a 2020 2020 2020 2020  id + 1..        
-0001b440: 416c 6c45 6467 6573 5661 6c75 6573 5b74  AllEdgesValues[t
-0001b450: 7261 636b 5f69 645d 203d 2054 6964 0d0a  rack_id] = Tid..
-0001b460: 0d0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
-0001b470: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001b480: 735f 6564 6765 735f 6b65 7973 2e76 616c  s_edges_keys.val
-0001b490: 7565 7328 293a 0d0a 0d0a 2020 2020 2020  ues():....      
-0001b4a0: 2020 2020 2020 6966 206b 2021 3d20 7472        if k != tr
-0001b4b0: 6163 6b5f 6964 3a0d 0a20 2020 2020 2020  ack_id:..       
-0001b4c0: 2020 2020 2020 2020 2078 203d 2065 6467           x = edg
-0001b4d0: 6573 5f64 6174 6173 6574 5b6b 5d2e 6173  es_dataset[k].as
-0001b4e0: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
-0001b4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b500: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
-0001b510: 6b5d 203d 2078 2020 200d 0a20 2020 2020  k] = x   ..     
-0001b520: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-0001b530: 7475 726e 2041 6c6c 4564 6765 7356 616c  turn AllEdgesVal
-0001b540: 7565 7320 2020 0d0a 2020 2020 0d0a 2020  ues   ..    ..  
-0001b550: 2020 2020 200d 0a20 2020 200d 0a64 6566       ..    ..def
-0001b560: 2073 6361 6c65 5f76 616c 7565 2878 2c20   scale_value(x, 
-0001b570: 7363 616c 6520 3d20 3235 3520 2a20 3235  scale = 255 * 25
-0001b580: 3529 3a0d 0a0d 0a0d 0a20 2020 2020 7265  5):......     re
-0001b590: 7475 726e 2078 202a 2073 6361 6c65 2020  turn x * scale  
-0001b5a0: 200d 0a20 2020 200d 0a0d 0a0d 0a64 6566   ..    ......def
-0001b5b0: 2070 726f 625f 7369 676d 6f69 6428 7829   prob_sigmoid(x)
-0001b5c0: 3a0d 0a20 2020 2072 6574 7572 6e20 3120  :..    return 1 
-0001b5d0: 2d20 6d61 7468 2e65 7870 282d 7829 0d0a  - math.exp(-x)..
-0001b5e0: 0d0a 0d0a 6465 6620 616e 6775 6c61 725f  ....def angular_
-0001b5f0: 6368 616e 6765 2876 6563 5f30 2c20 7665  change(vec_0, ve
-0001b600: 635f 3129 3a0d 0a20 2020 2020 2020 200d  c_1):..        .
-0001b610: 0a20 2020 2020 2020 2076 6563 5f30 203d  .        vec_0 =
-0001b620: 2076 6563 5f30 202f 206e 702e 6c69 6e61   vec_0 / np.lina
-0001b630: 6c67 2e6e 6f72 6d28 7665 635f 3029 0d0a  lg.norm(vec_0)..
-0001b640: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
-0001b650: 7665 635f 3120 2f20 6e70 2e6c 696e 616c  vec_1 / np.linal
-0001b660: 672e 6e6f 726d 2876 6563 5f31 290d 0a20  g.norm(vec_1).. 
-0001b670: 2020 2020 2020 2061 6e67 6c65 203d 206e         angle = n
-0001b680: 702e 6172 6363 6f73 286e 702e 636c 6970  p.arccos(np.clip
-0001b690: 286e 702e 646f 7428 7665 635f 302c 2076  (np.dot(vec_0, v
-0001b6a0: 6563 5f31 292c 202d 312e 302c 2031 2e30  ec_1), -1.0, 1.0
-0001b6b0: 2929 0d0a 2020 2020 2020 2020 616e 676c  ))..        angl
-0001b6c0: 6520 3d20 616e 676c 6520 2a20 3138 3020  e = angle * 180 
-0001b6d0: 2f20 6e70 2e70 690d 0a20 2020 2020 2020  / np.pi..       
-0001b6e0: 2072 6574 7572 6e20 616e 676c 650d 0a20   return angle.. 
-0001b6f0: 2020 2020 0d0a 0d0a 6465 6620 6576 616c      ....def eval
-0001b700: 5f62 6f6f 6c28 7661 6c75 6529 3a0d 0a20  _bool(value):.. 
-0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b720: 200d 0a20 2020 2020 2020 2069 6620 7661   ..        if va
-0001b730: 6c75 6520 203d 3d20 2754 7275 6527 3a20  lue  == 'True': 
-0001b740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b750: 2020 6469 765f 6b65 7920 3d20 5472 7565    div_key = True
-0001b760: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-0001b770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b780: 2064 6976 5f6b 6579 203d 2046 616c 7365   div_key = False
-0001b790: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
-0001b7a0: 7572 6e20 6469 765f 6b65 7920 2020 2020  urn div_key     
-0001b7b0: 2020 2020 2020 2020 2020 200d 0a0d 0a64             ....d
-0001b7c0: 6566 2063 6865 636b 5f61 6e64 5f75 7064  ef check_and_upd
-0001b7d0: 6174 655f 6d61 736b 286d 6173 6b2c 696d  ate_mask(mask,im
-0001b7e0: 6167 6529 3a0d 0a20 2020 2020 2020 0d0a  age):..       ..
-0001b7f0: 2020 2020 2020 2020 6966 206c 656e 286d          if len(m
-0001b800: 6173 6b2e 7368 6170 6529 203c 206c 656e  ask.shape) < len
-0001b810: 2869 6d61 6765 2e73 6861 7065 293a 0d0a  (image.shape):..
-0001b820: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-0001b830: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
-0001b840: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
-0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b860: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-0001b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b880: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
-0001b890: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
-0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8b0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001b8c0: 5b31 5d2c 0d0a 2020 2020 2020 2020 2020  [1],..          
-0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8e0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001b8f0: 655b 325d 2c0d 0a20 2020 2020 2020 2020  e[2],..         
-0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001b920: 7065 5b33 5d2c 0d0a 2020 2020 2020 2020  pe[3],..        
-0001b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b940: 2020 2020 5d2c 2064 7479 7065 3d22 7569      ], dtype="ui
-0001b950: 6e74 3822 0d0a 2020 2020 2020 2020 2020  nt8"..          
-0001b960: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-0001b970: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0001b980: 2069 2069 6e20 7261 6e67 6528 302c 2075   i in range(0, u
-0001b990: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
-0001b9a0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
-0001b9b0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0001b9c0: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
-0001b9d0: 6d61 736b 2e73 6861 7065 5b31 5d29 3a0d  mask.shape[1]):.
-0001b9e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001b9f0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001ba00: 736b 5b69 2c20 6a2c 203a 2c20 3a5d 203d  sk[i, j, :, :] =
-0001ba10: 206d 6173 6b5b 692c 203a 2c20 3a5d 0d0a   mask[i, :, :]..
-0001ba20: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0001ba30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001ba40: 7064 6174 655f 6d61 736b 203d 206d 6173  pdate_mask = mas
-0001ba50: 6b0d 0a0d 0a20 2020 2020 2020 2072 6574  k....        ret
-0001ba60: 7572 6e20 7570 6461 7465 5f6d 6173 6b20  urn update_mask 
-0001ba70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001ba80: 0d0a                                     ..
+00019980: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00019990: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
+000199a0: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f78  .mean(all_disp_x
+000199b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000199c0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+000199d0: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
+000199e0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+000199f0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00019a00: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00019a10: 6c74 6572 6564 5f76 616c 7565 7320 3d20  ltered_values = 
+00019a20: 5b76 616c 2066 6f72 2076 616c 2069 6e20  [val for val in 
+00019a30: 616c 6c5f 7261 6469 7573 2069 6620 7661  all_radius if va
+00019a40: 6c20 6973 206e 6f74 204e 6f6e 655d 0d0a  l is not None]..
+00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a60: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00019a70: 6e5f 7261 6469 7573 2e61 7070 656e 6428  n_radius.append(
+00019a80: 6e70 2e6d 6561 6e28 6669 6c74 6572 6564  np.mean(filtered
+00019a90: 5f76 616c 7565 7329 290d 0a20 2020 2020  _values))..     
+00019aa0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00019ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ac0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00019ad0: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
+00019ae0: 6e70 2e73 7464 2866 696c 7465 7265 645f  np.std(filtered_
+00019af0: 7661 6c75 6573 2929 0d0a 0d0a 2020 2020  values))....    
+00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b10: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7370  self.all_mean_sp
+00019b20: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
+00019b30: 616e 2861 6c6c 5f73 7065 6564 2929 0d0a  an(all_speed))..
+00019b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b50: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00019b60: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00019b70: 2e73 7464 2861 6c6c 5f73 7065 6564 2929  .std(all_speed))
+00019b80: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019b90: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00019ba0: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
+00019bb0: 286e 702e 6d65 616e 2861 6c6c 5f61 6363  (np.mean(all_acc
+00019bc0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00019bd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00019be0: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
+00019bf0: 6e70 2e73 7464 2861 6c6c 5f61 6363 2929  np.std(all_acc))
+00019c00: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+00019c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019c20: 2e61 6c6c 5f6d 6561 6e5f 6469 7265 6374  .all_mean_direct
+00019c30: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+00019c40: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
+00019c50: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00019c60: 6765 2929 0d0a 2020 2020 2020 2020 2020  ge))..          
+00019c70: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00019c80: 6c6c 5f76 6172 5f64 6972 6563 7469 6f6e  ll_var_direction
+00019c90: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+00019ca0: 286e 702e 7374 6428 616c 6c5f 6469 7265  (np.std(all_dire
+00019cb0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+00019cc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019cd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00019ce0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+00019cf0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00019d00: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7374  np.mean(all_dist
+00019d10: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+00019d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019d30: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00019d40: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00019d50: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+00019d60: 7374 6428 616c 6c5f 6469 7374 616e 6365  std(all_distance
+00019d70: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019da0: 2020 2020 0d0a 6465 6620 626f 756e 6461      ..def bounda
+00019db0: 7279 5f70 6f69 6e74 7328 6d61 736b 2c20  ry_points(mask, 
+00019dc0: 7863 616c 6962 7261 7469 6f6e 2c20 7963  xcalibration, yc
+00019dd0: 616c 6962 7261 7469 6f6e 2c20 7a63 616c  alibration, zcal
+00019de0: 6962 7261 7469 6f6e 293a 0d0a 0d0a 2020  ibration):....  
+00019df0: 2020 6e64 696d 203d 206c 656e 286d 6173    ndim = len(mas
+00019e00: 6b2e 7368 6170 6529 0d0a 2020 2020 7469  k.shape)..    ti
+00019e10: 6d65 645f 6d61 736b 203d 207b 7d0d 0a20  med_mask = {}.. 
+00019e20: 2020 206d 6173 6b20 3d20 6d61 736b 203e     mask = mask >
+00019e30: 2030 0d0a 2020 2020 6d61 736b 203d 206d   0..    mask = m
+00019e40: 6173 6b2e 6173 7479 7065 2827 7569 6e74  ask.astype('uint
+00019e50: 3827 290d 0a20 2020 2023 2059 5820 7368  8')..    # YX sh
+00019e60: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
+00019e70: 2069 6620 6e64 696d 203d 3d20 323a 0d0a   if ndim == 2:..
+00019e80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00019e90: 2020 626f 756e 6461 7279 203d 2066 696e    boundary = fin
+00019ea0: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+00019eb0: 6b29 0d0a 2020 2020 2020 2020 7265 6769  k)..        regi
+00019ec0: 6f6e 6365 6e74 726f 6964 203d 2028 302c  oncentroid = (0,
+00019ed0: 2920 2b20 636f 6d70 7574 655f 6365 6e74  ) + compute_cent
+00019ee0: 726f 6964 2862 6f75 6e64 6172 7929 200d  roid(boundary) .
+00019ef0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
+00019f00: 203d 206e 702e 7768 6572 6528 626f 756e   = np.where(boun
+00019f10: 6461 7279 203e 2030 290d 0a20 2020 2020  dary > 0)..     
+00019f20: 2020 2072 6561 6c5f 696e 6469 6365 7320     real_indices 
+00019f30: 3d20 6e70 2e74 7261 6e73 706f 7365 286e  = np.transpose(n
+00019f40: 702e 6173 6172 7261 7928 696e 6469 6365  p.asarray(indice
+00019f50: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
+00019f60: 7433 3229 292e 636f 7079 2829 0d0a 0d0a  t32)).copy()....
+00019f70: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00019f80: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
+00019f90: 616c 5f69 6e64 6963 6573 2929 3a0d 0a0d  al_indices)):...
+00019fa0: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00019fb0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00019fc0: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019fd0: 5d5b 305d 202a 2079 6361 6c69 6272 6174  ][0] * ycalibrat
+00019fe0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00019ff0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001a000: 5b31 5d20 3d20 7265 616c 5f69 6e64 6963  [1] = real_indic
+0001a010: 6573 5b6a 5d5b 315d 202a 2078 6361 6c69  es[j][1] * xcali
+0001a020: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
+0001a030: 2020 2074 7265 6520 3d20 7370 6174 6961     tree = spatia
+0001a040: 6c2e 634b 4454 7265 6528 7265 616c 5f69  l.cKDTree(real_i
+0001a050: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
+0001a060: 2023 2054 6869 7320 6f62 6a65 6374 2063   # This object c
+0001a070: 6f6e 7461 696e 7320 6c69 7374 206f 6620  ontains list of 
+0001a080: 616c 6c20 7468 6520 706f 696e 7473 2066  all the points f
+0001a090: 6f72 2061 6c6c 2074 6865 206c 6162 656c  or all the label
+0001a0a0: 7320 696e 2074 6865 204d 6173 6b20 696d  s in the Mask im
+0001a0b0: 6167 6520 7769 7468 2074 6865 206c 6162  age with the lab
+0001a0c0: 656c 2069 6420 616e 6420 766f 6c75 6d65  el id and volume
+0001a0d0: 206f 6620 6561 6368 206c 6162 656c 0d0a   of each label..
+0001a0e0: 2020 2020 2020 2020 7469 6d65 645f 6d61          timed_ma
+0001a0f0: 736b 5b73 7472 2830 295d 203d 205b 7472  sk[str(0)] = [tr
+0001a100: 6565 2c20 696e 6469 6365 732c 2072 6567  ee, indices, reg
+0001a110: 696f 6e63 656e 7472 6f69 645d 0d0a 0d0a  ioncentroid]....
+0001a120: 2020 2020 2320 5459 5820 7368 6170 6564      # TYX shaped
+0001a130: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
+0001a140: 6e64 696d 203d 3d20 333a 0d0a 0d0a 0d0a  ndim == 3:......
+0001a150: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0001a160: 2074 7164 6d28 7261 6e67 6528 302c 206d   tqdm(range(0, m
+0001a170: 6173 6b2e 7368 6170 655b 305d 2929 3a0d  ask.shape[0])):.
+0001a180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a190: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001a1a0: 2020 2062 6f75 6e64 6172 7920 3d20 6669     boundary = fi
+0001a1b0: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
+0001a1c0: 736b 5b69 2c3a 5d29 0d0a 2020 2020 2020  sk[i,:])..      
+0001a1d0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
+0001a1e0: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
+0001a1f0: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
+0001a200: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a220: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
+0001a230: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
+0001a240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a250: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
+0001a260: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
+0001a270: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
+0001a280: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+0001a290: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
+0001a2a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001a2b0: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
+0001a2c0: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
+0001a2d0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
+0001a2e0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+0001a2f0: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
+0001a300: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+0001a310: 305d 202a 2079 6361 6c69 6272 6174 696f  0] * ycalibratio
+0001a320: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+0001a330: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+0001a340: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
+0001a350: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
+0001a360: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
+0001a370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a380: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
+0001a390: 634b 4454 7265 6528 7265 616c 5f69 6e64  cKDTree(real_ind
+0001a3a0: 6963 6573 290d 0a0d 0a20 2020 2020 2020  ices)....       
+0001a3b0: 2020 2020 2020 2020 2074 696d 6564 5f6d           timed_m
+0001a3c0: 6173 6b5b 7374 7228 6929 5d20 3d20 5b74  ask[str(i)] = [t
+0001a3d0: 7265 652c 2069 6e64 6963 6573 2c20 7265  ree, indices, re
+0001a3e0: 6769 6f6e 6365 6e74 726f 6964 5d0d 0a20  gioncentroid].. 
+0001a3f0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001a400: 2023 2054 5a59 5820 7368 6170 6564 206f   # TZYX shaped o
+0001a410: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
+0001a420: 696d 203d 3d20 343a 0d0a 2020 2020 2020  im == 4:..      
+0001a430: 2020 7072 696e 7428 274d 616b 696e 6720    print('Making 
+0001a440: 6d61 736b 2069 6e20 3444 2729 0d0a 2020  mask in 4D')..  
+0001a450: 2020 2020 2020 626f 756e 6461 7279 203d        boundary =
+0001a460: 206e 702e 7a65 726f 7328 0d0a 2020 2020   np.zeros(..    
+0001a470: 2020 2020 2020 2020 5b6d 6173 6b2e 7368          [mask.sh
+0001a480: 6170 655b 305d 2c20 6d61 736b 2e73 6861  ape[0], mask.sha
+0001a490: 7065 5b31 5d2c 206d 6173 6b2e 7368 6170  pe[1], mask.shap
+0001a4a0: 655b 325d 2c20 6d61 736b 2e73 6861 7065  e[2], mask.shape
+0001a4b0: 5b33 5d5d 2c20 6474 7970 653d 6e70 2e75  [3]], dtype=np.u
+0001a4c0: 696e 7438 0d0a 2020 2020 2020 2020 290d  int8..        ).
+0001a4d0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0001a4e0: 6e20 7261 6e67 6528 302c 206d 6173 6b2e  n range(0, mask.
+0001a4f0: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
+0001a500: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a510: 2020 2020 2020 626f 756e 6461 7279 5b69        boundary[i
+0001a520: 2c3a 5d20 3d20 6669 6e64 5f62 6f75 6e64  ,:] = find_bound
+0001a530: 6172 6965 7328 6d61 736b 5b69 2c3a 5d29  aries(mask[i,:])
+0001a540: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001a550: 6769 6f6e 6365 6e74 726f 6964 203d 2063  gioncentroid = c
+0001a560: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+0001a570: 626f 756e 6461 7279 5b69 2c3a 5d29 200d  boundary[i,:]) .
+0001a580: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+0001a590: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
+0001a5a0: 626f 756e 6461 7279 5b69 2c3a 5d20 3e20  boundary[i,:] > 
+0001a5b0: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+0001a5c0: 7265 616c 5f69 6e64 6963 6573 203d 206e  real_indices = n
+0001a5d0: 702e 7472 616e 7370 6f73 6528 6e70 2e61  p.transpose(np.a
+0001a5e0: 7361 7272 6179 2869 6e64 6963 6573 2c20  sarray(indices, 
+0001a5f0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+0001a600: 2929 2e63 6f70 7928 290d 0a0d 0a20 2020  )).copy()....   
+0001a610: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0001a620: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+0001a630: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+0001a640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a650: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+0001a660: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
+0001a670: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
+0001a680: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+0001a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6a0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+0001a6b0: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+0001a6c0: 6365 735b 6a5d 5b31 5d20 2a20 7963 616c  ces[j][1] * ycal
+0001a6d0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001a6f0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+0001a700: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+0001a710: 6a5d 5b32 5d20 2a20 7863 616c 6962 7261  j][2] * xcalibra
+0001a720: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+0001a730: 2020 2020 7472 6565 203d 2073 7061 7469      tree = spati
+0001a740: 616c 2e63 4b44 5472 6565 2872 6561 6c5f  al.cKDTree(real_
+0001a750: 696e 6469 6365 7329 0d0a 2020 2020 2020  indices)..      
+0001a760: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
+0001a770: 5b73 7472 2869 295d 203d 205b 7472 6565  [str(i)] = [tree
+0001a780: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
+0001a790: 6e63 656e 7472 6f69 645d 0d0a 2020 2020  ncentroid]..    
+0001a7a0: 7072 696e 7428 2743 6f6d 7075 7465 6420  print('Computed 
+0001a7b0: 7468 6520 626f 756e 6461 7279 2070 6f69  the boundary poi
+0001a7c0: 6e74 7327 290d 0a0d 0a20 2020 2072 6574  nts')....    ret
+0001a7d0: 7572 6e20 7469 6d65 645f 6d61 736b 2c20  urn timed_mask, 
+0001a7e0: 626f 756e 6461 7279 2020 2020 2020 2020  boundary        
+0001a7f0: 0d0a 0d0a 6465 6620 636f 6d70 7574 655f  ....def compute_
+0001a800: 6365 6e74 726f 6964 2862 696e 6172 795f  centroid(binary_
+0001a810: 696d 6167 6529 3a0d 0a20 2020 2023 2045  image):..    # E
+0001a820: 6e73 7572 6520 6269 6e61 7279 2069 6d61  nsure binary ima
+0001a830: 6765 2069 7320 6120 4e75 6d50 7920 6172  ge is a NumPy ar
+0001a840: 7261 790d 0a20 2020 2062 696e 6172 795f  ray..    binary_
+0001a850: 696d 6167 6520 3d20 6e70 2e61 7272 6179  image = np.array
+0001a860: 2862 696e 6172 795f 696d 6167 6529 0d0a  (binary_image)..
+0001a870: 0d0a 2020 2020 7768 6974 655f 7069 7865  ..    white_pixe
+0001a880: 6c73 203d 206e 702e 7768 6572 6528 6269  ls = np.where(bi
+0001a890: 6e61 7279 5f69 6d61 6765 203d 3d20 3129  nary_image == 1)
+0001a8a0: 0d0a 2020 2020 6e75 6d5f 7069 7865 6c73  ..    num_pixels
+0001a8b0: 203d 206c 656e 2877 6869 7465 5f70 6978   = len(white_pix
+0001a8c0: 656c 735b 305d 290d 0a0d 0a20 2020 2023  els[0])....    #
+0001a8d0: 2043 6f6d 7075 7465 2074 6865 2063 656e   Compute the cen
+0001a8e0: 7472 6f69 6420 6f66 2074 6865 2077 6869  troid of the whi
+0001a8f0: 7465 2070 6978 656c 7320 696e 2074 6865  te pixels in the
+0001a900: 2062 6f75 6e64 6172 7920 696d 6167 650d   boundary image.
+0001a910: 0a20 2020 2063 656e 7472 6f69 6420 3d20  .    centroid = 
+0001a920: 6e70 2e7a 6572 6f73 2862 696e 6172 795f  np.zeros(binary_
+0001a930: 696d 6167 652e 6e64 696d 290d 0a20 2020  image.ndim)..   
+0001a940: 2066 6f72 2064 696d 2069 6e20 7261 6e67   for dim in rang
+0001a950: 6528 6269 6e61 7279 5f69 6d61 6765 2e6e  e(binary_image.n
+0001a960: 6469 6d29 3a0d 0a20 2020 2020 2020 2063  dim):..        c
+0001a970: 656e 7472 6f69 645b 6469 6d5d 203d 2077  entroid[dim] = w
+0001a980: 6869 7465 5f70 6978 656c 735b 6469 6d5d  hite_pixels[dim]
+0001a990: 2e73 756d 2829 202f 206e 756d 5f70 6978  .sum() / num_pix
+0001a9a0: 656c 730d 0a0d 0a20 2020 2072 6574 7572  els....    retur
+0001a9b0: 6e20 6365 6e74 726f 6964 0d0a 0d0a 0d0a  n centroid......
+0001a9c0: 0d0a 200d 0a0d 0a64 6566 2067 6574 5f63  .. ....def get_c
+0001a9d0: 7376 5f64 6174 6128 6373 7629 3a0d 0a0d  sv_data(csv):...
+0001a9e0: 0a20 2020 2020 2020 2064 6174 6173 6574  .        dataset
+0001a9f0: 203d 2070 642e 7265 6164 5f63 7376 280d   = pd.read_csv(.
+0001aa00: 0a20 2020 2020 2020 2020 2020 2063 7376  .            csv
+0001aa10: 2c20 6465 6c69 6d69 7465 723d 222c 222c  , delimiter=",",
+0001aa20: 2065 6e63 6f64 696e 673d 2275 6e69 636f   encoding="unico
+0001aa30: 6465 5f65 7363 6170 6522 2c20 6c6f 775f  de_escape", low_
+0001aa40: 6d65 6d6f 7279 3d46 616c 7365 0d0a 2020  memory=False..  
+0001aa50: 2020 2020 2020 295b 333a 5d0d 0a20 2020        )[3:]..   
+0001aa60: 2020 2020 2064 6174 6173 6574 5f69 6e64       dataset_ind
+0001aa70: 6578 203d 2064 6174 6173 6574 2e69 6e64  ex = dataset.ind
+0001aa80: 6578 0d0a 2020 2020 2020 2020 7265 7475  ex..        retu
+0001aa90: 726e 2064 6174 6173 6574 2c20 6461 7461  rn dataset, data
+0001aaa0: 7365 745f 696e 6465 780d 0a20 2020 200d  set_index..    .
+0001aab0: 0a64 6566 2067 6574 5f73 706f 745f 6461  .def get_spot_da
+0001aac0: 7461 7365 7428 7370 6f74 5f64 6174 6173  taset(spot_datas
+0001aad0: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
+0001aae0: 6973 5f73 706f 745f 6b65 7973 2c20 7863  is_spot_keys, xc
+0001aaf0: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
+0001ab00: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
+0001ab10: 7261 7469 6f6e 2c20 4174 7472 6962 7574  ration, Attribut
+0001ab20: 6542 6f78 6e61 6d65 2c20 6465 7465 6374  eBoxname, detect
+0001ab30: 696f 6e63 6861 6e6e 656c 293a 0d0a 2020  ionchannel):..  
+0001ab40: 2020 2020 2020 416c 6c56 616c 7565 7320        AllValues 
+0001ab50: 3d20 7b7d 0d0a 2020 2020 2020 2020 706f  = {}..        po
+0001ab60: 7369 7820 3d20 7472 6163 6b5f 616e 616c  six = track_anal
+0001ab70: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001ab80: 706f 7369 7822 5d0d 0a20 2020 2020 2020  posix"]..       
+0001ab90: 2070 6f73 6979 203d 2074 7261 636b 5f61   posiy = track_a
+0001aba0: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001abb0: 735b 2270 6f73 6979 225d 0d0a 2020 2020  s["posiy"]..    
+0001abc0: 2020 2020 706f 7369 7a20 3d20 7472 6163      posiz = trac
+0001abd0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001abe0: 6b65 7973 5b22 706f 7369 7a22 5d0d 0a20  keys["posiz"].. 
+0001abf0: 2020 2020 2020 2066 7261 6d65 203d 2074         frame = t
+0001ac00: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001ac10: 6f74 5f6b 6579 735b 2266 7261 6d65 225d  ot_keys["frame"]
+0001ac20: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0001ac30: 2020 2020 4c6f 6361 7469 6f6e 5820 3d20      LocationX = 
+0001ac40: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+0001ac50: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+0001ac60: 785d 2e61 7374 7970 6528 2266 6c6f 6174  x].astype("float
+0001ac70: 2229 202f 2078 6361 6c69 6272 6174 696f  ") / xcalibratio
+0001ac80: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+0001ac90: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001aca0: 2020 2020 4c6f 6361 7469 6f6e 5920 3d20      LocationY = 
+0001acb0: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+0001acc0: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+0001acd0: 795d 2e61 7374 7970 6528 2266 6c6f 6174  y].astype("float
+0001ace0: 2229 202f 2079 6361 6c69 6272 6174 696f  ") / ycalibratio
+0001acf0: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+0001ad00: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001ad10: 2020 2020 4c6f 6361 7469 6f6e 5a20 3d20      LocationZ = 
+0001ad20: 280d 0a20 2020 2020 2020 2020 2020 2073  (..            s
+0001ad30: 706f 745f 6461 7461 7365 745b 706f 7369  pot_dataset[posi
+0001ad40: 7a5d 2e61 7374 7970 6528 2266 6c6f 6174  z].astype("float
+0001ad50: 2229 202f 207a 6361 6c69 6272 6174 696f  ") / zcalibratio
+0001ad60: 6e0d 0a20 2020 2020 2020 2029 2e61 7374  n..        ).ast
+0001ad70: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001ad80: 2020 2020 4c6f 6361 7469 6f6e 5420 3d20      LocationT = 
+0001ad90: 2873 706f 745f 6461 7461 7365 745b 6672  (spot_dataset[fr
+0001ada0: 616d 655d 2e61 7374 7970 6528 2266 6c6f  ame].astype("flo
+0001adb0: 6174 2229 292e 6173 7479 7065 2822 696e  at")).astype("in
+0001adc0: 7422 290d 0a20 2020 2020 2020 200d 0a0d  t")..        ...
+0001add0: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
+0001ade0: 7661 6c75 6573 203d 205b 7472 6163 6b5f  values = [track_
+0001adf0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001ae00: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
+0001ae10: 7479 225d 2c74 7261 636b 5f61 6e61 6c79  ty"],track_analy
+0001ae20: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
+0001ae30: 6f74 616c 5f69 6e74 656e 7369 7479 225d  otal_intensity"]
+0001ae40: 5d0d 0a20 2020 2020 2020 2066 6f72 2028  ]..        for (
+0001ae50: 6b2c 7629 2069 6e20 7472 6163 6b5f 616e  k,v) in track_an
+0001ae60: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001ae70: 2e69 7465 6d73 2829 3a0d 0a0d 0a20 2020  .items():....   
+0001ae80: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001ae90: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
+0001aea0: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+0001aeb0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001aec0: 6b20 3d3d 2022 6d65 616e 5f69 6e74 656e  k == "mean_inten
+0001aed0: 7369 7479 5f63 6832 223a 0d0a 2020 2020  sity_ch2":..    
+0001aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aef0: 2020 2020 2020 2076 616c 7565 203d 2074         value = t
+0001af00: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001af10: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
+0001af20: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
+0001af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af40: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001af50: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
+0001af60: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001af70: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001af80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001af90: 6620 6b20 3d3d 2022 746f 7461 6c5f 696e  f k == "total_in
+0001afa0: 7465 6e73 6974 795f 6368 3222 3a0d 0a20  tensity_ch2":.. 
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afc0: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+0001afd0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001afe0: 5f73 706f 745f 6b65 7973 5b22 746f 7461  _spot_keys["tota
+0001aff0: 6c5f 696e 7465 6e73 6974 7922 5d0d 0a20  l_intensity"].. 
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b010: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
+0001b020: 7565 735b 7661 6c75 655d 203d 2073 706f  ues[value] = spo
+0001b030: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
+0001b040: 7970 6528 2266 6c6f 6174 2229 2020 2020  ype("float")    
+0001b050: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+0001b060: 2020 2020 2020 2069 6620 7620 6e6f 7420         if v not 
+0001b070: 696e 2069 676e 6f72 655f 7661 6c75 6573  in ignore_values
+0001b080: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001b090: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0b0: 2020 2041 6c6c 5661 6c75 6573 5b76 5d20     AllValues[v] 
+0001b0c0: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
+0001b0d0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001b0e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b0f0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+0001b100: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
+0001b110: 785d 203d 2072 6f75 6e64 284c 6f63 6174  x] = round(Locat
+0001b120: 696f 6e58 2c33 290d 0a20 2020 2020 2020  ionX,3)..       
+0001b130: 2041 6c6c 5661 6c75 6573 5b70 6f73 6979   AllValues[posiy
+0001b140: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
+0001b150: 6f6e 592c 3329 0d0a 2020 2020 2020 2020  onY,3)..        
+0001b160: 416c 6c56 616c 7565 735b 706f 7369 7a5d  AllValues[posiz]
+0001b170: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+0001b180: 6e5a 2c33 290d 0a20 2020 2020 2020 2041  nZ,3)..        A
+0001b190: 6c6c 5661 6c75 6573 5b66 7261 6d65 5d20  llValues[frame] 
+0001b1a0: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
+0001b1b0: 542c 3329 0d0a 2020 2020 2020 2020 4174  T,3)..        At
+0001b1c0: 7472 6962 7574 6569 6473 203d 205b 5d0d  tributeids = [].
+0001b1d0: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+0001b1e0: 7465 6964 732e 6170 7065 6e64 2841 7474  teids.append(Att
+0001b1f0: 7269 6275 7465 426f 786e 616d 6529 0d0a  ributeBoxname)..
+0001b200: 2020 2020 2020 2020 666f 7220 6174 7472          for attr
+0001b210: 6962 7574 656e 616d 6520 696e 2041 6c6c  ibutename in All
+0001b220: 5661 6c75 6573 2e6b 6579 7328 293a 0d0a  Values.keys():..
+0001b230: 2020 2020 2020 2020 2020 2020 2020 4174                At
+0001b240: 7472 6962 7574 6569 6473 2e61 7070 656e  tributeids.appen
+0001b250: 6428 6174 7472 6962 7574 656e 616d 6529  d(attributename)
+0001b260: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0001b270: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+0001b280: 2020 2020 2020 7265 7475 726e 2041 7474        return Att
+0001b290: 7269 6275 7465 6964 732c 2041 6c6c 5661  ributeids, AllVa
+0001b2a0: 6c75 6573 2020 2020 200d 0a20 2020 200d  lues     ..    .
+0001b2b0: 0a64 6566 2067 6574 5f74 7261 636b 5f64  .def get_track_d
+0001b2c0: 6174 6173 6574 2874 7261 636b 5f64 6174  ataset(track_dat
+0001b2d0: 6173 6574 2c20 7472 6163 6b5f 616e 616c  aset, track_anal
+0001b2e0: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+0001b2f0: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
+0001b300: 7261 636b 5f6b 6579 732c 2054 7261 636b  rack_keys, Track
+0001b310: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+0001b320: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
+0001b330: 6c54 7261 636b 5661 6c75 6573 203d 207b  lTrackValues = {
+0001b340: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
+0001b350: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
+0001b360: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001b370: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
+0001b380: 2020 2020 5469 6420 3d20 7472 6163 6b5f      Tid = track_
+0001b390: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
+0001b3a0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001b3b0: 290d 0a20 2020 2020 2020 0d0a 2020 2020  )..       ..    
+0001b3c0: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
+0001b3d0: 6573 5b74 7261 636b 5f69 645d 203d 2054  es[track_id] = T
+0001b3e0: 6964 0d0a 2020 2020 2020 0d0a 2020 2020  id..      ..    
+0001b3f0: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
+0001b400: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001b410: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
+0001b420: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001b430: 2020 2020 2020 2020 7820 3d20 7472 6163          x = trac
+0001b440: 6b5f 6461 7461 7365 745b 765d 2e61 7374  k_dataset[v].ast
+0001b450: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001b460: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+0001b470: 6e76 616c 203d 206d 696e 2878 290d 0a20  nval = min(x).. 
+0001b480: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001b490: 6178 7661 6c20 3d20 6d61 7828 7829 0d0a  axval = max(x)..
+0001b4a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b4b0: 2020 6966 206d 696e 7661 6c20 3e20 3020    if minval > 0 
+0001b4c0: 616e 6420 6d61 7876 616c 203c 3d20 313a  and maxval <= 1:
+0001b4d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001b4e0: 2020 2020 2020 2020 7820 3d20 7820 2b20          x = x + 
+0001b4f0: 310d 0a0d 0a20 2020 2020 2020 2020 2020  1....           
+0001b500: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
+0001b510: 7565 735b 6b5d 203d 2072 6f75 6e64 2878  ues[k] = round(x
+0001b520: 2c20 3329 0d0a 0d0a 2020 2020 2020 2020  , 3)....        
+0001b530: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001b540: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001b550: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
+0001b560: 732e 6170 7065 6e64 2854 7261 636b 4174  s.append(TrackAt
+0001b570: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
+0001b580: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
+0001b590: 7269 6275 7465 6e61 6d65 2069 6e20 7472  ributename in tr
+0001b5a0: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+0001b5b0: 636b 5f6b 6579 732e 6b65 7973 2829 3a0d  ck_keys.keys():.
+0001b5c0: 0a20 2020 2020 2020 2020 2020 2054 7261  .            Tra
+0001b5d0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
+0001b5e0: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
+0001b5f0: 616d 6529 2020 2020 0d0a 2020 2020 0d0a  ame)    ..    ..
+0001b600: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0001b610: 7261 636b 4174 7472 6962 7574 6569 6473  rackAttributeids
+0001b620: 2c20 416c 6c54 7261 636b 5661 6c75 6573  , AllTrackValues
+0001b630: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001b640: 6564 6765 735f 6461 7461 7365 7428 6564  edges_dataset(ed
+0001b650: 6765 735f 6461 7461 7365 742c 2065 6467  ges_dataset, edg
+0001b660: 6573 5f64 6174 6173 6574 5f69 6e64 6578  es_dataset_index
+0001b670: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001b680: 5f73 706f 745f 6b65 7973 2c20 7472 6163  _spot_keys, trac
+0001b690: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
+0001b6a0: 5f6b 6579 7329 3a0d 0a0d 0a20 2020 2020  _keys):....     
+0001b6b0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001b6c0: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+0001b6d0: 7472 6163 6b5f 6964 203d 2074 7261 636b  track_id = track
+0001b6e0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001b6f0: 6579 735b 2274 7261 636b 5f69 6422 5d0d  eys["track_id"].
+0001b700: 0a20 2020 2020 2020 2054 6964 203d 2065  .        Tid = e
+0001b710: 6467 6573 5f64 6174 6173 6574 5b74 7261  dges_dataset[tra
+0001b720: 636b 5f69 645d 2e61 7374 7970 6528 2266  ck_id].astype("f
+0001b730: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
+0001b740: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+0001b750: 7265 2854 6964 203d 3d20 3029 0d0a 2020  re(Tid == 0)..  
+0001b760: 2020 2020 2020 6d61 7874 7261 636b 5f69        maxtrack_i
+0001b770: 6420 3d20 6d61 7828 5469 6429 0d0a 2020  d = max(Tid)..  
+0001b780: 2020 2020 2020 636f 6e64 6974 696f 6e5f        condition_
+0001b790: 696e 6469 6365 7320 3d20 6564 6765 735f  indices = edges_
+0001b7a0: 6461 7461 7365 745f 696e 6465 785b 696e  dataset_index[in
+0001b7b0: 6469 6365 735d 0d0a 2020 2020 2020 2020  dices]..        
+0001b7c0: 5469 645b 636f 6e64 6974 696f 6e5f 696e  Tid[condition_in
+0001b7d0: 6469 6365 735d 203d 206d 6178 7472 6163  dices] = maxtrac
+0001b7e0: 6b5f 6964 202b 2031 0d0a 2020 2020 2020  k_id + 1..      
+0001b7f0: 2020 416c 6c45 6467 6573 5661 6c75 6573    AllEdgesValues
+0001b800: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
+0001b810: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+0001b820: 6b20 696e 2074 7261 636b 5f61 6e61 6c79  k in track_analy
+0001b830: 7369 735f 6564 6765 735f 6b65 7973 2e76  sis_edges_keys.v
+0001b840: 616c 7565 7328 293a 0d0a 0d0a 2020 2020  alues():....    
+0001b850: 2020 2020 2020 2020 6966 206b 2021 3d20          if k != 
+0001b860: 7472 6163 6b5f 6964 3a0d 0a20 2020 2020  track_id:..     
+0001b870: 2020 2020 2020 2020 2020 2078 203d 2065             x = e
+0001b880: 6467 6573 5f64 6174 6173 6574 5b6b 5d2e  dges_dataset[k].
+0001b890: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001b8a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b8b0: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
+0001b8c0: 735b 6b5d 203d 2078 2020 200d 0a20 2020  s[k] = x   ..   
+0001b8d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001b8e0: 7265 7475 726e 2041 6c6c 4564 6765 7356  return AllEdgesV
+0001b8f0: 616c 7565 7320 2020 0d0a 2020 2020 0d0a  alues   ..    ..
+0001b900: 2020 2020 2020 200d 0a20 2020 200d 0a64         ..    ..d
+0001b910: 6566 2073 6361 6c65 5f76 616c 7565 2878  ef scale_value(x
+0001b920: 2c20 7363 616c 6520 3d20 3235 3520 2a20  , scale = 255 * 
+0001b930: 3235 3529 3a0d 0a0d 0a0d 0a20 2020 2020  255):......     
+0001b940: 7265 7475 726e 2078 202a 2073 6361 6c65  return x * scale
+0001b950: 2020 200d 0a20 2020 200d 0a0d 0a0d 0a64     ..    ......d
+0001b960: 6566 2070 726f 625f 7369 676d 6f69 6428  ef prob_sigmoid(
+0001b970: 7829 3a0d 0a20 2020 2072 6574 7572 6e20  x):..    return 
+0001b980: 3120 2d20 6d61 7468 2e65 7870 282d 7829  1 - math.exp(-x)
+0001b990: 0d0a 0d0a 0d0a 6465 6620 616e 6775 6c61  ......def angula
+0001b9a0: 725f 6368 616e 6765 2876 6563 5f30 2c20  r_change(vec_0, 
+0001b9b0: 7665 635f 3129 3a0d 0a20 2020 2020 2020  vec_1):..       
+0001b9c0: 200d 0a20 2020 2020 2020 2076 6563 5f30   ..        vec_0
+0001b9d0: 203d 2076 6563 5f30 202f 206e 702e 6c69   = vec_0 / np.li
+0001b9e0: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3029  nalg.norm(vec_0)
+0001b9f0: 0d0a 2020 2020 2020 2020 7665 635f 3120  ..        vec_1 
+0001ba00: 3d20 7665 635f 3120 2f20 6e70 2e6c 696e  = vec_1 / np.lin
+0001ba10: 616c 672e 6e6f 726d 2876 6563 5f31 290d  alg.norm(vec_1).
+0001ba20: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+0001ba30: 206e 702e 6172 6363 6f73 286e 702e 636c   np.arccos(np.cl
+0001ba40: 6970 286e 702e 646f 7428 7665 635f 302c  ip(np.dot(vec_0,
+0001ba50: 2076 6563 5f31 292c 202d 312e 302c 2031   vec_1), -1.0, 1
+0001ba60: 2e30 2929 0d0a 2020 2020 2020 2020 616e  .0))..        an
+0001ba70: 676c 6520 3d20 616e 676c 6520 2a20 3138  gle = angle * 18
+0001ba80: 3020 2f20 6e70 2e70 690d 0a20 2020 2020  0 / np.pi..     
+0001ba90: 2020 2072 6574 7572 6e20 616e 676c 650d     return angle.
+0001baa0: 0a20 2020 2020 0d0a 0d0a 6465 6620 6576  .     ....def ev
+0001bab0: 616c 5f62 6f6f 6c28 7661 6c75 6529 3a0d  al_bool(value):.
+0001bac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bad0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001bae0: 7661 6c75 6520 203d 3d20 2754 7275 6527  value  == 'True'
+0001baf0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+0001bb00: 2020 2020 6469 765f 6b65 7920 3d20 5472      div_key = Tr
+0001bb10: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
+0001bb20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001bb30: 2020 2064 6976 5f6b 6579 203d 2046 616c     div_key = Fal
+0001bb40: 7365 200d 0a0d 0a20 2020 2020 2020 2072  se ....        r
+0001bb50: 6574 7572 6e20 6469 765f 6b65 7920 2020  eturn div_key   
+0001bb60: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001bb70: 0a64 6566 2063 6865 636b 5f61 6e64 5f75  .def check_and_u
+0001bb80: 7064 6174 655f 6d61 736b 286d 6173 6b2c  pdate_mask(mask,
+0001bb90: 696d 6167 6529 3a0d 0a20 2020 2020 2020  image):..       
+0001bba0: 0d0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0001bbb0: 286d 6173 6b2e 7368 6170 6529 203c 206c  (mask.shape) < l
+0001bbc0: 656e 2869 6d61 6765 2e73 6861 7065 293a  en(image.shape):
+0001bbd0: 0d0a 2020 2020 2020 2020 2020 2020 7570  ..            up
+0001bbe0: 6461 7465 5f6d 6173 6b20 3d20 6e70 2e7a  date_mask = np.z
+0001bbf0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc10: 2020 205b 0d0a 2020 2020 2020 2020 2020     [..          
+0001bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc30: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001bc40: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
+0001bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc60: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001bc70: 7065 5b31 5d2c 0d0a 2020 2020 2020 2020  pe[1],..        
+0001bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc90: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
+0001bca0: 6170 655b 325d 2c0d 0a20 2020 2020 2020  ape[2],..       
+0001bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcc0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
+0001bcd0: 6861 7065 5b33 5d2c 0d0a 2020 2020 2020  hape[3],..      
+0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcf0: 2020 2020 2020 5d2c 2064 7479 7065 3d22        ], dtype="
+0001bd00: 7569 6e74 3822 0d0a 2020 2020 2020 2020  uint8"..        
+0001bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd20: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+0001bd30: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+0001bd40: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
+0001bd50: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+0001bd60: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+0001bd70: 6e20 7261 6e67 6528 302c 2075 7064 6174  n range(0, updat
+0001bd80: 655f 6d61 736b 2e73 6861 7065 5b31 5d29  e_mask.shape[1])
+0001bd90: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0001bda0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001bdb0: 6d61 736b 5b69 2c20 6a2c 203a 2c20 3a5d  mask[i, j, :, :]
+0001bdc0: 203d 206d 6173 6b5b 692c 203a 2c20 3a5d   = mask[i, :, :]
+0001bdd0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0001bde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bdf0: 2075 7064 6174 655f 6d61 736b 203d 206d   update_mask = m
+0001be00: 6173 6b0d 0a0d 0a20 2020 2020 2020 2072  ask....        r
+0001be10: 6574 7572 6e20 7570 6461 7465 5f6d 6173  eturn update_mas
+0001be20: 6b20 2020 2020 2020 200d 0a20 2020 2020  k        ..     
+0001be30: 2020 0d0a                                  ..
```

### Comparing `napatrackmater-3.8.9/napatrackmater/Trackvector.py` & `napatrackmater-3.9.0/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/__init__.py` & `napatrackmater-3.9.0/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/clustering.py` & `napatrackmater-3.9.0/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.9.0/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/fate_mapping.py` & `napatrackmater-3.9.0/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater/pretrained.py` & `napatrackmater-3.9.0/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.9.0/napatrackmater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.9
+Version: 3.9.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
-Author: Varun Kapoor, Mari Tolonen
+Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `napatrackmater-3.8.9/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.9.0/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.9/setup.py` & `napatrackmater-3.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,72 +18,73 @@
 00000110: 6328 662e 7265 6164 2829 290d 0a73 6574  c(f.read())..set
 00000120: 7570 280d 0a20 2020 206e 616d 653d 226e  up(..    name="n
 00000130: 6170 6174 7261 636b 6d61 7465 7222 2c0d  apatrackmater",.
 00000140: 0a0d 0a20 2020 2076 6572 7369 6f6e 3d5f  ...    version=_
 00000150: 5f76 6572 7369 6f6e 5f5f 2c0d 0a0d 0a20  _version__,.... 
 00000160: 2020 2061 7574 686f 723d 2756 6172 756e     author='Varun
 00000170: 204b 6170 6f6f 722c 204d 6172 6920 546f   Kapoor, Mari To
-00000180: 6c6f 6e65 6e27 2c0d 0a20 2020 2061 7574  lonen',..    aut
-00000190: 686f 725f 656d 6169 6c3d 2772 616e 646f  hor_email='rando
-000001a0: 6d61 6363 6573 7369 626c 656b 6170 6f6f  maccessiblekapoo
-000001b0: 7240 676d 6169 6c2e 636f 6d27 2c0d 0a20  r@gmail.com',.. 
-000001c0: 2020 2075 726c 3d27 6874 7470 733a 2f2f     url='https://
-000001d0: 6769 7468 7562 2e63 6f6d 2f6b 6170 6f6f  github.com/kapoo
-000001e0: 726c 6162 2f4e 6170 6154 7261 636b 4d61  rlab/NapaTrackMa
-000001f0: 7465 722f 272c 0d0a 2020 2020 6465 7363  ter/',..    desc
-00000200: 7269 7074 696f 6e3d 2749 6d70 6f72 7420  ription='Import 
-00000210: 5472 6163 6b6d 6174 6520 584d 4c20 6669  Trackmate XML fi
-00000220: 6c65 7320 666f 7220 5472 6163 6b20 5669  les for Track Vi
-00000230: 7375 616c 697a 6174 696f 6e20 616e 6420  sualization and 
-00000240: 616e 616c 7973 6973 2069 6e20 4e61 7061  analysis in Napa
-00000250: 7269 2e27 2c0d 0a20 2020 206c 6f6e 675f  ri.',..    long_
-00000260: 6465 7363 7269 7074 696f 6e3d 6c6f 6e67  description=long
-00000270: 5f64 6573 6372 6970 7469 6f6e 2c0d 0a20  _description,.. 
-00000280: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
-00000290: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-000002a0: 3d27 7465 7874 2f6d 6172 6b64 6f77 6e27  ='text/markdown'
-000002b0: 2c0d 0a20 2020 2069 6e73 7461 6c6c 5f72  ,..    install_r
-000002c0: 6571 7569 7265 733d 5b0d 0a20 2020 2020  equires=[..     
-000002d0: 2020 2022 6c78 6d6c 222c 0d0a 2020 2020     "lxml",..    
-000002e0: 2020 2020 2276 6f6c 6c73 6567 222c 0d0a      "vollseg",..
-000002f0: 2020 2020 2020 2020 226e 6170 6172 6922          "napari"
-00000300: 2c0d 0a20 2020 2020 2020 2022 6e61 7473  ,..        "nats
-00000310: 6f72 7422 2c0d 0a20 2020 2020 2020 2022  ort",..        "
-00000320: 7365 6162 6f72 6e22 2c0d 0a20 2020 2020  seaborn",..     
-00000330: 2020 2022 6365 6c6c 7368 6170 652d 636c     "cellshape-cl
-00000340: 6f75 6422 2c0d 0a20 2020 2020 2020 2022  oud",..        "
-00000350: 6365 6c6c 7368 6170 652d 6865 6c70 6572  cellshape-helper
-00000360: 222c 0d0a 2020 2020 2020 2020 226b 6170  ",..        "kap
-00000370: 6f6f 726c 6162 732d 6c69 6768 746e 696e  oorlabs-lightnin
-00000380: 6722 2c0d 0a20 2020 2020 2020 2022 6c69  g",..        "li
-00000390: 6768 746e 696e 673e 3d32 2e30 2e34 220d  ghtning>=2.0.4".
-000003a0: 0a20 2020 205d 2c0d 0a20 2020 2065 6e74  .    ],..    ent
-000003b0: 7279 5f70 6f69 6e74 7320 3d20 7b0d 0a20  ry_points = {.. 
-000003c0: 2020 2020 2020 2027 636f 6e73 6f6c 655f         'console_
-000003d0: 7363 7269 7074 7327 3a20 5b0d 0a20 2020  scripts': [..   
-000003e0: 2020 2020 2020 2020 2027 7472 6163 6b20           'track 
-000003f0: 3d20 6e61 7061 7472 6163 6b6d 6174 6572  = napatrackmater
-00000400: 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e 272c  .__main__:main',
-00000410: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
-00000420: 207d 2c0d 0a20 2020 2070 6163 6b61 6765   },..    package
-00000430: 733d 7365 7475 7074 6f6f 6c73 2e66 696e  s=setuptools.fin
-00000440: 645f 7061 636b 6167 6573 2829 2c0d 0a20  d_packages(),.. 
-00000450: 2020 2063 6c61 7373 6966 6965 7273 3d5b     classifiers=[
-00000460: 0d0a 2020 2020 2020 2020 2744 6576 656c  ..        'Devel
-00000470: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000480: 2033 202d 2041 6c70 6861 272c 0d0a 2020   3 - Alpha',..  
-00000490: 2020 2020 2020 274e 6174 7572 616c 204c        'Natural L
-000004a0: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
-000004b0: 7368 272c 0d0a 2020 2020 2020 2020 274c  sh',..        'L
-000004c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000004d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000004e0: 6365 6e73 6527 2c0d 0a20 2020 2020 2020  cense',..       
-000004f0: 2027 4f70 6572 6174 696e 6720 5379 7374   'Operating Syst
-00000500: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000510: 6465 6e74 272c 0d0a 2020 2020 2020 2020  dent',..        
-00000520: 2750 726f 6772 616d 6d69 6e67 204c 616e  'Programming Lan
-00000530: 6775 6167 6520 3a3a 2050 7974 686f 6e27  guage :: Python'
-00000540: 2c0d 0a20 2020 2020 2020 2027 5072 6f67  ,..        'Prog
-00000550: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000560: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000570: 3727 2c0d 0a20 2020 205d 2c0d 0a29 0d0a  7',..    ],..)..
-00000580: 0d0a                                     ..
+00000180: 6c6f 6e65 6e2c 204a 616b 7562 2053 6564  lonen, Jakub Sed
+00000190: 7a69 6e73 6b69 272c 0d0a 2020 2020 6175  zinski',..    au
+000001a0: 7468 6f72 5f65 6d61 696c 3d27 7261 6e64  thor_email='rand
+000001b0: 6f6d 6163 6365 7373 6962 6c65 6b61 706f  omaccessiblekapo
+000001c0: 6f72 4067 6d61 696c 2e63 6f6d 272c 0d0a  or@gmail.com',..
+000001d0: 2020 2020 7572 6c3d 2768 7474 7073 3a2f      url='https:/
+000001e0: 2f67 6974 6875 622e 636f 6d2f 6b61 706f  /github.com/kapo
+000001f0: 6f72 6c61 622f 4e61 7061 5472 6163 6b4d  orlab/NapaTrackM
+00000200: 6174 6572 2f27 2c0d 0a20 2020 2064 6573  ater/',..    des
+00000210: 6372 6970 7469 6f6e 3d27 496d 706f 7274  cription='Import
+00000220: 2054 7261 636b 6d61 7465 2058 4d4c 2066   Trackmate XML f
+00000230: 696c 6573 2066 6f72 2054 7261 636b 2056  iles for Track V
+00000240: 6973 7561 6c69 7a61 7469 6f6e 2061 6e64  isualization and
+00000250: 2061 6e61 6c79 7369 7320 696e 204e 6170   analysis in Nap
+00000260: 6172 692e 272c 0d0a 2020 2020 6c6f 6e67  ari.',..    long
+00000270: 5f64 6573 6372 6970 7469 6f6e 3d6c 6f6e  _description=lon
+00000280: 675f 6465 7363 7269 7074 696f 6e2c 0d0a  g_description,..
+00000290: 2020 2020 6c6f 6e67 5f64 6573 6372 6970      long_descrip
+000002a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000002b0: 653d 2774 6578 742f 6d61 726b 646f 776e  e='text/markdown
+000002c0: 272c 0d0a 2020 2020 696e 7374 616c 6c5f  ',..    install_
+000002d0: 7265 7175 6972 6573 3d5b 0d0a 2020 2020  requires=[..    
+000002e0: 2020 2020 226c 786d 6c22 2c0d 0a20 2020      "lxml",..   
+000002f0: 2020 2020 2022 766f 6c6c 7365 6722 2c0d       "vollseg",.
+00000300: 0a20 2020 2020 2020 2022 6e61 7061 7269  .        "napari
+00000310: 222c 0d0a 2020 2020 2020 2020 226e 6174  ",..        "nat
+00000320: 736f 7274 222c 0d0a 2020 2020 2020 2020  sort",..        
+00000330: 2273 6561 626f 726e 222c 0d0a 2020 2020  "seaborn",..    
+00000340: 2020 2020 2263 656c 6c73 6861 7065 2d63      "cellshape-c
+00000350: 6c6f 7564 222c 0d0a 2020 2020 2020 2020  loud",..        
+00000360: 2263 656c 6c73 6861 7065 2d68 656c 7065  "cellshape-helpe
+00000370: 7222 2c0d 0a20 2020 2020 2020 2022 6b61  r",..        "ka
+00000380: 706f 6f72 6c61 6273 2d6c 6967 6874 6e69  poorlabs-lightni
+00000390: 6e67 222c 0d0a 2020 2020 2020 2020 226c  ng",..        "l
+000003a0: 6967 6874 6e69 6e67 3e3d 322e 302e 3422  ightning>=2.0.4"
+000003b0: 0d0a 2020 2020 5d2c 0d0a 2020 2020 656e  ..    ],..    en
+000003c0: 7472 795f 706f 696e 7473 203d 207b 0d0a  try_points = {..
+000003d0: 2020 2020 2020 2020 2763 6f6e 736f 6c65          'console
+000003e0: 5f73 6372 6970 7473 273a 205b 0d0a 2020  _scripts': [..  
+000003f0: 2020 2020 2020 2020 2020 2774 7261 636b            'track
+00000400: 203d 206e 6170 6174 7261 636b 6d61 7465   = napatrackmate
+00000410: 722e 5f5f 6d61 696e 5f5f 3a6d 6169 6e27  r.__main__:main'
+00000420: 2c0d 0a20 2020 2020 2020 205d 0d0a 2020  ,..        ]..  
+00000430: 2020 7d2c 0d0a 2020 2020 7061 636b 6167    },..    packag
+00000440: 6573 3d73 6574 7570 746f 6f6c 732e 6669  es=setuptools.fi
+00000450: 6e64 5f70 6163 6b61 6765 7328 292c 0d0a  nd_packages(),..
+00000460: 2020 2020 636c 6173 7369 6669 6572 733d      classifiers=
+00000470: 5b0d 0a20 2020 2020 2020 2027 4465 7665  [..        'Deve
+00000480: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+00000490: 3a20 3320 2d20 416c 7068 6127 2c0d 0a20  : 3 - Alpha',.. 
+000004a0: 2020 2020 2020 2027 4e61 7475 7261 6c20         'Natural 
+000004b0: 4c61 6e67 7561 6765 203a 3a20 456e 676c  Language :: Engl
+000004c0: 6973 6827 2c0d 0a20 2020 2020 2020 2027  ish',..        '
+000004d0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000004e0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000004f0: 6963 656e 7365 272c 0d0a 2020 2020 2020  icense',..      
+00000500: 2020 274f 7065 7261 7469 6e67 2053 7973    'Operating Sys
+00000510: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000520: 6e64 656e 7427 2c0d 0a20 2020 2020 2020  ndent',..       
+00000530: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
+00000540: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000550: 272c 0d0a 2020 2020 2020 2020 2750 726f  ',..        'Pro
+00000560: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000570: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000580: 2e37 272c 0d0a 2020 2020 5d2c 0d0a 290d  .7',..    ],..).
+00000590: 0a0d 0a                                  ...
```

