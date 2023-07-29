# Comparing `tmp/napatrackmater-3.9.9.tar.gz` & `tmp/napatrackmater-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.9.9.tar", last modified: Sat Jul 29 17:15:08 2023, max compression
+gzip compressed data, was "napatrackmater-4.0.0.tar", last modified: Sat Jul 29 17:21:37 2023, max compression
```

## Comparing `napatrackmater-3.9.9.tar` & `napatrackmater-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:15:08.370523 napatrackmater-3.9.9/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:15:08.370363 napatrackmater-3.9.9/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:15:08.369018 napatrackmater-3.9.9/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   116657 2023-07-29 17:12:25.000000 napatrackmater-3.9.9/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 17:14:48.000000 napatrackmater-3.9.9/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:15:08.370115 napatrackmater-3.9.9/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 17:15:08.000000 napatrackmater-3.9.9/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 17:15:08.370572 napatrackmater-3.9.9/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.9/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.747521 napatrackmater-4.0.0/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:21:37.747392 napatrackmater-4.0.0/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.746320 napatrackmater-4.0.0/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   116626 2023-07-29 17:20:59.000000 napatrackmater-4.0.0/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 17:21:03.000000 napatrackmater-4.0.0/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 17:21:37.747142 napatrackmater-4.0.0/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 17:21:37.000000 napatrackmater-4.0.0/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 17:21:37.747562 napatrackmater-4.0.0/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-4.0.0/setup.py
```

### Comparing `napatrackmater-3.9.9/LICENSE` & `napatrackmater-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/PKG-INFO` & `napatrackmater-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.9
+Version: 4.0.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.9/README.md` & `napatrackmater-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-4.0.0/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-4.0.0/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/Trackmate.py` & `napatrackmater-4.0.0/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2520,4773 +2520,4771 @@
 00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009d90: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
 00009da0: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
 00009db0: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
 00009dc0: 6965 7320 3d20 7365 6c66 2e5f 7472 6163  ies = self._trac
 00009dd0: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
-00009de0: 6965 7328 7472 6163 6b2c 2069 6e74 2874  ies(track, int(t
-00009df0: 7261 636b 5f69 6429 2c20 616c 6c5f 6469  rack_id), all_di
-00009e00: 6374 5f76 616c 7565 732c 2074 2c20 7a2c  ct_values, t, z,
-00009e10: 2079 2c20 782c 206b 2c20 6375 7272 656e   y, x, k, curren
-00009e20: 745f 7472 6163 6b5f 6964 2c20 756e 6971  t_track_id, uniq
-00009e30: 7565 5f69 642c 2063 7572 7265 6e74 5f74  ue_id, current_t
-00009e40: 7261 636b 6c65 7473 2c20 6375 7272 656e  racklets, curren
-00009e50: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-00009e60: 6572 7469 6573 290d 0a20 2020 2020 2020  erties)..       
-00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e80: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00009e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ea0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00009eb0: 7265 6e74 5f74 7261 636b 6c65 7473 203d  rent_tracklets =
-00009ec0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00009ed0: 656e 745f 7472 6163 6b6c 6574 735b 7374  ent_tracklets[st
-00009ee0: 7228 7472 6163 6b5f 6964 295d 2c20 6474  r(track_id)], dt
-00009ef0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00009f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009f10: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00009f20: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-00009f30: 726f 7065 7274 6965 7320 3d20 6e70 2e61  roperties = np.a
-00009f40: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
-00009f50: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
-00009f60: 6965 735b 7374 7228 7472 6163 6b5f 6964  ies[str(track_id
-00009f70: 295d 2c20 6474 7970 653d 6e70 2e66 6c6f  )], dtype=np.flo
-00009f80: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fa0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00009fd0: 636b 735b 7472 6163 6b5f 6964 5d20 3d20  cks[track_id] = 
-00009fe0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009ff0: 7320 2020 2020 0d0a 2020 2020 2020 2020  s     ..        
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a010: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-0000a020: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
-0000a030: 5b74 7261 636b 5f69 645d 203d 2063 7572  [track_id] = cur
-0000a040: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-0000a050: 726f 7065 7274 6965 7320 2020 200d 0a0d  roperties    ...
-0000a060: 0a20 2020 2064 6566 205f 7472 6163 6b6c  .    def _trackl
-0000a070: 6574 5f61 6e64 5f70 726f 7065 7274 6965  et_and_propertie
-0000a080: 7328 7365 6c66 2c20 7472 6163 6b2c 2020  s(self, track,  
-0000a090: 7472 6163 6b5f 6964 2c20 616c 6c5f 6469  track_id, all_di
-0000a0a0: 6374 5f76 616c 7565 732c 2074 2c20 7a2c  ct_values, t, z,
-0000a0b0: 2079 2c20 782c 206b 2c20 6375 7272 656e   y, x, k, curren
-0000a0c0: 745f 7472 6163 6b5f 6964 2c20 756e 6971  t_track_id, uniq
-0000a0d0: 7565 5f69 642c 2063 7572 7265 6e74 5f74  ue_id, current_t
-0000a0e0: 7261 636b 6c65 7473 2c20 6375 7272 656e  racklets, curren
-0000a0f0: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-0000a100: 6572 7469 6573 293a 0d0a 2020 2020 2020  erties):..      
-0000a110: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 2020 2020 2020 2020 2067 656e 5f69             gen_i
-0000a140: 6420 3d20 696e 7428 666c 6f61 7428 616c  d = int(float(al
-0000a150: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
-0000a160: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
-0000a170: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a190: 2020 2020 2020 2020 2020 2020 7370 6565              spee
-0000a1a0: 6420 3d20 666c 6f61 7428 616c 6c5f 6469  d = float(all_di
-0000a1b0: 6374 5f76 616c 7565 735b 7365 6c66 2e73  ct_values[self.s
-0000a1c0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1f0: 6163 6365 6c65 7261 7469 6f6e 203d 2066  acceleration = f
-0000a200: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-0000a210: 6c75 6573 5b73 656c 662e 6163 6365 6c65  lues[self.accele
-0000a220: 7261 7469 6f6e 5f6b 6579 5d29 0d0a 2020  ration_key])..  
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 2020 6d6f 7469 6f6e 5f61 6e67 6c65 203d    motion_angle =
-0000a260: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-0000a270: 7661 6c75 6573 5b73 656c 662e 6d6f 7469  values[self.moti
-0000a280: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
-0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 7261 6469 616c 5f61 6e67 6c65      radial_angle
-0000a2c0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-0000a2d0: 745f 7661 6c75 6573 5b73 656c 662e 7261  t_values[self.ra
-0000a2e0: 6469 616c 5f61 6e67 6c65 5f6b 6579 5d29  dial_angle_key])
-0000a2f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 2020 2020 2020 7261 6469 7573 203d 2066        radius = f
-0000a320: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-0000a330: 6c75 6573 5b73 656c 662e 7261 6469 7573  lues[self.radius
-0000a340: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a360: 2020 2020 2020 2020 2020 2020 766f 6c75              volu
-0000a370: 6d65 5f70 6978 656c 7320 3d20 696e 7428  me_pixels = int(
-0000a380: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-0000a390: 616c 7565 735b 7365 6c66 2e71 7561 6c69  alues[self.quali
-0000a3a0: 7479 5f6b 6579 5d29 290d 0a20 2020 2020  ty_key]))..     
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a3d0: 6f74 616c 5f69 6e74 656e 7369 7479 203d  otal_intensity =
-0000a3e0: 2020 666c 6f61 7428 616c 6c5f 6469 6374    float(all_dict
-0000a3f0: 5f76 616c 7565 735b 7365 6c66 2e74 6f74  _values[self.tot
-0000a400: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000a410: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00009de0: 6965 7328 7472 6163 6b2c 2020 616c 6c5f  ies(track,  all_
+00009df0: 6469 6374 5f76 616c 7565 732c 2074 2c20  dict_values, t, 
+00009e00: 7a2c 2079 2c20 782c 206b 2c20 6375 7272  z, y, x, k, curr
+00009e10: 656e 745f 7472 6163 6b5f 6964 2c20 756e  ent_track_id, un
+00009e20: 6971 7565 5f69 642c 2063 7572 7265 6e74  ique_id, current
+00009e30: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
+00009e40: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
+00009e50: 6f70 6572 7469 6573 290d 0a20 2020 2020  operties)..     
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00009e80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009ea0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009eb0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00009ec0: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
+00009ed0: 7374 7228 7472 6163 6b5f 6964 295d 2c20  str(track_id)], 
+00009ee0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00009ef0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009f00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009f10: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009f20: 5f70 726f 7065 7274 6965 7320 3d20 6e70  _properties = np
+00009f30: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00009f40: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+00009f50: 7274 6965 735b 7374 7228 7472 6163 6b5f  rties[str(track_
+00009f60: 6964 295d 2c20 6474 7970 653d 6e70 2e66  id)], dtype=np.f
+00009f70: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2073 656c 662e 756e 6971 7565 5f74     self.unique_t
+00009fc0: 7261 636b 735b 7472 6163 6b5f 6964 5d20  racks[track_id] 
+00009fd0: 3d20 6375 7272 656e 745f 7472 6163 6b6c  = current_trackl
+00009fe0: 6574 7320 2020 2020 0d0a 2020 2020 2020  ets     ..      
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000a010: 655f 7472 6163 6b5f 7072 6f70 6572 7469  e_track_properti
+0000a020: 6573 5b74 7261 636b 5f69 645d 203d 2063  es[track_id] = c
+0000a030: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+0000a040: 5f70 726f 7065 7274 6965 7320 2020 200d  _properties    .
+0000a050: 0a0d 0a20 2020 2064 6566 205f 7472 6163  ...    def _trac
+0000a060: 6b6c 6574 5f61 6e64 5f70 726f 7065 7274  klet_and_propert
+0000a070: 6965 7328 7365 6c66 2c20 7472 6163 6b2c  ies(self, track,
+0000a080: 2061 6c6c 5f64 6963 745f 7661 6c75 6573   all_dict_values
+0000a090: 2c20 742c 207a 2c20 792c 2078 2c20 6b2c  , t, z, y, x, k,
+0000a0a0: 2063 7572 7265 6e74 5f74 7261 636b 5f69   current_track_i
+0000a0b0: 642c 2075 6e69 7175 655f 6964 2c20 6375  d, unique_id, cu
+0000a0c0: 7272 656e 745f 7472 6163 6b6c 6574 732c  rrent_tracklets,
+0000a0d0: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
+0000a0e0: 7473 5f70 726f 7065 7274 6965 7329 3a0d  ts_properties):.
+0000a0f0: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a120: 2020 6765 6e5f 6964 203d 2069 6e74 2866    gen_id = int(f
+0000a130: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+0000a140: 6c75 6573 5b73 656c 662e 6765 6e65 7261  lues[self.genera
+0000a150: 7469 6f6e 6964 5f6b 6579 5d29 290d 0a20  tionid_key])).. 
+0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a180: 2020 2073 7065 6564 203d 2066 6c6f 6174     speed = float
+0000a190: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000a1a0: 5b73 656c 662e 7370 6565 645f 6b65 795d  [self.speed_key]
+0000a1b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1d0: 2020 2020 2020 2061 6363 656c 6572 6174         accelerat
+0000a1e0: 696f 6e20 3d20 666c 6f61 7428 616c 6c5f  ion = float(all_
+0000a1f0: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+0000a200: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
+0000a210: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a230: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
+0000a240: 616e 676c 6520 3d20 666c 6f61 7428 616c  angle = float(al
+0000a250: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+0000a260: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
+0000a270: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 2020 2020 2020 2020 2020 2072 6164 6961             radia
+0000a2a0: 6c5f 616e 676c 6520 3d20 666c 6f61 7428  l_angle = float(
+0000a2b0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
+0000a2c0: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
+0000a2d0: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2f0: 2020 2020 2020 2020 2020 2020 2072 6164               rad
+0000a300: 6975 7320 3d20 666c 6f61 7428 616c 6c5f  ius = float(all_
+0000a310: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+0000a320: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a350: 2020 2076 6f6c 756d 655f 7069 7865 6c73     volume_pixels
+0000a360: 203d 2069 6e74 2866 6c6f 6174 2861 6c6c   = int(float(all
+0000a370: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+0000a380: 662e 7175 616c 6974 795f 6b65 795d 2929  f.quality_key]))
+0000a390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3b0: 2020 2020 2020 746f 7461 6c5f 696e 7465        total_inte
+0000a3c0: 6e73 6974 7920 3d20 2066 6c6f 6174 2861  nsity =  float(a
+0000a3d0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000a3e0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000a3f0: 6974 795f 6b65 795d 290d 0a20 2020 2020  ity_key])..     
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a450: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-0000a460: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-0000a470: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-0000a480: 5f76 616c 7565 735b 7365 6c66 2e64 6973  _values[self.dis
-0000a490: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000a4a0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4c0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-0000a4d0: 5f64 6973 706c 6163 656d 656e 742c 746f  _displacement,to
-0000a4e0: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
-0000a4f0: 6365 2c20 6d61 785f 7472 6163 6b5f 6469  ce, max_track_di
-0000a500: 7374 616e 6365 2c20 7472 6163 6b5f 6475  stance, track_du
-0000a510: 7261 7469 6f6e 2020 3d20 2073 656c 662e  ration  =  self.
-0000a520: 5f67 6574 5f74 7261 636b 5f66 6561 7475  _get_track_featu
-0000a530: 7265 7328 7365 6c66 2c20 7472 6163 6b29  res(self, track)
-0000a540: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a440: 2020 2020 6469 7374 616e 6365 5f63 656c      distance_cel
+0000a450: 6c5f 6d61 736b 203d 2066 6c6f 6174 2861  l_mask = float(a
+0000a460: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+0000a470: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+0000a480: 6c5f 6d61 736b 5f6b 6579 5d29 0d0a 2020  l_mask_key])..  
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2020 7472 6163 6b5f 6469 7370 6c61 6365    track_displace
+0000a4c0: 6d65 6e74 2c74 6f74 616c 5f74 7261 636b  ment,total_track
+0000a4d0: 5f64 6973 7461 6e63 652c 206d 6178 5f74  _distance, max_t
+0000a4e0: 7261 636b 5f64 6973 7461 6e63 652c 2074  rack_distance, t
+0000a4f0: 7261 636b 5f64 7572 6174 696f 6e20 203d  rack_duration  =
+0000a500: 2020 7365 6c66 2e5f 6765 745f 7472 6163    self._get_trac
+0000a510: 6b5f 6665 6174 7572 6573 2874 7261 636b  k_features(track
+0000a520: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a540: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
 0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000a590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2020 2020 2069 6620 7365 6c66 2e73 7572       if self.sur
-0000a5c0: 6661 6365 5f61 7265 615f 6b65 7920 696e  face_area_key in
-0000a5d0: 2061 6c6c 5f64 6963 745f 7661 6c75 6573   all_dict_values
-0000a5e0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2020 2020 6966 2073 656c 662e 7375        if self.su
+0000a5a0: 7266 6163 655f 6172 6561 5f6b 6579 2069  rface_area_key i
+0000a5b0: 6e20 616c 6c5f 6469 6374 5f76 616c 7565  n all_dict_value
+0000a5c0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-0000a650: 6f6d 705f 6669 7273 7420 3d20 666c 6f61  omp_first = floa
-0000a660: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
-0000a670: 735b 7365 6c66 2e65 6363 656e 7472 6963  s[self.eccentric
-0000a680: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-0000a690: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6c0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000a6d0: 705f 7365 636f 6e64 203d 2066 6c6f 6174  p_second = float
-0000a6e0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
-0000a6f0: 5b73 656c 662e 6563 6365 6e74 7269 6369  [self.eccentrici
-0000a700: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-0000a710: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-0000a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a740: 7375 7266 6163 655f 6172 6561 203d 2066  surface_area = f
-0000a750: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
-0000a760: 6c75 6573 5b73 656c 662e 7375 7266 6163  lues[self.surfac
-0000a770: 655f 6172 6561 5f6b 6579 5d29 0d0a 2020  e_area_key])..  
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7a0: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-0000a7b0: 6973 5f6d 6173 6b20 3d20 666c 6f61 7428  is_mask = float(
-0000a7c0: 616c 6c5f 6469 6374 5f76 616c 7565 735b  all_dict_values[
-0000a7d0: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
-0000a7e0: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
-0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+0000a630: 636f 6d70 5f66 6972 7374 203d 2066 6c6f  comp_first = flo
+0000a640: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+0000a650: 6573 5b73 656c 662e 6563 6365 6e74 7269  es[self.eccentri
+0000a660: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
+0000a670: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+0000a6b0: 6d70 5f73 6563 6f6e 6420 3d20 666c 6f61  mp_second = floa
+0000a6c0: 7428 616c 6c5f 6469 6374 5f76 616c 7565  t(all_dict_value
+0000a6d0: 735b 7365 6c66 2e65 6363 656e 7472 6963  s[self.eccentric
+0000a6e0: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
+0000a6f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 2073 7572 6661 6365 5f61 7265 6120 3d20   surface_area = 
+0000a730: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+0000a740: 616c 7565 735b 7365 6c66 2e73 7572 6661  alues[self.surfa
+0000a750: 6365 5f61 7265 615f 6b65 795d 290d 0a20  ce_area_key]).. 
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a780: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
+0000a790: 7869 735f 6d61 736b 203d 2066 6c6f 6174  xis_mask = float
+0000a7a0: 2861 6c6c 5f64 6963 745f 7661 6c75 6573  (all_dict_values
+0000a7b0: 5b73 656c 662e 6365 6c6c 6178 6973 5f6d  [self.cellaxis_m
+0000a7c0: 6173 6b5f 6b65 795d 290d 0a20 2020 2020  ask_key])..     
+0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a810: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a820: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
 0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a860: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000a870: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a8a0: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-0000a8b0: 5f66 6972 7374 203d 202d 310d 0a20 2020  _first = -1..   
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-0000a8f0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
-0000a900: 6420 3d20 2d31 0d0a 2020 2020 2020 2020  d = -1..        
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a930: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
-0000a940: 203d 202d 310d 0a20 2020 2020 2020 2020   = -1..         
-0000a950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
-0000a980: 6b20 3d20 2d31 2020 2020 200d 0a0d 0a20  k = -1     .... 
-0000a990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9b0: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
-0000a9c0: 6e74 726f 6964 203d 2028 742c 726f 756e  ntroid = (t,roun
-0000a9d0: 6428 7a29 2f73 656c 662e 7a63 616c 6962  d(z)/self.zcalib
-0000a9e0: 7261 7469 6f6e 2c20 726f 756e 6428 7929  ration, round(y)
-0000a9f0: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
-0000aa00: 6f6e 2c20 726f 756e 6428 7829 2f73 656c  on, round(x)/sel
-0000aa10: 662e 7863 616c 6962 7261 7469 6f6e 2920  f.xcalibration) 
-0000aa20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa40: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000aa50: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
-0000aa60: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-0000aa70: 6f69 645d 203d 206b 0d0a 0d0a 2020 2020  oid] = k....    
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaa0: 6966 2063 7572 7265 6e74 5f74 7261 636b  if current_track
-0000aab0: 5f69 6420 696e 2063 7572 7265 6e74 5f74  _id in current_t
-0000aac0: 7261 636b 6c65 7473 3a0d 0a20 2020 2020  racklets:..     
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aaf0: 2020 2074 7261 636b 6c65 745f 6172 7261     tracklet_arra
-0000ab00: 7920 3d20 6375 7272 656e 745f 7472 6163  y = current_trac
-0000ab10: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
-0000ab20: 6163 6b5f 6964 5d0d 0a20 2020 2020 2020  ack_id]..       
-0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000ab60: 745f 6172 7261 7920 3d20 6e70 2e61 7272  t_array = np.arr
-0000ab70: 6179 285b 696e 7428 666c 6f61 7428 756e  ay([int(float(un
-0000ab80: 6971 7565 5f69 6429 292c 2074 2c20 7a2f  ique_id)), t, z/
-0000ab90: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-0000aba0: 6e2c 2079 2f73 656c 662e 7963 616c 6962  n, y/self.ycalib
-0000abb0: 7261 7469 6f6e 2c20 782f 7365 6c66 2e78  ration, x/self.x
-0000abc0: 6361 6c69 6272 6174 696f 6e5d 290d 0a20  calibration]).. 
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abf0: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
-0000ac00: 7261 636b 6c65 7473 5b63 7572 7265 6e74  racklets[current
-0000ac10: 5f74 7261 636b 5f69 645d 203d 206e 702e  _track_id] = np.
-0000ac20: 7673 7461 636b 2828 7472 6163 6b6c 6574  vstack((tracklet
-0000ac30: 5f61 7272 6179 2c20 6375 7272 656e 745f  _array, current_
-0000ac40: 7472 6163 6b6c 6574 5f61 7272 6179 2929  tracklet_array))
-0000ac50: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac70: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-0000ac80: 655f 6172 7261 7920 3d20 6375 7272 656e  e_array = curren
-0000ac90: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-0000aca0: 6572 7469 6573 5b63 7572 7265 6e74 5f74  erties[current_t
-0000acb0: 7261 636b 5f69 645d 0d0a 2020 2020 2020  rack_id]..      
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ace0: 2020 6375 7272 656e 745f 7661 6c75 655f    current_value_
-0000acf0: 6172 7261 7920 3d20 6e70 2e61 7272 6179  array = np.array
-0000ad00: 285b 742c 2069 6e74 2866 6c6f 6174 2875  ([t, int(float(u
-0000ad10: 6e69 7175 655f 6964 2929 2c20 6765 6e5f  nique_id)), gen_
-0000ad20: 6964 2c20 7261 6469 7573 2c20 766f 6c75  id, radius, volu
-0000ad30: 6d65 5f70 6978 656c 732c 2065 6363 656e  me_pixels, eccen
-0000ad40: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-0000ad50: 7374 2c20 6563 6365 6e74 7269 6369 7479  st, eccentricity
-0000ad60: 5f63 6f6d 705f 7365 636f 6e64 2c20 7375  _comp_second, su
-0000ad70: 7266 6163 655f 6172 6561 2c20 746f 7461  rface_area, tota
-0000ad80: 6c5f 696e 7465 6e73 6974 792c 2073 7065  l_intensity, spe
-0000ad90: 6564 2c20 6d6f 7469 6f6e 5f61 6e67 6c65  ed, motion_angle
-0000ada0: 2c20 6163 6365 6c65 7261 7469 6f6e 2c20  , acceleration, 
-0000adb0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000adc0: 736b 2c20 7261 6469 616c 5f61 6e67 6c65  sk, radial_angle
-0000add0: 2c20 6365 6c6c 5f61 7869 735f 6d61 736b  , cell_axis_mask
-0000ade0: 2c74 7261 636b 5f64 6973 706c 6163 656d  ,track_displacem
-0000adf0: 656e 742c 2074 6f74 616c 5f74 7261 636b  ent, total_track
-0000ae00: 5f64 6973 7461 6e63 652c 206d 6178 5f74  _distance, max_t
-0000ae10: 7261 636b 5f64 6973 7461 6e63 652c 2074  rack_distance, t
-0000ae20: 7261 636b 5f64 7572 6174 696f 6e20 5d29  rack_duration ])
-0000ae30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a840: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000a850: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+0000a890: 705f 6669 7273 7420 3d20 2d31 0d0a 2020  p_first = -1..  
+0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8c0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+0000a8d0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+0000a8e0: 6e64 203d 202d 310d 0a20 2020 2020 2020  nd = -1..       
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a910: 2020 2020 2073 7572 6661 6365 5f61 7265       surface_are
+0000a920: 6120 3d20 2d31 0d0a 2020 2020 2020 2020  a = -1..        
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a950: 2020 2020 6365 6c6c 5f61 7869 735f 6d61      cell_axis_ma
+0000a960: 736b 203d 202d 3120 2020 2020 0d0a 0d0a  sk = -1     ....
+0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a990: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
+0000a9a0: 656e 7472 6f69 6420 3d20 2874 2c72 6f75  entroid = (t,rou
+0000a9b0: 6e64 287a 292f 7365 6c66 2e7a 6361 6c69  nd(z)/self.zcali
+0000a9c0: 6272 6174 696f 6e2c 2072 6f75 6e64 2879  bration, round(y
+0000a9d0: 292f 7365 6c66 2e79 6361 6c69 6272 6174  )/self.ycalibrat
+0000a9e0: 696f 6e2c 2072 6f75 6e64 2878 292f 7365  ion, round(x)/se
+0000a9f0: 6c66 2e78 6361 6c69 6272 6174 696f 6e29  lf.xcalibration)
+0000aa00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000aa30: 7565 5f73 706f 745f 6365 6e74 726f 6964  ue_spot_centroid
+0000aa40: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
+0000aa50: 726f 6964 5d20 3d20 6b0d 0a0d 0a20 2020  roid] = k....   
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa80: 2069 6620 6375 7272 656e 745f 7472 6163   if current_trac
+0000aa90: 6b5f 6964 2069 6e20 6375 7272 656e 745f  k_id in current_
+0000aaa0: 7472 6163 6b6c 6574 733a 0d0a 2020 2020  tracklets:..    
+0000aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aad0: 2020 2020 7472 6163 6b6c 6574 5f61 7272      tracklet_arr
+0000aae0: 6179 203d 2063 7572 7265 6e74 5f74 7261  ay = current_tra
+0000aaf0: 636b 6c65 7473 5b63 7572 7265 6e74 5f74  cklets[current_t
+0000ab00: 7261 636b 5f69 645d 0d0a 2020 2020 2020  rack_id]..      
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
+0000ab40: 6574 5f61 7272 6179 203d 206e 702e 6172  et_array = np.ar
+0000ab50: 7261 7928 5b69 6e74 2866 6c6f 6174 2875  ray([int(float(u
+0000ab60: 6e69 7175 655f 6964 2929 2c20 742c 207a  nique_id)), t, z
+0000ab70: 2f73 656c 662e 7a63 616c 6962 7261 7469  /self.zcalibrati
+0000ab80: 6f6e 2c20 792f 7365 6c66 2e79 6361 6c69  on, y/self.ycali
+0000ab90: 6272 6174 696f 6e2c 2078 2f73 656c 662e  bration, x/self.
+0000aba0: 7863 616c 6962 7261 7469 6f6e 5d29 0d0a  xcalibration])..
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0000abe0: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
+0000abf0: 745f 7472 6163 6b5f 6964 5d20 3d20 6e70  t_track_id] = np
+0000ac00: 2e76 7374 6163 6b28 2874 7261 636b 6c65  .vstack((trackle
+0000ac10: 745f 6172 7261 792c 2063 7572 7265 6e74  t_array, current
+0000ac20: 5f74 7261 636b 6c65 745f 6172 7261 7929  _tracklet_array)
+0000ac30: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0000ac60: 7565 5f61 7272 6179 203d 2063 7572 7265  ue_array = curre
+0000ac70: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
+0000ac80: 7065 7274 6965 735b 6375 7272 656e 745f  perties[current_
+0000ac90: 7472 6163 6b5f 6964 5d0d 0a20 2020 2020  track_id]..     
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acc0: 2020 2063 7572 7265 6e74 5f76 616c 7565     current_value
+0000acd0: 5f61 7272 6179 203d 206e 702e 6172 7261  _array = np.arra
+0000ace0: 7928 5b74 2c20 696e 7428 666c 6f61 7428  y([t, int(float(
+0000acf0: 756e 6971 7565 5f69 6429 292c 2067 656e  unique_id)), gen
+0000ad00: 5f69 642c 2072 6164 6975 732c 2076 6f6c  _id, radius, vol
+0000ad10: 756d 655f 7069 7865 6c73 2c20 6563 6365  ume_pixels, ecce
+0000ad20: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+0000ad30: 7273 742c 2065 6363 656e 7472 6963 6974  rst, eccentricit
+0000ad40: 795f 636f 6d70 5f73 6563 6f6e 642c 2073  y_comp_second, s
+0000ad50: 7572 6661 6365 5f61 7265 612c 2074 6f74  urface_area, tot
+0000ad60: 616c 5f69 6e74 656e 7369 7479 2c20 7370  al_intensity, sp
+0000ad70: 6565 642c 206d 6f74 696f 6e5f 616e 676c  eed, motion_angl
+0000ad80: 652c 2061 6363 656c 6572 6174 696f 6e2c  e, acceleration,
+0000ad90: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
+0000ada0: 6173 6b2c 2072 6164 6961 6c5f 616e 676c  ask, radial_angl
+0000adb0: 652c 2063 656c 6c5f 6178 6973 5f6d 6173  e, cell_axis_mas
+0000adc0: 6b2c 7472 6163 6b5f 6469 7370 6c61 6365  k,track_displace
+0000add0: 6d65 6e74 2c20 746f 7461 6c5f 7472 6163  ment, total_trac
+0000ade0: 6b5f 6469 7374 616e 6365 2c20 6d61 785f  k_distance, max_
+0000adf0: 7472 6163 6b5f 6469 7374 616e 6365 2c20  track_distance, 
+0000ae00: 7472 6163 6b5f 6475 7261 7469 6f6e 205d  track_duration ]
+0000ae10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae30: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-0000ae90: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
-0000aea0: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
-0000aeb0: 645d 203d 206e 702e 7673 7461 636b 2828  d] = np.vstack((
-0000aec0: 7661 6c75 655f 6172 7261 792c 2063 7572  value_array, cur
-0000aed0: 7265 6e74 5f76 616c 7565 5f61 7272 6179  rent_value_array
-0000aee0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-0000af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000af40: 5f74 7261 636b 6c65 745f 6172 7261 7920  _tracklet_array 
-0000af50: 3d20 6e70 2e61 7272 6179 285b 696e 7428  = np.array([int(
-0000af60: 666c 6f61 7428 756e 6971 7565 5f69 6429  float(unique_id)
-0000af70: 292c 2074 2c20 7a2f 7365 6c66 2e7a 6361  ), t, z/self.zca
-0000af80: 6c69 6272 6174 696f 6e2c 2079 2f73 656c  libration, y/sel
-0000af90: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
-0000afa0: 782f 7365 6c66 2e78 6361 6c69 6272 6174  x/self.xcalibrat
-0000afb0: 696f 6e5d 290d 0a20 2020 2020 2020 2020  ion])..         
-0000afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000afe0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-0000aff0: 5b63 7572 7265 6e74 5f74 7261 636b 5f69  [current_track_i
-0000b000: 645d 203d 2063 7572 7265 6e74 5f74 7261  d] = current_tra
-0000b010: 636b 6c65 745f 6172 7261 7920 0d0a 0d0a  cklet_array ....
-0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b040: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0000b050: 7661 6c75 655f 6172 7261 7920 3d20 6e70  value_array = np
-0000b060: 2e61 7272 6179 285b 742c 2069 6e74 2866  .array([t, int(f
-0000b070: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
-0000b080: 2c20 6765 6e5f 6964 2c20 7261 6469 7573  , gen_id, radius
-0000b090: 2c20 766f 6c75 6d65 5f70 6978 656c 732c  , volume_pixels,
-0000b0a0: 2020 6563 6365 6e74 7269 6369 7479 5f63    eccentricity_c
-0000b0b0: 6f6d 705f 6669 7273 742c 2065 6363 656e  omp_first, eccen
-0000b0c0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-0000b0d0: 6f6e 642c 2073 7572 6661 6365 5f61 7265  ond, surface_are
-0000b0e0: 612c 2020 746f 7461 6c5f 696e 7465 6e73  a,  total_intens
-0000b0f0: 6974 792c 2073 7065 6564 2c20 6d6f 7469  ity, speed, moti
-0000b100: 6f6e 5f61 6e67 6c65 2c20 6163 6365 6c65  on_angle, accele
-0000b110: 7261 7469 6f6e 2c20 6469 7374 616e 6365  ration, distance
-0000b120: 5f63 656c 6c5f 6d61 736b 2c20 7261 6469  _cell_mask, radi
-0000b130: 616c 5f61 6e67 6c65 2c20 6365 6c6c 5f61  al_angle, cell_a
-0000b140: 7869 735f 6d61 736b 2c74 7261 636b 5f64  xis_mask,track_d
-0000b150: 6973 706c 6163 656d 656e 742c 2074 6f74  isplacement, tot
-0000b160: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
-0000b170: 652c 206d 6178 5f74 7261 636b 5f64 6973  e, max_track_dis
-0000b180: 7461 6e63 652c 2074 7261 636b 5f64 7572  tance, track_dur
-0000b190: 6174 696f 6e20 5d29 0d0a 2020 2020 2020  ation ])..      
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 6375 7272 656e 745f 7472 6163 6b6c    current_trackl
-0000b1d0: 6574 735f 7072 6f70 6572 7469 6573 5b63  ets_properties[c
-0000b1e0: 7572 7265 6e74 5f74 7261 636b 5f69 645d  urrent_track_id]
-0000b1f0: 203d 2063 7572 7265 6e74 5f76 616c 7565   = current_value
-0000b200: 5f61 7272 6179 0d0a 0d0a 2020 2020 2020  _array....      
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000b230: 7475 726e 2063 7572 7265 6e74 5f74 7261  turn current_tra
-0000b240: 636b 6c65 7473 2c20 6375 7272 656e 745f  cklets, current_
-0000b250: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
-0000b260: 7469 6573 2020 2020 200d 0a0d 0a20 2020  ties     ....   
-0000b270: 2064 6566 205f 6d61 7374 6572 5f73 706f   def _master_spo
-0000b280: 745f 636f 6d70 7574 6572 2873 656c 662c  t_computer(self,
-0000b290: 2066 7261 6d65 293a 0d0a 2020 2020 2020   frame):..      
-0000b2a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b2b0: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
-0000b2c0: 6e20 6672 616d 652e 6669 6e64 616c 6c28  n frame.findall(
-0000b2d0: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000b300: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-0000b310: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
-0000b320: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
-0000b330: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
-0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b350: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000b360: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000b370: 6c66 2e75 6e69 7175 6569 645f 6b65 7920  lf.uniqueid_key 
-0000b380: 696e 2053 706f 746f 626a 6563 742e 6b65  in Spotobject.ke
-0000b390: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000b3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3d0: 2072 6164 6975 7320 3d20 666c 6f61 7428   radius = float(
-0000b3e0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b3f0: 656c 662e 7261 6469 7573 5f6b 6579 2929  elf.radius_key))
-0000b400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b420: 2020 7175 616c 6974 7920 3d20 666c 6f61    quality = floa
-0000b430: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b440: 2873 656c 662e 7175 616c 6974 795f 6b65  (self.quality_ke
-0000b450: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2074 6f74 616c 5f69 6e74 656e       total_inten
-0000b480: 7369 7479 203d 2066 6c6f 6174 2853 706f  sity = float(Spo
-0000b490: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b4a0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000b4b0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4d0: 2020 2020 2020 2020 6d65 616e 5f69 6e74          mean_int
-0000b4e0: 656e 7369 7479 203d 2066 6c6f 6174 2853  ensity = float(S
-0000b4f0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b500: 6c66 2e6d 6561 6e5f 696e 7465 6e73 6974  lf.mean_intensit
-0000b510: 795f 6b65 7929 290d 0a0d 0a20 2020 2020  y_key))....     
-0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b540: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000b550: 6572 7469 6573 5b63 656c 6c5f 6964 5d20  erties[cell_id] 
-0000b560: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b580: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
-0000b590: 6c6c 6964 5f6b 6579 3a20 696e 7428 666c  llid_key: int(fl
-0000b5a0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b5b0: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000b5c0: 6579 2929 292c 200d 0a20 2020 2020 2020  ey))), ..       
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b5f0: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
-0000b600: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
-0000b610: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
-0000b620: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b650: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-0000b660: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000b670: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
-0000b680: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6b0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
-0000b6c0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
-0000b6d0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
-0000b6e0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-0000b720: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000b730: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
-0000b740: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b770: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000b780: 7369 7479 5f6b 6579 203a 2074 6f74 616c  sity_key : total
-0000b790: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
-0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-0000b7d0: 7369 7479 5f6b 6579 203a 206d 6561 6e5f  sity_key : mean_
-0000b7e0: 696e 7465 6e73 6974 792c 0d0a 2020 2020  intensity,..    
-0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b810: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
-0000b820: 3a20 7261 6469 7573 2c0d 0a20 2020 2020  : radius,..     
-0000b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b840: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b850: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
-0000b860: 3a20 7175 616c 6974 792c 0d0a 2020 2020  : quality,..    
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-0000b8a0: 6c6c 5f6d 6173 6b5f 6b65 793a 2028 666c  ll_mask_key: (fl
-0000b8b0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b8c0: 6574 2873 656c 662e 6469 7374 616e 6365  et(self.distance
-0000b8d0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 2929  _cell_mask_key))
-0000b8e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b900: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-0000b910: 7175 6569 645f 6b65 7920 3a20 7374 7228  queid_key : str(
-0000b920: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b930: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
-0000b940: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b960: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
-0000b970: 6163 6b6c 6574 6964 5f6b 6579 203a 2073  ackletid_key : s
-0000b980: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
-0000b990: 7428 7365 6c66 2e74 7261 636b 6c65 7469  t(self.trackleti
-0000b9a0: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b9d0: 6c66 2e67 656e 6572 6174 696f 6e69 645f  lf.generationid_
-0000b9e0: 6b65 7920 3a20 7374 7228 5370 6f74 6f62  key : str(Spotob
-0000b9f0: 6a65 6374 2e67 6574 2873 656c 662e 6765  ject.get(self.ge
-0000ba00: 6e65 7261 7469 6f6e 6964 5f6b 6579 2929  nerationid_key))
-0000ba10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 2020 2073 656c 662e 7472 6163         self.trac
-0000ba40: 6b69 645f 6b65 7920 3a20 7374 7228 5370  kid_key : str(Sp
-0000ba50: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000ba60: 662e 7472 6163 6b69 645f 6b65 7929 292c  f.trackid_key)),
-0000ba70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 2020 2020 2020 7365 6c66 2e6d 6f74 696f        self.motio
-0000baa0: 6e5f 616e 676c 655f 6b65 7920 3a20 2866  n_angle_key : (f
-0000bab0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000bac0: 6765 7428 7365 6c66 2e6d 6f74 696f 6e5f  get(self.motion_
-0000bad0: 616e 676c 655f 6b65 7929 2929 2c0d 0a20  angle_key))),.. 
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb00: 2020 2073 656c 662e 7370 6565 645f 6b65     self.speed_ke
-0000bb10: 7920 3a20 2866 6c6f 6174 2853 706f 746f  y : (float(Spoto
-0000bb20: 626a 6563 742e 6765 7428 7365 6c66 2e73  bject.get(self.s
-0000bb30: 7065 6564 5f6b 6579 2929 292c 0d0a 2020  peed_key))),..  
-0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb60: 2020 7365 6c66 2e61 6363 656c 6572 6174    self.accelerat
-0000bb70: 696f 6e5f 6b65 7920 3a20 2866 6c6f 6174  ion_key : (float
-0000bb80: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bb90: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
-0000bba0: 6e5f 6b65 7929 2929 2c0d 0a20 2020 2020  n_key))),..     
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bbd0: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
-0000bbe0: 5f6b 6579 3a20 666c 6f61 7428 5370 6f74  _key: float(Spot
-0000bbf0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000bc00: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-0000bc10: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae60: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+0000ae70: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
+0000ae80: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
+0000ae90: 6964 5d20 3d20 6e70 2e76 7374 6163 6b28  id] = np.vstack(
+0000aea0: 2876 616c 7565 5f61 7272 6179 2c20 6375  (value_array, cu
+0000aeb0: 7272 656e 745f 7661 6c75 655f 6172 7261  rrent_value_arra
+0000aec0: 7929 290d 0a0d 0a20 2020 2020 2020 2020  y))....         
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000aef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+0000af20: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
+0000af30: 203d 206e 702e 6172 7261 7928 5b69 6e74   = np.array([int
+0000af40: 2866 6c6f 6174 2875 6e69 7175 655f 6964  (float(unique_id
+0000af50: 2929 2c20 742c 207a 2f73 656c 662e 7a63  )), t, z/self.zc
+0000af60: 616c 6962 7261 7469 6f6e 2c20 792f 7365  alibration, y/se
+0000af70: 6c66 2e79 6361 6c69 6272 6174 696f 6e2c  lf.ycalibration,
+0000af80: 2078 2f73 656c 662e 7863 616c 6962 7261   x/self.xcalibra
+0000af90: 7469 6f6e 5d29 0d0a 2020 2020 2020 2020  tion])..        
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afc0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
+0000afd0: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
+0000afe0: 6964 5d20 3d20 6375 7272 656e 745f 7472  id] = current_tr
+0000aff0: 6163 6b6c 6574 5f61 7272 6179 200d 0a0d  acklet_array ...
+0000b000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b020: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+0000b030: 5f76 616c 7565 5f61 7272 6179 203d 206e  _value_array = n
+0000b040: 702e 6172 7261 7928 5b74 2c20 696e 7428  p.array([t, int(
+0000b050: 666c 6f61 7428 756e 6971 7565 5f69 6429  float(unique_id)
+0000b060: 292c 2067 656e 5f69 642c 2072 6164 6975  ), gen_id, radiu
+0000b070: 732c 2076 6f6c 756d 655f 7069 7865 6c73  s, volume_pixels
+0000b080: 2c20 2065 6363 656e 7472 6963 6974 795f  ,  eccentricity_
+0000b090: 636f 6d70 5f66 6972 7374 2c20 6563 6365  comp_first, ecce
+0000b0a0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+0000b0b0: 636f 6e64 2c20 7375 7266 6163 655f 6172  cond, surface_ar
+0000b0c0: 6561 2c20 2074 6f74 616c 5f69 6e74 656e  ea,  total_inten
+0000b0d0: 7369 7479 2c20 7370 6565 642c 206d 6f74  sity, speed, mot
+0000b0e0: 696f 6e5f 616e 676c 652c 2061 6363 656c  ion_angle, accel
+0000b0f0: 6572 6174 696f 6e2c 2064 6973 7461 6e63  eration, distanc
+0000b100: 655f 6365 6c6c 5f6d 6173 6b2c 2072 6164  e_cell_mask, rad
+0000b110: 6961 6c5f 616e 676c 652c 2063 656c 6c5f  ial_angle, cell_
+0000b120: 6178 6973 5f6d 6173 6b2c 7472 6163 6b5f  axis_mask,track_
+0000b130: 6469 7370 6c61 6365 6d65 6e74 2c20 746f  displacement, to
+0000b140: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
+0000b150: 6365 2c20 6d61 785f 7472 6163 6b5f 6469  ce, max_track_di
+0000b160: 7374 616e 6365 2c20 7472 6163 6b5f 6475  stance, track_du
+0000b170: 7261 7469 6f6e 205d 290d 0a20 2020 2020  ration ])..     
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+0000b1b0: 6c65 7473 5f70 726f 7065 7274 6965 735b  lets_properties[
+0000b1c0: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
+0000b1d0: 5d20 3d20 6375 7272 656e 745f 7661 6c75  ] = current_valu
+0000b1e0: 655f 6172 7261 790d 0a0d 0a20 2020 2020  e_array....     
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b210: 6574 7572 6e20 6375 7272 656e 745f 7472  eturn current_tr
+0000b220: 6163 6b6c 6574 732c 2063 7572 7265 6e74  acklets, current
+0000b230: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
+0000b240: 7274 6965 7320 2020 2020 0d0a 0d0a 2020  rties     ....  
+0000b250: 2020 6465 6620 5f6d 6173 7465 725f 7370    def _master_sp
+0000b260: 6f74 5f63 6f6d 7075 7465 7228 7365 6c66  ot_computer(self
+0000b270: 2c20 6672 616d 6529 3a0d 0a20 2020 2020  , frame):..     
+0000b280: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b290: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
+0000b2a0: 696e 2066 7261 6d65 2e66 696e 6461 6c6c  in frame.findall
+0000b2b0: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000b2e0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000b2f0: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
+0000b300: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
+0000b310: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000b340: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000b350: 656c 662e 756e 6971 7565 6964 5f6b 6579  elf.uniqueid_key
+0000b360: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
+0000b370: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3b0: 2020 7261 6469 7573 203d 2066 6c6f 6174    radius = float
+0000b3c0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b3d0: 7365 6c66 2e72 6164 6975 735f 6b65 7929  self.radius_key)
+0000b3e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 2020 2071 7561 6c69 7479 203d 2066 6c6f     quality = flo
+0000b410: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000b420: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
+0000b430: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2020 746f 7461 6c5f 696e 7465        total_inte
+0000b460: 6e73 6974 7920 3d20 666c 6f61 7428 5370  nsity = float(Sp
+0000b470: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b480: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000b490: 795f 6b65 7929 290d 0a20 2020 2020 2020  y_key))..       
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4b0: 2020 2020 2020 2020 206d 6561 6e5f 696e           mean_in
+0000b4c0: 7465 6e73 6974 7920 3d20 666c 6f61 7428  tensity = float(
+0000b4d0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b4e0: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
+0000b4f0: 7479 5f6b 6579 2929 0d0a 0d0a 2020 2020  ty_key))....    
+0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b510: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b520: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000b530: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000b540: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b560: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000b570: 656c 6c69 645f 6b65 793a 2069 6e74 2866  ellid_key: int(f
+0000b580: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000b590: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
+0000b5a0: 6b65 7929 2929 2c20 0d0a 2020 2020 2020  key))), ..      
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000b5d0: 6c66 2e66 7261 6d65 6964 5f6b 6579 203a  lf.frameid_key :
+0000b5e0: 2069 6e74 2866 6c6f 6174 2853 706f 746f   int(float(Spoto
+0000b5f0: 626a 6563 742e 6765 7428 7365 6c66 2e66  bject.get(self.f
+0000b600: 7261 6d65 6964 5f6b 6579 2929 292c 0d0a  rameid_key))),..
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
+0000b640: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000b650: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000b660: 7a70 6f73 6964 5f6b 6579 2929 2c0d 0a20  zposid_key)),.. 
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2073 656c 662e 7970 6f73 6964 5f6b     self.yposid_k
+0000b6a0: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
+0000b6b0: 626a 6563 742e 6765 7428 7365 6c66 2e79  bject.get(self.y
+0000b6c0: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
+0000b700: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000b710: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
+0000b720: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b750: 2073 656c 662e 746f 7461 6c5f 696e 7465   self.total_inte
+0000b760: 6e73 6974 795f 6b65 7920 3a20 746f 7461  nsity_key : tota
+0000b770: 6c5f 696e 7465 6e73 6974 792c 0d0a 2020  l_intensity,..  
+0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
+0000b7b0: 6e73 6974 795f 6b65 7920 3a20 6d65 616e  nsity_key : mean
+0000b7c0: 5f69 6e74 656e 7369 7479 2c0d 0a20 2020  _intensity,..   
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7f0: 2073 656c 662e 7261 6469 7573 5f6b 6579   self.radius_key
+0000b800: 203a 2072 6164 6975 732c 0d0a 2020 2020   : radius,..    
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+0000b840: 203a 2071 7561 6c69 7479 2c0d 0a20 2020   : quality,..   
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
+0000b880: 656c 6c5f 6d61 736b 5f6b 6579 3a20 2866  ell_mask_key: (f
+0000b890: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000b8a0: 6765 7428 7365 6c66 2e64 6973 7461 6e63  get(self.distanc
+0000b8b0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 7929  e_cell_mask_key)
+0000b8c0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+0000b8f0: 6971 7565 6964 5f6b 6579 203a 2073 7472  iqueid_key : str
+0000b900: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b910: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+0000b920: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000b950: 7261 636b 6c65 7469 645f 6b65 7920 3a20  rackletid_key : 
+0000b960: 7374 7228 5370 6f74 6f62 6a65 6374 2e67  str(Spotobject.g
+0000b970: 6574 2873 656c 662e 7472 6163 6b6c 6574  et(self.tracklet
+0000b980: 6964 5f6b 6579 2929 2c0d 0a20 2020 2020  id_key)),..     
+0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b9b0: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
+0000b9c0: 5f6b 6579 203a 2073 7472 2853 706f 746f  _key : str(Spoto
+0000b9d0: 626a 6563 742e 6765 7428 7365 6c66 2e67  bject.get(self.g
+0000b9e0: 656e 6572 6174 696f 6e69 645f 6b65 7929  enerationid_key)
+0000b9f0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+0000ba20: 636b 6964 5f6b 6579 203a 2073 7472 2853  ckid_key : str(S
+0000ba30: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ba40: 6c66 2e74 7261 636b 6964 5f6b 6579 2929  lf.trackid_key))
+0000ba50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 2020 2020 2020 2073 656c 662e 6d6f 7469         self.moti
+0000ba80: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 2028  on_angle_key : (
+0000ba90: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000baa0: 2e67 6574 2873 656c 662e 6d6f 7469 6f6e  .get(self.motion
+0000bab0: 5f61 6e67 6c65 5f6b 6579 2929 292c 0d0a  _angle_key))),..
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 7365 6c66 2e73 7065 6564 5f6b      self.speed_k
+0000baf0: 6579 203a 2028 666c 6f61 7428 5370 6f74  ey : (float(Spot
+0000bb00: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000bb10: 7370 6565 645f 6b65 7929 2929 2c0d 0a20  speed_key))),.. 
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 2073 656c 662e 6163 6365 6c65 7261     self.accelera
+0000bb50: 7469 6f6e 5f6b 6579 203a 2028 666c 6f61  tion_key : (floa
+0000bb60: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bb70: 2873 656c 662e 6163 6365 6c65 7261 7469  (self.accelerati
+0000bb80: 6f6e 5f6b 6579 2929 292c 0d0a 2020 2020  on_key))),..    
+0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
+0000bbc0: 655f 6b65 793a 2066 6c6f 6174 2853 706f  e_key: float(Spo
+0000bbd0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000bbe0: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
+0000bbf0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
 0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000bc60: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
-0000bc70: 2069 6e20 5370 6f74 6f62 6a65 6374 2e6b   in Spotobject.k
-0000bc80: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bcb0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-0000bcc0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-0000bcd0: 5f69 6429 5d2e 7570 6461 7465 287b 0d0a  _id)].update({..
+0000bc30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000bc40: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
+0000bc50: 7920 696e 2053 706f 746f 626a 6563 742e  y in Spotobject.
+0000bc60: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000bc90: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+0000bca0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+0000bcb0: 6c5f 6964 295d 2e75 7064 6174 6528 7b0d  l_id)].update({.
+0000bcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 2020 7365 6c66 2e65 6363          self.ecc
-0000bd40: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-0000bd50: 6972 7374 6b65 7920 3a20 666c 6f61 7428  irstkey : float(
-0000bd60: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000bd70: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
-0000bd80: 5f63 6f6d 705f 6669 7273 746b 6579 2929  _comp_firstkey))
-0000bd90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000bd10: 2020 2020 2020 2020 2073 656c 662e 6563           self.ec
+0000bd20: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+0000bd30: 6669 7273 746b 6579 203a 2066 6c6f 6174  firstkey : float
+0000bd40: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000bd50: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
+0000bd60: 795f 636f 6d70 5f66 6972 7374 6b65 7929  y_comp_firstkey)
+0000bd70: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000bdf0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000be00: 705f 7365 636f 6e64 6b65 7920 3a20 666c  p_secondkey : fl
-0000be10: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000be20: 6574 2873 656c 662e 6563 6365 6e74 7269  et(self.eccentri
-0000be30: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-0000be40: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000bdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bdd0: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+0000bde0: 6d70 5f73 6563 6f6e 646b 6579 203a 2066  mp_secondkey : f
+0000bdf0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000be00: 6765 7428 7365 6c66 2e65 6363 656e 7472  get(self.eccentr
+0000be10: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+0000be20: 646b 6579 2929 2c0d 0a20 2020 2020 2020  dkey)),..       
+0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
-0000beb0: 615f 6b65 7920 3a20 666c 6f61 7428 5370  a_key : float(Sp
-0000bec0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000bed0: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
-0000bee0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000be80: 2073 656c 662e 7375 7266 6163 655f 6172   self.surface_ar
+0000be90: 6561 5f6b 6579 203a 2066 6c6f 6174 2853  ea_key : float(S
+0000bea0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000beb0: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
+0000bec0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000bf40: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-0000bf50: 6b5f 6b65 793a 2066 6c6f 6174 2853 706f  k_key: float(Spo
-0000bf60: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000bf70: 2e63 656c 6c61 7869 735f 6d61 736b 5f6b  .cellaxis_mask_k
-0000bf80: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+0000bf20: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
+0000bf30: 736b 5f6b 6579 3a20 666c 6f61 7428 5370  sk_key: float(Sp
+0000bf40: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000bf50: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
+0000bf60: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 207d 290d 0a20 2020 2020 2020 2020     })..         
 0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 7d29 0d0a 2020 2020 2020 2020 2020    })..          
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c020: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 0000c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c040: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c070: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c080: 6c69 6620 7365 6c66 2e75 6e69 7175 6569  lif self.uniquei
-0000c090: 645f 6b65 7920 6e6f 7420 696e 2053 706f  d_key not in Spo
-0000c0a0: 746f 626a 6563 742e 6b65 7973 2829 3a0d  tobject.keys():.
-0000c0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 656c 6966 2073 656c 662e 756e 6971 7565  elif self.unique
+0000c070: 6964 5f6b 6579 206e 6f74 2069 6e20 5370  id_key not in Sp
+0000c080: 6f74 6f62 6a65 6374 2e6b 6579 7328 293a  otobject.keys():
+0000c090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000c120: 2e64 6574 6563 746f 7263 6861 6e6e 656c  .detectorchannel
-0000c130: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c160: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
-0000c170: 4c5f 494e 5445 4e53 4954 5920 3d20 5370  L_INTENSITY = Sp
-0000c180: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000c190: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-0000c1a0: 795f 6368 325f 6b65 7929 0d0a 2020 2020  y_ch2_key)..    
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000c100: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
+0000c110: 6c20 3d3d 2031 3a0d 0a20 2020 2020 2020  l == 1:..       
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c140: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000c150: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
+0000c160: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000c170: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+0000c180: 7479 5f63 6832 5f6b 6579 290d 0a20 2020  ty_ch2_key)..   
+0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1e0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000c1f0: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
-0000c200: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000c210: 6974 795f 6368 325f 6b65 7929 0d0a 2020  ity_ch2_key)..  
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c240: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-0000c250: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c280: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
-0000c290: 414c 5f49 4e54 454e 5349 5459 203d 2053  AL_INTENSITY = S
-0000c2a0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c2b0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000c2c0: 7479 5f63 6831 5f6b 6579 290d 0a20 2020  ty_ch1_key)..   
+0000c1c0: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000c1d0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
+0000c1e0: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
+0000c1f0: 7369 7479 5f63 6832 5f6b 6579 290d 0a20  sity_ch2_key).. 
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c220: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000c230: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c260: 2020 2020 2020 2020 2020 2020 2020 544f                TO
+0000c270: 5441 4c5f 494e 5445 4e53 4954 5920 3d20  TAL_INTENSITY = 
+0000c280: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c290: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000c2a0: 6974 795f 6368 315f 6b65 7929 0d0a 2020  ity_ch1_key)..  
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c300: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
-0000c310: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
-0000c320: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-0000c330: 7369 7479 5f63 6831 5f6b 6579 290d 0a20  sity_ch1_key).. 
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
-0000c370: 5320 3d20 666c 6f61 7428 5370 6f74 6f62  S = float(Spotob
-0000c380: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
-0000c390: 6469 7573 5f6b 6579 2929 0d0a 2020 2020  dius_key))..    
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3c0: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
-0000c3d0: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
-0000c3e0: 6374 2e67 6574 2873 656c 662e 7175 616c  ct.get(self.qual
-0000c3f0: 6974 795f 6b65 7929 2920 2020 2020 0d0a  ity_key))     ..
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
-0000c430: 4c5f 494e 5445 4e53 4954 5920 3d20 666c  L_INTENSITY = fl
-0000c440: 6f61 7428 544f 5441 4c5f 494e 5445 4e53  oat(TOTAL_INTENS
-0000c450: 4954 5929 0d0a 2020 2020 2020 2020 2020  ITY)..          
-0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
-0000c490: 203d 2066 6c6f 6174 284d 4541 4e5f 494e   = float(MEAN_IN
-0000c4a0: 5445 4e53 4954 5929 0d0a 2020 2020 2020  TENSITY)..      
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-0000c4e0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000c4f0: 735b 6365 6c6c 5f69 645d 203d 207b 0d0a  s[cell_id] = {..
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c530: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
-0000c540: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2020 2020 2020 2020 2073 656c 662e 6672           self.fr
-0000c580: 616d 6569 645f 6b65 7920 3a20 696e 7428  ameid_key : int(
-0000c590: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000c5a0: 2e67 6574 2873 656c 662e 6672 616d 6569  .get(self.framei
-0000c5b0: 645f 6b65 7929 2929 2c0d 0a20 2020 2020  d_key))),..     
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
-0000c5f0: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
-0000c600: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c610: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
-0000c620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c650: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
-0000c660: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000c670: 2e67 6574 2873 656c 662e 7970 6f73 6964  .get(self.yposid
-0000c680: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6b0: 2020 2020 2073 656c 662e 7870 6f73 6964       self.xposid
-0000c6c0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-0000c6d0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000c6e0: 2e78 706f 7369 645f 6b65 7929 292c 0d0a  .xposid_key)),..
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c720: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-0000c730: 5f6b 6579 203a 2054 4f54 414c 5f49 4e54  _key : TOTAL_INT
-0000c740: 454e 5349 5459 2c0d 0a20 2020 2020 2020  ENSITY,..       
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
-0000c780: 6e74 656e 7369 7479 5f6b 6579 203a 204d  ntensity_key : M
-0000c790: 4541 4e5f 494e 5445 4e53 4954 592c 0d0a  EAN_INTENSITY,..
-0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c7d0: 2e72 6164 6975 735f 6b65 7920 3a20 5241  .radius_key : RA
-0000c7e0: 4449 5553 2c0d 0a20 2020 2020 2020 2020  DIUS,..         
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c810: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
-0000c820: 6b65 7920 3a20 5155 414c 4954 590d 0a20  key : QUALITY.. 
-0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c850: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-0000c860: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c870: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000c880: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8a0: 2020 2020 2020 0d0a 0d0a 2020 2020 6465        ....    de
-0000c8b0: 6620 5f73 706f 745f 636f 6d70 7574 6572  f _spot_computer
-0000c8c0: 2873 656c 662c 2066 7261 6d65 293a 0d0a  (self, frame):..
-0000c8d0: 0d0a 2020 2020 2020 2020 2020 666f 7220  ..          for 
-0000c8e0: 5370 6f74 6f62 6a65 6374 2069 6e20 6672  Spotobject in fr
-0000c8f0: 616d 652e 6669 6e64 616c 6c28 2753 706f  ame.findall('Spo
-0000c900: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
-0000c910: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000c920: 4372 6561 7465 206f 626a 6563 7420 7769  Create object wi
-0000c930: 7468 2075 6e69 7175 6520 6365 6c6c 2049  th unique cell I
-0000c940: 440d 0a20 2020 2020 2020 2020 2020 2020  D..             
-0000c950: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-0000c960: 6964 203d 2069 6e74 2853 706f 746f 626a  id = int(Spotobj
-0000c970: 6563 742e 6765 7428 7365 6c66 2e73 706f  ect.get(self.spo
-0000c980: 7469 645f 6b65 7929 290d 0a20 2020 2020  tid_key))..     
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 2023 2047 6574 2074 6865 2054 5a59     # Get the TZY
-0000c9b0: 5820 6c6f 6361 7469 6f6e 206f 6620 7468  X location of th
-0000c9c0: 6520 6365 6c6c 7320 696e 2074 6861 7420  e cells in that 
-0000c9d0: 6672 616d 650d 0a20 2020 2020 2020 2020  frame..         
-0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000c9f0: 6620 7365 6c66 2e64 6574 6563 746f 7263  f self.detectorc
-0000ca00: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
-0000ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000ca30: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
-0000ca40: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000ca50: 7369 7479 5f63 6832 5f6b 6579 2920 6973  sity_ch2_key) is
-0000ca60: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 2020 544f 5441 4c5f 494e 5445 4e53      TOTAL_INTENS
-0000caa0: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
-0000cab0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000cac0: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000cad0: 6368 325f 6b65 7929 290d 0a20 2020 2020  ch2_key))..     
-0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000cb10: 5920 3d20 666c 6f61 7428 5370 6f74 6f62  Y = float(Spotob
-0000cb20: 6a65 6374 2e67 6574 2873 656c 662e 6d65  ject.get(self.me
-0000cb30: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-0000cb40: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000c2e0: 2020 4d45 414e 5f49 4e54 454e 5349 5459    MEAN_INTENSITY
+0000c2f0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000c300: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
+0000c310: 6e73 6974 795f 6368 315f 6b65 7929 0d0a  nsity_ch1_key)..
+0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c340: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
+0000c350: 5553 203d 2066 6c6f 6174 2853 706f 746f  US = float(Spoto
+0000c360: 626a 6563 742e 6765 7428 7365 6c66 2e72  bject.get(self.r
+0000c370: 6164 6975 735f 6b65 7929 290d 0a20 2020  adius_key))..   
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3a0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
+0000c3b0: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
+0000c3c0: 6563 742e 6765 7428 7365 6c66 2e71 7561  ect.get(self.qua
+0000c3d0: 6c69 7479 5f6b 6579 2929 2020 2020 200d  lity_key))     .
+0000c3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000c410: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
+0000c420: 6c6f 6174 2854 4f54 414c 5f49 4e54 454e  loat(TOTAL_INTEN
+0000c430: 5349 5459 290d 0a20 2020 2020 2020 2020  SITY)..         
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
+0000c470: 5920 3d20 666c 6f61 7428 4d45 414e 5f49  Y = float(MEAN_I
+0000c480: 4e54 454e 5349 5459 290d 0a20 2020 2020  NTENSITY)..     
+0000c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+0000c4c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000c4d0: 6573 5b63 656c 6c5f 6964 5d20 3d20 7b0d  es[cell_id] = {.
+0000c4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c510: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
+0000c520: 7428 6365 6c6c 5f69 6429 2c20 0d0a 2020  t(cell_id), ..  
+0000c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c550: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+0000c560: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
+0000c570: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
+0000c580: 742e 6765 7428 7365 6c66 2e66 7261 6d65  t.get(self.frame
+0000c590: 6964 5f6b 6579 2929 292c 0d0a 2020 2020  id_key))),..    
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5c0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
+0000c5d0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+0000c5e0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c5f0: 656c 662e 7a70 6f73 6964 5f6b 6579 2929  elf.zposid_key))
+0000c600: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c630: 656c 662e 7970 6f73 6964 5f6b 6579 203a  elf.yposid_key :
+0000c640: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000c650: 742e 6765 7428 7365 6c66 2e79 706f 7369  t.get(self.yposi
+0000c660: 645f 6b65 7929 292c 0d0a 2020 2020 2020  d_key)),..      
+0000c670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
+0000c6a0: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
+0000c6b0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c6c0: 662e 7870 6f73 6964 5f6b 6579 2929 2c0d  f.xposid_key)),.
+0000c6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c700: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000c710: 795f 6b65 7920 3a20 544f 5441 4c5f 494e  y_key : TOTAL_IN
+0000c720: 5445 4e53 4954 592c 0d0a 2020 2020 2020  TENSITY,..      
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c750: 2020 2020 2020 7365 6c66 2e6d 6561 6e5f        self.mean_
+0000c760: 696e 7465 6e73 6974 795f 6b65 7920 3a20  intensity_key : 
+0000c770: 4d45 414e 5f49 4e54 454e 5349 5459 2c0d  MEAN_INTENSITY,.
+0000c780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c7b0: 662e 7261 6469 7573 5f6b 6579 203a 2052  f.radius_key : R
+0000c7c0: 4144 4955 532c 0d0a 2020 2020 2020 2020  ADIUS,..        
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7f0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
+0000c800: 5f6b 6579 203a 2051 5541 4c49 5459 0d0a  _key : QUALITY..
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c830: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
+0000c840: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000c850: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c880: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
+0000c890: 6566 205f 7370 6f74 5f63 6f6d 7075 7465  ef _spot_compute
+0000c8a0: 7228 7365 6c66 2c20 6672 616d 6529 3a0d  r(self, frame):.
+0000c8b0: 0a0d 0a20 2020 2020 2020 2020 2066 6f72  ...          for
+0000c8c0: 2053 706f 746f 626a 6563 7420 696e 2066   Spotobject in f
+0000c8d0: 7261 6d65 2e66 696e 6461 6c6c 2827 5370  rame.findall('Sp
+0000c8e0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
+0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c900: 2043 7265 6174 6520 6f62 6a65 6374 2077   Create object w
+0000c910: 6974 6820 756e 6971 7565 2063 656c 6c20  ith unique cell 
+0000c920: 4944 0d0a 2020 2020 2020 2020 2020 2020  ID..            
+0000c930: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000c940: 5f69 6420 3d20 696e 7428 5370 6f74 6f62  _id = int(Spotob
+0000c950: 6a65 6374 2e67 6574 2873 656c 662e 7370  ject.get(self.sp
+0000c960: 6f74 6964 5f6b 6579 2929 0d0a 2020 2020  otid_key))..    
+0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c980: 2020 2020 2320 4765 7420 7468 6520 545a      # Get the TZ
+0000c990: 5958 206c 6f63 6174 696f 6e20 6f66 2074  YX location of t
+0000c9a0: 6865 2063 656c 6c73 2069 6e20 7468 6174  he cells in that
+0000c9b0: 2066 7261 6d65 0d0a 2020 2020 2020 2020   frame..        
+0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9d0: 6966 2073 656c 662e 6465 7465 6374 6f72  if self.detector
+0000c9e0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000ca10: 6620 5370 6f74 6f62 6a65 6374 2e67 6574  f Spotobject.get
+0000ca20: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
+0000ca30: 6e73 6974 795f 6368 325f 6b65 7929 2069  nsity_ch2_key) i
+0000ca40: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca70: 2020 2020 2054 4f54 414c 5f49 4e54 454e       TOTAL_INTEN
+0000ca80: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
+0000ca90: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000caa0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000cab0: 5f63 6832 5f6b 6579 2929 0d0a 2020 2020  _ch2_key))..    
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
+0000caf0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
+0000cb00: 626a 6563 742e 6765 7428 7365 6c66 2e6d  bject.get(self.m
+0000cb10: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
+0000cb20: 325f 6b65 7929 290d 0a20 2020 2020 2020  2_key))..       
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb40: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb60: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb90: 2020 2020 2020 544f 5441 4c5f 494e 5445        TOTAL_INTE
-0000cba0: 4e53 4954 5920 3d20 2d31 0d0a 2020 2020  NSITY = -1..    
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbd0: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000cbe0: 5920 3d20 2d31 2020 2020 2020 200d 0a20  Y = -1       .. 
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 2020 2020 2020 2065 6c73 653a 2020 2020         else:    
-0000cc10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc30: 2020 2020 2020 6966 2053 706f 746f 626a        if Spotobj
-0000cc40: 6563 742e 6765 7428 7365 6c66 2e74 6f74  ect.get(self.tot
-0000cc50: 616c 5f69 6e74 656e 7369 7479 5f63 6831  al_intensity_ch1
-0000cc60: 5f6b 6579 2920 6973 206e 6f74 204e 6f6e  _key) is not Non
-0000cc70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc90: 2020 2020 2020 2020 2020 2020 544f 5441              TOTA
-0000cca0: 4c5f 494e 5445 4e53 4954 5920 3d20 666c  L_INTENSITY = fl
-0000ccb0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000ccc0: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000ccd0: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000cce0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd00: 2020 2020 2020 2020 2020 204d 4541 4e5f             MEAN_
-0000cd10: 494e 5445 4e53 4954 5920 3d20 666c 6f61  INTENSITY = floa
-0000cd20: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000cd30: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-0000cd40: 7369 7479 5f63 6831 5f6b 6579 2929 0d0a  sity_ch1_key))..
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb70: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
+0000cb80: 454e 5349 5459 203d 202d 310d 0a20 2020  ENSITY = -1..   
+0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
+0000cbc0: 5459 203d 202d 3120 2020 2020 2020 0d0a  TY = -1       ..
+0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbe0: 2020 2020 2020 2020 656c 7365 3a20 2020          else:   
+0000cbf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc10: 2020 2020 2020 2069 6620 5370 6f74 6f62         if Spotob
+0000cc20: 6a65 6374 2e67 6574 2873 656c 662e 746f  ject.get(self.to
+0000cc30: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
+0000cc40: 315f 6b65 7929 2069 7320 6e6f 7420 4e6f  1_key) is not No
+0000cc50: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc70: 2020 2020 2020 2020 2020 2020 2054 4f54               TOT
+0000cc80: 414c 5f49 4e54 454e 5349 5459 203d 2066  AL_INTENSITY = f
+0000cc90: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000cca0: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
+0000ccb0: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
+0000ccc0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 2020 2020 2020 2020 2020 4d45 414e              MEAN
+0000ccf0: 5f49 4e54 454e 5349 5459 203d 2066 6c6f  _INTENSITY = flo
+0000cd00: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000cd10: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
+0000cd20: 6e73 6974 795f 6368 315f 6b65 7929 290d  nsity_ch1_key)).
+0000cd30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
 0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000cda0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000cdb0: 202d 310d 0a20 2020 2020 2020 2020 2020   -1..           
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 2020 2020 2020 2020 2020 204d 4541               MEA
-0000cde0: 4e5f 494e 5445 4e53 4954 5920 3d20 2d31  N_INTENSITY = -1
-0000cdf0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd80: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000cd90: 3d20 2d31 0d0a 2020 2020 2020 2020 2020  = -1..          
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
+0000cdc0: 414e 5f49 4e54 454e 5349 5459 203d 202d  AN_INTENSITY = -
+0000cdd0: 3120 2020 2020 2020 2020 0d0a 0d0a 2020  1         ....  
+0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 2020 2020 2020 2052 4144 4955 5320 3d20         RADIUS = 
-0000ce40: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
-0000ce50: 2e67 6574 2873 656c 662e 7261 6469 7573  .get(self.radius
-0000ce60: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
-0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce80: 5155 414c 4954 5920 3d20 666c 6f61 7428  QUALITY = float(
-0000ce90: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000cea0: 656c 662e 7175 616c 6974 795f 6b65 7929  elf.quality_key)
-0000ceb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000cec0: 2020 2020 2020 2020 2020 2074 6573 746c             testl
-0000ced0: 6f63 6174 696f 6e20 3d20 2866 6c6f 6174  ocation = (float
-0000cee0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000cef0: 7365 6c66 2e7a 706f 7369 645f 6b65 7929  self.zposid_key)
-0000cf00: 292c 2066 6c6f 6174 2853 706f 746f 626a  ), float(Spotobj
-0000cf10: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
-0000cf20: 7369 645f 6b65 7929 292c 2020 666c 6f61  sid_key)),  floa
-0000cf30: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000cf40: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000cf50: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
-0000cf60: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-0000cf70: 6d65 203d 2053 706f 746f 626a 6563 742e  me = Spotobject.
-0000cf80: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000cf90: 5f6b 6579 290d 0a20 2020 2020 2020 2020  _key)..         
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000cfb0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000cfc0: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
-0000cfd0: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
-0000cfe0: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
-0000cff0: 2074 6573 746c 6f63 6174 696f 6e29 0d0a   testlocation)..
+0000ce10: 2020 2020 2020 2020 5241 4449 5553 203d          RADIUS =
+0000ce20: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
+0000ce30: 742e 6765 7428 7365 6c66 2e72 6164 6975  t.get(self.radiu
+0000ce40: 735f 6b65 7929 290d 0a20 2020 2020 2020  s_key))..       
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2051 5541 4c49 5459 203d 2066 6c6f 6174   QUALITY = float
+0000ce70: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000ce80: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+0000ce90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000cea0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+0000ceb0: 6c6f 6361 7469 6f6e 203d 2028 666c 6f61  location = (floa
+0000cec0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000ced0: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
+0000cee0: 2929 2c20 666c 6f61 7428 5370 6f74 6f62  )), float(Spotob
+0000cef0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
+0000cf00: 6f73 6964 5f6b 6579 2929 2c20 2066 6c6f  osid_key)),  flo
+0000cf10: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000cf20: 7428 7365 6c66 2e78 706f 7369 645f 6b65  t(self.xposid_ke
+0000cf30: 7929 2929 0d0a 2020 2020 2020 2020 2020  y)))..          
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+0000cf50: 616d 6520 3d20 5370 6f74 6f62 6a65 6374  ame = Spotobject
+0000cf60: 2e67 6574 2873 656c 662e 6672 616d 6569  .get(self.framei
+0000cf70: 645f 6b65 7929 0d0a 2020 2020 2020 2020  d_key)..        
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000cfa0: 736b 2c20 6d61 736b 6365 6e74 726f 6964  sk, maskcentroid
+0000cfb0: 203d 2073 656c 662e 5f67 6574 5f62 6f75   = self._get_bou
+0000cfc0: 6e64 6172 795f 6469 7374 2866 7261 6d65  ndary_dist(frame
+0000cfd0: 2c20 7465 7374 6c6f 6361 7469 6f6e 290d  , testlocation).
+0000cfe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cff0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-0000d040: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
-0000d050: 6c6c 5f69 645d 203d 207b 0d0a 2020 2020  ll_id] = {..    
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 2020 2020 2020 2020 7365 6c66 2e63 656c          self.cel
-0000d080: 6c69 645f 6b65 793a 2069 6e74 2863 656c  lid_key: int(cel
-0000d090: 6c5f 6964 292c 200d 0a20 2020 2020 2020  l_id), ..       
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0b0: 2020 2020 2073 656c 662e 6672 616d 6569       self.framei
-0000d0c0: 645f 6b65 7920 3a20 696e 7428 666c 6f61  d_key : int(floa
-0000d0d0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000d0e0: 2873 656c 662e 6672 616d 6569 645f 6b65  (self.frameid_ke
-0000d0f0: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
-0000d120: 6579 203a 2066 6c6f 6174 2853 706f 746f  ey : float(Spoto
-0000d130: 626a 6563 742e 6765 7428 7365 6c66 2e7a  bject.get(self.z
-0000d140: 706f 7369 645f 6b65 7929 292c 0d0a 2020  posid_key)),..  
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-0000d170: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000d180: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000d190: 2873 656c 662e 7970 6f73 6964 5f6b 6579  (self.yposid_key
-0000d1a0: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1c0: 2073 656c 662e 7870 6f73 6964 5f6b 6579   self.xposid_key
-0000d1d0: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000d1e0: 6563 742e 6765 7428 7365 6c66 2e78 706f  ect.get(self.xpo
-0000d1f0: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
-0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d210: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-0000d220: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000d230: 203a 2054 4f54 414c 5f49 4e54 454e 5349   : TOTAL_INTENSI
-0000d240: 5459 2c0d 0a20 2020 2020 2020 2020 2020  TY,..           
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-0000d270: 7369 7479 5f6b 6579 203a 204d 4541 4e5f  sity_key : MEAN_
-0000d280: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-0000d2b0: 6975 735f 6b65 7920 3a20 5241 4449 5553  ius_key : RADIUS
-0000d2c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d2e0: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
-0000d2f0: 3a20 5155 414c 4954 592c 0d0a 2020 2020  : QUALITY,..    
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-0000d320: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b5f  tance_cell_mask_
-0000d330: 6b65 793a 2066 6c6f 6174 2864 6973 7461  key: float(dista
-0000d340: 6e63 655f 6365 6c6c 5f6d 6173 6b29 2c0d  nce_cell_mask),.
-0000d350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d360: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000d370: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-0000d380: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-0000d390: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
-0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d3c0: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-0000d3d0: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
-0000d3e0: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
-0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d400: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000d410: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-0000d420: 3a20 666c 6f61 7428 6d61 736b 6365 6e74  : float(maskcent
-0000d430: 726f 6964 5b32 5d29 200d 0a20 2020 2020  roid[2]) ..     
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 207d 0d0a 2020 2020 2020 200d 0a20     }..       .. 
-0000d460: 2020 2064 6566 205f 6765 745f 6d61 7374     def _get_mast
-0000d470: 6572 5f78 6d6c 5f64 6174 6128 7365 6c66  er_xml_data(self
-0000d480: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000d490: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-0000d4a0: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000d4b0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d4d0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f63  lf.channel_xml_c
-0000d4e0: 6f6e 7465 6e74 203d 2073 656c 662e 786d  ontent = self.xm
-0000d4f0: 6c5f 636f 6e74 656e 740d 0a20 2020 2020  l_content..     
-0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2073 656c 662e 786d 6c5f 7472 6565 203d   self.xml_tree =
-0000d520: 2065 742e 7061 7273 6528 7365 6c66 2e78   et.parse(self.x
-0000d530: 6d6c 5f70 6174 6829 0d0a 2020 2020 2020  ml_path)..      
-0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d550: 7365 6c66 2e78 6d6c 5f72 6f6f 7420 3d20  self.xml_root = 
-0000d560: 7365 6c66 2e78 6d6c 5f74 7265 652e 6765  self.xml_tree.ge
-0000d570: 7472 6f6f 7428 290d 0a20 2020 2020 2020  troot()..       
-0000d580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d590: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000d5a0: 6e61 6d65 203d 2027 7365 636f 6e64 5f63  name = 'second_c
-0000d5b0: 6861 6e6e 656c 5f27 202b 206f 732e 7061  hannel_' + os.pa
-0000d5c0: 7468 2e73 706c 6974 6578 7428 6f73 2e70  th.splitext(os.p
-0000d5d0: 6174 682e 6261 7365 6e61 6d65 2873 656c  ath.basename(sel
-0000d5e0: 662e 786d 6c5f 7061 7468 2929 5b30 5d20  f.xml_path))[0] 
-0000d5f0: 2b20 272e 786d 6c27 0d0a 2020 2020 2020  + '.xml'..      
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
-0000d620: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0000d630: 6469 726e 616d 6528 7365 6c66 2e78 6d6c  dirname(self.xml
-0000d640: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-0000d650: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d660: 6c66 2e5f 6372 6561 7465 5f63 6861 6e6e  lf._create_chann
-0000d670: 656c 5f74 7265 6528 290d 0a0d 0a20 2020  el_tree()....   
-0000d680: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-0000d690: 6971 7565 5f6f 626a 6563 7473 203d 207b  ique_objects = {
-0000d6a0: 7d0d 0a20 2020 2020 2020 2020 2020 2073  }..            s
-0000d6b0: 656c 662e 756e 6971 7565 5f70 726f 7065  elf.unique_prope
-0000d6c0: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-0000d6d0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
-0000d6e0: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000d6f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d700: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000d710: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-0000d720: 2020 2073 656c 662e 4e6f 726d 616c 5472     self.NormalTr
-0000d730: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
-0000d740: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-0000d750: 6c5f 7472 6163 6b5f 7072 6f70 6572 7469  l_track_properti
-0000d760: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000d770: 2020 2020 2073 656c 662e 7370 6c69 745f       self.split_
-0000d780: 706f 696e 7473 5f74 696d 6573 203d 205b  points_times = [
-0000d790: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000d7a0: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
-0000d7b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d7c0: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-0000d7d0: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
-0000d7e0: 2020 2020 2020 2020 7365 6c66 2e44 6976          self.Div
-0000d7f0: 6964 696e 6754 7261 636b 4964 732e 6170  idingTrackIds.ap
-0000d800: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
-0000d810: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-0000d820: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-0000d830: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
-0000d840: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000d850: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-0000d860: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000d870: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000d880: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
-0000d890: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
-0000d8a0: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
-0000d8b0: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
-0000d8c0: 2020 2020 2073 656c 662e 4e6f 726d 616c       self.Normal
-0000d8d0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
-0000d8e0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
-0000d8f0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000d900: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000d910: 2020 2020 2020 2020 2020 7365 6c66 2e53            self.S
-0000d920: 706f 746f 626a 6563 7473 203d 2073 656c  potobjects = sel
-0000d930: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
-0000d940: 6e64 2827 4d6f 6465 6c27 292e 6669 6e64  nd('Model').find
-0000d950: 2827 416c 6c53 706f 7473 2729 0d0a 2020  ('AllSpots')..  
-0000d960: 2020 2020 2020 2020 2020 2320 4578 7472            # Extr
-0000d970: 6163 7420 7468 6520 7472 6163 6b73 2066  act the tracks f
-0000d980: 726f 6d20 786d 6c0d 0a20 2020 2020 2020  rom xml..       
-0000d990: 2020 2020 2073 656c 662e 7472 6163 6b73       self.tracks
-0000d9a0: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000d9b0: 656e 742e 6669 6e64 2822 4d6f 6465 6c22  ent.find("Model"
-0000d9c0: 292e 6669 6e64 2822 416c 6c54 7261 636b  ).find("AllTrack
-0000d9d0: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0000d9e0: 2073 656c 662e 7365 7474 696e 6773 203d   self.settings =
-0000d9f0: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000da00: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000da10: 2229 2e66 696e 6428 2249 6d61 6765 4461  ").find("ImageDa
-0000da20: 7461 2229 0d0a 2020 2020 2020 2020 2020  ta")..          
-0000da30: 2020 7365 6c66 2e78 6361 6c69 6272 6174    self.xcalibrat
-0000da40: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
-0000da50: 2e73 6574 7469 6e67 732e 6765 7428 2270  .settings.get("p
-0000da60: 6978 656c 7769 6474 6822 2929 0d0a 2020  ixelwidth"))..  
-0000da70: 2020 2020 2020 2020 2020 7365 6c66 2e79            self.y
-0000da80: 6361 6c69 6272 6174 696f 6e20 3d20 666c  calibration = fl
-0000da90: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000daa0: 732e 6765 7428 2270 6978 656c 6865 6967  s.get("pixelheig
-0000dab0: 6874 2229 290d 0a20 2020 2020 2020 2020  ht"))..         
-0000dac0: 2020 2073 656c 662e 7a63 616c 6962 7261     self.zcalibra
-0000dad0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000dae0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000daf0: 766f 7865 6c64 6570 7468 2229 290d 0a20  voxeldepth")).. 
-0000db00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000db10: 7463 616c 6962 7261 7469 6f6e 203d 2069  tcalibration = i
-0000db20: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
-0000db30: 7474 696e 6773 2e67 6574 2822 7469 6d65  ttings.get("time
-0000db40: 696e 7465 7276 616c 2229 2929 0d0a 2020  interval")))..  
-0000db50: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000db60: 6574 6563 746f 7273 6574 7469 6e67 7320  etectorsettings 
-0000db70: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000db80: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000db90: 7322 292e 6669 6e64 2822 4465 7465 6374  s").find("Detect
-0000dba0: 6f72 5365 7474 696e 6773 2229 0d0a 2020  orSettings")..  
-0000dbb0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000dbc0: 6173 6963 7365 7474 696e 6773 203d 2073  asicsettings = s
-0000dbd0: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000dbe0: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
-0000dbf0: 2e66 696e 6428 2242 6173 6963 5365 7474  .find("BasicSett
-0000dc00: 696e 6773 2229 0d0a 2020 2020 2020 2020  ings")..        
-0000dc10: 2020 2020 7365 6c66 2e64 6574 6563 746f      self.detecto
-0000dc20: 7263 6861 6e6e 656c 203d 2069 6e74 2866  rchannel = int(f
-0000dc30: 6c6f 6174 2873 656c 662e 6465 7465 6374  loat(self.detect
-0000dc40: 6f72 7365 7474 696e 6773 2e67 6574 2822  orsettings.get("
-0000dc50: 5441 5247 4554 5f43 4841 4e4e 454c 2229  TARGET_CHANNEL")
-0000dc60: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000dc70: 7365 6c66 2e74 7374 6172 7420 3d20 696e  self.tstart = in
-0000dc80: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
-0000dc90: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
-0000dca0: 7473 7461 7274 2229 2929 0d0a 2020 2020  tstart")))..    
-0000dcb0: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
-0000dcc0: 6420 3d20 696e 7428 666c 6f61 7428 7365  d = int(float(se
-0000dcd0: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
-0000dce0: 2e67 6574 2822 7465 6e64 2229 2929 2020  .get("tend")))  
-0000dcf0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000dd00: 2020 2020 7072 696e 7428 2749 7465 7261      print('Itera
-0000dd10: 7469 6e67 206f 7665 7220 7370 6f74 7320  ting over spots 
-0000dd20: 696e 2066 7261 6d65 2729 0d0a 2020 2020  in frame')..    
-0000dd30: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-0000dd40: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-0000dd50: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
-0000dd60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000dd70: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-0000dd80: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-0000dd90: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-0000dda0: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-0000ddb0: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-0000ddc0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-0000ddd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000dde0: 2020 2020 2020 2020 2066 6f72 2066 7261           for fra
-0000ddf0: 6d65 2069 6e20 7365 6c66 2e53 706f 746f  me in self.Spoto
-0000de00: 626a 6563 7473 2e66 696e 6461 6c6c 2827  bjects.findall('
-0000de10: 5370 6f74 7349 6e46 7261 6d65 2729 3a0d  SpotsInFrame'):.
-0000de20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de30: 2020 2020 2020 2020 2020 2020 2066 7574               fut
-0000de40: 7572 6573 2e61 7070 656e 6428 6578 6563  ures.append(exec
-0000de50: 7574 6f72 2e73 7562 6d69 7428 7365 6c66  utor.submit(self
-0000de60: 2e5f 6d61 7374 6572 5f73 706f 745f 636f  ._master_spot_co
-0000de70: 6d70 7574 6572 2c20 6672 616d 6529 290d  mputer, frame)).
-0000de80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de90: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000dea0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000deb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000d010: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+0000d020: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+0000d030: 656c 6c5f 6964 5d20 3d20 7b0d 0a20 2020  ell_id] = {..   
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 2020 2020 2073 656c 662e 6365           self.ce
+0000d060: 6c6c 6964 5f6b 6579 3a20 696e 7428 6365  llid_key: int(ce
+0000d070: 6c6c 5f69 6429 2c20 0d0a 2020 2020 2020  ll_id), ..      
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
+0000d0a0: 6964 5f6b 6579 203a 2069 6e74 2866 6c6f  id_key : int(flo
+0000d0b0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000d0c0: 7428 7365 6c66 2e66 7261 6d65 6964 5f6b  t(self.frameid_k
+0000d0d0: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
+0000d100: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
+0000d110: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000d120: 7a70 6f73 6964 5f6b 6579 2929 2c0d 0a20  zposid_key)),.. 
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d150: 7970 6f73 6964 5f6b 6579 203a 2066 6c6f  yposid_key : flo
+0000d160: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000d170: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
+0000d180: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1a0: 2020 7365 6c66 2e78 706f 7369 645f 6b65    self.xposid_ke
+0000d1b0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000d1c0: 6a65 6374 2e67 6574 2873 656c 662e 7870  ject.get(self.xp
+0000d1d0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+0000d200: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+0000d210: 7920 3a20 544f 5441 4c5f 494e 5445 4e53  y : TOTAL_INTENS
+0000d220: 4954 592c 0d0a 2020 2020 2020 2020 2020  ITY,..          
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 2020 7365 6c66 2e6d 6561 6e5f 696e 7465    self.mean_inte
+0000d250: 6e73 6974 795f 6b65 7920 3a20 4d45 414e  nsity_key : MEAN
+0000d260: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000d290: 6469 7573 5f6b 6579 203a 2052 4144 4955  dius_key : RADIU
+0000d2a0: 532c 0d0a 2020 2020 2020 2020 2020 2020  S,..            
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 7365 6c66 2e71 7561 6c69 7479 5f6b 6579  self.quality_key
+0000d2d0: 203a 2051 5541 4c49 5459 2c0d 0a20 2020   : QUALITY,..   
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2f0: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
+0000d300: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0000d310: 5f6b 6579 3a20 666c 6f61 7428 6469 7374  _key: float(dist
+0000d320: 616e 6365 5f63 656c 6c5f 6d61 736b 292c  ance_cell_mask),
+0000d330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d340: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d350: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+0000d360: 7a5f 6b65 793a 2066 6c6f 6174 286d 6173  z_key: float(mas
+0000d370: 6b63 656e 7472 6f69 645b 305d 292c 0d0a  kcentroid[0]),..
+0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d3a0: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
+0000d3b0: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
+0000d3c0: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
+0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000d3f0: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+0000d400: 793a 2066 6c6f 6174 286d 6173 6b63 656e  y: float(maskcen
+0000d410: 7472 6f69 645b 325d 2920 0d0a 2020 2020  troid[2]) ..    
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 2020 2020 7d0d 0a20 2020 2020 2020 0d0a      }..       ..
+0000d440: 2020 2020 6465 6620 5f67 6574 5f6d 6173      def _get_mas
+0000d450: 7465 725f 786d 6c5f 6461 7461 2873 656c  ter_xml_data(sel
+0000d460: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+0000d470: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000d480: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+0000d490: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d4b0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
+0000d4c0: 636f 6e74 656e 7420 3d20 7365 6c66 2e78  content = self.x
+0000d4d0: 6d6c 5f63 6f6e 7465 6e74 0d0a 2020 2020  ml_content..    
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4f0: 2020 7365 6c66 2e78 6d6c 5f74 7265 6520    self.xml_tree 
+0000d500: 3d20 6574 2e70 6172 7365 2873 656c 662e  = et.parse(self.
+0000d510: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 2073 656c 662e 786d 6c5f 726f 6f74 203d   self.xml_root =
+0000d540: 2073 656c 662e 786d 6c5f 7472 6565 2e67   self.xml_tree.g
+0000d550: 6574 726f 6f74 2829 0d0a 2020 2020 2020  etroot()..      
+0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d570: 7365 6c66 2e63 6861 6e6e 656c 5f78 6d6c  self.channel_xml
+0000d580: 5f6e 616d 6520 3d20 2773 6563 6f6e 645f  _name = 'second_
+0000d590: 6368 616e 6e65 6c5f 2720 2b20 6f73 2e70  channel_' + os.p
+0000d5a0: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
+0000d5b0: 7061 7468 2e62 6173 656e 616d 6528 7365  path.basename(se
+0000d5c0: 6c66 2e78 6d6c 5f70 6174 6829 295b 305d  lf.xml_path))[0]
+0000d5d0: 202b 2027 2e78 6d6c 270d 0a20 2020 2020   + '.xml'..     
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
+0000d600: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
+0000d610: 2e64 6972 6e61 6d65 2873 656c 662e 786d  .dirname(self.xm
+0000d620: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d640: 656c 662e 5f63 7265 6174 655f 6368 616e  elf._create_chan
+0000d650: 6e65 6c5f 7472 6565 2829 0d0a 0d0a 2020  nel_tree()....  
+0000d660: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000d670: 6e69 7175 655f 6f62 6a65 6374 7320 3d20  nique_objects = 
+0000d680: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+0000d690: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
+0000d6a0: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
+0000d6b0: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
+0000d6c0: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
+0000d6d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d6e0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
+0000d6f0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000d700: 2020 2020 7365 6c66 2e4e 6f72 6d61 6c54      self.NormalT
+0000d710: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
+0000d720: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000d730: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
+0000d740: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
+0000d750: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
+0000d760: 5f70 6f69 6e74 735f 7469 6d65 7320 3d20  _points_times = 
+0000d770: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+0000d780: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d790: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d7a0: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000d7b0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000d7c0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
+0000d7d0: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
+0000d7e0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000d7f0: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000d800: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
+0000d810: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
+0000d820: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000d830: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000d840: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000d850: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000d860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d870: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000d880: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
+0000d890: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
+0000d8a0: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
+0000d8b0: 6c54 7261 636b 4964 732e 6170 7065 6e64  lTrackIds.append
+0000d8c0: 2873 656c 662e 5472 6163 6b69 6442 6f78  (self.TrackidBox
+0000d8d0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+0000d8e0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000d8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d900: 5370 6f74 6f62 6a65 6374 7320 3d20 7365  Spotobjects = se
+0000d910: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000d920: 696e 6428 274d 6f64 656c 2729 2e66 696e  ind('Model').fin
+0000d930: 6428 2741 6c6c 5370 6f74 7327 290d 0a20  d('AllSpots').. 
+0000d940: 2020 2020 2020 2020 2020 2023 2045 7874             # Ext
+0000d950: 7261 6374 2074 6865 2074 7261 636b 7320  ract the tracks 
+0000d960: 6672 6f6d 2078 6d6c 0d0a 2020 2020 2020  from xml..      
+0000d970: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+0000d980: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
+0000d990: 7465 6e74 2e66 696e 6428 224d 6f64 656c  tent.find("Model
+0000d9a0: 2229 2e66 696e 6428 2241 6c6c 5472 6163  ").find("AllTrac
+0000d9b0: 6b73 2229 0d0a 2020 2020 2020 2020 2020  ks")..          
+0000d9c0: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
+0000d9d0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000d9e0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
+0000d9f0: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
+0000da00: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
+0000da10: 2020 2073 656c 662e 7863 616c 6962 7261     self.xcalibra
+0000da20: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
+0000da30: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
+0000da40: 7069 7865 6c77 6964 7468 2229 290d 0a20  pixelwidth")).. 
+0000da50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000da60: 7963 616c 6962 7261 7469 6f6e 203d 2066  ycalibration = f
+0000da70: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000da80: 6773 2e67 6574 2822 7069 7865 6c68 6569  gs.get("pixelhei
+0000da90: 6768 7422 2929 0d0a 2020 2020 2020 2020  ght"))..        
+0000daa0: 2020 2020 7365 6c66 2e7a 6361 6c69 6272      self.zcalibr
+0000dab0: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
+0000dac0: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000dad0: 2276 6f78 656c 6465 7074 6822 2929 0d0a  "voxeldepth"))..
+0000dae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000daf0: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
+0000db00: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
+0000db10: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
+0000db20: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
+0000db30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000db40: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
+0000db50: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000db60: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
+0000db70: 6773 2229 2e66 696e 6428 2244 6574 6563  gs").find("Detec
+0000db80: 746f 7253 6574 7469 6e67 7322 290d 0a20  torSettings").. 
+0000db90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dba0: 6261 7369 6373 6574 7469 6e67 7320 3d20  basicsettings = 
+0000dbb0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000dbc0: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000dbd0: 292e 6669 6e64 2822 4261 7369 6353 6574  ).find("BasicSet
+0000dbe0: 7469 6e67 7322 290d 0a20 2020 2020 2020  tings")..       
+0000dbf0: 2020 2020 2073 656c 662e 6465 7465 6374       self.detect
+0000dc00: 6f72 6368 616e 6e65 6c20 3d20 696e 7428  orchannel = int(
+0000dc10: 666c 6f61 7428 7365 6c66 2e64 6574 6563  float(self.detec
+0000dc20: 746f 7273 6574 7469 6e67 732e 6765 7428  torsettings.get(
+0000dc30: 2254 4152 4745 545f 4348 414e 4e45 4c22  "TARGET_CHANNEL"
+0000dc40: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+0000dc50: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
+0000dc60: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+0000dc70: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+0000dc80: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
+0000dc90: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+0000dca0: 6e64 203d 2069 6e74 2866 6c6f 6174 2873  nd = int(float(s
+0000dcb0: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
+0000dcc0: 732e 6765 7428 2274 656e 6422 2929 2920  s.get("tend"))) 
+0000dcd0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0000dce0: 2020 2020 2070 7269 6e74 2827 4974 6572       print('Iter
+0000dcf0: 6174 696e 6720 6f76 6572 2073 706f 7473  ating over spots
+0000dd00: 2069 6e20 6672 616d 6527 290d 0a20 2020   in frame')..   
+0000dd10: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000dd20: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
+0000dd30: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
+0000dd40: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+0000dd50: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+0000dd60: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+0000dd70: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+0000dd80: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+0000dd90: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+0000dda0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+0000ddb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ddc0: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
+0000ddd0: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
+0000dde0: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
+0000ddf0: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
+0000de00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000de10: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000de20: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+0000de30: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+0000de40: 662e 5f6d 6173 7465 725f 7370 6f74 5f63  f._master_spot_c
+0000de50: 6f6d 7075 7465 722c 2066 7261 6d65 2929  omputer, frame))
+0000de60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000de70: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000de80: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000de90: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000deb0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000dee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000def0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-0000df00: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-0000df10: 2243 6f6c 6c65 6374 696e 6720 5370 6f74  "Collecting Spot
-0000df20: 7322 0d0a 2020 2020 2020 2020 2020 2020  s"..            
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000df50: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ded0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+0000dee0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+0000def0: 2022 436f 6c6c 6563 7469 6e67 2053 706f   "Collecting Spo
+0000df00: 7473 220d 0a20 2020 2020 2020 2020 2020  ts"..           
+0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df20: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000df30: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000df40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
 0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df80: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
-0000df90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfa0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-0000dfb0: 2866 7574 7572 6573 292c 0d0a 2020 2020  (futures),..    
+0000df80: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000df90: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfb0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
 0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfd0: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-0000dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dff0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e000: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000e010: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
-0000e020: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-0000e030: 2069 6e20 636f 6e63 7572 7265 6e74 2e66   in concurrent.f
-0000e040: 7574 7572 6573 2e61 735f 636f 6d70 6c65  utures.as_comple
-0000e050: 7465 6428 6675 7475 7265 7329 3a0d 0a20  ted(futures):.. 
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e080: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-0000e090: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
-0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0c0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000e0d0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000e0e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e110: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000e120: 2e76 616c 7565 203d 2020 7365 6c66 2e63  .value =  self.c
-0000e130: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
-0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2020 2020 2020 2020 722e 7265 7375            r.resu
-0000e160: 6c74 2829 2020 2020 0d0a 0d0a 2020 2020  lt()    ....    
-0000e170: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-0000e180: 4974 6572 6174 696e 6720 6f76 6572 2074  Iterating over t
-0000e190: 7261 636b 7320 7b6c 656e 2873 656c 662e  racks {len(self.
-0000e1a0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000e1b0: 6473 297d 2729 2020 0d0a 2020 2020 2020  ds)}')  ..      
-0000e1c0: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000e1d0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-0000e1e0: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-0000e1f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e200: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000e210: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-0000e220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e230: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-0000e240: 2e6c 6162 656c 203d 2022 436f 6c6c 6563  .label = "Collec
-0000e250: 7469 6e67 2054 7261 636b 7322 0d0a 2020  ting Tracks"..  
-0000e260: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e270: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000e280: 7261 6e67 6520 3d20 2830 2c20 6c65 6e28  range = (0, len(
-0000e290: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-0000e2a0: 6163 6b5f 6964 7329 290d 0a20 2020 2020  ack_ids))..     
-0000e2b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e2c0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-0000e2d0: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-0000e2e0: 2020 2066 6f72 2074 7261 636b 2069 6e20     for track in 
-0000e2f0: 7365 6c66 2e74 7261 636b 732e 6669 6e64  self.tracks.find
-0000e300: 616c 6c28 2754 7261 636b 2729 3a0d 0a20  all('Track'):.. 
-0000e310: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000e320: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
-0000e330: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
-0000e340: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
-0000e350: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000e360: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
-0000e370: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-0000e380: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
-0000e390: 2020 2020 2020 2020 2073 656c 662e 5f6d           self._m
-0000e3a0: 6173 7465 725f 7472 6163 6b5f 636f 6d70  aster_track_comp
-0000e3b0: 7574 6572 2874 7261 636b 2c20 7472 6163  uter(track, trac
-0000e3c0: 6b5f 6964 290d 0a20 2020 2020 2020 2020  k_id)..         
-0000e3d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e3e0: 636f 756e 7420 2b3d 2031 0d0a 2020 2020  count += 1..    
-0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e400: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000e410: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000e420: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000e430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e440: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-0000e450: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-0000e460: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000e470: 7365 6c66 2e63 6861 6e6e 656c 5f73 6567  self.channel_seg
-0000e480: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
-0000e490: 6e65 3a20 200d 0a20 2020 2020 2020 2020  ne:  ..         
-0000e4a0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-0000e4d0: 6174 655f 7365 636f 6e64 5f63 6861 6e6e  ate_second_chann
-0000e4e0: 656c 5f78 6d6c 2829 0d0a 2020 2020 2020  el_xml()..      
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e500: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000e510: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
-0000e520: 2073 656c 662e 6772 6170 685f 7370 6c69   self.graph_spli
-0000e530: 742e 6974 656d 7328 293a 0d0a 2020 2020  t.items():..    
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfe0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000dff0: 722e 7368 6f77 2829 0d0a 0d0a 2020 2020  r.show()....    
+0000e000: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e010: 7220 696e 2063 6f6e 6375 7272 656e 742e  r in concurrent.
+0000e020: 6675 7475 7265 732e 6173 5f63 6f6d 706c  futures.as_compl
+0000e030: 6574 6564 2866 7574 7572 6573 293a 0d0a  eted(futures):..
+0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e060: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+0000e070: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+0000e080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0a0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+0000e0b0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+0000e0c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000e100: 722e 7661 6c75 6520 3d20 2073 656c 662e  r.value =  self.
+0000e110: 636f 756e 740d 0a20 2020 2020 2020 2020  count..         
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 2020 2020 2020 2020 2072 2e72 6573             r.res
+0000e140: 756c 7428 2920 2020 200d 0a0d 0a20 2020  ult()    ....   
+0000e150: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0000e160: 2749 7465 7261 7469 6e67 206f 7665 7220  'Iterating over 
+0000e170: 7472 6163 6b73 207b 6c65 6e28 7365 6c66  tracks {len(self
+0000e180: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000e190: 6964 7329 7d27 2920 200d 0a20 2020 2020  ids)}')  ..     
+0000e1a0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000e1b0: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
+0000e1c0: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+0000e1d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000e1e0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000e1f0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e210: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+0000e220: 722e 6c61 6265 6c20 3d20 2243 6f6c 6c65  r.label = "Colle
+0000e230: 6374 696e 6720 5472 6163 6b73 220d 0a20  cting Tracks".. 
+0000e240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e250: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000e260: 2e72 616e 6765 203d 2028 302c 206c 656e  .range = (0, len
+0000e270: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
+0000e280: 7261 636b 5f69 6473 2929 0d0a 2020 2020  rack_ids))..    
+0000e290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e2a0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+0000e2b0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
+0000e2c0: 2020 2020 666f 7220 7472 6163 6b20 696e      for track in
+0000e2d0: 2073 656c 662e 7472 6163 6b73 2e66 696e   self.tracks.fin
+0000e2e0: 6461 6c6c 2827 5472 6163 6b27 293a 0d0a  dall('Track'):..
+0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e300: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
+0000e310: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
+0000e320: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
+0000e330: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000e340: 7472 6163 6b5f 6964 2069 6e20 7365 6c66  track_id in self
+0000e350: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
+0000e360: 6964 733a 0d0a 2020 2020 2020 2020 2020  ids:..          
+0000e370: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000e380: 6d61 7374 6572 5f74 7261 636b 5f63 6f6d  master_track_com
+0000e390: 7075 7465 7228 7472 6163 6b2c 2074 7261  puter(track, tra
+0000e3a0: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
+0000e3b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e3c0: 2e63 6f75 6e74 202b 3d20 310d 0a20 2020  .count += 1..   
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000e3f0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000e400: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e420: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+0000e430: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+0000e440: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000e450: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000e460: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000e470: 6f6e 653a 2020 0d0a 2020 2020 2020 2020  one:  ..        
+0000e480: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000e490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e4a0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0000e4b0: 6561 7465 5f73 6563 6f6e 645f 6368 616e  eate_second_chan
+0000e4c0: 6e65 6c5f 786d 6c28 290d 0a20 2020 2020  nel_xml()..     
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0000e4f0: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
+0000e500: 6e20 7365 6c66 2e67 7261 7068 5f73 706c  n self.graph_spl
+0000e510: 6974 2e69 7465 6d73 2829 3a0d 0a20 2020  it.items():..   
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e570: 2020 2020 2064 6175 6768 7465 725f 7472       daughter_tr
-0000e580: 6163 6b5f 6964 203d 2020 696e 7428 666c  ack_id =  int(fl
-0000e590: 6f61 7428 7374 7228 7365 6c66 2e75 6e69  oat(str(self.uni
-0000e5a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000e5b0: 6965 735b 696e 7428 666c 6f61 7428 6b29  ies[int(float(k)
-0000e5c0: 295d 5b73 656c 662e 756e 6971 7565 6964  )][self.uniqueid
-0000e5d0: 5f6b 6579 5d29 2929 0d0a 2020 2020 2020  _key])))..      
-0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5f0: 2020 2020 2020 7061 7265 6e74 5f74 7261        parent_tra
-0000e600: 636b 5f69 6420 3d20 696e 7428 666c 6f61  ck_id = int(floa
-0000e610: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
-0000e620: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-0000e630: 735b 696e 7428 666c 6f61 7428 7629 295d  s[int(float(v))]
-0000e640: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
-0000e650: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 2020 2020 7365 6c66 2e67 7261 7068 5f74      self.graph_t
-0000e680: 7261 636b 735b 6461 7567 6874 6572 5f74  racks[daughter_t
-0000e690: 7261 636b 5f69 645d 203d 2070 6172 656e  rack_id] = paren
-0000e6a0: 745f 7472 6163 6b5f 6964 0d0a 0d0a 2020  t_track_id....  
-0000e6b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000e6c0: 2767 6574 7469 6e67 2061 7474 7269 6275  'getting attribu
-0000e6d0: 7465 7327 2920 2020 2020 2020 2020 2020  tes')           
-0000e6e0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000e6f0: 2020 2073 656c 662e 5f67 6574 5f61 7474     self._get_att
-0000e700: 7269 6275 7465 7328 290d 0a20 2020 2020  ributes()..     
-0000e710: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000e720: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-0000e730: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-0000e740: 666f 7220 696e 6465 782c 2074 7261 636b  for index, track
-0000e750: 5f69 6420 696e 2065 6e75 6d65 7261 7465  _id in enumerate
-0000e760: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-0000e770: 7261 636b 5f69 6473 293a 0d0a 2020 2020  rack_ids):..    
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7a0: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-0000e7b0: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-0000e7c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e7f0: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
-0000e800: 656c 203d 2022 4a75 7374 206f 6e65 206d  el = "Just one m
-0000e810: 6f72 6520 7468 696e 6722 0d0a 2020 2020  ore thing"..    
-0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e840: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-0000e850: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
-0000e860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2020 2020 2020 6461 7567 6874 6572 5f74        daughter_t
+0000e560: 7261 636b 5f69 6420 3d20 2069 6e74 2866  rack_id =  int(f
+0000e570: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
+0000e580: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000e590: 7469 6573 5b69 6e74 2866 6c6f 6174 286b  ties[int(float(k
+0000e5a0: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
+0000e5b0: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 2020 2020 2070 6172 656e 745f 7472         parent_tr
+0000e5e0: 6163 6b5f 6964 203d 2069 6e74 2866 6c6f  ack_id = int(flo
+0000e5f0: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
+0000e600: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000e610: 6573 5b69 6e74 2866 6c6f 6174 2876 2929  es[int(float(v))
+0000e620: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
+0000e630: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 2020 2073 656c 662e 6772 6170 685f       self.graph_
+0000e660: 7472 6163 6b73 5b64 6175 6768 7465 725f  tracks[daughter_
+0000e670: 7472 6163 6b5f 6964 5d20 3d20 7061 7265  track_id] = pare
+0000e680: 6e74 5f74 7261 636b 5f69 640d 0a0d 0a20  nt_track_id.... 
+0000e690: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000e6a0: 2827 6765 7474 696e 6720 6174 7472 6962  ('getting attrib
+0000e6b0: 7574 6573 2729 2020 2020 2020 2020 2020  utes')          
+0000e6c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000e6d0: 2020 2020 7365 6c66 2e5f 6765 745f 6174      self._get_at
+0000e6e0: 7472 6962 7574 6573 2829 0d0a 2020 2020  tributes()..    
+0000e6f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000e700: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
+0000e710: 3d20 300d 0a20 2020 2020 2020 2020 2020  = 0..           
+0000e720: 2066 6f72 2069 6e64 6578 2c20 7472 6163   for index, trac
+0000e730: 6b5f 6964 2069 6e20 656e 756d 6572 6174  k_id in enumerat
+0000e740: 6528 7365 6c66 2e66 696c 7465 7265 645f  e(self.filtered_
+0000e750: 7472 6163 6b5f 6964 7329 3a0d 0a20 2020  track_ids):..   
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e780: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+0000e790: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+0000e7a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e7d0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
+0000e7e0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
+0000e7f0: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e820: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+0000e830: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+0000e840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e870: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
 0000e880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e890: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
-0000e8d0: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
-0000e8e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8a0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
+0000e8b0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+0000e8c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8f0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
 0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e910: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e940: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-0000e950: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
-0000e960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e980: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
-0000e990: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000e9d0: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
-0000e9e0: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 2020 2020 2020 2020 7472 6163              trac
-0000ea10: 6b20 3d20 7365 6c66 2e66 696c 7465 7265  k = self.filtere
-0000ea20: 645f 7472 6163 6b73 5b69 6e64 6578 5d20  d_tracks[index] 
-0000ea30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
-0000ea60: 696e 616c 5f74 7261 636b 7328 7472 6163  inal_tracks(trac
-0000ea70: 6b2c 2074 7261 636b 5f69 6429 200d 0a0d  k, track_id) ...
-0000ea80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000ea90: 7365 6c66 2e66 6f75 7269 6572 3a0d 0a20  self.fourier:.. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eab0: 2020 7072 696e 7428 2763 6f6d 7075 7469    print('computi
-0000eac0: 6e67 2046 6f75 7269 6572 2729 0d0a 2020  ng Fourier')..  
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2073 656c 662e 5f63 6f6d 7075 7465 5f70   self._compute_p
-0000eaf0: 6865 6e6f 7479 7065 7328 2920 2020 2020  henotypes()     
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000eb20: 2073 656c 662e 5f74 656d 706f 7261 6c5f   self._temporal_
-0000eb30: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
-0000eb40: 2920 2020 2020 2020 200d 0a0d 0a0d 0a20  )        ...... 
-0000eb50: 2020 2064 6566 205f 6372 6561 7465 5f73     def _create_s
-0000eb60: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-0000eb70: 6c28 7365 6c66 293a 0d0a 2020 2020 2020  l(self):..      
-0000eb80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000eb90: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000eba0: 2827 5472 616e 7366 6572 7269 6e67 2058  ('Transferring X
-0000ebb0: 4d4c 2729 2020 200d 0a20 2020 2020 2020  ML')   ..       
-0000ebc0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-0000ebd0: 6e6e 656c 5f66 696c 7465 7265 645f 7472  nnel_filtered_tr
-0000ebe0: 6163 6b73 203d 205b 5d20 2020 2020 2020  acks = []       
-0000ebf0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000ec00: 2020 2020 2020 2020 2020 2066 6f72 2053             for S
-0000ec10: 706f 746f 626a 6563 7420 696e 2073 656c  potobject in sel
-0000ec20: 662e 786d 6c5f 726f 6f74 2e69 7465 7228  f.xml_root.iter(
-0000ec30: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
-0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec50: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
-0000ec60: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
-0000ec70: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
-0000ec80: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 6966 2063 656c 6c5f 6964 2069 6e20    if cell_id in 
-0000ecb0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000ecc0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000ecd0: 6965 732e 6b65 7973 2829 3a20 2020 2020  ies.keys():     
-0000ece0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e920: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+0000e930: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
+0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e950: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e960: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
+0000e970: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000e9b0: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
+0000e9c0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
+0000e9f0: 636b 203d 2073 656c 662e 6669 6c74 6572  ck = self.filter
+0000ea00: 6564 5f74 7261 636b 735b 696e 6465 785d  ed_tracks[index]
+0000ea10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000ea40: 6669 6e61 6c5f 7472 6163 6b73 2874 7261  final_tracks(tra
+0000ea50: 636b 2c20 7472 6163 6b5f 6964 2920 0d0a  ck, track_id) ..
+0000ea60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000ea70: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
+0000eaa0: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
+0000ead0: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
+0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaf0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000eb00: 2020 7365 6c66 2e5f 7465 6d70 6f72 616c    self._temporal
+0000eb10: 5f70 6c6f 7473 5f74 7261 636b 6d61 7465  _plots_trackmate
+0000eb20: 2829 2020 2020 2020 2020 0d0a 0d0a 0d0a  ()        ......
+0000eb30: 2020 2020 6465 6620 5f63 7265 6174 655f      def _create_
+0000eb40: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
+0000eb50: 6d6c 2873 656c 6629 3a0d 0a20 2020 2020  ml(self):..     
+0000eb60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000eb70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000eb80: 7428 2754 7261 6e73 6665 7272 696e 6720  t('Transferring 
+0000eb90: 584d 4c27 2920 2020 0d0a 2020 2020 2020  XML')   ..      
+0000eba0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+0000ebb0: 616e 6e65 6c5f 6669 6c74 6572 6564 5f74  annel_filtered_t
+0000ebc0: 7261 636b 7320 3d20 5b5d 2020 2020 2020  racks = []      
+0000ebd0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000ebe0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000ebf0: 5370 6f74 6f62 6a65 6374 2069 6e20 7365  Spotobject in se
+0000ec00: 6c66 2e78 6d6c 5f72 6f6f 742e 6974 6572  lf.xml_root.iter
+0000ec10: 2827 5370 6f74 2729 3a0d 0a20 2020 2020  ('Spot'):..     
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
+0000ec40: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
+0000ec50: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
+0000ec60: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 2020 2069 6620 6365 6c6c 5f69 6420 696e     if cell_id in
+0000ec90: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000eca0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000ecb0: 7469 6573 2e6b 6579 7328 293a 2020 2020  ties.keys():    
+0000ecc0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ece0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed20: 2020 2020 2020 206e 6577 5f70 6f73 6974         new_posit
-0000ed30: 696f 6e78 203d 2020 7365 6c66 2e63 6861  ionx =  self.cha
-0000ed40: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000ed50: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000ed60: 5f69 645d 5b73 656c 662e 7870 6f73 6964  _id][self.xposid
-0000ed70: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 2020 2020 2020 2020 206e 6577 5f70             new_p
-0000eda0: 6f73 6974 696f 6e79 203d 2020 7365 6c66  ositiony =  self
-0000edb0: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000edc0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000edd0: 6365 6c6c 5f69 645d 5b73 656c 662e 7970  cell_id][self.yp
-0000ede0: 6f73 6964 5f6b 6579 5d0d 0a20 2020 2020  osid_key]..     
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000ee10: 6577 5f70 6f73 6974 696f 6e7a 203d 2020  ew_positionz =  
-0000ee20: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000ee30: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000ee40: 6965 735b 6365 6c6c 5f69 645d 5b73 656c  ies[cell_id][sel
-0000ee50: 662e 7a70 6f73 6964 5f6b 6579 5d0d 0a0d  f.zposid_key]...
-0000ee60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2020 2020 206e 6577 5f74 6f74 616c 5f69       new_total_i
-0000ee90: 6e74 656e 7369 7479 203d 2073 656c 662e  ntensity = self.
-0000eea0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
-0000eeb0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-0000eec0: 656c 6c5f 6964 5d5b 7365 6c66 2e74 6f74  ell_id][self.tot
-0000eed0: 616c 5f69 6e74 656e 7369 7479 5f6b 6579  al_intensity_key
-0000eee0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef00: 2020 2020 2020 206e 6577 5f6d 6561 6e5f         new_mean_
-0000ef10: 696e 7465 6e73 6974 7920 3d20 7365 6c66  intensity = self
-0000ef20: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-0000ef30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-0000ef40: 6365 6c6c 5f69 645d 5b73 656c 662e 6d65  cell_id][self.me
-0000ef50: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
-0000ef60: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef80: 2020 2020 2020 2020 206e 6577 5f72 6164           new_rad
-0000ef90: 6975 7320 3d20 7365 6c66 2e63 6861 6e6e  ius = self.chann
-0000efa0: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000efb0: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000efc0: 645d 5b73 656c 662e 7261 6469 7573 5f6b  d][self.radius_k
-0000efd0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
-0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eff0: 2020 2020 2020 2020 206e 6577 5f71 7561           new_qua
-0000f000: 6c69 7479 203d 2073 656c 662e 6368 616e  lity = self.chan
-0000f010: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-0000f020: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-0000f030: 6964 5d5b 7365 6c66 2e71 7561 6c69 7479  id][self.quality
-0000f040: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
-0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f060: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
-0000f070: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-0000f080: 6b20 3d20 7365 6c66 2e63 6861 6e6e 656c  k = self.channel
-0000f090: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000f0a0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000f0b0: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
-0000f0c0: 656c 6c5f 6d61 736b 5f6b 6579 5d0d 0a0d  ell_mask_key]...
-0000f0d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000f100: 7365 7428 7365 6c66 2e78 706f 7369 645f  set(self.xposid_
-0000f110: 6b65 792c 2073 7472 286e 6577 5f70 6f73  key, str(new_pos
-0000f120: 6974 696f 6e78 2929 2020 2020 200d 0a20  itionx))     .. 
-0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
-0000f160: 7428 7365 6c66 2e79 706f 7369 645f 6b65  t(self.yposid_ke
-0000f170: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
-0000f180: 696f 6e79 2929 0d0a 2020 2020 2020 2020  iony))..        
-0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1a0: 2020 2020 2020 2020 2020 2020 5370 6f74              Spot
-0000f1b0: 6f62 6a65 6374 2e73 6574 2873 656c 662e  object.set(self.
-0000f1c0: 7a70 6f73 6964 5f6b 6579 2c20 7374 7228  zposid_key, str(
-0000f1d0: 6e65 775f 706f 7369 7469 6f6e 7a29 290d  new_positionz)).
-0000f1e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f200: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000f210: 742e 7365 7428 7365 6c66 2e74 6f74 616c  t.set(self.total
-0000f220: 5f69 6e74 656e 7369 7479 5f6b 6579 2c20  _intensity_key, 
-0000f230: 7374 7228 6e65 775f 746f 7461 6c5f 696e  str(new_total_in
-0000f240: 7465 6e73 6974 7929 2920 2020 2020 0d0a  tensity))     ..
-0000f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f270: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000f280: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000f290: 656e 7369 7479 5f6b 6579 2c20 7374 7228  ensity_key, str(
-0000f2a0: 6e65 775f 6d65 616e 5f69 6e74 656e 7369  new_mean_intensi
-0000f2b0: 7479 2929 0d0a 2020 2020 2020 2020 2020  ty))..          
-0000f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2d0: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000f2e0: 6a65 6374 2e73 6574 2873 656c 662e 7261  ject.set(self.ra
-0000f2f0: 6469 7573 5f6b 6579 2c20 7374 7228 6e65  dius_key, str(ne
-0000f300: 775f 7261 6469 7573 2929 2020 2020 200d  w_radius))     .
-0000f310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f330: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-0000f340: 7365 7428 7365 6c66 2e71 7561 6c69 7479  set(self.quality
-0000f350: 5f6b 6579 2c20 7374 7228 6e65 775f 7175  _key, str(new_qu
-0000f360: 616c 6974 7929 290d 0a20 2020 2020 2020  ality))..       
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
-0000f390: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
-0000f3a0: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-0000f3b0: 6173 6b5f 6b65 792c 2073 7472 286e 6577  ask_key, str(new
-0000f3c0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-0000f3d0: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3f0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-0000f400: 5f69 6420 3d20 7365 6c66 2e63 6861 6e6e  _id = self.chann
-0000f410: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-0000f420: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-0000f430: 6c6c 5f69 6429 5d5b 7365 6c66 2e74 7261  ll_id)][self.tra
-0000f440: 636b 6964 5f6b 6579 5d0d 0a20 2020 2020  ckid_key]..     
-0000f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f470: 6861 6e6e 656c 5f66 696c 7465 7265 645f  hannel_filtered_
-0000f480: 7472 6163 6b73 2e61 7070 656e 6428 7472  tracks.append(tr
-0000f490: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
+0000ed00: 2020 2020 2020 2020 6e65 775f 706f 7369          new_posi
+0000ed10: 7469 6f6e 7820 3d20 2073 656c 662e 6368  tionx =  self.ch
+0000ed20: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+0000ed30: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+0000ed40: 6c5f 6964 5d5b 7365 6c66 2e78 706f 7369  l_id][self.xposi
+0000ed50: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed70: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000ed80: 706f 7369 7469 6f6e 7920 3d20 2073 656c  positiony =  sel
+0000ed90: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000eda0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000edb0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e79  [cell_id][self.y
+0000edc0: 706f 7369 645f 6b65 795d 0d0a 2020 2020  posid_key]..    
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edf0: 6e65 775f 706f 7369 7469 6f6e 7a20 3d20  new_positionz = 
+0000ee00: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
+0000ee10: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+0000ee20: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
+0000ee30: 6c66 2e7a 706f 7369 645f 6b65 795d 0d0a  lf.zposid_key]..
+0000ee40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee60: 2020 2020 2020 6e65 775f 746f 7461 6c5f        new_total_
+0000ee70: 696e 7465 6e73 6974 7920 3d20 7365 6c66  intensity = self
+0000ee80: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+0000ee90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+0000eea0: 6365 6c6c 5f69 645d 5b73 656c 662e 746f  cell_id][self.to
+0000eeb0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
+0000eec0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
+0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eee0: 2020 2020 2020 2020 6e65 775f 6d65 616e          new_mean
+0000eef0: 5f69 6e74 656e 7369 7479 203d 2073 656c  _intensity = sel
+0000ef00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+0000ef10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+0000ef20: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e6d  [cell_id][self.m
+0000ef30: 6561 6e5f 696e 7465 6e73 6974 795f 6b65  ean_intensity_ke
+0000ef40: 795d 0d0a 0d0a 2020 2020 2020 2020 2020  y]....          
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 2020 2020 2020 2020 2020 6e65 775f 7261            new_ra
+0000ef70: 6469 7573 203d 2073 656c 662e 6368 616e  dius = self.chan
+0000ef80: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000ef90: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000efa0: 6964 5d5b 7365 6c66 2e72 6164 6975 735f  id][self.radius_
+0000efb0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efd0: 2020 2020 2020 2020 2020 6e65 775f 7175            new_qu
+0000efe0: 616c 6974 7920 3d20 7365 6c66 2e63 6861  ality = self.cha
+0000eff0: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+0000f000: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+0000f010: 5f69 645d 5b73 656c 662e 7175 616c 6974  _id][self.qualit
+0000f020: 795f 6b65 795d 0d0a 2020 2020 2020 2020  y_key]..        
+0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f040: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+0000f050: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+0000f060: 736b 203d 2073 656c 662e 6368 616e 6e65  sk = self.channe
+0000f070: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+0000f080: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000f090: 5d5b 7365 6c66 2e64 6973 7461 6e63 655f  ][self.distance_
+0000f0a0: 6365 6c6c 5f6d 6173 6b5f 6b65 795d 0d0a  cell_mask_key]..
+0000f0b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+0000f0e0: 2e73 6574 2873 656c 662e 7870 6f73 6964  .set(self.xposid
+0000f0f0: 5f6b 6579 2c20 7374 7228 6e65 775f 706f  _key, str(new_po
+0000f100: 7369 7469 6f6e 7829 2920 2020 2020 0d0a  sitionx))     ..
+0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f130: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
+0000f140: 6574 2873 656c 662e 7970 6f73 6964 5f6b  et(self.yposid_k
+0000f150: 6579 2c20 7374 7228 6e65 775f 706f 7369  ey, str(new_posi
+0000f160: 7469 6f6e 7929 290d 0a20 2020 2020 2020  tiony))..       
+0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f180: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+0000f190: 746f 626a 6563 742e 7365 7428 7365 6c66  tobject.set(self
+0000f1a0: 2e7a 706f 7369 645f 6b65 792c 2073 7472  .zposid_key, str
+0000f1b0: 286e 6577 5f70 6f73 6974 696f 6e7a 2929  (new_positionz))
+0000f1c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1e0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
+0000f1f0: 6374 2e73 6574 2873 656c 662e 746f 7461  ct.set(self.tota
+0000f200: 6c5f 696e 7465 6e73 6974 795f 6b65 792c  l_intensity_key,
+0000f210: 2073 7472 286e 6577 5f74 6f74 616c 5f69   str(new_total_i
+0000f220: 6e74 656e 7369 7479 2929 2020 2020 200d  ntensity))     .
+0000f230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f250: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000f260: 7365 7428 7365 6c66 2e6d 6561 6e5f 696e  set(self.mean_in
+0000f270: 7465 6e73 6974 795f 6b65 792c 2073 7472  tensity_key, str
+0000f280: 286e 6577 5f6d 6561 6e5f 696e 7465 6e73  (new_mean_intens
+0000f290: 6974 7929 290d 0a20 2020 2020 2020 2020  ity))..         
+0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2b0: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000f2c0: 626a 6563 742e 7365 7428 7365 6c66 2e72  bject.set(self.r
+0000f2d0: 6164 6975 735f 6b65 792c 2073 7472 286e  adius_key, str(n
+0000f2e0: 6577 5f72 6164 6975 7329 2920 2020 2020  ew_radius))     
+0000f2f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f310: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+0000f320: 2e73 6574 2873 656c 662e 7175 616c 6974  .set(self.qualit
+0000f330: 795f 6b65 792c 2073 7472 286e 6577 5f71  y_key, str(new_q
+0000f340: 7561 6c69 7479 2929 0d0a 2020 2020 2020  uality))..      
+0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f360: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
+0000f370: 6f74 6f62 6a65 6374 2e73 6574 2873 656c  otobject.set(sel
+0000f380: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+0000f390: 6d61 736b 5f6b 6579 2c20 7374 7228 6e65  mask_key, str(ne
+0000f3a0: 775f 6469 7374 616e 6365 5f63 656c 6c5f  w_distance_cell_
+0000f3b0: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
+0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3d0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+0000f3e0: 6b5f 6964 203d 2073 656c 662e 6368 616e  k_id = self.chan
+0000f3f0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+0000f400: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+0000f410: 656c 6c5f 6964 295d 5b73 656c 662e 7472  ell_id)][self.tr
+0000f420: 6163 6b69 645f 6b65 795d 0d0a 2020 2020  ackid_key]..    
+0000f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f450: 6368 616e 6e65 6c5f 6669 6c74 6572 6564  channel_filtered
+0000f460: 5f74 7261 636b 732e 6170 7065 6e64 2874  _tracks.append(t
+0000f470: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4d0: 2020 2073 656c 662e 786d 6c5f 7472 6565     self.xml_tree
-0000f4e0: 2e77 7269 7465 286f 732e 7061 7468 2e6a  .write(os.path.j
-0000f4f0: 6f69 6e28 7365 6c66 2e63 6861 6e6e 656c  oin(self.channel
-0000f500: 5f78 6d6c 5f70 6174 682c 2073 656c 662e  _xml_path, self.
-0000f510: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
-0000f520: 2929 200d 0a0d 0a20 2020 2064 6566 205f  )) ....    def _
-0000f530: 6765 745f 786d 6c5f 6461 7461 2873 656c  get_xml_data(sel
-0000f540: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
-0000f550: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-0000f560: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f570: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
-0000f580: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
-0000f590: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000f5a0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-0000f5b0: 616e 6e65 6c5f 786d 6c5f 636f 6e74 656e  annel_xml_conten
-0000f5c0: 7420 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  t = self.xml_con
-0000f5d0: 7465 6e74 0d0a 2020 2020 2020 2020 2020  tent..          
-0000f5e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f5f0: 2e78 6d6c 5f74 7265 6520 3d20 6574 2e70  .xml_tree = et.p
-0000f600: 6172 7365 2873 656c 662e 786d 6c5f 7061  arse(self.xml_pa
-0000f610: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-0000f620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f630: 786d 6c5f 726f 6f74 203d 2073 656c 662e  xml_root = self.
-0000f640: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
-0000f650: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0000f660: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f670: 6861 6e6e 656c 5f78 6d6c 5f6e 616d 6520  hannel_xml_name 
-0000f680: 3d20 2773 6563 6f6e 645f 6368 616e 6e65  = 'second_channe
-0000f690: 6c5f 2720 2b20 6f73 2e70 6174 682e 7370  l_' + os.path.sp
-0000f6a0: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
-0000f6b0: 6173 656e 616d 6528 7365 6c66 2e78 6d6c  asename(self.xml
-0000f6c0: 5f70 6174 6829 295b 305d 202b 2027 2e78  _path))[0] + '.x
-0000f6d0: 6d6c 270d 0a20 2020 2020 2020 2020 2020  ml'..           
-0000f6e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f6f0: 6368 616e 6e65 6c5f 786d 6c5f 7061 7468  channel_xml_path
-0000f700: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-0000f710: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000f720: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f730: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-0000f740: 7265 6174 655f 6368 616e 6e65 6c5f 7472  reate_channel_tr
-0000f750: 6565 2829 0d0a 2020 2020 2020 2020 2020  ee()..          
-0000f760: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
-0000f770: 746f 656e 636f 6465 725f 6d6f 6465 6c20  toencoder_model 
-0000f780: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000f790: 7365 6c66 2e73 6567 5f69 6d61 6765 2069  self.seg_image i
-0000f7a0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-0000f7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7c0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000f7d0: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
-0000f7e0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f800: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-0000f810: 6572 5f78 6d6c 5f74 7265 6520 3d20 6574  er_xml_tree = et
-0000f820: 2e70 6172 7365 2873 656c 662e 786d 6c5f  .parse(self.xml_
-0000f830: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000f840: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f850: 6c66 2e6d 6173 7465 725f 786d 6c5f 726f  lf.master_xml_ro
-0000f860: 6f74 203d 2073 656c 662e 6d61 7374 6572  ot = self.master
-0000f870: 5f78 6d6c 5f74 7265 652e 6765 7472 6f6f  _xml_tree.getroo
-0000f880: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000f890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f8a0: 2e6d 6173 7465 725f 786d 6c5f 6e61 6d65  .master_xml_name
-0000f8b0: 203d 2027 6d61 7374 6572 5f27 202b 2073   = 'master_' + s
-0000f8c0: 656c 662e 6d61 7374 6572 5f65 7874 7261  elf.master_extra
-0000f8d0: 5f6e 616d 6520 202b 206f 732e 7061 7468  _name  + os.path
-0000f8e0: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
-0000f8f0: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
-0000f900: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
-0000f910: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
-0000f920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f930: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-0000f940: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
-0000f950: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
-0000f960: 6174 6829 2020 2020 2020 0d0a 2020 2020  ath)      ..    
-0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f980: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000f990: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000f9a0: 5f6f 626a 6563 7473 203d 207b 7d0d 0a20  _objects = {}.. 
-0000f9b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f9c0: 656c 662e 756e 6971 7565 5f70 726f 7065  elf.unique_prope
-0000f9d0: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-0000f9e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f9f0: 2e41 6c6c 5472 6163 6b49 6473 203d 205b  .AllTrackIds = [
-0000fa00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000fa10: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000fa20: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000fa30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fa40: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-0000fa50: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000fa60: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-0000fa70: 6c5f 7472 6163 6b5f 7072 6f70 6572 7469  l_track_properti
-0000fa80: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000fa90: 2020 2020 2020 2020 2073 656c 662e 7370           self.sp
-0000faa0: 6c69 745f 706f 696e 7473 5f74 696d 6573  lit_points_times
-0000fab0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-0000fac0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000fad0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000fae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000faf0: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-0000fb00: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
-0000fb10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fb20: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000fb30: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
-0000fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fb50: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000fb60: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000fb70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fb80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000fb90: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-0000fba0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000fbb0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fbd0: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000fbe0: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000fbf0: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000fc00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fc10: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-0000fc20: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000fc30: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000fc40: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fc50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fc70: 6c66 2e53 706f 746f 626a 6563 7473 203d  lf.Spotobjects =
-0000fc80: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000fc90: 742e 6669 6e64 2827 4d6f 6465 6c27 292e  t.find('Model').
-0000fca0: 6669 6e64 2827 416c 6c53 706f 7473 2729  find('AllSpots')
-0000fcb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fcc0: 2020 2320 4578 7472 6163 7420 7468 6520    # Extract the 
-0000fcd0: 7472 6163 6b73 2066 726f 6d20 786d 6c0d  tracks from xml.
-0000fce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fcf0: 2073 656c 662e 7472 6163 6b73 203d 2073   self.tracks = s
-0000fd00: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000fd10: 6669 6e64 2822 4d6f 6465 6c22 292e 6669  find("Model").fi
-0000fd20: 6e64 2822 416c 6c54 7261 636b 7322 290d  nd("AllTracks").
-0000fd30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd40: 2073 656c 662e 7365 7474 696e 6773 203d   self.settings =
-0000fd50: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000fd60: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000fd70: 2229 2e66 696e 6428 2249 6d61 6765 4461  ").find("ImageDa
-0000fd80: 7461 2229 0d0a 2020 2020 2020 2020 2020  ta")..          
-0000fd90: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
-0000fda0: 7369 7a65 203d 2028 696e 7428 666c 6f61  size = (int(floa
-0000fdb0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
-0000fdc0: 6765 7428 226e 6672 616d 6573 2229 2929  get("nframes")))
-0000fdd0: 2c69 6e74 2866 6c6f 6174 2873 656c 662e  ,int(float(self.
-0000fde0: 7365 7474 696e 6773 2e67 6574 2822 6e73  settings.get("ns
-0000fdf0: 6c69 6365 7322 2929 292c 696e 7428 666c  lices"))),int(fl
-0000fe00: 6f61 7428 7365 6c66 2e73 6574 7469 6e67  oat(self.setting
-0000fe10: 732e 6765 7428 2268 6569 6768 7422 2929  s.get("height"))
-0000fe20: 292c 2020 696e 7428 666c 6f61 7428 7365  ),  int(float(se
-0000fe30: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
-0000fe40: 2277 6964 7468 2229 2929 290d 0a20 2020  "width"))))..   
-0000fe50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000fe60: 6e74 2866 2758 4d4c 2066 696c 6520 6d61  nt(f'XML file ma
-0000fe70: 6465 2075 7369 6e67 2069 6d61 6765 206f  de using image o
-0000fe80: 6620 7b73 656c 662e 696d 6167 6573 697a  f {self.imagesiz
-0000fe90: 657d 2729 0d0a 2020 2020 2020 2020 2020  e}')..          
-0000fea0: 2020 2020 2020 7365 6c66 2e78 6361 6c69        self.xcali
-0000feb0: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000fec0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000fed0: 7428 2270 6978 656c 7769 6474 6822 2929  t("pixelwidth"))
-0000fee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fef0: 2020 7365 6c66 2e79 6361 6c69 6272 6174    self.ycalibrat
-0000ff00: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
-0000ff10: 2e73 6574 7469 6e67 732e 6765 7428 2270  .settings.get("p
-0000ff20: 6978 656c 6865 6967 6874 2229 290d 0a20  ixelheight")).. 
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ff40: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-0000ff50: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
-0000ff60: 7474 696e 6773 2e67 6574 2822 766f 7865  ttings.get("voxe
-0000ff70: 6c64 6570 7468 2229 290d 0a20 2020 2020  ldepth"))..     
-0000ff80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ff90: 7463 616c 6962 7261 7469 6f6e 203d 2069  tcalibration = i
-0000ffa0: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
-0000ffb0: 7474 696e 6773 2e67 6574 2822 7469 6d65  ttings.get("time
-0000ffc0: 696e 7465 7276 616c 2229 2929 0d0a 2020  interval")))..  
-0000ffd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ffe0: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000fff0: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-00010000: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-00010010: 7469 6e67 7322 292e 6669 6e64 2822 4465  tings").find("De
-00010020: 7465 6374 6f72 5365 7474 696e 6773 2229  tectorSettings")
-00010030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010040: 2020 7365 6c66 2e62 6173 6963 7365 7474    self.basicsett
-00010050: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-00010060: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-00010070: 7474 696e 6773 2229 2e66 696e 6428 2242  ttings").find("B
-00010080: 6173 6963 5365 7474 696e 6773 2229 0d0a  asicSettings")..
-00010090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100a0: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
-000100b0: 6e6e 656c 203d 2069 6e74 2866 6c6f 6174  nnel = int(float
-000100c0: 2873 656c 662e 6465 7465 6374 6f72 7365  (self.detectorse
-000100d0: 7474 696e 6773 2e67 6574 2822 5441 5247  ttings.get("TARG
-000100e0: 4554 5f43 4841 4e4e 454c 2229 2929 0d0a  ET_CHANNEL")))..
-000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010100: 7365 6c66 2e74 7374 6172 7420 3d20 696e  self.tstart = in
-00010110: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
-00010120: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
-00010130: 7473 7461 7274 2229 2929 0d0a 2020 2020  tstart")))..    
-00010140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010150: 2e74 656e 6420 3d20 696e 7428 666c 6f61  .tend = int(floa
-00010160: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
-00010170: 696e 6773 2e67 6574 2822 7465 6e64 2229  ings.get("tend")
-00010180: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00010190: 2020 2020 7365 6c66 2e5f 6765 745f 626f      self._get_bo
-000101a0: 756e 6461 7279 5f70 6f69 6e74 7328 290d  undary_points().
-000101b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101c0: 2070 7269 6e74 2827 4974 6572 6174 696e   print('Iteratin
-000101d0: 6720 6f76 6572 2073 706f 7473 2069 6e20  g over spots in 
-000101e0: 6672 616d 6527 290d 0a20 2020 2020 2020  frame')..       
-000101f0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010200: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-00010210: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00010220: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00010230: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-00010240: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-00010250: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-00010260: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-00010270: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-00010280: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
-00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000102b0: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
-000102c0: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
-000102d0: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
-000102e0: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
-000102f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010310: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-00010320: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-00010330: 6c66 2e5f 7370 6f74 5f63 6f6d 7075 7465  lf._spot_compute
-00010340: 722c 2066 7261 6d65 2929 0d0a 2020 2020  r, frame))..    
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00010370: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00010380: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f4b0: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
+0000f4c0: 652e 7772 6974 6528 6f73 2e70 6174 682e  e.write(os.path.
+0000f4d0: 6a6f 696e 2873 656c 662e 6368 616e 6e65  join(self.channe
+0000f4e0: 6c5f 786d 6c5f 7061 7468 2c20 7365 6c66  l_xml_path, self
+0000f4f0: 2e63 6861 6e6e 656c 5f78 6d6c 5f6e 616d  .channel_xml_nam
+0000f500: 6529 2920 0d0a 0d0a 2020 2020 6465 6620  e)) ....    def 
+0000f510: 5f67 6574 5f78 6d6c 5f64 6174 6128 7365  _get_xml_data(se
+0000f520: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
+0000f530: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000f540: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000f550: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
+0000f560: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
+0000f570: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000f580: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000f590: 6861 6e6e 656c 5f78 6d6c 5f63 6f6e 7465  hannel_xml_conte
+0000f5a0: 6e74 203d 2073 656c 662e 786d 6c5f 636f  nt = self.xml_co
+0000f5b0: 6e74 656e 740d 0a20 2020 2020 2020 2020  ntent..         
+0000f5c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f5d0: 662e 786d 6c5f 7472 6565 203d 2065 742e  f.xml_tree = et.
+0000f5e0: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000f5f0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000f600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f610: 2e78 6d6c 5f72 6f6f 7420 3d20 7365 6c66  .xml_root = self
+0000f620: 2e78 6d6c 5f74 7265 652e 6765 7472 6f6f  .xml_tree.getroo
+0000f630: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+0000f640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f650: 6368 616e 6e65 6c5f 786d 6c5f 6e61 6d65  channel_xml_name
+0000f660: 203d 2027 7365 636f 6e64 5f63 6861 6e6e   = 'second_chann
+0000f670: 656c 5f27 202b 206f 732e 7061 7468 2e73  el_' + os.path.s
+0000f680: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+0000f690: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
+0000f6a0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
+0000f6b0: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
+0000f6c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f6d0: 2e63 6861 6e6e 656c 5f78 6d6c 5f70 6174  .channel_xml_pat
+0000f6e0: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
+0000f6f0: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000f700: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+0000f710: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000f720: 6372 6561 7465 5f63 6861 6e6e 656c 5f74  create_channel_t
+0000f730: 7265 6528 290d 0a20 2020 2020 2020 2020  ree()..         
+0000f740: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+0000f750: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
+0000f760: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+0000f770: 2073 656c 662e 7365 675f 696d 6167 6520   self.seg_image 
+0000f780: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7a0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000f7b0: 5f78 6d6c 5f63 6f6e 7465 6e74 203d 2073  _xml_content = s
+0000f7c0: 656c 662e 786d 6c5f 636f 6e74 656e 740d  elf.xml_content.
+0000f7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7e0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+0000f7f0: 7465 725f 786d 6c5f 7472 6565 203d 2065  ter_xml_tree = e
+0000f800: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000f810: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000f820: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f830: 656c 662e 6d61 7374 6572 5f78 6d6c 5f72  elf.master_xml_r
+0000f840: 6f6f 7420 3d20 7365 6c66 2e6d 6173 7465  oot = self.maste
+0000f850: 725f 786d 6c5f 7472 6565 2e67 6574 726f  r_xml_tree.getro
+0000f860: 6f74 2829 0d0a 2020 2020 2020 2020 2020  ot()..          
+0000f870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f880: 662e 6d61 7374 6572 5f78 6d6c 5f6e 616d  f.master_xml_nam
+0000f890: 6520 3d20 276d 6173 7465 725f 2720 2b20  e = 'master_' + 
+0000f8a0: 7365 6c66 2e6d 6173 7465 725f 6578 7472  self.master_extr
+0000f8b0: 615f 6e61 6d65 2020 2b20 6f73 2e70 6174  a_name  + os.pat
+0000f8c0: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
+0000f8d0: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
+0000f8e0: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
+0000f8f0: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f910: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+0000f920: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
+0000f930: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
+0000f940: 7061 7468 2920 2020 2020 200d 0a20 2020  path)      ..   
+0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f960: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000f970: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000f980: 655f 6f62 6a65 6374 7320 3d20 7b7d 0d0a  e_objects = {}..
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 7365 6c66 2e75 6e69 7175 655f 7072 6f70  self.unique_prop
+0000f9b0: 6572 7469 6573 203d 207b 7d0d 0a20 2020  erties = {}..   
+0000f9c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f9d0: 662e 416c 6c54 7261 636b 4964 7320 3d20  f.AllTrackIds = 
+0000f9e0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000f9f0: 2020 2020 7365 6c66 2e44 6976 6964 696e      self.Dividin
+0000fa00: 6754 7261 636b 4964 7320 3d20 5b5d 0d0a  gTrackIds = []..
+0000fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa20: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
+0000fa30: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
+0000fa40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000fa50: 6c6c 5f74 7261 636b 5f70 726f 7065 7274  ll_track_propert
+0000fa60: 6965 7320 3d20 5b5d 0d0a 2020 2020 2020  ies = []..      
+0000fa70: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000fa80: 706c 6974 5f70 6f69 6e74 735f 7469 6d65  plit_points_time
+0000fa90: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000faa0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000fab0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fad0: 6c66 2e41 6c6c 5472 6163 6b49 6473 2e61  lf.AllTrackIds.a
+0000fae0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
+0000faf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fb00: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000fb10: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
+0000fb20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fb30: 2073 656c 662e 4e6f 726d 616c 5472 6163   self.NormalTrac
+0000fb40: 6b49 6473 2e61 7070 656e 6428 4e6f 6e65  kIds.append(None
+0000fb50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fb60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000fb70: 2020 2020 2073 656c 662e 416c 6c54 7261       self.AllTra
+0000fb80: 636b 4964 732e 6170 7065 6e64 2873 656c  ckIds.append(sel
+0000fb90: 662e 5472 6163 6b69 6442 6f78 290d 0a20  f.TrackidBox).. 
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fbb0: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
+0000fbc0: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
+0000fbd0: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fbf0: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000fc00: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
+0000fc10: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
+0000fc20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000fc30: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fc50: 656c 662e 5370 6f74 6f62 6a65 6374 7320  elf.Spotobjects 
+0000fc60: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000fc70: 6e74 2e66 696e 6428 274d 6f64 656c 2729  nt.find('Model')
+0000fc80: 2e66 696e 6428 2741 6c6c 5370 6f74 7327  .find('AllSpots'
+0000fc90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fca0: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
+0000fcb0: 2074 7261 636b 7320 6672 6f6d 2078 6d6c   tracks from xml
+0000fcc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fcd0: 2020 7365 6c66 2e74 7261 636b 7320 3d20    self.tracks = 
+0000fce0: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000fcf0: 2e66 696e 6428 224d 6f64 656c 2229 2e66  .find("Model").f
+0000fd00: 696e 6428 2241 6c6c 5472 6163 6b73 2229  ind("AllTracks")
+0000fd10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fd20: 2020 7365 6c66 2e73 6574 7469 6e67 7320    self.settings 
+0000fd30: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000fd40: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
+0000fd50: 7322 292e 6669 6e64 2822 496d 6167 6544  s").find("ImageD
+0000fd60: 6174 6122 290d 0a20 2020 2020 2020 2020  ata")..         
+0000fd70: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
+0000fd80: 6573 697a 6520 3d20 2869 6e74 2866 6c6f  esize = (int(flo
+0000fd90: 6174 2873 656c 662e 7365 7474 696e 6773  at(self.settings
+0000fda0: 2e67 6574 2822 6e66 7261 6d65 7322 2929  .get("nframes"))
+0000fdb0: 292c 696e 7428 666c 6f61 7428 7365 6c66  ),int(float(self
+0000fdc0: 2e73 6574 7469 6e67 732e 6765 7428 226e  .settings.get("n
+0000fdd0: 736c 6963 6573 2229 2929 2c69 6e74 2866  slices"))),int(f
+0000fde0: 6c6f 6174 2873 656c 662e 7365 7474 696e  loat(self.settin
+0000fdf0: 6773 2e67 6574 2822 6865 6967 6874 2229  gs.get("height")
+0000fe00: 2929 2c20 2069 6e74 2866 6c6f 6174 2873  )),  int(float(s
+0000fe10: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000fe20: 2822 7769 6474 6822 2929 2929 0d0a 2020  ("width"))))..  
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fe40: 696e 7428 6627 584d 4c20 6669 6c65 206d  int(f'XML file m
+0000fe50: 6164 6520 7573 696e 6720 696d 6167 6520  ade using image 
+0000fe60: 6f66 207b 7365 6c66 2e69 6d61 6765 7369  of {self.imagesi
+0000fe70: 7a65 7d27 290d 0a20 2020 2020 2020 2020  ze}')..         
+0000fe80: 2020 2020 2020 2073 656c 662e 7863 616c         self.xcal
+0000fe90: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000fea0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000feb0: 6574 2822 7069 7865 6c77 6964 7468 2229  et("pixelwidth")
+0000fec0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fed0: 2020 2073 656c 662e 7963 616c 6962 7261     self.ycalibra
+0000fee0: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
+0000fef0: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
+0000ff00: 7069 7865 6c68 6569 6768 7422 2929 0d0a  pixelheight"))..
+0000ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff20: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+0000ff30: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000ff40: 6574 7469 6e67 732e 6765 7428 2276 6f78  ettings.get("vox
+0000ff50: 656c 6465 7074 6822 2929 0d0a 2020 2020  eldepth"))..    
+0000ff60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ff70: 2e74 6361 6c69 6272 6174 696f 6e20 3d20  .tcalibration = 
+0000ff80: 696e 7428 666c 6f61 7428 7365 6c66 2e73  int(float(self.s
+0000ff90: 6574 7469 6e67 732e 6765 7428 2274 696d  ettings.get("tim
+0000ffa0: 6569 6e74 6572 7661 6c22 2929 290d 0a20  einterval"))).. 
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ffc0: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
+0000ffd0: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
+0000ffe0: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
+0000fff0: 7474 696e 6773 2229 2e66 696e 6428 2244  ttings").find("D
+00010000: 6574 6563 746f 7253 6574 7469 6e67 7322  etectorSettings"
+00010010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010020: 2020 2073 656c 662e 6261 7369 6373 6574     self.basicset
+00010030: 7469 6e67 7320 3d20 7365 6c66 2e78 6d6c  tings = self.xml
+00010040: 5f63 6f6e 7465 6e74 2e66 696e 6428 2253  _content.find("S
+00010050: 6574 7469 6e67 7322 292e 6669 6e64 2822  ettings").find("
+00010060: 4261 7369 6353 6574 7469 6e67 7322 290d  BasicSettings").
+00010070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010080: 2073 656c 662e 6465 7465 6374 6f72 6368   self.detectorch
+00010090: 616e 6e65 6c20 3d20 696e 7428 666c 6f61  annel = int(floa
+000100a0: 7428 7365 6c66 2e64 6574 6563 746f 7273  t(self.detectors
+000100b0: 6574 7469 6e67 732e 6765 7428 2254 4152  ettings.get("TAR
+000100c0: 4745 545f 4348 414e 4e45 4c22 2929 290d  GET_CHANNEL"))).
+000100d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100e0: 2073 656c 662e 7473 7461 7274 203d 2069   self.tstart = i
+000100f0: 6e74 2866 6c6f 6174 2873 656c 662e 6261  nt(float(self.ba
+00010100: 7369 6373 6574 7469 6e67 732e 6765 7428  sicsettings.get(
+00010110: 2274 7374 6172 7422 2929 290d 0a20 2020  "tstart")))..   
+00010120: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010130: 662e 7465 6e64 203d 2069 6e74 2866 6c6f  f.tend = int(flo
+00010140: 6174 2873 656c 662e 6261 7369 6373 6574  at(self.basicset
+00010150: 7469 6e67 732e 6765 7428 2274 656e 6422  tings.get("tend"
+00010160: 2929 290d 0a20 2020 2020 2020 2020 2020  )))..           
+00010170: 2020 2020 2073 656c 662e 5f67 6574 5f62       self._get_b
+00010180: 6f75 6e64 6172 795f 706f 696e 7473 2829  oundary_points()
+00010190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000101a0: 2020 7072 696e 7428 2749 7465 7261 7469    print('Iterati
+000101b0: 6e67 206f 7665 7220 7370 6f74 7320 696e  ng over spots in
+000101c0: 2066 7261 6d65 2729 0d0a 2020 2020 2020   frame')..      
+000101d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000101e0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+000101f0: 2020 2020 2020 2020 2020 6675 7475 7265            future
+00010200: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+00010210: 2020 2020 2020 2020 2020 7769 7468 2063            with c
+00010220: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+00010230: 732e 5468 7265 6164 506f 6f6c 4578 6563  s.ThreadPoolExec
+00010240: 7574 6f72 286d 6178 5f77 6f72 6b65 7273  utor(max_workers
+00010250: 203d 206f 732e 6370 755f 636f 756e 7428   = os.cpu_count(
+00010260: 2929 2061 7320 6578 6563 7574 6f72 3a0d  )) as executor:.
+00010270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010280: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00010290: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+000102a0: 7261 6d65 2069 6e20 7365 6c66 2e53 706f  rame in self.Spo
+000102b0: 746f 626a 6563 7473 2e66 696e 6461 6c6c  tobjects.findall
+000102c0: 2827 5370 6f74 7349 6e46 7261 6d65 2729  ('SpotsInFrame')
+000102d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
+00010300: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
+00010310: 656c 662e 5f73 706f 745f 636f 6d70 7574  elf._spot_comput
+00010320: 6572 2c20 6672 616d 6529 290d 0a20 2020  er, frame))..   
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+00010350: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+00010360: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010380: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000103b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000103c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000103d0: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-000103e0: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-000103f0: 5370 6f74 7322 0d0a 2020 2020 2020 2020  Spots"..        
-00010400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010410: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010420: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-00010430: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
-00010440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000103b0: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+000103c0: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
+000103d0: 2053 706f 7473 220d 0a20 2020 2020 2020   Spots"..       
+000103e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010400: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
+00010410: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
+00010420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010440: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
 00010450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010460: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
-00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00010490: 2866 7574 7572 6573 292c 0d0a 2020 2020  (futures),..    
-000104a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010460: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00010470: 6e28 6675 7475 7265 7329 2c0d 0a20 2020  n(futures),..   
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104a0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
 000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000104d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000104f0: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-00010500: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00010510: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-00010520: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-00010530: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
-00010540: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-00010580: 7365 6c66 2e63 6f75 6e74 202b 2031 0d0a  self.count + 1..
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000105c0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-000105d0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00010610: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
-00010620: 2073 656c 662e 636f 756e 740d 0a20 2020   self.count..   
-00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010650: 2020 2020 2072 2e72 6573 756c 7428 290d       r.result().
-00010660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010670: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
-00010680: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
-00010690: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
-000106a0: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
-000106b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000106c0: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
-000106d0: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-000106e0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-000106f0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-00010700: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00010710: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010720: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-00010730: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-00010740: 5472 6163 6b73 220d 0a20 2020 2020 2020  Tracks"..       
-00010750: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010760: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
-00010770: 616e 6765 203d 2028 302c 206c 656e 2873  ange = (0, len(s
-00010780: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-00010790: 636b 5f69 6473 2929 0d0a 2020 2020 2020  ck_ids))..      
-000107a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000107b0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-000107c0: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
-000107d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000107e0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-000107f0: 6c65 6e67 7468 203d 2030 2020 2020 0d0a  length = 0    ..
-00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 666f 7220 7472 6163 6b20 696e 2073 656c  for track in sel
-00010820: 662e 7472 6163 6b73 2e66 696e 6461 6c6c  f.tracks.findall
-00010830: 2827 5472 6163 6b27 293a 0d0a 2020 2020  ('Track'):..    
-00010840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010850: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
-00010860: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
-00010870: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
-00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010890: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
-000108a0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
-000108b0: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
-000108c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108d0: 2020 2020 2020 6469 6769 745f 6c65 6e67        digit_leng
-000108e0: 7468 203d 206c 656e 2873 7472 2874 7261  th = len(str(tra
-000108f0: 636b 5f69 6429 290d 0a20 2020 2020 2020  ck_id))..       
-00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010910: 2020 2020 2069 6620 6469 6769 745f 6c65       if digit_le
-00010920: 6e67 7468 203e 206d 6178 5f6c 656e 6774  ngth > max_lengt
-00010930: 683a 0d0a 2020 2020 2020 2020 2020 2020  h:..            
-00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2020 2020 6d61 785f 6c65 6e67 7468 203d      max_length =
-00010960: 2064 6967 6974 5f6c 656e 6774 680d 0a20   digit_length.. 
-00010970: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010980: 656c 662e 6d61 785f 7472 6163 6b5f 6469  elf.max_track_di
-00010990: 6769 7420 3d20 6d61 785f 6c65 6e67 7468  git = max_length
-000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000109c0: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
-000109d0: 656c 662e 7472 6163 6b73 2e66 696e 6461  elf.tracks.finda
-000109e0: 6c6c 2827 5472 6163 6b27 293a 0d0a 2020  ll('Track'):..  
-000109f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a00: 2020 7472 6163 6b5f 6964 203d 2069 6e74    track_id = int
-00010a10: 2874 7261 636b 2e67 6574 2873 656c 662e  (track.get(self.
-00010a20: 7472 6163 6b69 645f 6b65 7929 290d 0a20  trackid_key)).. 
-00010a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a40: 2020 2069 6620 7472 6163 6b5f 6964 2069     if track_id i
-00010a50: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
-00010a60: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
-00010a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a80: 2020 2020 7365 6c66 2e5f 7472 6163 6b5f      self._track_
-00010a90: 636f 6d70 7574 6572 2874 7261 636b 2c20  computer(track, 
-00010aa0: 7472 6163 6b5f 6964 290d 0a20 2020 2020  track_id)..     
-00010ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ac0: 2020 2073 656c 662e 636f 756e 7420 2b3d     self.count +=
-00010ad0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00010ae0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00010af0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00010b00: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010b30: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
-00010b40: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
-00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010b60: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
-00010b70: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
-00010b80: 7420 4e6f 6e65 3a20 200d 0a20 2020 2020  t None:  ..     
-00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ba0: 2020 7365 6c66 2e5f 6372 6561 7465 5f73    self._create_s
-00010bb0: 6563 6f6e 645f 6368 616e 6e65 6c5f 786d  econd_channel_xm
-00010bc0: 6c28 290d 0a20 2020 2020 2020 2020 2020  l()..           
-00010bd0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-00010be0: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
-00010bf0: 7629 2069 6e20 7365 6c66 2e67 7261 7068  v) in self.graph
-00010c00: 5f73 706c 6974 2e69 7465 6d73 2829 3a0d  _split.items():.
-00010c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010c20: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c40: 2020 2020 2020 2020 2020 6461 7567 6874            daught
-00010c50: 6572 5f74 7261 636b 5f69 6420 3d20 2069  er_track_id =  i
-00010c60: 6e74 2866 6c6f 6174 2873 7472 2873 656c  nt(float(str(sel
-00010c70: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00010c80: 6f70 6572 7469 6573 5b69 6e74 2866 6c6f  operties[int(flo
-00010c90: 6174 286b 2929 5d5b 7365 6c66 2e75 6e69  at(k))][self.uni
-00010ca0: 7175 6569 645f 6b65 795d 2929 290d 0a20  queid_key]))).. 
-00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cc0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
-00010cd0: 745f 7472 6163 6b5f 6964 203d 2069 6e74  t_track_id = int
-00010ce0: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
-00010cf0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00010d00: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
-00010d10: 2876 2929 5d5b 7365 6c66 2e75 6e69 7175  (v))][self.uniqu
-00010d20: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
-00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d40: 2020 2020 2020 2020 2073 656c 662e 6772           self.gr
-00010d50: 6170 685f 7472 6163 6b73 5b64 6175 6768  aph_tracks[daugh
-00010d60: 7465 725f 7472 6163 6b5f 6964 5d20 3d20  ter_track_id] = 
-00010d70: 7061 7265 6e74 5f74 7261 636b 5f69 640d  parent_track_id.
-00010d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010d90: 2073 656c 662e 5f67 6574 5f61 7474 7269   self._get_attri
-00010da0: 6275 7465 7328 290d 0a20 2020 2020 2020  butes()..       
-00010db0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010dc0: 2e61 7574 6f65 6e63 6f64 6572 5f6d 6f64  .autoencoder_mod
-00010dd0: 656c 2061 6e64 2073 656c 662e 7365 675f  el and self.seg_
-00010de0: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-00010df0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00010e00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00010e10: 2827 4765 7474 696e 6720 6175 746f 656e  ('Getting autoen
-00010e20: 636f 6465 7220 636c 6f75 6473 2729 0d0a  coder clouds')..
-00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e40: 2020 2020 2020 2073 656c 662e 5f61 7373         self._ass
-00010e50: 6967 6e5f 636c 7573 7465 725f 636c 6173  ign_cluster_clas
-00010e60: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00010e70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010e80: 7428 2743 7265 6174 696e 6720 6d61 7374  t('Creating mast
-00010e90: 6572 2078 6d6c 2729 0d0a 2020 2020 2020  er xml')..      
-00010ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010eb0: 2073 656c 662e 5f63 7265 6174 655f 6d61   self._create_ma
-00010ec0: 7374 6572 5f78 6d6c 2829 0d0a 2020 2020  ster_xml()..    
-00010ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010ee0: 2e63 6f75 6e74 203d 2030 200d 0a20 2020  .count = 0 ..   
-00010ef0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00010f00: 2069 6e64 6578 2c20 7472 6163 6b5f 6964   index, track_id
-00010f10: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-00010f20: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-00010f30: 6b5f 6964 7329 3a0d 0a20 2020 2020 2020  k_ids):..       
-00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010f60: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010f70: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-00010f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fa0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00010fb0: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
-00010fc0: 3d20 224a 7573 7420 6f6e 6520 6d6f 7265  = "Just one more
-00010fd0: 2074 6869 6e67 220d 0a20 2020 2020 2020   thing"..       
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00011010: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00011050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 2020 6c65 6e28 7365 6c66 2e66 696c 7465    len(self.filte
-00011090: 7265 645f 7472 6163 6b5f 6964 7329 2c0d  red_track_ids),.
-000110a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110c0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-00011100: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
-00011110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00011140: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
-00011150: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
-00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011180: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-00011190: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
-000111a0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 2020 2020 2020 2074 7261 636b 203d           track =
-000111d0: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-000111e0: 7261 636b 735b 696e 6465 785d 2020 2020  racks[index]    
-000111f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011210: 2020 2020 2020 7365 6c66 2e5f 6669 6e61        self._fina
-00011220: 6c5f 7472 6163 6b73 2874 7261 636b 2c20  l_tracks(track, 
-00011230: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-00011240: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011250: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
-00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011270: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
-00011280: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
-000112b0: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
-000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000112e0: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-000112f0: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-00011300: 6d61 7465 2829 0d0a 2020 2020 2020 2020  mate()..        
-00011310: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00011320: 6465 6620 5f63 7265 6174 655f 6d61 7374  def _create_mast
-00011330: 6572 5f78 6d6c 2873 656c 6629 3a0d 0a20  er_xml(self):.. 
-00011340: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00011350: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011360: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-00011370: 696e 2073 656c 662e 6d61 7374 6572 5f78  in self.master_x
-00011380: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-00011390: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
-000113c0: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
-000113d0: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-000113e0: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-00011410: 6420 696e 2073 656c 662e 756e 6971 7565  d in self.unique
-00011420: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011430: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+000104d0: 6772 6573 735f 6261 722e 7368 6f77 2829  gress_bar.show()
+000104e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000104f0: 2020 2020 2020 2020 666f 7220 7220 696e          for r in
+00010500: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+00010510: 7265 732e 6173 5f63 6f6d 706c 6574 6564  res.as_completed
+00010520: 2866 7574 7572 6573 293a 0d0a 2020 2020  (futures):..    
+00010530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010550: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+00010560: 2073 656c 662e 636f 756e 7420 2b20 310d   self.count + 1.
+00010570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010590: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000105a0: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+000105b0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+000105f0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
+00010600: 2020 7365 6c66 2e63 6f75 6e74 0d0a 2020    self.count..  
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010630: 2020 2020 2020 722e 7265 7375 6c74 2829        r.result()
+00010640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010650: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
+00010660: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
+00010670: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
+00010680: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
+00010690: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000106a0: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
+000106b0: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
+000106c0: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+000106d0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+000106e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000106f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010700: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+00010710: 656c 203d 2022 436f 6c6c 6563 7469 6e67  el = "Collecting
+00010720: 2054 7261 636b 7322 0d0a 2020 2020 2020   Tracks"..      
+00010730: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010740: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00010750: 7261 6e67 6520 3d20 2830 2c20 6c65 6e28  range = (0, len(
+00010760: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+00010770: 6163 6b5f 6964 7329 290d 0a20 2020 2020  ack_ids))..     
+00010780: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010790: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+000107a0: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+000107b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000107c0: 2020 2020 2020 2020 2020 2020 206d 6178               max
+000107d0: 5f6c 656e 6774 6820 3d20 3020 2020 200d  _length = 0    .
+000107e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000107f0: 2066 6f72 2074 7261 636b 2069 6e20 7365   for track in se
+00010800: 6c66 2e74 7261 636b 732e 6669 6e64 616c  lf.tracks.findal
+00010810: 6c28 2754 7261 636b 2729 3a0d 0a20 2020  l('Track'):..   
+00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010830: 2074 7261 636b 5f69 6420 3d20 696e 7428   track_id = int(
+00010840: 7472 6163 6b2e 6765 7428 7365 6c66 2e74  track.get(self.t
+00010850: 7261 636b 6964 5f6b 6579 2929 0d0a 2020  rackid_key))..  
+00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010870: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
+00010880: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
+00010890: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+000108a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108b0: 2020 2020 2020 2064 6967 6974 5f6c 656e         digit_len
+000108c0: 6774 6820 3d20 6c65 6e28 7374 7228 7472  gth = len(str(tr
+000108d0: 6163 6b5f 6964 2929 0d0a 2020 2020 2020  ack_id))..      
+000108e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000108f0: 2020 2020 2020 6966 2064 6967 6974 5f6c        if digit_l
+00010900: 656e 6774 6820 3e20 6d61 785f 6c65 6e67  ength > max_leng
+00010910: 7468 3a0d 0a20 2020 2020 2020 2020 2020  th:..           
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 206d 6178 5f6c 656e 6774 6820       max_length 
+00010940: 3d20 6469 6769 745f 6c65 6e67 7468 0d0a  = digit_length..
+00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010960: 7365 6c66 2e6d 6178 5f74 7261 636b 5f64  self.max_track_d
+00010970: 6967 6974 203d 206d 6178 5f6c 656e 6774  igit = max_lengt
+00010980: 6820 2020 2020 2020 2020 2020 2020 2020  h               
+00010990: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000109a0: 2020 2066 6f72 2074 7261 636b 2069 6e20     for track in 
+000109b0: 7365 6c66 2e74 7261 636b 732e 6669 6e64  self.tracks.find
+000109c0: 616c 6c28 2754 7261 636b 2729 3a0d 0a20  all('Track'):.. 
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
+000109f0: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+00010a00: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
+00010a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a20: 2020 2020 6966 2074 7261 636b 5f69 6420      if track_id 
+00010a30: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
+00010a40: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2020 2020 2073 656c 662e 5f74 7261 636b       self._track
+00010a70: 5f63 6f6d 7075 7465 7228 7472 6163 6b2c  _computer(track,
+00010a80: 2074 7261 636b 5f69 6429 0d0a 2020 2020   track_id)..    
+00010a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010aa0: 2020 2020 7365 6c66 2e63 6f75 6e74 202b      self.count +
+00010ab0: 3d20 310d 0a20 2020 2020 2020 2020 2020  = 1..           
+00010ac0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010ad0: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010ae0: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
+00010af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010b10: 2e70 726f 6772 6573 735f 6261 722e 7661  .progress_bar.va
+00010b20: 6c75 6520 3d20 7365 6c66 2e63 6f75 6e74  lue = self.count
+00010b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010b40: 2020 6966 2073 656c 662e 6368 616e 6e65    if self.channe
+00010b50: 6c5f 7365 675f 696d 6167 6520 6973 206e  l_seg_image is n
+00010b60: 6f74 204e 6f6e 653a 2020 0d0a 2020 2020  ot None:  ..    
+00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b80: 2020 2073 656c 662e 5f63 7265 6174 655f     self._create_
+00010b90: 7365 636f 6e64 5f63 6861 6e6e 656c 5f78  second_channel_x
+00010ba0: 6d6c 2829 0d0a 2020 2020 2020 2020 2020  ml()..          
+00010bb0: 2020 2020 2020 0d0a 0d0a 2020 2020 2020        ....      
+00010bc0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+00010bd0: 2c76 2920 696e 2073 656c 662e 6772 6170  ,v) in self.grap
+00010be0: 685f 7370 6c69 742e 6974 656d 7328 293a  h_split.items():
+00010bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010c00: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c20: 2020 2020 2020 2020 2020 2064 6175 6768             daugh
+00010c30: 7465 725f 7472 6163 6b5f 6964 203d 2020  ter_track_id =  
+00010c40: 696e 7428 666c 6f61 7428 7374 7228 7365  int(float(str(se
+00010c50: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00010c60: 726f 7065 7274 6965 735b 696e 7428 666c  roperties[int(fl
+00010c70: 6f61 7428 6b29 295d 5b73 656c 662e 756e  oat(k))][self.un
+00010c80: 6971 7565 6964 5f6b 6579 5d29 2929 0d0a  iqueid_key])))..
+00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ca0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
+00010cb0: 6e74 5f74 7261 636b 5f69 6420 3d20 696e  nt_track_id = in
+00010cc0: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
+00010cd0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00010ce0: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
+00010cf0: 7428 7629 295d 5b73 656c 662e 756e 6971  t(v))][self.uniq
+00010d00: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d20: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+00010d30: 7261 7068 5f74 7261 636b 735b 6461 7567  raph_tracks[daug
+00010d40: 6874 6572 5f74 7261 636b 5f69 645d 203d  hter_track_id] =
+00010d50: 2070 6172 656e 745f 7472 6163 6b5f 6964   parent_track_id
+00010d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010d70: 2020 7365 6c66 2e5f 6765 745f 6174 7472    self._get_attr
+00010d80: 6962 7574 6573 2829 0d0a 2020 2020 2020  ibutes()..      
+00010d90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00010da0: 662e 6175 746f 656e 636f 6465 725f 6d6f  f.autoencoder_mo
+00010db0: 6465 6c20 616e 6420 7365 6c66 2e73 6567  del and self.seg
+00010dc0: 5f69 6d61 6765 2069 7320 6e6f 7420 4e6f  _image is not No
+00010dd0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00010de0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010df0: 7428 2747 6574 7469 6e67 2061 7574 6f65  t('Getting autoe
+00010e00: 6e63 6f64 6572 2063 6c6f 7564 7327 290d  ncoder clouds').
+00010e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e20: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00010e30: 7369 676e 5f63 6c75 7374 6572 5f63 6c61  sign_cluster_cla
+00010e40: 7373 2829 0d0a 2020 2020 2020 2020 2020  ss()..          
+00010e50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00010e60: 6e74 2827 4372 6561 7469 6e67 206d 6173  nt('Creating mas
+00010e70: 7465 7220 786d 6c27 290d 0a20 2020 2020  ter xml')..     
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2020 7365 6c66 2e5f 6372 6561 7465 5f6d    self._create_m
+00010ea0: 6173 7465 725f 786d 6c28 290d 0a20 2020  aster_xml()..   
+00010eb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010ec0: 662e 636f 756e 7420 3d20 3020 0d0a 2020  f.count = 0 ..  
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010ee0: 7220 696e 6465 782c 2074 7261 636b 5f69  r index, track_i
+00010ef0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
+00010f00: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+00010f10: 636b 5f69 6473 293a 0d0a 2020 2020 2020  ck_ids):..      
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010f40: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00010f50: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+00010f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010f90: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+00010fa0: 203d 2022 4a75 7374 206f 6e65 206d 6f72   = "Just one mor
+00010fb0: 6520 7468 696e 6722 0d0a 2020 2020 2020  e thing"..      
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010ff0: 6261 722e 7261 6e67 6520 3d20 280d 0a20  bar.range = (.. 
+00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011020: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00011030: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011060: 2020 206c 656e 2873 656c 662e 6669 6c74     len(self.filt
+00011070: 6572 6564 5f74 7261 636b 5f69 6473 292c  ered_track_ids),
+00011080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110a0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+000110b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110d0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000110e0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+000110f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011120: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
+00011130: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00011140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00011170: 722e 7661 6c75 6520 3d20 7365 6c66 2e63  r.value = self.c
+00011180: 6f75 6e74 0d0a 2020 2020 2020 2020 2020  ount..          
+00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111a0: 2020 2020 2020 2020 2020 7472 6163 6b20            track 
+000111b0: 3d20 7365 6c66 2e66 696c 7465 7265 645f  = self.filtered_
+000111c0: 7472 6163 6b73 5b69 6e64 6578 5d20 2020  tracks[index]   
+000111d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 2020 2020 2073 656c 662e 5f66 696e         self._fin
+00011200: 616c 5f74 7261 636b 7328 7472 6163 6b2c  al_tracks(track,
+00011210: 2074 7261 636b 5f69 6429 200d 0a0d 0a20   track_id) .... 
+00011220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011230: 6620 7365 6c66 2e66 6f75 7269 6572 3a0d  f self.fourier:.
+00011240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011250: 2020 2020 7072 696e 7428 2763 6f6d 7075      print('compu
+00011260: 7469 6e67 2046 6f75 7269 6572 2729 0d0a  ting Fourier')..
+00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011280: 2020 2073 656c 662e 5f63 6f6d 7075 7465     self._compute
+00011290: 5f70 6865 6e6f 7479 7065 7328 2920 2020  _phenotypes()   
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000112c0: 2020 2020 2020 2073 656c 662e 5f74 656d         self._tem
+000112d0: 706f 7261 6c5f 706c 6f74 735f 7472 6163  poral_plots_trac
+000112e0: 6b6d 6174 6528 290d 0a20 2020 2020 2020  kmate()..       
+000112f0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00011300: 2064 6566 205f 6372 6561 7465 5f6d 6173   def _create_mas
+00011310: 7465 725f 786d 6c28 7365 6c66 293a 0d0a  ter_xml(self):..
+00011320: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00011330: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011340: 2020 666f 7220 5370 6f74 6f62 6a65 6374    for Spotobject
+00011350: 2069 6e20 7365 6c66 2e6d 6173 7465 725f   in self.master_
+00011360: 786d 6c5f 726f 6f74 2e69 7465 7228 2753  xml_root.iter('S
+00011370: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011390: 2020 2020 2020 2020 6365 6c6c 5f69 6420          cell_id 
+000113a0: 3d20 696e 7428 5370 6f74 6f62 6a65 6374  = int(Spotobject
+000113b0: 2e67 6574 2873 656c 662e 7370 6f74 6964  .get(self.spotid
+000113c0: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+000113d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113e0: 2020 2020 2020 2020 6966 2063 656c 6c5f          if cell_
+000113f0: 6964 2069 6e20 7365 6c66 2e75 6e69 7175  id in self.uniqu
+00011400: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00011410: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011480: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-00011490: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
-000114a0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-000114b0: 656c 6c5f 6964 5d2e 6b65 7973 2829 3a0d  ell_id].keys():.
-000114c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-000114f0: 6f74 6f62 6a65 6374 2e73 6574 286b 2c20  otobject.set(k, 
-00011500: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-00011510: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00011520: 6365 6c6c 5f69 645d 5b6b 5d29 2920 2020  cell_id][k]))   
-00011530: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-00011560: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-00011570: 7374 6572 5f78 6d6c 5f74 7265 652e 7772  ster_xml_tree.wr
-00011580: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
-00011590: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
-000115a0: 5f70 6174 682c 2073 656c 662e 6d61 7374  _path, self.mast
-000115b0: 6572 5f78 6d6c 5f6e 616d 6529 290d 0a20  er_xml_name)).. 
-000115c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000115d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011460: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00011470: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
+00011480: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00011490: 6365 6c6c 5f69 645d 2e6b 6579 7328 293a  cell_id].keys():
+000114a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+000114d0: 706f 746f 626a 6563 742e 7365 7428 6b2c  potobject.set(k,
+000114e0: 2073 7472 2873 656c 662e 756e 6971 7565   str(self.unique
+000114f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011500: 5b63 656c 6c5f 6964 5d5b 6b5d 2929 2020  [cell_id][k]))  
+00011510: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011530: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00011540: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00011550: 6173 7465 725f 786d 6c5f 7472 6565 2e77  aster_xml_tree.w
+00011560: 7269 7465 286f 732e 7061 7468 2e6a 6f69  rite(os.path.joi
+00011570: 6e28 7365 6c66 2e6d 6173 7465 725f 786d  n(self.master_xm
+00011580: 6c5f 7061 7468 2c20 7365 6c66 2e6d 6173  l_path, self.mas
+00011590: 7465 725f 786d 6c5f 6e61 6d65 2929 0d0a  ter_xml_name))..
+000115a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00011620: 2020 2020 6465 6620 5f61 7373 6967 6e5f      def _assign_
-00011630: 636c 7573 7465 725f 636c 6173 7328 7365  cluster_class(se
-00011640: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-00011650: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00011660: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
-00011670: 203d 2073 656c 662e 6178 6573 2e72 6570   = self.axes.rep
-00011680: 6c61 6365 2822 5422 2c20 2222 290d 0a20  lace("T", "").. 
-00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000116b0: 2020 2020 2020 2020 2066 6f72 2063 6f75           for cou
-000116c0: 6e74 2c20 7469 6d65 5f6b 6579 2069 6e20  nt, time_key in 
-000116d0: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
-000116e0: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
-000116f0: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
+000115f0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00011600: 0a20 2020 2064 6566 205f 6173 7369 676e  .    def _assign
+00011610: 5f63 6c75 7374 6572 5f63 6c61 7373 2873  _cluster_class(s
+00011620: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+00011630: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00011640: 2020 2020 2020 2020 7365 6c66 2e61 7865          self.axe
+00011650: 7320 3d20 7365 6c66 2e61 7865 732e 7265  s = self.axes.re
+00011660: 706c 6163 6528 2254 222c 2022 2229 0d0a  place("T", "")..
+00011670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011680: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00011690: 2020 2020 2020 2020 2020 666f 7220 636f            for co
+000116a0: 756e 742c 2074 696d 655f 6b65 7920 696e  unt, time_key in
+000116b0: 2065 6e75 6d65 7261 7465 2873 656c 662e   enumerate(self.
+000116c0: 5f74 696d 6564 5f63 656e 7472 6f69 642e  _timed_centroid.
+000116d0: 6b65 7973 2829 293a 0d0a 2020 2020 2020  keys()):..      
+000116e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 00011700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011710: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
-00011740: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
-00011750: 6d65 645f 6365 6e74 726f 6964 5b74 696d  med_centroid[tim
-00011760: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-00011790: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-000117a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000117b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117c0: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-000117d0: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-000117e0: 2241 7574 6f65 6e63 6f64 6572 2066 6f72  "Autoencoder for
-000117f0: 2072 6566 696e 696e 6720 706f 696e 7420   refining point 
-00011800: 636c 6f75 6473 220d 0a20 2020 2020 2020  clouds"..       
-00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00011830: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-00011840: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00011710: 2020 7472 6565 2c20 7370 6f74 5f63 656e    tree, spot_cen
+00011720: 7472 6f69 6473 203d 2073 656c 662e 5f74  troids = self._t
+00011730: 696d 6564 5f63 656e 7472 6f69 645b 7469  imed_centroid[ti
+00011740: 6d65 5f6b 6579 5d0d 0a20 2020 2020 2020  me_key]..       
+00011750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011760: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+00011770: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+00011780: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
+000117b0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
+000117c0: 2022 4175 746f 656e 636f 6465 7220 666f   "Autoencoder fo
+000117d0: 7220 7265 6669 6e69 6e67 2070 6f69 6e74  r refining point
+000117e0: 2063 6c6f 7564 7322 0d0a 2020 2020 2020   clouds"..      
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00011810: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+00011820: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011860: 2020 2020 2020 2030 2c0d 0a20 2020 2020         0,..     
 00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 2020 2020 302c 0d0a 2020 2020 2020        0,..      
+00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118c0: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-000118d0: 6c66 2e5f 7469 6d65 645f 6365 6e74 726f  lf._timed_centro
-000118e0: 6964 2e6b 6579 7328 2929 202b 2031 2c0d  id.keys()) + 1,.
-000118f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00011930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011950: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011960: 722e 7661 6c75 6520 3d20 2063 6f75 6e74  r.value =  count
-00011970: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00011980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011990: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000119a0: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
-000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2020 2020 2020 2020 2020 636c 7573 7465            cluste
-000119d0: 725f 6576 616c 203d 2043 6c75 7374 6572  r_eval = Cluster
-000119e0: 696e 6728 7365 6c66 2e61 6363 656c 6572  ing(self.acceler
-000119f0: 6174 6f72 2c20 7365 6c66 2e64 6576 6963  ator, self.devic
-00011a00: 6573 2c20 7365 6c66 2e73 6567 5f69 6d61  es, self.seg_ima
-00011a10: 6765 5b69 6e74 2874 696d 655f 6b65 7929  ge[int(time_key)
-00011a20: 2c3a 5d2c 2020 7365 6c66 2e61 7865 732c  ,:],  self.axes,
-00011a30: 2073 656c 662e 6e75 6d5f 706f 696e 7473   self.num_points
-00011a40: 2c20 7365 6c66 2e61 7574 6f65 6e63 6f64  , self.autoencod
-00011a50: 6572 5f6d 6f64 656c 2c20 6b65 7920 3d20  er_model, key = 
-00011a60: 7469 6d65 5f6b 6579 2c20 7072 6f67 7265  time_key, progre
-00011a70: 7373 5f62 6172 3d73 656c 662e 7072 6f67  ss_bar=self.prog
-00011a80: 7265 7373 5f62 6172 2c20 6261 7463 685f  ress_bar, batch_
-00011a90: 7369 7a65 203d 2073 656c 662e 6261 7463  size = self.batc
-00011aa0: 685f 7369 7a65 2c20 7363 616c 655f 7a3d  h_size, scale_z=
-00011ab0: 7365 6c66 2e73 6361 6c65 5f7a 2c20 7363  self.scale_z, sc
-00011ac0: 616c 655f 7879 3d20 7365 6c66 2e73 6361  ale_xy= self.sca
-00011ad0: 6c65 5f78 792c 2063 656e 7465 7220 3d20  le_xy, center = 
-00011ae0: 7365 6c66 2e63 656e 7465 7229 2020 2020  self.center)    
-00011af0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b10: 636c 7573 7465 725f 6576 616c 2e5f 6372  cluster_eval._cr
-00011b20: 6561 7465 5f63 6c75 7374 6572 5f6c 6162  eate_cluster_lab
-00011b30: 656c 7328 290d 0a20 2020 2020 2020 2020  els()..         
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 7469 6d65 645f 636c 7573 7465 725f    timed_cluster_
-00011b60: 6c61 6265 6c20 3d20 636c 7573 7465 725f  label = cluster_
-00011b70: 6576 616c 2e74 696d 6564 5f63 6c75 7374  eval.timed_clust
-00011b80: 6572 5f6c 6162 656c 200d 0a20 2020 2020  er_label ..     
-00011b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ba0: 2020 2020 2020 6f75 7470 7574 5f6c 6162        output_lab
-00011bb0: 656c 732c 2020 6f75 7470 7574 5f63 6c75  els,  output_clu
-00011bc0: 7374 6572 5f63 656e 7472 6f69 642c 206f  ster_centroid, o
-00011bd0: 7574 7075 745f 636c 6f75 645f 6563 6365  utput_cloud_ecce
-00011be0: 6e74 7269 6369 7479 2c20 6f75 7470 7574  ntricity, output
-00011bf0: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
-00011c00: 6374 6f72 2c20 6f75 7470 7574 5f6c 6172  ctor, output_lar
-00011c10: 6765 7374 5f65 6967 656e 7661 6c75 652c  gest_eigenvalue,
-00011c20: 206f 7574 7075 745f 6469 6d65 6e73 696f   output_dimensio
-00011c30: 6e73 2c20 6f75 7470 7574 5f63 6c6f 7564  ns, output_cloud
-00011c40: 5f73 7572 6661 6365 5f61 7265 6120 3d20  _surface_area = 
-00011c50: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
-00011c60: 6265 6c5b 7469 6d65 5f6b 6579 5d0d 0a20  bel[time_key].. 
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00011c90: 3120 3d20 310d 0a20 2020 2020 2020 2020  1 = 1..         
+000118a0: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
+000118b0: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
+000118c0: 6f69 642e 6b65 7973 2829 2920 2b20 312c  oid.keys()) + 1,
+000118d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011900: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+00011910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011930: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00011940: 6172 2e76 616c 7565 203d 2020 636f 756e  ar.value =  coun
+00011950: 7420 0d0a 2020 2020 2020 2020 2020 2020  t ..            
+00011960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011970: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00011980: 735f 6261 722e 7368 6f77 2829 0d0a 0d0a  s_bar.show()....
+00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119a0: 2020 2020 2020 2020 2020 2063 6c75 7374             clust
+000119b0: 6572 5f65 7661 6c20 3d20 436c 7573 7465  er_eval = Cluste
+000119c0: 7269 6e67 2873 656c 662e 6163 6365 6c65  ring(self.accele
+000119d0: 7261 746f 722c 2073 656c 662e 6465 7669  rator, self.devi
+000119e0: 6365 732c 2073 656c 662e 7365 675f 696d  ces, self.seg_im
+000119f0: 6167 655b 696e 7428 7469 6d65 5f6b 6579  age[int(time_key
+00011a00: 292c 3a5d 2c20 2073 656c 662e 6178 6573  ),:],  self.axes
+00011a10: 2c20 7365 6c66 2e6e 756d 5f70 6f69 6e74  , self.num_point
+00011a20: 732c 2073 656c 662e 6175 746f 656e 636f  s, self.autoenco
+00011a30: 6465 725f 6d6f 6465 6c2c 206b 6579 203d  der_model, key =
+00011a40: 2074 696d 655f 6b65 792c 2070 726f 6772   time_key, progr
+00011a50: 6573 735f 6261 723d 7365 6c66 2e70 726f  ess_bar=self.pro
+00011a60: 6772 6573 735f 6261 722c 2062 6174 6368  gress_bar, batch
+00011a70: 5f73 697a 6520 3d20 7365 6c66 2e62 6174  _size = self.bat
+00011a80: 6368 5f73 697a 652c 2073 6361 6c65 5f7a  ch_size, scale_z
+00011a90: 3d73 656c 662e 7363 616c 655f 7a2c 2073  =self.scale_z, s
+00011aa0: 6361 6c65 5f78 793d 2073 656c 662e 7363  cale_xy= self.sc
+00011ab0: 616c 655f 7879 2c20 6365 6e74 6572 203d  ale_xy, center =
+00011ac0: 2073 656c 662e 6365 6e74 6572 2920 2020   self.center)   
+00011ad0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2063 6c75 7374 6572 5f65 7661 6c2e 5f63   cluster_eval._c
+00011b00: 7265 6174 655f 636c 7573 7465 725f 6c61  reate_cluster_la
+00011b10: 6265 6c73 2829 0d0a 2020 2020 2020 2020  bels()..        
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2020 2074 696d 6564 5f63 6c75 7374 6572     timed_cluster
+00011b40: 5f6c 6162 656c 203d 2063 6c75 7374 6572  _label = cluster
+00011b50: 5f65 7661 6c2e 7469 6d65 645f 636c 7573  _eval.timed_clus
+00011b60: 7465 725f 6c61 6265 6c20 0d0a 2020 2020  ter_label ..    
+00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b80: 2020 2020 2020 206f 7574 7075 745f 6c61         output_la
+00011b90: 6265 6c73 2c20 206f 7574 7075 745f 636c  bels,  output_cl
+00011ba0: 7573 7465 725f 6365 6e74 726f 6964 2c20  uster_centroid, 
+00011bb0: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
+00011bc0: 656e 7472 6963 6974 792c 206f 7574 7075  entricity, outpu
+00011bd0: 745f 6c61 7267 6573 745f 6569 6765 6e76  t_largest_eigenv
+00011be0: 6563 746f 722c 206f 7574 7075 745f 6c61  ector, output_la
+00011bf0: 7267 6573 745f 6569 6765 6e76 616c 7565  rgest_eigenvalue
+00011c00: 2c20 6f75 7470 7574 5f64 696d 656e 7369  , output_dimensi
+00011c10: 6f6e 732c 206f 7574 7075 745f 636c 6f75  ons, output_clou
+00011c20: 645f 7375 7266 6163 655f 6172 6561 203d  d_surface_area =
+00011c30: 2074 696d 6564 5f63 6c75 7374 6572 5f6c   timed_cluster_l
+00011c40: 6162 656c 5b74 696d 655f 6b65 795d 0d0a  abel[time_key]..
+00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c60: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011c70: 5f31 203d 2031 0d0a 2020 2020 2020 2020  _1 = 1..        
+00011c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c90: 2020 2073 6361 6c65 5f32 203d 2031 0d0a     scale_2 = 1..
 00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cb0: 2020 7363 616c 655f 3220 3d20 310d 0a20    scale_2 = 1.. 
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cd0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-00011ce0: 696e 2072 616e 6765 286c 656e 286f 7574  in range(len(out
-00011cf0: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
-00011d00: 726f 6964 2929 3a0d 0a20 2020 2020 2020  roid)):..       
-00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d20: 2020 2020 2020 2020 2020 2020 2063 656e               cen
-00011d30: 7472 6f69 6420 3d20 6f75 7470 7574 5f63  troid = output_c
-00011d40: 6c75 7374 6572 5f63 656e 7472 6f69 645b  luster_centroid[
-00011d50: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 2020 2020 2020 7175 616c 6974 7920          quality 
-00011d80: 3d20 6f75 7470 7574 5f6c 6172 6765 7374  = output_largest
-00011d90: 5f65 6967 656e 7661 6c75 655b 695d 0d0a  _eigenvalue[i]..
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dc0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-00011dd0: 5f63 6f6d 705f 6669 7273 7479 7a20 3d20  _comp_firstyz = 
-00011de0: 6f75 7470 7574 5f63 6c6f 7564 5f65 6363  output_cloud_ecc
-00011df0: 656e 7472 6963 6974 795b 695d 0d0a 2020  entricity[i]..  
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2020 6573 7365 6e74 7269 6369 7479 5f64    essentricity_d
-00011e30: 696d 656e 7369 6f6e 203d 206f 7574 7075  imension = outpu
-00011e40: 745f 6469 6d65 6e73 696f 6e73 5b69 5d20  t_dimensions[i] 
-00011e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011e80: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011e90: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-00011ed0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00011ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011f10: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011f20: 656e 7369 6f6e 5b31 5d20 3d3d 2031 3a0d  ension[1] == 1:.
-00011f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f60: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-00011f70: 662e 7963 616c 6962 7261 7469 6f6e 0d0a  f.ycalibration..
-00011f80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00011f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fa0: 2020 2020 2020 6966 2065 7373 656e 7472        if essentr
-00011fb0: 6963 6974 795f 6469 6d65 6e73 696f 6e5b  icity_dimension[
-00011fc0: 305d 203d 3d20 323a 0d0a 2020 2020 2020  0] == 2:..      
-00011fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ff0: 2020 2020 2073 6361 6c65 5f31 203d 2073       scale_1 = s
-00012000: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00012010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012030: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012040: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00012050: 656e 7369 6f6e 5b31 5d20 3d3d 2030 3a0d  ension[1] == 0:.
-00012060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012090: 2020 2073 6361 6c65 5f32 203d 2073 656c     scale_2 = sel
-000120a0: 662e 7863 616c 6962 7261 7469 6f6e 2020  f.xcalibration  
-000120b0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-000120e0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-000120f0: 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20 2020  on[0] == 1:..   
-00012100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012120: 2020 2020 2020 2020 7363 616c 655f 3120          scale_1 
-00012130: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
-00012140: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012170: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-00012180: 6469 6d65 6e73 696f 6e5b 315d 203d 3d20  dimension[1] == 
-00012190: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 2020 2020 2020 7363 616c 655f 3220 3d20        scale_2 = 
-000121d0: 7365 6c66 2e78 6361 6c69 6272 6174 696f  self.xcalibratio
-000121e0: 6e20 200d 0a0d 0a20 2020 2020 2020 2020  n  ....         
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2020 2020 2020 2020 2020 2069 6620 6573             if es
-00012210: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
-00012220: 7369 6f6e 5b30 5d20 3d3d 2031 3a0d 0a20  sion[0] == 1:.. 
-00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012250: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00012260: 3120 3d20 7365 6c66 2e79 6361 6c69 6272  1 = self.ycalibr
-00012270: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
-00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-000122b0: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
-000122c0: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
-000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122f0: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
-00012300: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
-00012310: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00012320: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012340: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00012350: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00012360: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
-00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-000123a0: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-000123b0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-000123c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123e0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-000123f0: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00012400: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
-00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012430: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00012440: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00012450: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
-00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012470: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
-00012480: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
-00012490: 696f 6e5b 305d 203d 3d20 303a 0d0a 2020  ion[0] == 0:..  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124c0: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
-000124d0: 203d 2073 656c 662e 7863 616c 6962 7261   = self.xcalibra
-000124e0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00012520: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
-00012530: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
-00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012560: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
-00012570: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00012580: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00011cb0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00011cc0: 2069 6e20 7261 6e67 6528 6c65 6e28 6f75   in range(len(ou
+00011cd0: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+00011ce0: 7472 6f69 6429 293a 0d0a 2020 2020 2020  troid)):..      
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00011d10: 6e74 726f 6964 203d 206f 7574 7075 745f  ntroid = output_
+00011d20: 636c 7573 7465 725f 6365 6e74 726f 6964  cluster_centroid
+00011d30: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d50: 2020 2020 2020 2020 2071 7561 6c69 7479           quality
+00011d60: 203d 206f 7574 7075 745f 6c61 7267 6573   = output_larges
+00011d70: 745f 6569 6765 6e76 616c 7565 5b69 5d0d  t_eigenvalue[i].
+00011d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011da0: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
+00011db0: 795f 636f 6d70 5f66 6972 7374 797a 203d  y_comp_firstyz =
+00011dc0: 206f 7574 7075 745f 636c 6f75 645f 6563   output_cloud_ec
+00011dd0: 6365 6e74 7269 6369 7479 5b69 5d0d 0a20  centricity[i].. 
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 2020 2065 7373 656e 7472 6963 6974 795f     essentricity_
+00011e10: 6469 6d65 6e73 696f 6e20 3d20 6f75 7470  dimension = outp
+00011e20: 7574 5f64 696d 656e 7369 6f6e 735b 695d  ut_dimensions[i]
+00011e30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e50: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011e60: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011e70: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
+00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ea0: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
+00011eb0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00011ec0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011ef0: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011f00: 6d65 6e73 696f 6e5b 315d 203d 3d20 313a  mension[1] == 1:
+00011f10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f40: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
+00011f50: 6c66 2e79 6361 6c69 6272 6174 696f 6e0d  lf.ycalibration.
+00011f60: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f80: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
+00011f90: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011fa0: 5b30 5d20 3d3d 2032 3a0d 0a20 2020 2020  [0] == 2:..     
+00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fd0: 2020 2020 2020 7363 616c 655f 3120 3d20        scale_1 = 
+00011fe0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+00011ff0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012010: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012020: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00012030: 6d65 6e73 696f 6e5b 315d 203d 3d20 303a  mension[1] == 0:
+00012040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012070: 2020 2020 7363 616c 655f 3220 3d20 7365      scale_2 = se
+00012080: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+00012090: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+000120c0: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+000120d0: 696f 6e5b 305d 203d 3d20 313a 0d0a 2020  ion[0] == 1:..  
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 2020 2020 2020 2073 6361 6c65 5f31           scale_1
+00012110: 203d 2073 656c 662e 7963 616c 6962 7261   = self.ycalibra
+00012120: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00012160: 5f64 696d 656e 7369 6f6e 5b31 5d20 3d3d  _dimension[1] ==
+00012170: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121a0: 2020 2020 2020 2073 6361 6c65 5f32 203d         scale_2 =
+000121b0: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
+000121c0: 6f6e 2020 0d0a 0d0a 2020 2020 2020 2020  on  ....        
+000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121e0: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+000121f0: 7373 656e 7472 6963 6974 795f 6469 6d65  ssentricity_dime
+00012200: 6e73 696f 6e5b 305d 203d 3d20 313a 0d0a  nsion[0] == 1:..
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00012240: 5f31 203d 2073 656c 662e 7963 616c 6962  _1 = self.ycalib
+00012250: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012280: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+00012290: 7479 5f64 696d 656e 7369 6f6e 5b31 5d20  ty_dimension[1] 
+000122a0: 3d3d 2032 3a0d 0a20 2020 2020 2020 2020  == 2:..         
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122d0: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
+000122e0: 203d 2073 656c 662e 7a63 616c 6962 7261   = self.zcalibra
+000122f0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
+00012300: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012320: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00012330: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00012340: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
+00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012370: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00012380: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
+00012390: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123c0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+000123d0: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+000123e0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012410: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00012420: 3d20 7365 6c66 2e79 6361 6c69 6272 6174  = self.ycalibrat
+00012430: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
+00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012450: 2020 2020 2020 2020 2020 2069 6620 6573             if es
+00012460: 7365 6e74 7269 6369 7479 5f64 696d 656e  sentricity_dimen
+00012470: 7369 6f6e 5b30 5d20 3d3d 2030 3a0d 0a20  sion[0] == 0:.. 
+00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+000124b0: 3120 3d20 7365 6c66 2e78 6361 6c69 6272  1 = self.xcalibr
+000124c0: 6174 696f 6e0d 0a20 2020 2020 2020 2020  ation..         
+000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124f0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00012500: 795f 6469 6d65 6e73 696f 6e5b 315d 203d  y_dimension[1] =
+00012510: 3d20 323a 0d0a 2020 2020 2020 2020 2020  = 2:..          
+00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012540: 2020 2020 2020 2020 7363 616c 655f 3220          scale_2 
+00012550: 3d20 7365 6c66 2e7a 6361 6c69 6272 6174  = self.zcalibrat
+00012560: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125c0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
 000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125e0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012610: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012630: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-00012640: 6c5f 6178 6973 203d 206f 7574 7075 745f  l_axis = output_
-00012650: 6c61 7267 6573 745f 6569 6765 6e76 6563  largest_eigenvec
-00012660: 746f 725b 695d 0d0a 2020 2020 2020 2020  tor[i]..        
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 2020 2020 2020 7375 7266              surf
-00012690: 6163 655f 6172 6561 203d 206f 7574 7075  ace_area = outpu
-000126a0: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-000126b0: 6172 6561 5b69 5d20 2a20 7365 6c66 2e7a  area[i] * self.z
-000126c0: 6361 6c69 6272 6174 696f 6e20 2a20 7365  calibration * se
-000126d0: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
-000126e0: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-000126f0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-00012700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012710: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-00012720: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00012730: 7928 6365 6e74 726f 6964 290d 0a20 2020  y(centroid)..   
-00012740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2072 6164 6975 7320 3d20 7175 616c 6974   radius = qualit
-00012770: 7920 2a20 6d61 7468 2e70 6f77 2873 656c  y * math.pow(sel
-00012780: 662e 7a63 616c 6962 7261 7469 6f6e 202a  f.zcalibration *
-00012790: 2073 656c 662e 7863 616c 6962 7261 7469   self.xcalibrati
-000127a0: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
-000127b0: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
-000127c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 2020 6966 2064 6973 7420 3c20        if dist < 
-000127f0: 7175 616c 6974 793a 0d0a 2020 2020 2020  quality:..      
-00012800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
-00012830: 6e74 726f 6964 203d 2073 706f 745f 6365  ntroid = spot_ce
-00012840: 6e74 726f 6964 735b 696e 6465 785d 0d0a  ntroids[index]..
-00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012870: 2020 2020 2020 2020 2020 2020 6672 616d              fram
-00012880: 655f 7370 6f74 5f63 656e 7472 6f69 6420  e_spot_centroid 
-00012890: 3d20 2869 6e74 2874 696d 655f 6b65 7929  = (int(time_key)
-000128a0: 2c63 6c6f 7365 7374 5f63 656e 7472 6f69  ,closest_centroi
-000128b0: 645b 305d 2c20 636c 6f73 6573 745f 6365  d[0], closest_ce
-000128c0: 6e74 726f 6964 5b31 5d2c 2063 6c6f 7365  ntroid[1], close
-000128d0: 7374 5f63 656e 7472 6f69 645b 325d 290d  st_centroid[2]).
-000128e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
-00012910: 7365 7374 5f63 656c 6c5f 6964 203d 2073  sest_cell_id = s
-00012920: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00012930: 6365 6e74 726f 6964 5b66 7261 6d65 5f73  centroid[frame_s
-00012940: 706f 745f 6365 6e74 726f 6964 5d0d 0a20  pot_centroid].. 
-00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
-00012980: 7665 6374 6f72 203d 205b 2066 6c6f 6174  vector = [ float
-00012990: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000129a0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000129b0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-000129c0: 295d 5b73 656c 662e 6d61 736b 6365 6e74  )][self.maskcent
-000129d0: 726f 6964 5f78 5f6b 6579 5d29 2c20 666c  roid_x_key]), fl
-000129e0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-000129f0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012a00: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012a10: 5f69 6429 5d5b 7365 6c66 2e6d 6173 6b63  _id)][self.maskc
-00012a20: 656e 7472 6f69 645f 795f 6b65 795d 292c  entroid_y_key]),
-00012a30: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00012a40: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012a50: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012a60: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00012a70: 736b 6365 6e74 726f 6964 5f7a 5f6b 6579  skcentroid_z_key
-00012a80: 5d29 205d 0d0a 2020 2020 2020 2020 2020  ]) ]..          
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ab0: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-00012ac0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
-00012ad0: 6528 6365 6c6c 5f61 7869 732c 206d 6173  e(cell_axis, mas
-00012ae0: 6b5f 7665 6374 6f72 290d 0a20 2020 2020  k_vector)..     
-00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012610: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+00012620: 6c6c 5f61 7869 7320 3d20 6f75 7470 7574  ll_axis = output
+00012630: 5f6c 6172 6765 7374 5f65 6967 656e 7665  _largest_eigenve
+00012640: 6374 6f72 5b69 5d0d 0a20 2020 2020 2020  ctor[i]..       
+00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012660: 2020 2020 2020 2020 2020 2020 2073 7572               sur
+00012670: 6661 6365 5f61 7265 6120 3d20 6f75 7470  face_area = outp
+00012680: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
+00012690: 5f61 7265 615b 695d 202a 2073 656c 662e  _area[i] * self.
+000126a0: 7a63 616c 6962 7261 7469 6f6e 202a 2073  zcalibration * s
+000126b0: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+000126c0: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
+000126d0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+000126e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126f0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
+00012700: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+00012710: 7279 2863 656e 7472 6f69 6429 0d0a 2020  ry(centroid)..  
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012740: 2020 7261 6469 7573 203d 2071 7561 6c69    radius = quali
+00012750: 7479 202a 206d 6174 682e 706f 7728 7365  ty * math.pow(se
+00012760: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
+00012770: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
+00012780: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
+00012790: 6272 6174 696f 6e2c 2031 2e30 2f33 2e30  bration, 1.0/3.0
+000127a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2069 6620 6469 7374 203c         if dist <
+000127d0: 2071 7561 6c69 7479 3a0d 0a20 2020 2020   quality:..     
+000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012800: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
+00012810: 656e 7472 6f69 6420 3d20 7370 6f74 5f63  entroid = spot_c
+00012820: 656e 7472 6f69 6473 5b69 6e64 6578 5d0d  entroids[index].
+00012830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+00012860: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+00012870: 203d 2028 696e 7428 7469 6d65 5f6b 6579   = (int(time_key
+00012880: 292c 636c 6f73 6573 745f 6365 6e74 726f  ),closest_centro
+00012890: 6964 5b30 5d2c 2063 6c6f 7365 7374 5f63  id[0], closest_c
+000128a0: 656e 7472 6f69 645b 315d 2c20 636c 6f73  entroid[1], clos
+000128b0: 6573 745f 6365 6e74 726f 6964 5b32 5d29  est_centroid[2])
+000128c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128e0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000128f0: 6f73 6573 745f 6365 6c6c 5f69 6420 3d20  osest_cell_id = 
+00012900: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00012910: 5f63 656e 7472 6f69 645b 6672 616d 655f  _centroid[frame_
+00012920: 7370 6f74 5f63 656e 7472 6f69 645d 0d0a  spot_centroid]..
+00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012950: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+00012960: 5f76 6563 746f 7220 3d20 5b20 666c 6f61  _vector = [ floa
+00012970: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00012980: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012990: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+000129a0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+000129b0: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+000129c0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000129d0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000129e0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+000129f0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
+00012a00: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
+00012a10: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
+00012a20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012a30: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012a40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00012a50: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00012a60: 795d 2920 5d0d 0a20 2020 2020 2020 2020  y]) ]..         
+00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a90: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
+00012aa0: 6b20 3d20 616e 6775 6c61 725f 6368 616e  k = angular_chan
+00012ab0: 6765 2863 656c 6c5f 6178 6973 2c20 6d61  ge(cell_axis, ma
+00012ac0: 736b 5f76 6563 746f 7229 0d0a 2020 2020  sk_vector)..    
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00012b50: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00012b60: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
-00012b70: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00012b80: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-00012b90: 6b5f 6b65 7920 3a20 6365 6c6c 5f61 7869  k_key : cell_axi
-00012ba0: 735f 6d61 736b 7d29 0d0a 2020 2020 2020  s_mask})..      
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bd0: 2020 2020 2020 6966 2073 656c 662e 756e        if self.un
-00012be0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00012bf0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00012c00: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
-00012c10: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
-00012c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c50: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012c60: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012c70: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012c80: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00012c90: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00012ca0: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
-00012cb0: 3a20 6563 6365 6e74 7269 6369 7479 5f63  : eccentricity_c
-00012cc0: 6f6d 705f 6669 7273 7479 7a5b 305d 202a  omp_firstyz[0] *
-00012cd0: 2073 6361 6c65 5f31 7d29 0d0a 2020 2020   scale_1})..    
+00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00012b30: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00012b40: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+00012b50: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00012b60: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
+00012b70: 736b 5f6b 6579 203a 2063 656c 6c5f 6178  sk_key : cell_ax
+00012b80: 6973 5f6d 6173 6b7d 290d 0a20 2020 2020  is_mask})..     
+00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 2020 2020 2069 6620 7365 6c66 2e75         if self.u
+00012bc0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00012bd0: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+00012be0: 745f 6365 6c6c 5f69 6429 5d5b 7365 6c66  t_cell_id)][self
+00012bf0: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
+00012c00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012c40: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012c50: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00012c60: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00012c70: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+00012c80: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+00012c90: 203a 2065 6363 656e 7472 6963 6974 795f   : eccentricity_
+00012ca0: 636f 6d70 5f66 6972 7374 797a 5b30 5d20  comp_firstyz[0] 
+00012cb0: 2a20 7363 616c 655f 317d 290d 0a20 2020  * scale_1})..   
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d10: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012d20: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00012d30: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012d40: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00012d50: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00012d60: 5f73 6563 6f6e 646b 6579 203a 2065 6363  _secondkey : ecc
-00012d70: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
-00012d80: 6972 7374 797a 5b31 5d20 2a20 7363 616c  irstyz[1] * scal
-00012d90: 655f 327d 290d 0a20 2020 2020 2020 2020  e_2})..         
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012dd0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00012de0: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00012df0: 7374 5f63 656c 6c5f 6964 295d 2e75 7064  st_cell_id)].upd
-00012e00: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
-00012e10: 655f 6172 6561 5f6b 6579 203a 2073 7572  e_area_key : sur
-00012e20: 6661 6365 5f61 7265 617d 290d 0a20 2020  face_area})..   
+00012cf0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012d00: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012d10: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012d20: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00012d30: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00012d40: 705f 7365 636f 6e64 6b65 7920 3a20 6563  p_secondkey : ec
+00012d50: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00012d60: 6669 7273 7479 7a5b 315d 202a 2073 6361  firstyz[1] * sca
+00012d70: 6c65 5f32 7d29 0d0a 2020 2020 2020 2020  le_2})..        
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012db0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00012dc0: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00012dd0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
+00012de0: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
+00012df0: 6365 5f61 7265 615f 6b65 7920 3a20 7375  ce_area_key : su
+00012e00: 7266 6163 655f 6172 6561 7d29 0d0a 2020  rface_area})..  
+00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e60: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00012e70: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00012e80: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
-00012e90: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00012ea0: 7175 616c 6974 795f 6b65 7920 3a20 7175  quality_key : qu
-00012eb0: 616c 6974 797d 290d 0a20 2020 2020 2020  ality})..       
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012ef0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00012f00: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00012f10: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00012f20: 7064 6174 6528 7b73 656c 662e 7261 6469  pdate({self.radi
-00012f30: 7573 5f6b 6579 203a 2072 6164 6975 7320  us_key : radius 
-00012f40: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00012e50: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00012e60: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00012e70: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00012e80: 2e71 7561 6c69 7479 5f6b 6579 203a 2071  .quality_key : q
+00012e90: 7561 6c69 7479 7d29 0d0a 2020 2020 2020  uality})..      
+00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012ed0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00012ee0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012ef0: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00012f00: 7570 6461 7465 287b 7365 6c66 2e72 6164  update({self.rad
+00012f10: 6975 735f 6b65 7920 3a20 7261 6469 7573  ius_key : radius
+00012f20: 207d 290d 0a20 2020 2020 2020 2020 2020   })..           
+00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
 00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00012f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f80: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fa0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fe0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012ff0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00013000: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00013010: 5d2e 7570 6461 7465 287b 7365 6c66 2e65  ].update({self.e
-00013020: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00013030: 5f66 6972 7374 6b65 7920 3a20 2d31 7d29  _firstkey : -1})
-00013040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013070: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00013080: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00013090: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-000130a0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-000130b0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-000130c0: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
-000130d0: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013110: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00013120: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00013130: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00013140: 7064 6174 6528 7b73 656c 662e 7375 7266  pdate({self.surf
-00013150: 6163 655f 6172 6561 5f6b 6579 203a 202d  ace_area_key : -
-00013160: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-00013170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-000131a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000131b0: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-000131c0: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
-000131d0: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
-000131e0: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
+00012fc0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012fd0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012fe0: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012ff0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00013000: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013010: 705f 6669 7273 746b 6579 203a 202d 317d  p_firstkey : -1}
+00013020: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013050: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00013060: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00013070: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00013080: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00013090: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+000130a0: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
+000130b0: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
+000130c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000130e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000130f0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00013100: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00013110: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00013120: 7570 6461 7465 287b 7365 6c66 2e73 7572  update({self.sur
+00013130: 6661 6365 5f61 7265 615f 6b65 7920 3a20  face_area_key : 
+00013140: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
+00013150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013170: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00013180: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00013190: 7274 6965 735b 696e 7428 636c 6f73 6573  rties[int(closes
+000131a0: 745f 6365 6c6c 5f69 6429 5d2e 7570 6461  t_cell_id)].upda
+000131b0: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
+000131c0: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00013230: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00013240: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00013250: 5d2e 7570 6461 7465 287b 7365 6c66 2e72  ].update({self.r
-00013260: 6164 6975 735f 6b65 7920 3a20 2d31 207d  adius_key : -1 }
-00013270: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2020 2020 2020 0d0a 0d0a 0d0a 0d0a 0d0a        ..........
-000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00013210: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00013220: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00013230: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00013240: 7261 6469 7573 5f6b 6579 203a 202d 3120  radius_key : -1 
+00013250: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013280: 2020 2020 2020 200d 0a0d 0a0d 0a0d 0a0d         .........
+00013290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
 000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132d0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132f0: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00013300: 6c66 2e72 6f6f 745f 7370 6f74 732e 6974  lf.root_spots.it
-00013310: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00013340: 6f6f 745f 7370 6f74 735b 6b5d 203d 2073  oot_spots[k] = s
-00013350: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00013360: 7072 6f70 6572 7469 6573 5b6b 5d20 2020  properties[k]   
-00013370: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00013380: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00013390: 6620 5f63 6f6d 7075 7465 5f70 6865 6e6f  f _compute_pheno
-000133a0: 7479 7065 7328 7365 6c66 293a 0d0a 0d0a  types(self):....
-000133b0: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
-000133c0: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
-000133d0: 7565 5f74 7261 636b 732e 6974 656d 7328  ue_tracks.items(
-000133e0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000133f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00013400: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-00013410: 206b 0d0a 2020 2020 2020 2020 2020 2020   k..            
-00013420: 2020 2020 7472 6163 6b6c 6574 5f70 726f      tracklet_pro
-00013430: 7065 7274 6965 7320 3d20 7365 6c66 2e75  perties = self.u
-00013440: 6e69 7175 655f 7472 6163 6b5f 7072 6f70  nique_track_prop
-00013450: 6572 7469 6573 5b6b 5d0d 0a20 2020 2020  erties[k]..     
-00013460: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00013470: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00013480: 7472 6163 6b73 5b6b 5d0d 0a20 2020 2020  tracks[k]..     
-00013490: 2020 2020 2020 2020 2020 205a 203d 2074             Z = t
-000134a0: 7261 636b 735b 3a2c 325d 0d0a 2020 2020  racks[:,2]..    
-000134b0: 2020 2020 2020 2020 2020 2020 5920 3d20              Y = 
-000134c0: 7472 6163 6b73 5b3a 2c33 5d0d 0a20 2020  tracks[:,3]..   
-000134d0: 2020 2020 2020 2020 2020 2020 2058 203d               X =
-000134e0: 2074 7261 636b 735b 3a2c 345d 0d0a 2020   tracks[:,4]..  
-000134f0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00013500: 6d65 203d 2074 7261 636b 6c65 745f 7072  me = tracklet_pr
-00013510: 6f70 6572 7469 6573 5b3a 2c30 5d0d 0a20  operties[:,0].. 
-00013520: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00013530: 6e69 7175 655f 6964 7320 3d20 7472 6163  nique_ids = trac
-00013540: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00013550: 3a2c 315d 0d0a 2020 2020 2020 2020 2020  :,1]..          
-00013560: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
-00013570: 5f73 6574 203d 2073 6574 2875 6e69 7175  _set = set(uniqu
-00013580: 655f 6964 7329 0d0a 2020 2020 2020 2020  e_ids)..        
-00013590: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
-000135a0: 6f6e 5f69 6473 203d 2074 7261 636b 6c65  on_ids = trackle
-000135b0: 745f 7072 6f70 6572 7469 6573 5b3a 2c32  t_properties[:,2
-000135c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000135d0: 2020 2072 6164 6975 7320 3d20 7472 6163     radius = trac
-000135e0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-000135f0: 3a2c 335d 0d0a 2020 2020 2020 2020 2020  :,3]..          
-00013600: 2020 2020 2020 766f 6c75 6d65 203d 2074        volume = t
-00013610: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00013620: 6573 5b3a 2c34 5d0d 0a20 2020 2020 2020  es[:,4]..       
-00013630: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-00013640: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00013650: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013660: 6572 7469 6573 5b3a 2c35 5d0d 0a20 2020  erties[:,5]..   
-00013670: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
-00013680: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-00013690: 6563 6f6e 6420 3d20 7472 6163 6b6c 6574  econd = tracklet
-000136a0: 5f70 726f 7065 7274 6965 735b 3a2c 365d  _properties[:,6]
-000136b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000136c0: 2020 7375 7266 6163 655f 6172 6561 203d    surface_area =
-000136d0: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-000136e0: 7469 6573 5b3a 2c37 5d0d 0a20 2020 2020  ties[:,7]..     
-000136f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00013700: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-00013710: 6e73 6974 7920 3d20 7472 6163 6b6c 6574  nsity = tracklet
-00013720: 5f70 726f 7065 7274 6965 735b 3a2c 385d  _properties[:,8]
-00013730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013740: 2020 7370 6565 6420 3d20 7472 6163 6b6c    speed = trackl
-00013750: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-00013760: 395d 0d0a 2020 2020 2020 2020 2020 2020  9]..            
-00013770: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
-00013780: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013790: 6572 7469 6573 5b3a 2c31 305d 0d0a 2020  erties[:,10]..  
-000137a0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000137b0: 6365 6c65 7261 7469 6f6e 203d 2074 7261  celeration = tra
-000137c0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-000137d0: 5b3a 2c31 315d 0d0a 2020 2020 2020 2020  [:,11]..        
-000137e0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-000137f0: 5f63 656c 6c5f 6d61 736b 203d 2074 7261  _cell_mask = tra
-00013800: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00013810: 5b3a 2c31 325d 0d0a 2020 2020 2020 2020  [:,12]..        
-00013820: 2020 2020 2020 2020 7261 6469 616c 5f61          radial_a
-00013830: 6e67 6c65 203d 2074 7261 636b 6c65 745f  ngle = tracklet_
-00013840: 7072 6f70 6572 7469 6573 5b3a 2c31 335d  properties[:,13]
-00013850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013860: 2020 6365 6c6c 5f61 7869 735f 6d61 736b    cell_axis_mask
-00013870: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013880: 6572 7469 6573 5b3a 2c31 345d 0d0a 2020  erties[:,14]..  
-00013890: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000138a0: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
-000138b0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-000138c0: 6572 7469 6573 5b3a 2c31 355d 0d0a 2020  erties[:,15]..  
-000138d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000138e0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-000138f0: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
-00013900: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013910: 6572 7469 6573 5b3a 2c31 365d 0d0a 2020  erties[:,16]..  
-00013920: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00013930: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-00013940: 7472 6163 6b5f 6469 7374 616e 6365 203d  track_distance =
-00013950: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00013960: 7469 6573 5b3a 2c31 375d 0d0a 2020 2020  ties[:,17]..    
-00013970: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00013980: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00013990: 5f64 7572 6174 696f 6e20 3d20 7472 6163  _duration = trac
-000139a0: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-000139b0: 3a2c 3138 5d0d 0a0d 0a0d 0a20 2020 2020  :,18]......     
-000139c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000139d0: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-000139e0: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
-000139f0: 6573 5f74 7261 636b 6c65 7420 3d20 7b7d  es_tracklet = {}
-00013a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013a10: 2020 756e 6971 7565 5f63 6c75 7374 6572    unique_cluster
-00013a20: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00013a30: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
-00013a40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013a50: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
-00013a60: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
-00013a70: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00013a80: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00013a90: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
-00013aa0: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
-00013ab0: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
-00013ac0: 2020 2020 2020 2075 6e69 7175 655f 7368         unique_sh
-00013ad0: 6170 655f 7072 6f70 6572 7469 6573 5f74  ape_properties_t
-00013ae0: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
-00013af0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00013b00: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
-00013b10: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00013b20: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00013b30: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00013b40: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
-00013b50: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00013b60: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00013b70: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00013b80: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
-00013b90: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-00013ba0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00013bb0: 2020 2065 7870 616e 6465 645f 7469 6d65     expanded_time
-00013bc0: 203d 206e 702e 7a65 726f 7328 7365 6c66   = np.zeros(self
-00013bd0: 2e74 656e 6420 2d20 7365 6c66 2e74 7374  .tend - self.tst
-00013be0: 6172 7420 2b20 3129 0d0a 2020 2020 2020  art + 1)..      
-00013bf0: 2020 2020 2020 2020 2020 706f 696e 745f            point_
-00013c00: 7361 6d70 6c65 203d 2065 7870 616e 6465  sample = expande
-00013c10: 645f 7469 6d65 2e73 6861 7065 5b30 5d0d  d_time.shape[0].
-00013c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c30: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00013c40: 6c65 6e28 6578 7061 6e64 6564 5f74 696d  len(expanded_tim
-00013c50: 6529 293a 0d0a 2020 2020 2020 2020 2020  e)):..          
-00013c60: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00013c70: 616e 6465 645f 7469 6d65 5b69 5d20 3d20  anded_time[i] = 
-00013c80: 6920 0d0a 2020 2020 2020 2020 2020 2020  i ..            
-00013c90: 2020 2020 666f 7220 6375 7272 656e 745f      for current_
-00013ca0: 756e 6971 7565 5f69 6420 696e 2075 6e69  unique_id in uni
-00013cb0: 7175 655f 6964 735f 7365 743a 0d0a 2020  que_ids_set:..  
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013ce0: 2020 2020 2020 6578 7061 6e64 6564 5f69        expanded_i
-00013cf0: 6e74 656e 7369 7479 203d 206e 702e 7a65  ntensity = np.ze
-00013d00: 726f 7328 7365 6c66 2e74 656e 6420 2d20  ros(self.tend - 
-00013d10: 7365 6c66 2e74 7374 6172 7420 2b20 3129  self.tstart + 1)
-00013d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013d30: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00013d40: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013d60: 7572 7265 6e74 5f74 696d 6520 3d20 5b5d  urrent_time = []
-00013d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013d80: 2020 2020 2063 7572 7265 6e74 5f7a 203d       current_z =
-00013d90: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00013da0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013db0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-00013dc0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00013dd0: 6e74 5f78 203d 205b 5d0d 0a20 2020 2020  nt_x = []..     
-00013de0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013df0: 7272 656e 745f 696e 7465 6e73 6974 7920  rrent_intensity 
-00013e00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00013e10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013e20: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
-00013e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e40: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
-00013e50: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00013e60: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013e70: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-00013e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e90: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
-00013ea0: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
-00013eb0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013ec0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
-00013ed0: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
-00013ee0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013ef0: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
-00013f00: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00013f30: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-00013f40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00013f50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013f60: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00013f70: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
-00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f90: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
-00013fa0: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
-00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fc0: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
-00013fd0: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
-00014000: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
-00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
-00014030: 6469 7370 6c61 6365 6d65 6e74 203d 205b  displacement = [
-00014040: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00014050: 2020 2020 2020 6375 7272 656e 745f 746f        current_to
-00014060: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
-00014070: 6365 203d 205b 5d0d 0a20 2020 2020 2020  ce = []..       
-00014080: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00014090: 656e 745f 6d61 785f 7472 6163 6b5f 6469  ent_max_track_di
-000140a0: 7374 616e 6365 203d 205b 5d0d 0a20 2020  stance = []..   
-000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140c0: 6375 7272 656e 745f 7472 6163 6b5f 6475  current_track_du
-000140d0: 7261 7469 6f6e 203d 205b 5d0d 0a20 2020  ration = []..   
-000140e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014100: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00014110: 6e67 6528 7469 6d65 2e73 6861 7065 5b30  nge(time.shape[0
-00014120: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-00014130: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014140: 6620 6375 7272 656e 745f 756e 6971 7565  f current_unique
-00014150: 5f69 6420 3d3d 2075 6e69 7175 655f 6964  _id == unique_id
-00014160: 735b 6a5d 3a0d 0a20 2020 2020 2020 2020  s[j]:..         
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014190: 7469 6d65 2e61 7070 656e 6428 7469 6d65  time.append(time
-000141a0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141c0: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
-000141d0: 2e61 7070 656e 6428 5a5b 6a5d 290d 0a20  .append(Z[j]).. 
-000141e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014200: 6375 7272 656e 745f 792e 6170 7065 6e64  current_y.append
-00014210: 2859 5b6a 5d29 0d0a 2020 2020 2020 2020  (Y[j])..        
-00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014230: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00014240: 5f78 2e61 7070 656e 6428 585b 6a5d 290d  _x.append(X[j]).
-00014250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
-00014280: 7369 7479 5b69 6e74 2874 696d 655b 6a5d  sity[int(time[j]
-00014290: 295d 203d 2069 6e74 656e 7369 7479 5b6a  )] = intensity[j
-000142a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000142b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142c0: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
-000142d0: 6e73 6974 792e 6170 7065 6e64 2869 6e74  nsity.append(int
-000142e0: 656e 7369 7479 5b6a 5d29 0d0a 2020 2020  ensity[j])..    
-000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014300: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00014310: 7265 6e74 5f72 6164 6975 732e 6170 7065  rent_radius.appe
-00014320: 6e64 2872 6164 6975 735b 6a5d 290d 0a20  nd(radius[j]).. 
-00014330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014350: 6375 7272 656e 745f 766f 6c75 6d65 2e61  current_volume.a
-00014360: 7070 656e 6428 766f 6c75 6d65 5b6a 5d29  ppend(volume[j])
-00014370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
-000143a0: 2e61 7070 656e 6428 7370 6565 645b 6a5d  .append(speed[j]
-000143b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143d0: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
-000143e0: 6f6e 5f61 6e67 6c65 2e61 7070 656e 6428  on_angle.append(
-000143f0: 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a 5d29  motion_angle[j])
-00014400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
-00014430: 6572 6174 696f 6e2e 6170 7065 6e64 2861  eration.append(a
-00014440: 6363 656c 6572 6174 696f 6e5b 6a5d 290d  cceleration[j]).
-00014450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014470: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
-00014480: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00014490: 656e 6428 6469 7374 616e 6365 5f63 656c  end(distance_cel
-000144a0: 6c5f 6d61 736b 5b6a 5d29 0d0a 2020 2020  l_mask[j])..    
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000144d0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-000144e0: 795f 636f 6d70 5f66 6972 7374 2e61 7070  y_comp_first.app
-000144f0: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
-00014500: 5f63 6f6d 705f 6669 7273 745b 6a5d 290d  _comp_first[j]).
-00014510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00014540: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00014550: 6e64 2e61 7070 656e 6428 6563 6365 6e74  nd.append(eccent
-00014560: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00014570: 6e64 5b6a 5d29 0d0a 2020 2020 2020 2020  nd[j])..        
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000145a0: 5f73 7572 6661 6365 5f61 7265 612e 6170  _surface_area.ap
-000145b0: 7065 6e64 2873 7572 6661 6365 5f61 7265  pend(surface_are
-000145c0: 615b 6a5d 290d 0a20 2020 2020 2020 2020  a[j])..         
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000145f0: 7261 6469 616c 5f61 6e67 6c65 2e61 7070  radial_angle.app
-00014600: 656e 6428 7261 6469 616c 5f61 6e67 6c65  end(radial_angle
-00014610: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014630: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00014640: 656c 6c5f 6178 6973 5f6d 6173 6b2e 6170  ell_axis_mask.ap
-00014650: 7065 6e64 2863 656c 6c5f 6178 6973 5f6d  pend(cell_axis_m
-00014660: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
-00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014680: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014690: 745f 7472 6163 6b5f 6469 7370 6c61 6365  t_track_displace
-000146a0: 6d65 6e74 2e61 7070 656e 6428 7472 6163  ment.append(trac
-000146b0: 6b5f 6469 7370 6c61 6365 6d65 6e74 5b6a  k_displacement[j
-000146c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2020 2063 7572 7265 6e74 5f74 6f74       current_tot
-000146f0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
-00014700: 652e 6170 7065 6e64 2874 6f74 616c 5f74  e.append(total_t
-00014710: 7261 636b 5f64 6973 7461 6e63 655b 6a5d  rack_distance[j]
-00014720: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014740: 2020 2020 6375 7272 656e 745f 6d61 785f      current_max_
-00014750: 7472 6163 6b5f 6469 7374 616e 6365 2e61  track_distance.a
-00014760: 7070 656e 6428 6d61 785f 7472 6163 6b5f  ppend(max_track_
-00014770: 6469 7374 616e 6365 5b6a 5d29 0d0a 2020  distance[j])..  
-00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014790: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000147a0: 7572 7265 6e74 5f74 7261 636b 5f64 7572  urrent_track_dur
-000147b0: 6174 696f 6e2e 6170 7065 6e64 2874 7261  ation.append(tra
-000147c0: 636b 5f64 7572 6174 696f 6e5b 6a5d 290d  ck_duration[j]).
-000147d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00014800: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014810: 745f 7469 6d65 203d 206e 702e 6173 6172  t_time = np.asar
-00014820: 7261 7928 6375 7272 656e 745f 7469 6d65  ray(current_time
-00014830: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00014840: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00014850: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014860: 696e 7465 6e73 6974 7920 3d20 6e70 2e61  intensity = np.a
-00014870: 7361 7272 6179 2863 7572 7265 6e74 5f69  sarray(current_i
-00014880: 6e74 656e 7369 7479 2c20 6474 7970 653d  ntensity, dtype=
-00014890: 6e70 2e66 6c6f 6174 3332 290d 0a0d 0a0d  np.float32).....
-000148a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000148b0: 2020 2020 2020 6375 7272 656e 745f 7261        current_ra
-000148c0: 6469 7573 203d 206e 702e 6173 6172 7261  dius = np.asarra
-000148d0: 7928 6375 7272 656e 745f 7261 6469 7573  y(current_radius
-000148e0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000148f0: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00014900: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014910: 766f 6c75 6d65 203d 206e 702e 6173 6172  volume = np.asar
-00014920: 7261 7928 6375 7272 656e 745f 766f 6c75  ray(current_volu
-00014930: 6d65 2c20 6474 7970 653d 6e70 2e66 6c6f  me, dtype=np.flo
-00014940: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014950: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014960: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00014970: 6f6d 705f 6669 7273 7420 3d20 6e70 2e61  omp_first = np.a
-00014980: 7361 7272 6179 2863 7572 7265 6e74 5f65  sarray(current_e
-00014990: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-000149a0: 5f66 6972 7374 2c20 6474 7970 653d 6e70  _first, dtype=np
-000149b0: 2e66 6c6f 6174 3332 290d 0a20 2020 2020  .float32)..     
-000149c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000149d0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-000149e0: 7479 5f63 6f6d 705f 7365 636f 6e64 203d  ty_comp_second =
-000149f0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014a00: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
-00014a10: 5f63 6f6d 705f 7365 636f 6e64 2c20 6474  _comp_second, dt
-00014a20: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00014a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014a40: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
-00014a50: 6163 655f 6172 6561 203d 206e 702e 6173  ace_area = np.as
-00014a60: 6172 7261 7928 6375 7272 656e 745f 7375  array(current_su
-00014a70: 7266 6163 655f 6172 6561 2c20 6474 7970  rface_area, dtyp
-00014a80: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
-00014a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014aa0: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
-00014ab0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
-00014ac0: 7572 7265 6e74 5f73 7065 6564 2c20 6474  urrent_speed, dt
-00014ad0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00014ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014af0: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
-00014b00: 6f6e 5f61 6e67 6c65 203d 206e 702e 6173  on_angle = np.as
-00014b10: 6172 7261 7928 6375 7272 656e 745f 6d6f  array(current_mo
-00014b20: 7469 6f6e 5f61 6e67 6c65 2c20 6474 7970  tion_angle, dtyp
-00014b30: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b50: 2020 6375 7272 656e 745f 6163 6365 6c65    current_accele
-00014b60: 7261 7469 6f6e 203d 206e 702e 6173 6172  ration = np.asar
-00014b70: 7261 7928 6375 7272 656e 745f 6163 6365  ray(current_acce
-00014b80: 6c65 7261 7469 6f6e 2c20 6474 7970 653d  leration, dtype=
-00014b90: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bb0: 6375 7272 656e 745f 6469 7374 616e 6365  current_distance
-00014bc0: 5f63 656c 6c5f 6d61 736b 203d 206e 702e  _cell_mask = np.
-00014bd0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00014be0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00014bf0: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
-00014c00: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014c10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014c20: 745f 7261 6469 616c 5f61 6e67 6c65 203d  t_radial_angle =
-00014c30: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014c40: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
-00014c50: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00014c60: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
-00014c70: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014c80: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-00014c90: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00014ca0: 656e 745f 6365 6c6c 5f61 7869 735f 6d61  ent_cell_axis_ma
-00014cb0: 736b 2c20 6474 7970 653d 6e70 2e66 6c6f  sk, dtype=np.flo
-00014cc0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014cd0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014cf0: 7572 7265 6e74 5f74 7261 636b 5f64 6973  urrent_track_dis
-00014d00: 706c 6163 656d 656e 7420 3d20 6e70 2e61  placement = np.a
-00014d10: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
-00014d20: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
-00014d30: 742c 2064 7479 7065 3d6e 702e 666c 6f61  t, dtype=np.floa
-00014d40: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
-00014d50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00014d60: 5f74 6f74 616c 5f74 7261 636b 5f64 6973  _total_track_dis
-00014d70: 7461 6e63 6520 3d20 6e70 2e61 7361 7272  tance = np.asarr
-00014d80: 6179 2863 7572 7265 6e74 5f74 6f74 616c  ay(current_total
-00014d90: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
-00014da0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00014db0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
-00014dc0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
-00014dd0: 6178 5f74 7261 636b 5f64 6973 7461 6e63  ax_track_distanc
-00014de0: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
-00014df0: 7572 7265 6e74 5f6d 6178 5f74 7261 636b  urrent_max_track
-00014e00: 5f64 6973 7461 6e63 652c 2064 7479 7065  _distance, dtype
-00014e10: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
-00014e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e30: 2063 7572 7265 6e74 5f74 7261 636b 5f64   current_track_d
-00014e40: 7572 6174 696f 6e20 3d20 6e70 2e61 7361  uration = np.asa
-00014e50: 7272 6179 2863 7572 7265 6e74 5f74 7261  rray(current_tra
-00014e60: 636b 5f64 7572 6174 696f 6e2c 2064 7479  ck_duration, dty
-00014e70: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
-00014e80: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00014e90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00014ea0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ec0: 2069 6620 706f 696e 745f 7361 6d70 6c65   if point_sample
-00014ed0: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00014ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ef0: 2020 2020 2020 2078 665f 7361 6d70 6c65         xf_sample
-00014f00: 203d 2066 6674 6672 6571 2870 6f69 6e74   = fftfreq(point
-00014f10: 5f73 616d 706c 652c 2073 656c 662e 7463  _sample, self.tc
-00014f20: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
-00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f40: 2020 2020 2020 2020 2020 2020 2066 6674               fft
-00014f50: 7374 7269 705f 7361 6d70 6c65 203d 2066  strip_sample = f
-00014f60: 6674 2865 7870 616e 6465 645f 696e 7465  ft(expanded_inte
-00014f70: 6e73 6974 7929 0d0a 2020 2020 2020 2020  nsity)..        
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f90: 2020 2020 2020 2020 6666 7474 6f74 616c          ffttotal
-00014fa0: 5f73 616d 706c 6520 3d20 6e70 2e61 6273  _sample = np.abs
-00014fb0: 2866 6674 7374 7269 705f 7361 6d70 6c65  (fftstrip_sample
-00014fc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fe0: 2020 2078 665f 7361 6d70 6c65 203d 2078     xf_sample = x
-00014ff0: 665f 7361 6d70 6c65 5b30 203a 206c 656e  f_sample[0 : len
-00015000: 2878 665f 7361 6d70 6c65 2920 2f2f 2032  (xf_sample) // 2
-00015010: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015030: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
-00015040: 6c65 203d 2066 6674 746f 7461 6c5f 7361  le = ffttotal_sa
-00015050: 6d70 6c65 5b30 203a 206c 656e 2866 6674  mple[0 : len(fft
-00015060: 746f 7461 6c5f 7361 6d70 6c65 2920 2f2f  total_sample) //
-00015070: 2032 5d0d 0a0d 0a20 2020 2020 2020 2020   2]....         
-00015080: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00015090: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
-000150a0: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-000150b0: 5f75 6e69 7175 655f 6964 5d20 3d20 6578  _unique_id] = ex
-000150c0: 7061 6e64 6564 5f74 696d 652c 2065 7870  panded_time, exp
-000150d0: 616e 6465 645f 696e 7465 6e73 6974 792c  anded_intensity,
-000150e0: 2078 665f 7361 6d70 6c65 2c20 6666 7474   xf_sample, fftt
-000150f0: 6f74 616c 5f73 616d 706c 650d 0a20 2020  otal_sample..   
-00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015110: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
-00015120: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00015130: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
-00015140: 655f 6964 5d20 3d20 2063 7572 7265 6e74  e_id] =  current
-00015150: 5f74 696d 650d 0a20 2020 2020 2020 2020  _time..         
-00015160: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-00015170: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00015180: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-00015190: 6e74 5f75 6e69 7175 655f 6964 5d20 3d20  nt_unique_id] = 
-000151a0: 6375 7272 656e 745f 7469 6d65 2c20 6375  current_time, cu
-000151b0: 7272 656e 745f 7a2c 2063 7572 7265 6e74  rrent_z, current
-000151c0: 5f79 2c20 6375 7272 656e 745f 782c 2063  _y, current_x, c
-000151d0: 7572 7265 6e74 5f72 6164 6975 732c 2063  urrent_radius, c
-000151e0: 7572 7265 6e74 5f76 6f6c 756d 652c 2063  urrent_volume, c
-000151f0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00015200: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
-00015210: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00015220: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00015230: 2c20 6375 7272 656e 745f 7375 7266 6163  , current_surfac
-00015240: 655f 6172 6561 0d0a 2020 2020 2020 2020  e_area..        
-00015250: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00015260: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
-00015270: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00015280: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00015290: 203d 2063 7572 7265 6e74 5f74 696d 652c   = current_time,
-000152a0: 2063 7572 7265 6e74 5f73 7065 6564 2c20   current_speed, 
-000152b0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
-000152c0: 6e67 6c65 2c20 6375 7272 656e 745f 6163  ngle, current_ac
-000152d0: 6365 6c65 7261 7469 6f6e 2c20 6375 7272  celeration, curr
-000152e0: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
-000152f0: 6c5f 6d61 736b 2c20 6375 7272 656e 745f  l_mask, current_
-00015300: 7261 6469 616c 5f61 6e67 6c65 2c20 6375  radial_angle, cu
-00015310: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
-00015320: 6d61 736b 2c20 6375 7272 656e 745f 7472  mask, current_tr
-00015330: 6163 6b5f 6469 7370 6c61 6365 6d65 6e74  ack_displacement
-00015340: 2c20 6375 7272 656e 745f 746f 7461 6c5f  , current_total_
-00015350: 7472 6163 6b5f 6469 7374 616e 6365 2c20  track_distance, 
-00015360: 6375 7272 656e 745f 6d61 785f 7472 6163  current_max_trac
-00015370: 6b5f 6469 7374 616e 6365 2c20 6375 7272  k_distance, curr
-00015380: 656e 745f 7472 6163 6b5f 6475 7261 7469  ent_track_durati
-00015390: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000153a0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000153b0: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
-000153c0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-000153d0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-000153e0: 7565 5f69 643a 756e 6971 7565 5f66 6674  ue_id:unique_fft
-000153f0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00015400: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00015410: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
-00015420: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015430: 6c66 2e75 6e69 7175 655f 636c 7573 7465  lf.unique_cluste
-00015440: 725f 7072 6f70 6572 7469 6573 5b74 7261  r_properties[tra
-00015450: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00015460: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00015470: 3a75 6e69 7175 655f 636c 7573 7465 725f  :unique_cluster_
-00015480: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00015490: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-000154a0: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
-000154b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000154c0: 656c 662e 756e 6971 7565 5f73 6861 7065  elf.unique_shape
-000154d0: 5f70 726f 7065 7274 6965 735b 7472 6163  _properties[trac
-000154e0: 6b5f 6964 5d2e 7570 6461 7465 287b 6375  k_id].update({cu
-000154f0: 7272 656e 745f 756e 6971 7565 5f69 643a  rrent_unique_id:
-00015500: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
-00015510: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00015520: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-00015530: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
-00015540: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00015550: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
-00015560: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
-00015570: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
-00015580: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
-00015590: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
-000155a0: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-000155b0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-000155c0: 645d 7d29 0d0a 0d0a 2020 2020 6465 6620  d]})....    def 
-000155d0: 5f73 6563 6f6e 645f 6368 616e 6e65 6c5f  _second_channel_
-000155e0: 7370 6f74 7328 7365 6c66 2c20 6672 616d  spots(self, fram
-000155f0: 652c 207a 2c20 792c 2078 2c20 6365 6c6c  e, z, y, x, cell
-00015600: 5f69 642c 2074 7261 636b 5f69 6429 3a0d  _id, track_id):.
-00015610: 0a20 2020 2020 2020 2020 2020 0d0a 2020  .           ..  
-00015620: 2020 2020 2020 2020 2020 7472 6565 2c20            tree, 
-00015630: 6365 6e74 726f 6964 732c 206c 6162 656c  centroids, label
-00015640: 732c 2076 6f6c 756d 652c 2069 6e74 656e  s, volume, inten
-00015650: 7369 7479 5f6d 6561 6e2c 2069 6e74 656e  sity_mean, inten
-00015660: 7369 7479 5f74 6f74 616c 2c20 626f 756e  sity_total, boun
-00015670: 6469 6e67 5f62 6f78 6573 203d 2073 656c  ding_boxes = sel
-00015680: 662e 5f74 696d 6564 5f63 6861 6e6e 656c  f._timed_channel
-00015690: 5f73 6567 5f69 6d61 6765 5b73 7472 2869  _seg_image[str(i
-000156a0: 6e74 2866 6c6f 6174 2866 7261 6d65 2929  nt(float(frame))
-000156b0: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-000156c0: 7069 7865 6c74 6573 746c 6f63 6174 696f  pixeltestlocatio
-000156d0: 6e20 3d20 287a 2c79 2c78 290d 0a20 2020  n = (z,y,x)..   
-000156e0: 2020 2020 2020 2020 2064 6973 742c 2069           dist, i
-000156f0: 6e64 6578 203d 2074 7265 652e 7175 6572  ndex = tree.quer
-00015700: 7928 7069 7865 6c74 6573 746c 6f63 6174  y(pixeltestlocat
-00015710: 696f 6e29 0d0a 0d0a 0d0a 2020 2020 2020  ion)......      
-00015720: 2020 2020 2020 6262 6f78 203d 2062 6f75        bbox = bou
-00015730: 6e64 696e 675f 626f 7865 735b 696e 6465  nding_boxes[inde
-00015740: 785d 0d0a 2020 2020 2020 2020 2020 2020  x]..            
-00015750: 7369 7a65 7a20 3d20 6162 7328 6262 6f78  sizez = abs(bbox
-00015760: 5b30 5d20 2d20 6262 6f78 5b33 5d29 0d0a  [0] - bbox[3])..
-00015770: 2020 2020 2020 2020 2020 2020 7369 7a65              size
-00015780: 7920 3d20 6162 7328 6262 6f78 5b31 5d20  y = abs(bbox[1] 
-00015790: 2d20 6262 6f78 5b34 5d29 0d0a 2020 2020  - bbox[4])..    
-000157a0: 2020 2020 2020 2020 7369 7a65 7820 3d20          sizex = 
-000157b0: 6162 7328 6262 6f78 5b32 5d20 2d20 6262  abs(bbox[2] - bb
-000157c0: 6f78 5b35 5d29 200d 0a20 2020 2020 2020  ox[5]) ..       
-000157d0: 2020 2020 2076 6574 6f5f 766f 6c75 6d65       veto_volume
-000157e0: 203d 2073 697a 6578 202a 2073 697a 6579   = sizex * sizey
-000157f0: 202a 2073 697a 657a 0d0a 2020 2020 2020   * sizez..      
-00015800: 2020 2020 2020 7665 746f 5f72 6164 6975        veto_radiu
-00015810: 7320 3d20 6d61 7468 2e70 6f77 2833 202a  s = math.pow(3 *
-00015820: 2076 6574 6f5f 766f 6c75 6d65 202f 2028   veto_volume / (
-00015830: 3420 2a20 6d61 7468 2e70 6929 2c20 312e  4 * math.pi), 1.
-00015840: 3020 2f20 332e 3029 0d0a 0d0a 2020 2020  0 / 3.0)....    
-00015850: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00015860: 203d 2028 6365 6e74 726f 6964 735b 696e   = (centroids[in
-00015870: 6465 785d 5b30 5d20 2a20 7365 6c66 2e7a  dex][0] * self.z
-00015880: 6361 6c69 6272 6174 696f 6e2c 2063 656e  calibration, cen
-00015890: 7472 6f69 6473 5b69 6e64 6578 5d5b 315d  troids[index][1]
-000158a0: 2a73 656c 662e 7963 616c 6962 7261 7469  *self.ycalibrati
-000158b0: 6f6e 2c20 6365 6e74 726f 6964 735b 696e  on, centroids[in
-000158c0: 6465 785d 5b32 5d2a 7365 6c66 2e78 6361  dex][2]*self.xca
-000158d0: 6c69 6272 6174 696f 6e29 0d0a 2020 2020  libration)..    
-000158e0: 2020 2020 2020 2020 5155 414c 4954 5920          QUALITY 
-000158f0: 3d20 6d61 7468 2e70 6f77 2876 6f6c 756d  = math.pow(volum
-00015900: 655b 696e 6465 785d 2c20 312e 302f 332e  e[index], 1.0/3.
-00015910: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00015920: 5241 4449 5553 203d 206d 6174 682e 706f  RADIUS = math.po
-00015930: 7728 766f 6c75 6d65 5b69 6e64 6578 5d20  w(volume[index] 
-00015940: 2a20 7365 6c66 2e78 6361 6c69 6272 6174  * self.xcalibrat
-00015950: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
-00015960: 6272 6174 696f 6e20 2a20 7365 6c66 2e7a  bration * self.z
-00015970: 6361 6c69 6272 6174 696f 6e2c 2031 2e30  calibration, 1.0
-00015980: 2f33 2e30 2920 0d0a 0d0a 2020 2020 2020  /3.0) ....      
-00015990: 2020 2020 2020 6469 7374 616e 6365 5f63        distance_c
-000159a0: 656c 6c5f 6d61 736b 2c20 6d61 736b 6365  ell_mask, maskce
-000159b0: 6e74 726f 6964 203d 2073 656c 662e 5f67  ntroid = self._g
-000159c0: 6574 5f62 6f75 6e64 6172 795f 6469 7374  et_boundary_dist
-000159d0: 2866 7261 6d65 2c20 6c6f 6361 7469 6f6e  (frame, location
-000159e0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-000159f0: 6620 6469 7374 203c 3d20 3220 2a20 7665  f dist <= 2 * ve
-00015a00: 746f 5f72 6164 6975 733a 0d0a 2020 2020  to_radius:..    
-00015a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015a20: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
-00015a30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00015a40: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
-00015a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a60: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
-00015a70: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
-00015a80: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
-00015a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015aa0: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
-00015ab0: 3a20 696e 7428 6672 616d 6529 2c0d 0a20  : int(frame),.. 
-00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ad0: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
-00015ae0: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
-00015af0: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00015b00: 305d 2a20 7365 6c66 2e7a 6361 6c69 6272  0]* self.zcalibr
-00015b10: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
-00015b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b30: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-00015b40: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
-00015b50: 6473 5b69 6e64 6578 5d5b 315d 2a20 7365  ds[index][1]* se
-00015b60: 6c66 2e79 6361 6c69 6272 6174 696f 6e29  lf.ycalibration)
-00015b70: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00015b80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015b90: 7870 6f73 6964 5f6b 6579 203a 2066 6c6f  xposid_key : flo
-00015ba0: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
-00015bb0: 6578 5d5b 325d 2a20 7365 6c66 2e78 6361  ex][2]* self.xca
-00015bc0: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
-00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015be0: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
-00015bf0: 645f 6b65 793a 2069 6e74 2874 7261 636b  d_key: int(track
-00015c00: 5f69 6429 2c0d 0a20 2020 2020 2020 2020  _id),..         
-00015c10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015c20: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-00015c30: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
-00015c40: 2869 6e74 656e 7369 7479 5f74 6f74 616c  (intensity_total
-00015c50: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
-00015c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c70: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-00015c80: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
-00015c90: 6c6f 6174 2869 6e74 656e 7369 7479 5f6d  loat(intensity_m
-00015ca0: 6561 6e5b 696e 6465 785d 2929 2c0d 0a20  ean[index])),.. 
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
-00015cd0: 7573 5f6b 6579 203a 2028 666c 6f61 7428  us_key : (float(
-00015ce0: 5241 4449 5553 2929 2c0d 0a20 2020 2020  RADIUS)),..     
-00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d00: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
-00015d10: 6b65 7920 3a20 2866 6c6f 6174 2851 5541  key : (float(QUA
-00015d20: 4c49 5459 2929 2c0d 0a20 2020 2020 2020  LITY)),..       
-00015d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d40: 2073 656c 662e 6469 7374 616e 6365 5f63   self.distance_c
-00015d50: 656c 6c5f 6d61 736b 5f6b 6579 3a20 666c  ell_mask_key: fl
-00015d60: 6f61 7428 6469 7374 616e 6365 5f63 656c  oat(distance_cel
-00015d70: 6c5f 6d61 736b 292c 0d0a 2020 2020 2020  l_mask),..      
-00015d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d90: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
-00015da0: 6f69 645f 7a5f 6b65 793a 2066 6c6f 6174  oid_z_key: float
-00015db0: 286d 6173 6b63 656e 7472 6f69 645b 305d  (maskcentroid[0]
-00015dc0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00015dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015de0: 2e6d 6173 6b63 656e 7472 6f69 645f 795f  .maskcentroid_y_
-00015df0: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-00015e00: 656e 7472 6f69 645b 315d 292c 0d0a 2020  entroid[1]),..  
-00015e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e20: 2020 2020 2020 7365 6c66 2e6d 6173 6b63        self.maskc
-00015e30: 656e 7472 6f69 645f 785f 6b65 793a 2066  entroid_x_key: f
-00015e40: 6c6f 6174 286d 6173 6b63 656e 7472 6f69  loat(maskcentroi
-00015e50: 645b 325d 2920 0d0a 0d0a 2020 2020 2020  d[2]) ....      
-00015e60: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-00015e70: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
-00015ea0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-00015eb0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-00015ec0: 203d 2073 656c 662e 756e 6971 7565 5f73   = self.unique_s
-00015ed0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00015ee0: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
-00015ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015f00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-00015f10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015f20: 5b63 656c 6c5f 6964 5d2e 7570 6461 7465  [cell_id].update
-00015f30: 287b 7365 6c66 2e74 6f74 616c 5f69 6e74  ({self.total_int
-00015f40: 656e 7369 7479 5f6b 6579 3a20 2d31 7d29  ensity_key: -1})
-00015f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015f60: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-00015f70: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
-00015f80: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00015f90: 645d 2e75 7064 6174 6528 7b73 656c 662e  d].update({self.
-00015fa0: 6d65 616e 5f69 6e74 656e 7369 7479 5f6b  mean_intensity_k
-00015fb0: 6579 3a20 2d31 7d29 0d0a 2020 2020 2020  ey: -1})..      
-00015fc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015fd0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-00015fe0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015ff0: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
-00016000: 6528 7b73 656c 662e 7261 6469 7573 5f6b  e({self.radius_k
-00016010: 6579 3a20 2d31 7d29 0d0a 2020 2020 2020  ey: -1})..      
-00016020: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016030: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
-00016040: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00016050: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
-00016060: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
-00016070: 6b65 793a 202d 317d 290d 0a0d 0a0d 0a0d  key: -1}).......
-00016080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160a0: 2020 0d0a 2020 2020 6465 6620 5f64 6963    ..    def _dic
-000160b0: 745f 7570 6461 7465 2873 656c 662c 2075  t_update(self, u
-000160c0: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-000160d0: 6473 3a20 4c69 7374 2c20 2063 656c 6c5f  ds: List,  cell_
-000160e0: 6964 3a20 696e 742c 2074 7261 636b 5f69  id: int, track_i
-000160f0: 643a 2069 6e74 2c20 736f 7572 6365 5f69  d: int, source_i
-00016100: 643a 2069 6e74 2c20 7461 7267 6574 5f69  d: int, target_i
-00016110: 643a 2069 6e74 293a 0d0a 0d0a 200d 0a20  d: int):.... .. 
-00016120: 2020 2020 2020 2067 656e 6572 6174 696f         generatio
-00016130: 6e5f 6964 203d 2073 656c 662e 6765 6e65  n_id = self.gene
-00016140: 7261 7469 6f6e 5f64 6963 745b 6365 6c6c  ration_dict[cell
-00016150: 5f69 645d 0d0a 2020 2020 2020 2020 7472  _id]..        tr
-00016160: 6163 6b6c 6574 5f69 6420 3d20 7365 6c66  acklet_id = self
-00016170: 2e74 7261 636b 6c65 745f 6469 6374 5b63  .tracklet_dict[c
-00016180: 656c 6c5f 6964 5d0d 0a20 2020 2020 2020  ell_id]..       
-00016190: 0d0a 0d0a 2020 2020 2020 2020 756e 6971  ....        uniq
-000161a0: 7565 5f69 6420 3d20 7374 7228 7472 6163  ue_id = str(trac
-000161b0: 6b5f 6964 2920 2b20 2073 7472 2867 656e  k_id) +  str(gen
-000161c0: 6572 6174 696f 6e5f 6964 2920 2b20 7374  eration_id) + st
-000161d0: 7228 7472 6163 6b6c 6574 5f69 6429 0d0a  r(tracklet_id)..
-000161e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000161f0: 2020 7665 635f 6d61 736b 203d 205b 666c    vec_mask = [fl
-00016200: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00016210: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016220: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
-00016230: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-00016240: 785f 6b65 795d 292c 2066 6c6f 6174 2873  x_key]), float(s
-00016250: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016260: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00016270: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00016280: 736b 6365 6e74 726f 6964 5f79 5f6b 6579  skcentroid_y_key
-00016290: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-000162a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000162b0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000162c0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
-000162d0: 7472 6f69 645f 7a5f 6b65 795d 2920 5d0d  troid_z_key]) ].
-000162e0: 0a0d 0a20 2020 2020 2020 2076 6563 5f63  ...        vec_c
-000162f0: 656c 6c20 3d20 5b66 6c6f 6174 2873 656c  ell = [float(sel
-00016300: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016310: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00016320: 6c5f 6964 295d 5b73 656c 662e 7870 6f73  l_id)][self.xpos
-00016330: 6964 5f6b 6579 5d29 202c 200d 0a20 2020  id_key]) , ..   
-00016340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016350: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00016360: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016370: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00016380: 656c 6c5f 6964 295d 5b73 656c 662e 7970  ell_id)][self.yp
-00016390: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-000163a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163b0: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-000163c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000163d0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000163e0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
-000163f0: 706f 7369 645f 6b65 795d 295d 0d0a 0d0a  posid_key])]....
-00016400: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-00016410: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
-00016420: 6563 5f6d 6173 6b2c 2076 6563 5f63 656c  ec_mask, vec_cel
-00016430: 6c29 0d0a 0d0a 2020 2020 2020 2020 7365  l)....        se
-00016440: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016450: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00016460: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00016470: 7365 6c66 2e72 6164 6961 6c5f 616e 676c  self.radial_angl
-00016480: 655f 6b65 7920 3a20 616e 676c 657d 2920  e_key : angle}) 
-00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164a0: 2020 200d 0a0d 0a20 2020 2020 2020 2075     ....        u
-000164b0: 6e69 7175 655f 7472 6163 6b6c 6574 5f69  nique_tracklet_i
-000164c0: 6473 2e61 7070 656e 6428 7374 7228 756e  ds.append(str(un
-000164d0: 6971 7565 5f69 6429 290d 0a20 2020 2020  ique_id))..     
-000164e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000164f0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016500: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00016510: 6174 6528 7b73 656c 662e 756e 6971 7565  ate({self.unique
-00016520: 6964 5f6b 6579 203a 2073 7472 2875 6e69  id_key : str(uni
-00016530: 7175 655f 6964 297d 290d 0a20 2020 2020  que_id)})..     
-00016540: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00016550: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016560: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00016570: 6174 6528 7b73 656c 662e 7472 6163 6b6c  ate({self.trackl
-00016580: 6574 6964 5f6b 6579 203a 2073 7472 2874  etid_key : str(t
-00016590: 7261 636b 6c65 745f 6964 297d 2920 0d0a  racklet_id)}) ..
-000165a0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000165b0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000165c0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000165d0: 5d2e 7570 6461 7465 287b 7365 6c66 2e67  ].update({self.g
-000165e0: 656e 6572 6174 696f 6e69 645f 6b65 7920  enerationid_key 
-000165f0: 3a20 7374 7228 6765 6e65 7261 7469 6f6e  : str(generation
-00016600: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
-00016610: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00016620: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00016630: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00016640: 6528 7b73 656c 662e 7472 6163 6b69 645f  e({self.trackid_
-00016650: 6b65 7920 3a20 7374 7228 7472 6163 6b5f  key : str(track_
-00016660: 6964 297d 290d 0a20 2020 2020 2020 2073  id)})..        s
-00016670: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016680: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00016690: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-000166a0: 7b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  {self.motion_ang
-000166b0: 6c65 5f6b 6579 203a 2030 2e30 7d29 0d0a  le_key : 0.0})..
-000166c0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-000166d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000166e0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000166f0: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
-00016700: 7065 6564 5f6b 6579 203a 2030 2e30 7d29  peed_key : 0.0})
-00016710: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00016720: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00016730: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00016740: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00016750: 2e61 6363 656c 6572 6174 696f 6e5f 6b65  .acceleration_ke
-00016760: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
-00016770: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00016780: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016790: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-000167a0: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-000167b0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000167c0: 746b 6579 203a 202d 317d 290d 0a20 2020  tkey : -1})..   
-000167d0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-000167e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000167f0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00016800: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-00016810: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00016820: 636f 6e64 6b65 7920 3a20 2d31 7d29 0d0a  condkey : -1})..
-00016830: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00016840: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016850: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00016860: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
-00016870: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
-00016880: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
-00016890: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000168a0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000168b0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000168c0: 287b 7365 6c66 2e63 656c 6c61 7869 735f  ({self.cellaxis_
-000168d0: 6d61 736b 5f6b 6579 203a 202d 317d 290d  mask_key : -1}).
-000168e0: 0a0d 0a20 2020 2020 2020 2069 6620 736f  ...        if so
-000168f0: 7572 6365 5f69 6420 6973 206e 6f74 204e  urce_id is not N
-00016900: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00016910: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016920: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016930: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016940: 7465 287b 7365 6c66 2e62 6566 6f72 6569  te({self.beforei
-00016950: 645f 6b65 7920 3a20 696e 7428 736f 7572  d_key : int(sour
-00016960: 6365 5f69 6429 7d29 0d0a 2020 2020 2020  ce_id)})..      
-00016970: 2020 2020 2020 7665 635f 3120 3d20 5b66        vec_1 = [f
-00016980: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00016990: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000169a0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-000169b0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-000169c0: 202d 2066 6c6f 6174 2873 656c 662e 756e   - float(self.un
-000169d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000169e0: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
-000169f0: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
-00016a00: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
-00016a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a20: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
-00016a30: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00016a40: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00016a50: 5f69 6429 5d5b 7365 6c66 2e79 706f 7369  _id)][self.yposi
-00016a60: 645f 6b65 795d 2920 2d20 666c 6f61 7428  d_key]) - float(
-00016a70: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016a80: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016a90: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00016aa0: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
-00016ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ac0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00016ad0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016ae0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016af0: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00016b00: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
-00016b10: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
-00016b20: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016b30: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00016b40: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00016b50: 6b65 795d 295d 0d0a 2020 2020 2020 2020  key])]..        
-00016b60: 2020 2020 7370 6565 6420 3d20 6e70 2e73      speed = np.s
-00016b70: 7172 7428 6e70 2e64 6f74 2876 6563 5f31  qrt(np.dot(vec_1
-00016b80: 2c20 7665 635f 3129 292f 7365 6c66 2e74  , vec_1))/self.t
-00016b90: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00016ba0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00016bb0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016bc0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00016bd0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00016be0: 7370 6565 645f 6b65 7920 3a20 7370 6565  speed_key : spee
-00016bf0: 647d 290d 0a0d 0a20 2020 2020 2020 2020  d})....         
-00016c00: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
-00016c10: 3d20 616e 6775 6c61 725f 6368 616e 6765  = angular_change
-00016c20: 2876 6563 5f6d 6173 6b2c 2076 6563 5f31  (vec_mask, vec_1
-00016c30: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00016c40: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
-00016c50: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-00016c60: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
-00016c70: 6528 7b73 656c 662e 6d6f 7469 6f6e 5f61  e({self.motion_a
-00016c80: 6e67 6c65 5f6b 6579 203a 206d 6f74 696f  ngle_key : motio
-00016c90: 6e5f 616e 676c 657d 2920 0d0a 0d0a 2020  n_angle}) ....  
-00016ca0: 2020 2020 2020 2020 2020 6966 2073 6f75            if sou
-00016cb0: 7263 655f 6964 2069 6e20 7365 6c66 2e65  rce_id in self.e
-00016cc0: 6467 655f 736f 7572 6365 5f6c 6f6f 6b75  dge_source_looku
-00016cd0: 703a 0d0a 2020 2020 2020 2020 2020 2020  p:..            
-00016ce0: 2020 2020 2020 2020 7072 655f 736f 7572          pre_sour
-00016cf0: 6365 5f69 6420 3d20 7365 6c66 2e65 6467  ce_id = self.edg
-00016d00: 655f 736f 7572 6365 5f6c 6f6f 6b75 705b  e_source_lookup[
-00016d10: 736f 7572 6365 5f69 645d 0d0a 2020 2020  source_id]..    
-00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016d40: 2020 2020 2020 7665 635f 3220 3d20 5b66        vec_2 = [f
-00016d50: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00016d60: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00016d70: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00016d80: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-00016d90: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
-00016da0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016db0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-00016dc0: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
-00016dd0: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
-00016de0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016df0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016e00: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
-00016e10: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-00016e20: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00016e50: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00016e60: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00016e70: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00016e80: 6b65 795d 2920 2d20 3220 2a20 666c 6f61  key]) - 2 * floa
-00016e90: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-00016ea0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016eb0: 7428 736f 7572 6365 5f69 6429 5d5b 7365  t(source_id)][se
-00016ec0: 6c66 2e79 706f 7369 645f 6b65 795d 2920  lf.yposid_key]) 
-00016ed0: 2b20 666c 6f61 7428 7365 6c66 2e75 6e69  + float(self.uni
-00016ee0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016ef0: 6965 735b 696e 7428 7072 655f 736f 7572  ies[int(pre_sour
-00016f00: 6365 5f69 6429 5d5b 7365 6c66 2e79 706f  ce_id)][self.ypo
-00016f10: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
-00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f30: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
-00016f40: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00016f50: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00016f60: 656c 6c5f 6964 295d 5b73 656c 662e 7a70  ell_id)][self.zp
-00016f70: 6f73 6964 5f6b 6579 5d29 202d 2020 3220  osid_key]) -  2 
-00016f80: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
-00016f90: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016fa0: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00016fb0: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00016fc0: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
-00016fd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016fe0: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
-00016ff0: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
-00017000: 6c66 2e7a 706f 7369 645f 6b65 795d 295d  lf.zposid_key])]
-00017010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017020: 2020 2020 2020 6163 6320 3d20 6e70 2e73        acc = np.s
-00017030: 7172 7428 6e70 2e64 6f74 2876 6563 5f32  qrt(np.dot(vec_2
-00017040: 2c20 7665 635f 3229 292f 7365 6c66 2e74  , vec_2))/self.t
-00017050: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00017080: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00017090: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000170a0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000170b0: 2e75 7064 6174 6528 7b73 656c 662e 6163  .update({self.ac
-000170c0: 6365 6c65 7261 7469 6f6e 5f6b 6579 203a  celeration_key :
-000170d0: 2061 6363 7d29 0d0a 2020 2020 2020 2020   acc})..        
-000170e0: 656c 6966 2073 6f75 7263 655f 6964 2069  elif source_id i
-000170f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00017100: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00017110: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00017120: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00017130: 7064 6174 6528 7b73 656c 662e 6265 666f  pdate({self.befo
-00017140: 7265 6964 5f6b 6579 203a 204e 6f6e 657d  reid_key : None}
-00017150: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00017160: 0d0a 0d0a 2020 2020 2020 2020 6966 2074  ....        if t
-00017170: 6172 6765 745f 6964 2069 7320 6e6f 7420  arget_id is not 
-00017180: 4e6f 6e65 3a20 2020 2020 2020 0d0a 2020  None:       ..  
-00017190: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000171a0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000171b0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000171c0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000171d0: 2e61 6674 6572 6964 5f6b 6579 203a 2069  .afterid_key : i
-000171e0: 6e74 2874 6172 6765 745f 6964 297d 2920  nt(target_id)}) 
-000171f0: 0d0a 2020 2020 2020 2020 656c 6966 2074  ..        elif t
-00017200: 6172 6765 745f 6964 2069 7320 4e6f 6e65  arget_id is None
-00017210: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00017220: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00017230: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00017240: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00017250: 7b73 656c 662e 6166 7465 7269 645f 6b65  {self.afterid_ke
-00017260: 7920 3a20 4e6f 6e65 7d29 0d0a 2020 2020  y : None})..    
-00017270: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00017280: 2020 7365 6c66 2e5f 7365 636f 6e64 5f63    self._second_c
-00017290: 6861 6e6e 656c 5f75 7064 6174 6528 6365  hannel_update(ce
-000172a0: 6c6c 5f69 642c 2074 7261 636b 5f69 6429  ll_id, track_id)
-000172b0: 2020 2020 0d0a 0d0a 0d0a 2020 2020 6465      ......    de
-000172c0: 6620 5f74 656d 706f 7261 6c5f 706c 6f74  f _temporal_plot
-000172d0: 735f 7472 6163 6b6d 6174 6528 7365 6c66  s_trackmate(self
-000172e0: 293a 0d0a 2020 2020 0d0a 2020 2020 0d0a  ):..    ..    ..
-000172f0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00017300: 2020 2020 2020 7365 6c66 2e41 7474 7220        self.Attr 
-00017310: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-00017320: 2020 2020 2020 7374 6172 7474 696d 6520        starttime 
-00017330: 3d20 696e 7428 6d69 6e28 7365 6c66 2e41  = int(min(self.A
-00017340: 6c6c 5661 6c75 6573 5b73 656c 662e 6672  llValues[self.fr
-00017350: 616d 6569 645f 6b65 795d 2929 0d0a 2020  ameid_key]))..  
-00017360: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00017370: 6474 696d 6520 3d20 696e 7428 6d61 7828  dtime = int(max(
-00017380: 7365 6c66 2e41 6c6c 5661 6c75 6573 5b73  self.AllValues[s
-00017390: 656c 662e 6672 616d 6569 645f 6b65 795d  elf.frameid_key]
-000173a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000173b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000173c0: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-000173d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000173e0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000173f0: 7469 635f 6d65 616e 5f64 6973 705f 7a20  tic_mean_disp_z 
-00017400: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00017410: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017420: 6963 5f76 6172 5f64 6973 705f 7a20 3d20  ic_var_disp_z = 
-00017430: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-00017440: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00017450: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
-00017460: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017470: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00017480: 635f 7661 725f 6469 7370 5f79 203d 205b  c_var_disp_y = [
-00017490: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000174a0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-000174b0: 635f 6d65 616e 5f64 6973 705f 7820 3d20  c_mean_disp_x = 
-000174c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000174d0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000174e0: 5f76 6172 5f64 6973 705f 7820 3d20 5b5d  _var_disp_x = []
-000174f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00017500: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017510: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
-00017520: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017530: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00017540: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
-00017550: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017560: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00017570: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
-00017580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017590: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-000175a0: 725f 7370 6565 6420 3d20 5b5d 0d0a 0d0a  r_speed = []....
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000175d0: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
-000175e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000175f0: 2e6d 6974 6f74 6963 5f76 6172 5f61 6363  .mitotic_var_acc
-00017600: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017610: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00017620: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
-00017630: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00017640: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017650: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00017660: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
-00017670: 5f63 6861 6e67 6520 3d20 5b5d 0d0a 0d0a  _change = []....
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017690: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000176a0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-000176b0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-000176c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000176d0: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
-000176e0: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-000176f0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00017700: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00017710: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00017720: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00017730: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00017740: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00017750: 6973 705f 7a20 3d20 5b5d 0d0a 0d0a 2020  isp_z = []....  
-00017760: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017770: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00017780: 6561 6e5f 6469 7370 5f79 203d 205b 5d0d  ean_disp_y = [].
-00017790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000177a0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000177b0: 635f 7661 725f 6469 7370 5f79 203d 205b  c_var_disp_y = [
-000177c0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-000177d0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000177e0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-000177f0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00017800: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017810: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00017820: 705f 7820 3d20 5b5d 0d0a 0d0a 2020 2020  p_x = []....    
-00017830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017840: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00017850: 6e5f 7261 6469 7573 203d 205b 5d0d 0a20  n_radius = [].. 
-00017860: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017870: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00017880: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
-00017890: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000178a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-000178b0: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
-000178c0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000178d0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000178e0: 746f 7469 635f 7661 725f 7370 6565 6420  totic_var_speed 
-000178f0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00017900: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017910: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6163  _mitotic_mean_ac
-00017920: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
-00017930: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00017940: 5f6d 6974 6f74 6963 5f76 6172 5f61 6363  _mitotic_var_acc
-00017950: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017960: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00017970: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00017980: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00017990: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-000179a0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000179b0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6972  _mitotic_var_dir
-000179c0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-000179d0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-000179e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000179f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00017a00: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00017a10: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017a20: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00017a30: 6d69 746f 7469 635f 7661 725f 6469 7374  mitotic_var_dist
-00017a40: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00017a50: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00017a60: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00017a70: 6d65 616e 5f64 6973 705f 7a20 3d20 5b5d  mean_disp_z = []
-00017a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017a90: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00017aa0: 6973 705f 7a20 3d20 5b5d 0d0a 0d0a 2020  isp_z = []....  
-00017ab0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017ac0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-00017ad0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00017ae0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017af0: 6c5f 7661 725f 6469 7370 5f79 203d 205b  l_var_disp_y = [
-00017b00: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-00017b10: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-00017b20: 616e 5f64 6973 705f 7820 3d20 5b5d 0d0a  an_disp_x = []..
-00017b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b40: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
-00017b50: 705f 7820 3d20 5b5d 0d0a 0d0a 2020 2020  p_x = []....    
-00017b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00017b70: 2e61 6c6c 5f6d 6561 6e5f 7261 6469 7573  .all_mean_radius
-00017b80: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017b90: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00017ba0: 7661 725f 7261 6469 7573 203d 205b 5d0d  var_radius = [].
-00017bb0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017bc0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00017bd0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
-00017be0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017bf0: 662e 616c 6c5f 7661 725f 7370 6565 6420  f.all_var_speed 
-00017c00: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00017c10: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017c20: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
-00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c40: 7365 6c66 2e61 6c6c 5f76 6172 5f61 6363  self.all_var_acc
-00017c50: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017c60: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017c70: 6c5f 6d65 616e 5f64 6972 6563 7469 6f6e  l_mean_direction
-00017c80: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ca0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
-00017cb0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00017cc0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00017cd0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017ce0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
-00017cf0: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017d10: 656c 662e 616c 6c5f 7661 725f 6469 7374  elf.all_var_dist
-00017d20: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00017d30: 205b 5d0d 0a0d 0a0d 0a20 2020 2020 2020   []......       
-00017d40: 2020 2020 2020 2020 2061 6c6c 5f73 706f           all_spo
-00017d50: 7473 5f74 7261 636b 7320 3d20 7b7d 0d0a  ts_tracks = {}..
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 666f 7220 286b 2c76 2920 696e 2073 656c  for (k,v) in sel
-00017d80: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00017d90: 6f70 6572 7469 6573 2e69 7465 6d73 2829  operties.items()
-00017da0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00017db0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dd0: 2061 6c6c 5f73 706f 7473 203d 2073 656c   all_spots = sel
-00017de0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00017df0: 6f70 6572 7469 6573 5b6b 5d0d 0a20 2020  operties[k]..   
-00017e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e10: 2020 2069 6620 7365 6c66 2e74 7261 636b     if self.track
-00017e20: 6964 5f6b 6579 2069 6e20 616c 6c5f 7370  id_key in all_sp
-00017e30: 6f74 733a 0d0a 2020 2020 2020 2020 2020  ots:..          
-00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e50: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017e60: 5b6b 5d20 3d20 616c 6c5f 7370 6f74 730d  [k] = all_spots.
-00017e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e80: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00017e90: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017ea0: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
-00017eb0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00017ec0: 2020 2020 2077 6974 6820 636f 6e63 7572       with concur
-00017ed0: 7265 6e74 2e66 7574 7572 6573 2e54 6872  rent.futures.Thr
-00017ee0: 6561 6450 6f6f 6c45 7865 6375 746f 7228  eadPoolExecutor(
-00017ef0: 6d61 785f 776f 726b 6572 7320 3d20 6f73  max_workers = os
-00017f00: 2e63 7075 5f63 6f75 6e74 2829 2920 6173  .cpu_count()) as
-00017f10: 2065 7865 6375 746f 723a 0d0a 2020 2020   executor:..    
-00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00017f40: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00017f50: 2074 7164 6d28 7261 6e67 6528 7374 6172   tqdm(range(star
-00017f60: 7474 696d 652c 2065 6e64 7469 6d65 292c  ttime, endtime),
-00017f70: 2074 6f74 616c 3d65 6e64 7469 6d65 202d   total=endtime -
-00017f80: 2073 7461 7274 7469 6d65 293a 0d0a 2020   starttime):..  
-00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fa0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00017fb0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00017fc0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
-00017fd0: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
-00017fe0: 662e 5f63 6f6d 7075 7465 5f74 656d 706f  f._compute_tempo
-00017ff0: 7261 6c2c 2069 2c20 616c 6c5f 7370 6f74  ral, i, all_spot
-00018000: 735f 7472 6163 6b73 2929 0d0a 200d 0a20  s_tracks)).. .. 
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 205b 722e 7265 7375 6c74 2829 2066     [r.result() f
-00018030: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
-00018040: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
-00018050: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
-00018060: 5d0d 0a0d 0a0d 0a20 2020 2064 6566 205f  ]......    def _
-00018070: 636f 6d70 7574 655f 7465 6d70 6f72 616c  compute_temporal
-00018080: 2873 656c 662c 2069 2c20 616c 6c5f 7370  (self, i, all_sp
-00018090: 6f74 735f 7472 6163 6b73 293a 2020 2020  ots_tracks):    
-000180a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 2020 6d69 746f 7469 635f 6469 7370 5f7a    mitotic_disp_z
-000180d0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000180e0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-000180f0: 6963 5f64 6973 705f 7920 3d20 5b5d 0d0a  ic_disp_y = []..
-00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018110: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00018120: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-00018130: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00018140: 6f74 6963 5f72 6164 6975 7320 3d20 5b5d  otic_radius = []
-00018150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018160: 2020 2020 2020 6d69 746f 7469 635f 7370        mitotic_sp
-00018170: 6565 6420 3d20 5b5d 0d0a 2020 2020 2020  eed = []..      
-00018180: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00018190: 746f 7469 635f 6163 6320 3d20 5b5d 0d0a  totic_acc = []..
-000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181b0: 2020 2020 6d69 746f 7469 635f 6469 7265      mitotic_dire
-000181c0: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
-000181d0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000181e0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-000181f0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018200: 6173 6b20 3d20 5b5d 0d0a 0d0a 2020 2020  ask = []....    
-00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018220: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018230: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
-00018240: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00018250: 5f6d 6974 6f74 6963 5f64 6973 705f 7920  _mitotic_disp_y 
-00018260: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00018270: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018280: 746f 7469 635f 6469 7370 5f78 203d 205b  totic_disp_x = [
-00018290: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000182a0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-000182b0: 6963 5f72 6164 6975 7320 3d20 5b5d 0d0a  ic_radius = []..
-000182c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182d0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-000182e0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
-000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018300: 6e6f 6e5f 6d69 746f 7469 635f 6163 6320  non_mitotic_acc 
-00018310: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00018320: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018330: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-00018340: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
-00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018360: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00018370: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00018380: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
-00018390: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183b0: 2020 616c 6c5f 6469 7370 5f7a 203d 205b    all_disp_z = [
-000183c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000183d0: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-000183e0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
-000183f0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00018400: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
-00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018420: 2061 6c6c 5f72 6164 6975 7320 3d20 5b5d   all_radius = []
-00018430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018440: 2020 2020 2020 616c 6c5f 7370 6565 6420        all_speed 
-00018450: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00018460: 2020 2020 2020 2020 2020 616c 6c5f 6163            all_ac
-00018470: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
-00018480: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00018490: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000184a0: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
-000184b0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000184c0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-000184d0: 6173 6b20 3d20 5b5d 0d0a 0d0a 0d0a 0d0a  ask = []........
-000184e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000184f0: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
-00018500: 696e 2061 6c6c 5f73 706f 7473 5f74 7261  in all_spots_tra
-00018510: 636b 732e 6974 656d 7328 293a 0d0a 2020  cks.items():..  
+000132d0: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+000132e0: 656c 662e 726f 6f74 5f73 706f 7473 2e69  elf.root_spots.i
+000132f0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013320: 726f 6f74 5f73 706f 7473 5b6b 5d20 3d20  root_spots[k] = 
+00013330: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00013340: 5f70 726f 7065 7274 6965 735b 6b5d 2020  _properties[k]  
+00013350: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00013360: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00013370: 6566 205f 636f 6d70 7574 655f 7068 656e  ef _compute_phen
+00013380: 6f74 7970 6573 2873 656c 6629 3a0d 0a0d  otypes(self):...
+00013390: 0a20 2020 2020 2020 2020 2066 6f72 2028  .          for (
+000133a0: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
+000133b0: 7175 655f 7472 6163 6b73 2e69 7465 6d73  que_tracks.items
+000133c0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000133d0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000133e0: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
+000133f0: 3d20 6b0d 0a20 2020 2020 2020 2020 2020  = k..           
+00013400: 2020 2020 2074 7261 636b 6c65 745f 7072       tracklet_pr
+00013410: 6f70 6572 7469 6573 203d 2073 656c 662e  operties = self.
+00013420: 756e 6971 7565 5f74 7261 636b 5f70 726f  unique_track_pro
+00013430: 7065 7274 6965 735b 6b5d 0d0a 2020 2020  perties[k]..    
+00013440: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00013450: 6b73 203d 2073 656c 662e 756e 6971 7565  ks = self.unique
+00013460: 5f74 7261 636b 735b 6b5d 0d0a 2020 2020  _tracks[k]..    
+00013470: 2020 2020 2020 2020 2020 2020 5a20 3d20              Z = 
+00013480: 7472 6163 6b73 5b3a 2c32 5d0d 0a20 2020  tracks[:,2]..   
+00013490: 2020 2020 2020 2020 2020 2020 2059 203d               Y =
+000134a0: 2074 7261 636b 735b 3a2c 335d 0d0a 2020   tracks[:,3]..  
+000134b0: 2020 2020 2020 2020 2020 2020 2020 5820                X 
+000134c0: 3d20 7472 6163 6b73 5b3a 2c34 5d0d 0a20  = tracks[:,4].. 
+000134d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000134e0: 696d 6520 3d20 7472 6163 6b6c 6574 5f70  ime = tracklet_p
+000134f0: 726f 7065 7274 6965 735b 3a2c 305d 0d0a  roperties[:,0]..
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 756e 6971 7565 5f69 6473 203d 2074 7261  unique_ids = tra
+00013520: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00013530: 5b3a 2c31 5d0d 0a20 2020 2020 2020 2020  [:,1]..         
+00013540: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
+00013550: 735f 7365 7420 3d20 7365 7428 756e 6971  s_set = set(uniq
+00013560: 7565 5f69 6473 290d 0a20 2020 2020 2020  ue_ids)..       
+00013570: 2020 2020 2020 2020 2067 656e 6572 6174           generat
+00013580: 696f 6e5f 6964 7320 3d20 7472 6163 6b6c  ion_ids = trackl
+00013590: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
+000135a0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
+000135b0: 2020 2020 7261 6469 7573 203d 2074 7261      radius = tra
+000135c0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000135d0: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
+000135e0: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
+000135f0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00013600: 6965 735b 3a2c 345d 0d0a 2020 2020 2020  ies[:,4]..      
+00013610: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
+00013620: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00013630: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
+00013640: 7065 7274 6965 735b 3a2c 355d 0d0a 2020  perties[:,5]..  
+00013650: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+00013660: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
+00013670: 7365 636f 6e64 203d 2074 7261 636b 6c65  second = trackle
+00013680: 745f 7072 6f70 6572 7469 6573 5b3a 2c36  t_properties[:,6
+00013690: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000136a0: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
+000136b0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+000136c0: 7274 6965 735b 3a2c 375d 0d0a 2020 2020  rties[:,7]..    
+000136d0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000136e0: 2020 2020 2020 2020 2020 2020 2069 6e74               int
+000136f0: 656e 7369 7479 203d 2074 7261 636b 6c65  ensity = trackle
+00013700: 745f 7072 6f70 6572 7469 6573 5b3a 2c38  t_properties[:,8
+00013710: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013720: 2020 2073 7065 6564 203d 2074 7261 636b     speed = track
+00013730: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00013740: 2c39 5d0d 0a20 2020 2020 2020 2020 2020  ,9]..           
+00013750: 2020 2020 206d 6f74 696f 6e5f 616e 676c       motion_angl
+00013760: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+00013770: 7065 7274 6965 735b 3a2c 3130 5d0d 0a20  perties[:,10].. 
+00013780: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013790: 6363 656c 6572 6174 696f 6e20 3d20 7472  cceleration = tr
+000137a0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000137b0: 735b 3a2c 3131 5d0d 0a20 2020 2020 2020  s[:,11]..       
+000137c0: 2020 2020 2020 2020 2064 6973 7461 6e63           distanc
+000137d0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 7472  e_cell_mask = tr
+000137e0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000137f0: 735b 3a2c 3132 5d0d 0a20 2020 2020 2020  s[:,12]..       
+00013800: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
+00013810: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
+00013820: 5f70 726f 7065 7274 6965 735b 3a2c 3133  _properties[:,13
+00013830: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013840: 2020 2063 656c 6c5f 6178 6973 5f6d 6173     cell_axis_mas
+00013850: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
+00013860: 7065 7274 6965 735b 3a2c 3134 5d0d 0a20  perties[:,14].. 
+00013870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00013880: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+00013890: 7420 3d20 7472 6163 6b6c 6574 5f70 726f  t = tracklet_pro
+000138a0: 7065 7274 6965 735b 3a2c 3135 5d0d 0a20  perties[:,15].. 
+000138b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000138c0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
+000138d0: 616c 5f74 7261 636b 5f64 6973 7461 6e63  al_track_distanc
+000138e0: 6520 3d20 7472 6163 6b6c 6574 5f70 726f  e = tracklet_pro
+000138f0: 7065 7274 6965 735b 3a2c 3136 5d0d 0a20  perties[:,16].. 
+00013900: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00013910: 2020 2020 2020 2020 2020 2020 206d 6178               max
+00013920: 5f74 7261 636b 5f64 6973 7461 6e63 6520  _track_distance 
+00013930: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00013940: 7274 6965 735b 3a2c 3137 5d0d 0a20 2020  rties[:,17]..   
+00013950: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013960: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+00013970: 6b5f 6475 7261 7469 6f6e 203d 2074 7261  k_duration = tra
+00013980: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+00013990: 5b3a 2c31 385d 0d0a 0d0a 0d0a 2020 2020  [:,18]......    
+000139a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000139b0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000139c0: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
+000139d0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
+000139e0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+000139f0: 2020 2075 6e69 7175 655f 636c 7573 7465     unique_cluste
+00013a00: 725f 7072 6f70 6572 7469 6573 5f74 7261  r_properties_tra
+00013a10: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
+00013a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013a30: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
+00013a40: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
+00013a50: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00013a60: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00013a70: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
+00013a80: 7274 6965 735b 7472 6163 6b5f 6964 5d20  rties[track_id] 
+00013a90: 3d20 7b7d 0d0a 0d0a 2020 2020 2020 2020  = {}....        
+00013aa0: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
+00013ab0: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
+00013ac0: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
+00013ad0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00013ae0: 6e69 7175 655f 6479 6e61 6d69 635f 7072  nique_dynamic_pr
+00013af0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00013b00: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
+00013b10: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00013b20: 7175 655f 7368 6170 655f 7072 6f70 6572  que_shape_proper
+00013b30: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
+00013b40: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+00013b50: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00013b60: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+00013b70: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+00013b80: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
+00013b90: 2020 2020 6578 7061 6e64 6564 5f74 696d      expanded_tim
+00013ba0: 6520 3d20 6e70 2e7a 6572 6f73 2873 656c  e = np.zeros(sel
+00013bb0: 662e 7465 6e64 202d 2073 656c 662e 7473  f.tend - self.ts
+00013bc0: 7461 7274 202b 2031 290d 0a20 2020 2020  tart + 1)..     
+00013bd0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
+00013be0: 5f73 616d 706c 6520 3d20 6578 7061 6e64  _sample = expand
+00013bf0: 6564 5f74 696d 652e 7368 6170 655b 305d  ed_time.shape[0]
+00013c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013c10: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00013c20: 286c 656e 2865 7870 616e 6465 645f 7469  (len(expanded_ti
+00013c30: 6d65 2929 3a0d 0a20 2020 2020 2020 2020  me)):..         
+00013c40: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00013c50: 7061 6e64 6564 5f74 696d 655b 695d 203d  panded_time[i] =
+00013c60: 2069 200d 0a20 2020 2020 2020 2020 2020   i ..           
+00013c70: 2020 2020 2066 6f72 2063 7572 7265 6e74       for current
+00013c80: 5f75 6e69 7175 655f 6964 2069 6e20 756e  _unique_id in un
+00013c90: 6971 7565 5f69 6473 5f73 6574 3a0d 0a20  ique_ids_set:.. 
+00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00013cc0: 2020 2020 2020 2065 7870 616e 6465 645f         expanded_
+00013cd0: 696e 7465 6e73 6974 7920 3d20 6e70 2e7a  intensity = np.z
+00013ce0: 6572 6f73 2873 656c 662e 7465 6e64 202d  eros(self.tend -
+00013cf0: 2073 656c 662e 7473 7461 7274 202b 2031   self.tstart + 1
+00013d00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013d10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00013d20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d40: 6375 7272 656e 745f 7469 6d65 203d 205b  current_time = [
+00013d50: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013d60: 2020 2020 2020 6375 7272 656e 745f 7a20        current_z 
+00013d70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00013d80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013d90: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+00013da0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013db0: 656e 745f 7820 3d20 5b5d 0d0a 2020 2020  ent_x = []..    
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013dd0: 7572 7265 6e74 5f69 6e74 656e 7369 7479  urrent_intensity
+00013de0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00013df0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013e00: 745f 7261 6469 7573 203d 205b 5d0d 0a20  t_radius = [].. 
+00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e20: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
+00013e30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00013e40: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013e50: 745f 7370 6565 6420 3d20 5b5d 0d0a 2020  t_speed = []..  
+00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e70: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
+00013e80: 616e 676c 6520 3d20 5b5d 0d0a 2020 2020  angle = []..    
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013ea0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
+00013eb0: 696f 6e20 3d20 5b5d 0d0a 2020 2020 2020  ion = []..      
+00013ec0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013ed0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+00013ee0: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+00013f10: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+00013f20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00013f30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013f40: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00013f50: 6f6d 705f 7365 636f 6e64 203d 205b 5d0d  omp_second = [].
+00013f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013f70: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
+00013f80: 6163 655f 6172 6561 203d 205b 5d0d 0a0d  ace_area = []...
+00013f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013fa0: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
+00013fb0: 616c 5f61 6e67 6c65 203d 205b 5d0d 0a20  al_angle = [].. 
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
+00013fe0: 7869 735f 6d61 736b 203d 205b 5d20 0d0a  xis_mask = [] ..
+00013ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014000: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+00014010: 5f64 6973 706c 6163 656d 656e 7420 3d20  _displacement = 
+00014020: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00014030: 2020 2020 2020 2063 7572 7265 6e74 5f74         current_t
+00014040: 6f74 616c 5f74 7261 636b 5f64 6973 7461  otal_track_dista
+00014050: 6e63 6520 3d20 5b5d 0d0a 2020 2020 2020  nce = []..      
+00014060: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00014070: 7265 6e74 5f6d 6178 5f74 7261 636b 5f64  rent_max_track_d
+00014080: 6973 7461 6e63 6520 3d20 5b5d 0d0a 2020  istance = []..  
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140a0: 2063 7572 7265 6e74 5f74 7261 636b 5f64   current_track_d
+000140b0: 7572 6174 696f 6e20 3d20 5b5d 0d0a 2020  uration = []..  
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000140e0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+000140f0: 616e 6765 2874 696d 652e 7368 6170 655b  ange(time.shape[
+00014100: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014120: 6966 2063 7572 7265 6e74 5f75 6e69 7175  if current_uniqu
+00014130: 655f 6964 203d 3d20 756e 6971 7565 5f69  e_id == unique_i
+00014140: 6473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ds[j]:..        
+00014150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014160: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014170: 5f74 696d 652e 6170 7065 6e64 2874 696d  _time.append(tim
+00014180: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+00014190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141a0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000141b0: 7a2e 6170 7065 6e64 285a 5b6a 5d29 0d0a  z.append(Z[j])..
+000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141e0: 2063 7572 7265 6e74 5f79 2e61 7070 656e   current_y.appen
+000141f0: 6428 595b 6a5d 290d 0a20 2020 2020 2020  d(Y[j])..       
+00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014210: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00014220: 745f 782e 6170 7065 6e64 2858 5b6a 5d29  t_x.append(X[j])
+00014230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014250: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
+00014260: 6e73 6974 795b 696e 7428 7469 6d65 5b6a  nsity[int(time[j
+00014270: 5d29 5d20 3d20 696e 7465 6e73 6974 795b  ])] = intensity[
+00014280: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
+00014290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142a0: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
+000142b0: 656e 7369 7479 2e61 7070 656e 6428 696e  ensity.append(in
+000142c0: 7465 6e73 6974 795b 6a5d 290d 0a20 2020  tensity[j])..   
+000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000142f0: 7272 656e 745f 7261 6469 7573 2e61 7070  rrent_radius.app
+00014300: 656e 6428 7261 6469 7573 5b6a 5d29 0d0a  end(radius[j])..
+00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014330: 2063 7572 7265 6e74 5f76 6f6c 756d 652e   current_volume.
+00014340: 6170 7065 6e64 2876 6f6c 756d 655b 6a5d  append(volume[j]
+00014350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014370: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
+00014380: 642e 6170 7065 6e64 2873 7065 6564 5b6a  d.append(speed[j
+00014390: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143b0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
+000143c0: 696f 6e5f 616e 676c 652e 6170 7065 6e64  ion_angle.append
+000143d0: 286d 6f74 696f 6e5f 616e 676c 655b 6a5d  (motion_angle[j]
+000143e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014400: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
+00014410: 6c65 7261 7469 6f6e 2e61 7070 656e 6428  leration.append(
+00014420: 6163 6365 6c65 7261 7469 6f6e 5b6a 5d29  acceleration[j])
+00014430: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014450: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
+00014460: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00014470: 7065 6e64 2864 6973 7461 6e63 655f 6365  pend(distance_ce
+00014480: 6c6c 5f6d 6173 6b5b 6a5d 290d 0a20 2020  ll_mask[j])..   
+00014490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144a0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000144b0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+000144c0: 7479 5f63 6f6d 705f 6669 7273 742e 6170  ty_comp_first.ap
+000144d0: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
+000144e0: 795f 636f 6d70 5f66 6972 7374 5b6a 5d29  y_comp_first[j])
+000144f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+00014520: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00014530: 6f6e 642e 6170 7065 6e64 2865 6363 656e  ond.append(eccen
+00014540: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00014550: 6f6e 645b 6a5d 290d 0a20 2020 2020 2020  ond[j])..       
+00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014570: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00014580: 745f 7375 7266 6163 655f 6172 6561 2e61  t_surface_area.a
+00014590: 7070 656e 6428 7375 7266 6163 655f 6172  ppend(surface_ar
+000145a0: 6561 5b6a 5d29 0d0a 2020 2020 2020 2020  ea[j])..        
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145c0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000145d0: 5f72 6164 6961 6c5f 616e 676c 652e 6170  _radial_angle.ap
+000145e0: 7065 6e64 2872 6164 6961 6c5f 616e 676c  pend(radial_angl
+000145f0: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014610: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00014620: 6365 6c6c 5f61 7869 735f 6d61 736b 2e61  cell_axis_mask.a
+00014630: 7070 656e 6428 6365 6c6c 5f61 7869 735f  ppend(cell_axis_
+00014640: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
+00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014660: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014670: 6e74 5f74 7261 636b 5f64 6973 706c 6163  nt_track_displac
+00014680: 656d 656e 742e 6170 7065 6e64 2874 7261  ement.append(tra
+00014690: 636b 5f64 6973 706c 6163 656d 656e 745b  ck_displacement[
+000146a0: 6a5d 290d 0a20 2020 2020 2020 2020 2020  j])..           
+000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146c0: 2020 2020 2020 6375 7272 656e 745f 746f        current_to
+000146d0: 7461 6c5f 7472 6163 6b5f 6469 7374 616e  tal_track_distan
+000146e0: 6365 2e61 7070 656e 6428 746f 7461 6c5f  ce.append(total_
+000146f0: 7472 6163 6b5f 6469 7374 616e 6365 5b6a  track_distance[j
+00014700: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014720: 2020 2020 2063 7572 7265 6e74 5f6d 6178       current_max
+00014730: 5f74 7261 636b 5f64 6973 7461 6e63 652e  _track_distance.
+00014740: 6170 7065 6e64 286d 6178 5f74 7261 636b  append(max_track
+00014750: 5f64 6973 7461 6e63 655b 6a5d 290d 0a20  _distance[j]).. 
+00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014780: 6375 7272 656e 745f 7472 6163 6b5f 6475  current_track_du
+00014790: 7261 7469 6f6e 2e61 7070 656e 6428 7472  ration.append(tr
+000147a0: 6163 6b5f 6475 7261 7469 6f6e 5b6a 5d29  ack_duration[j])
+000147b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000147e0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+000147f0: 6e74 5f74 696d 6520 3d20 6e70 2e61 7361  nt_time = np.asa
+00014800: 7272 6179 2863 7572 7265 6e74 5f74 696d  rray(current_tim
+00014810: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00014820: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00014830: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014840: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
+00014850: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00014860: 696e 7465 6e73 6974 792c 2064 7479 7065  intensity, dtype
+00014870: 3d6e 702e 666c 6f61 7433 3229 0d0a 0d0a  =np.float32)....
+00014880: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00014890: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
+000148a0: 6164 6975 7320 3d20 6e70 2e61 7361 7272  adius = np.asarr
+000148b0: 6179 2863 7572 7265 6e74 5f72 6164 6975  ay(current_radiu
+000148c0: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
+000148d0: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+000148e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000148f0: 5f76 6f6c 756d 6520 3d20 6e70 2e61 7361  _volume = np.asa
+00014900: 7272 6179 2863 7572 7265 6e74 5f76 6f6c  rray(current_vol
+00014910: 756d 652c 2064 7479 7065 3d6e 702e 666c  ume, dtype=np.fl
+00014920: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014930: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014940: 6e74 5f65 6363 656e 7472 6963 6974 795f  nt_eccentricity_
+00014950: 636f 6d70 5f66 6972 7374 203d 206e 702e  comp_first = np.
+00014960: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00014970: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00014980: 705f 6669 7273 742c 2064 7479 7065 3d6e  p_first, dtype=n
+00014990: 702e 666c 6f61 7433 3229 0d0a 2020 2020  p.float32)..    
+000149a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000149b0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+000149c0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
+000149d0: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+000149e0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+000149f0: 795f 636f 6d70 5f73 6563 6f6e 642c 2064  y_comp_second, d
+00014a00: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014a20: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
+00014a30: 6661 6365 5f61 7265 6120 3d20 6e70 2e61  face_area = np.a
+00014a40: 7361 7272 6179 2863 7572 7265 6e74 5f73  sarray(current_s
+00014a50: 7572 6661 6365 5f61 7265 612c 2064 7479  urface_area, dty
+00014a60: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+00014a70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014a80: 2020 2020 2063 7572 7265 6e74 5f73 7065       current_spe
+00014a90: 6564 203d 206e 702e 6173 6172 7261 7928  ed = np.asarray(
+00014aa0: 6375 7272 656e 745f 7370 6565 642c 2064  current_speed, d
+00014ab0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014ac0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014ad0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
+00014ae0: 696f 6e5f 616e 676c 6520 3d20 6e70 2e61  ion_angle = np.a
+00014af0: 7361 7272 6179 2863 7572 7265 6e74 5f6d  sarray(current_m
+00014b00: 6f74 696f 6e5f 616e 676c 652c 2064 7479  otion_angle, dty
+00014b10: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b30: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
+00014b40: 6572 6174 696f 6e20 3d20 6e70 2e61 7361  eration = np.asa
+00014b50: 7272 6179 2863 7572 7265 6e74 5f61 6363  rray(current_acc
+00014b60: 656c 6572 6174 696f 6e2c 2064 7479 7065  eleration, dtype
+00014b70: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+00014b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b90: 2063 7572 7265 6e74 5f64 6973 7461 6e63   current_distanc
+00014ba0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 6e70  e_cell_mask = np
+00014bb0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00014bc0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00014bd0: 6173 6b2c 2064 7479 7065 3d6e 702e 666c  ask, dtype=np.fl
+00014be0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014bf0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014c00: 6e74 5f72 6164 6961 6c5f 616e 676c 6520  nt_radial_angle 
+00014c10: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00014c20: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
+00014c30: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00014c40: 7433 3229 0d0a 2020 2020 2020 2020 2020  t32)..          
+00014c50: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014c60: 5f63 656c 6c5f 6178 6973 5f6d 6173 6b20  _cell_axis_mask 
+00014c70: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
+00014c80: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+00014c90: 6173 6b2c 2064 7479 7065 3d6e 702e 666c  ask, dtype=np.fl
+00014ca0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014cb0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cd0: 6375 7272 656e 745f 7472 6163 6b5f 6469  current_track_di
+00014ce0: 7370 6c61 6365 6d65 6e74 203d 206e 702e  splacement = np.
+00014cf0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
+00014d00: 7472 6163 6b5f 6469 7370 6c61 6365 6d65  track_displaceme
+00014d10: 6e74 2c20 6474 7970 653d 6e70 2e66 6c6f  nt, dtype=np.flo
+00014d20: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
+00014d30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00014d40: 745f 746f 7461 6c5f 7472 6163 6b5f 6469  t_total_track_di
+00014d50: 7374 616e 6365 203d 206e 702e 6173 6172  stance = np.asar
+00014d60: 7261 7928 6375 7272 656e 745f 746f 7461  ray(current_tota
+00014d70: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+00014d80: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00014d90: 3332 290d 0a20 2020 2020 2020 2020 2020  32)..           
+00014da0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00014db0: 6d61 785f 7472 6163 6b5f 6469 7374 616e  max_track_distan
+00014dc0: 6365 203d 206e 702e 6173 6172 7261 7928  ce = np.asarray(
+00014dd0: 6375 7272 656e 745f 6d61 785f 7472 6163  current_max_trac
+00014de0: 6b5f 6469 7374 616e 6365 2c20 6474 7970  k_distance, dtyp
+00014df0: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
+00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e10: 2020 6375 7272 656e 745f 7472 6163 6b5f    current_track_
+00014e20: 6475 7261 7469 6f6e 203d 206e 702e 6173  duration = np.as
+00014e30: 6172 7261 7928 6375 7272 656e 745f 7472  array(current_tr
+00014e40: 6163 6b5f 6475 7261 7469 6f6e 2c20 6474  ack_duration, dt
+00014e50: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
+00014e60: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00014e70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00014e80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 2020 6966 2070 6f69 6e74 5f73 616d 706c    if point_sampl
+00014eb0: 6520 3e20 303a 0d0a 2020 2020 2020 2020  e > 0:..        
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ed0: 2020 2020 2020 2020 7866 5f73 616d 706c          xf_sampl
+00014ee0: 6520 3d20 6666 7466 7265 7128 706f 696e  e = fftfreq(poin
+00014ef0: 745f 7361 6d70 6c65 2c20 7365 6c66 2e74  t_sample, self.t
+00014f00: 6361 6c69 6272 6174 696f 6e29 0d0a 2020  calibration)..  
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2020 2020 2020 2020 2020 2020 6666                ff
+00014f30: 7473 7472 6970 5f73 616d 706c 6520 3d20  tstrip_sample = 
+00014f40: 6666 7428 6578 7061 6e64 6564 5f69 6e74  fft(expanded_int
+00014f50: 656e 7369 7479 290d 0a20 2020 2020 2020  ensity)..       
+00014f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f70: 2020 2020 2020 2020 2066 6674 746f 7461           ffttota
+00014f80: 6c5f 7361 6d70 6c65 203d 206e 702e 6162  l_sample = np.ab
+00014f90: 7328 6666 7473 7472 6970 5f73 616d 706c  s(fftstrip_sampl
+00014fa0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fc0: 2020 2020 7866 5f73 616d 706c 6520 3d20      xf_sample = 
+00014fd0: 7866 5f73 616d 706c 655b 3020 3a20 6c65  xf_sample[0 : le
+00014fe0: 6e28 7866 5f73 616d 706c 6529 202f 2f20  n(xf_sample) // 
+00014ff0: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
+00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015010: 2020 2020 6666 7474 6f74 616c 5f73 616d      ffttotal_sam
+00015020: 706c 6520 3d20 6666 7474 6f74 616c 5f73  ple = ffttotal_s
+00015030: 616d 706c 655b 3020 3a20 6c65 6e28 6666  ample[0 : len(ff
+00015040: 7474 6f74 616c 5f73 616d 706c 6529 202f  ttotal_sample) /
+00015050: 2f20 325d 0d0a 0d0a 2020 2020 2020 2020  / 2]....        
+00015060: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00015070: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
+00015080: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
+00015090: 745f 756e 6971 7565 5f69 645d 203d 2065  t_unique_id] = e
+000150a0: 7870 616e 6465 645f 7469 6d65 2c20 6578  xpanded_time, ex
+000150b0: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
+000150c0: 2c20 7866 5f73 616d 706c 652c 2066 6674  , xf_sample, fft
+000150d0: 746f 7461 6c5f 7361 6d70 6c65 0d0a 2020  total_sample..  
+000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150f0: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
+00015100: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00015110: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+00015120: 7565 5f69 645d 203d 2020 6375 7272 656e  ue_id] =  curren
+00015130: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
+00015140: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
+00015150: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
+00015160: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+00015170: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
+00015180: 2063 7572 7265 6e74 5f74 696d 652c 2063   current_time, c
+00015190: 7572 7265 6e74 5f7a 2c20 6375 7272 656e  urrent_z, curren
+000151a0: 745f 792c 2063 7572 7265 6e74 5f78 2c20  t_y, current_x, 
+000151b0: 6375 7272 656e 745f 7261 6469 7573 2c20  current_radius, 
+000151c0: 6375 7272 656e 745f 766f 6c75 6d65 2c20  current_volume, 
+000151d0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+000151e0: 6369 7479 5f63 6f6d 705f 6669 7273 742c  city_comp_first,
+000151f0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+00015200: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+00015210: 642c 2063 7572 7265 6e74 5f73 7572 6661  d, current_surfa
+00015220: 6365 5f61 7265 610d 0a20 2020 2020 2020  ce_area..       
+00015230: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00015240: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
+00015250: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
+00015260: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00015270: 5d20 3d20 6375 7272 656e 745f 7469 6d65  ] = current_time
+00015280: 2c20 6375 7272 656e 745f 7370 6565 642c  , current_speed,
+00015290: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
+000152a0: 616e 676c 652c 2063 7572 7265 6e74 5f61  angle, current_a
+000152b0: 6363 656c 6572 6174 696f 6e2c 2063 7572  cceleration, cur
+000152c0: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
+000152d0: 6c6c 5f6d 6173 6b2c 2063 7572 7265 6e74  ll_mask, current
+000152e0: 5f72 6164 6961 6c5f 616e 676c 652c 2063  _radial_angle, c
+000152f0: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
+00015300: 5f6d 6173 6b2c 2063 7572 7265 6e74 5f74  _mask, current_t
+00015310: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
+00015320: 742c 2063 7572 7265 6e74 5f74 6f74 616c  t, current_total
+00015330: 5f74 7261 636b 5f64 6973 7461 6e63 652c  _track_distance,
+00015340: 2063 7572 7265 6e74 5f6d 6178 5f74 7261   current_max_tra
+00015350: 636b 5f64 6973 7461 6e63 652c 2063 7572  ck_distance, cur
+00015360: 7265 6e74 5f74 7261 636b 5f64 7572 6174  rent_track_durat
+00015370: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+00015380: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015390: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
+000153a0: 6573 5b74 7261 636b 5f69 645d 2e75 7064  es[track_id].upd
+000153b0: 6174 6528 7b63 7572 7265 6e74 5f75 6e69  ate({current_uni
+000153c0: 7175 655f 6964 3a75 6e69 7175 655f 6666  que_id:unique_ff
+000153d0: 745f 7072 6f70 6572 7469 6573 5f74 7261  t_properties_tra
+000153e0: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
+000153f0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
+00015400: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015410: 656c 662e 756e 6971 7565 5f63 6c75 7374  elf.unique_clust
+00015420: 6572 5f70 726f 7065 7274 6965 735b 7472  er_properties[tr
+00015430: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+00015440: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00015450: 643a 756e 6971 7565 5f63 6c75 7374 6572  d:unique_cluster
+00015460: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00015470: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00015480: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
+00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154a0: 7365 6c66 2e75 6e69 7175 655f 7368 6170  self.unique_shap
+000154b0: 655f 7072 6f70 6572 7469 6573 5b74 7261  e_properties[tra
+000154c0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+000154d0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+000154e0: 3a75 6e69 7175 655f 7368 6170 655f 7072  :unique_shape_pr
+000154f0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
+00015500: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
+00015510: 5f69 645d 7d29 0d0a 2020 2020 2020 2020  _id]})..        
+00015520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015530: 756e 6971 7565 5f64 796e 616d 6963 5f70  unique_dynamic_p
+00015540: 726f 7065 7274 6965 735b 7472 6163 6b5f  roperties[track_
+00015550: 6964 5d2e 7570 6461 7465 287b 6375 7272  id].update({curr
+00015560: 656e 745f 756e 6971 7565 5f69 643a 756e  ent_unique_id:un
+00015570: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
+00015580: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00015590: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+000155a0: 6964 5d7d 290d 0a0d 0a20 2020 2064 6566  id]})....    def
+000155b0: 205f 7365 636f 6e64 5f63 6861 6e6e 656c   _second_channel
+000155c0: 5f73 706f 7473 2873 656c 662c 2066 7261  _spots(self, fra
+000155d0: 6d65 2c20 7a2c 2079 2c20 782c 2063 656c  me, z, y, x, cel
+000155e0: 6c5f 6964 2c20 7472 6163 6b5f 6964 293a  l_id, track_id):
+000155f0: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
+00015600: 2020 2020 2020 2020 2020 2074 7265 652c             tree,
+00015610: 2063 656e 7472 6f69 6473 2c20 6c61 6265   centroids, labe
+00015620: 6c73 2c20 766f 6c75 6d65 2c20 696e 7465  ls, volume, inte
+00015630: 6e73 6974 795f 6d65 616e 2c20 696e 7465  nsity_mean, inte
+00015640: 6e73 6974 795f 746f 7461 6c2c 2062 6f75  nsity_total, bou
+00015650: 6e64 696e 675f 626f 7865 7320 3d20 7365  nding_boxes = se
+00015660: 6c66 2e5f 7469 6d65 645f 6368 616e 6e65  lf._timed_channe
+00015670: 6c5f 7365 675f 696d 6167 655b 7374 7228  l_seg_image[str(
+00015680: 696e 7428 666c 6f61 7428 6672 616d 6529  int(float(frame)
+00015690: 2929 5d0d 0a20 2020 2020 2020 2020 2020  ))]..           
+000156a0: 2070 6978 656c 7465 7374 6c6f 6361 7469   pixeltestlocati
+000156b0: 6f6e 203d 2028 7a2c 792c 7829 0d0a 2020  on = (z,y,x)..  
+000156c0: 2020 2020 2020 2020 2020 6469 7374 2c20            dist, 
+000156d0: 696e 6465 7820 3d20 7472 6565 2e71 7565  index = tree.que
+000156e0: 7279 2870 6978 656c 7465 7374 6c6f 6361  ry(pixeltestloca
+000156f0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
+00015700: 2020 2020 2020 2062 626f 7820 3d20 626f         bbox = bo
+00015710: 756e 6469 6e67 5f62 6f78 6573 5b69 6e64  unding_boxes[ind
+00015720: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+00015730: 2073 697a 657a 203d 2061 6273 2862 626f   sizez = abs(bbo
+00015740: 785b 305d 202d 2062 626f 785b 335d 290d  x[0] - bbox[3]).
+00015750: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
+00015760: 6579 203d 2061 6273 2862 626f 785b 315d  ey = abs(bbox[1]
+00015770: 202d 2062 626f 785b 345d 290d 0a20 2020   - bbox[4])..   
+00015780: 2020 2020 2020 2020 2073 697a 6578 203d           sizex =
+00015790: 2061 6273 2862 626f 785b 325d 202d 2062   abs(bbox[2] - b
+000157a0: 626f 785b 355d 2920 0d0a 2020 2020 2020  box[5]) ..      
+000157b0: 2020 2020 2020 7665 746f 5f76 6f6c 756d        veto_volum
+000157c0: 6520 3d20 7369 7a65 7820 2a20 7369 7a65  e = sizex * size
+000157d0: 7920 2a20 7369 7a65 7a0d 0a20 2020 2020  y * sizez..     
+000157e0: 2020 2020 2020 2076 6574 6f5f 7261 6469         veto_radi
+000157f0: 7573 203d 206d 6174 682e 706f 7728 3320  us = math.pow(3 
+00015800: 2a20 7665 746f 5f76 6f6c 756d 6520 2f20  * veto_volume / 
+00015810: 2834 202a 206d 6174 682e 7069 292c 2031  (4 * math.pi), 1
+00015820: 2e30 202f 2033 2e30 290d 0a0d 0a20 2020  .0 / 3.0)....   
+00015830: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+00015840: 6e20 3d20 2863 656e 7472 6f69 6473 5b69  n = (centroids[i
+00015850: 6e64 6578 5d5b 305d 202a 2073 656c 662e  ndex][0] * self.
+00015860: 7a63 616c 6962 7261 7469 6f6e 2c20 6365  zcalibration, ce
+00015870: 6e74 726f 6964 735b 696e 6465 785d 5b31  ntroids[index][1
+00015880: 5d2a 7365 6c66 2e79 6361 6c69 6272 6174  ]*self.ycalibrat
+00015890: 696f 6e2c 2063 656e 7472 6f69 6473 5b69  ion, centroids[i
+000158a0: 6e64 6578 5d5b 325d 2a73 656c 662e 7863  ndex][2]*self.xc
+000158b0: 616c 6962 7261 7469 6f6e 290d 0a20 2020  alibration)..   
+000158c0: 2020 2020 2020 2020 2051 5541 4c49 5459           QUALITY
+000158d0: 203d 206d 6174 682e 706f 7728 766f 6c75   = math.pow(volu
+000158e0: 6d65 5b69 6e64 6578 5d2c 2031 2e30 2f33  me[index], 1.0/3
+000158f0: 2e30 290d 0a20 2020 2020 2020 2020 2020  .0)..           
+00015900: 2052 4144 4955 5320 3d20 6d61 7468 2e70   RADIUS = math.p
+00015910: 6f77 2876 6f6c 756d 655b 696e 6465 785d  ow(volume[index]
+00015920: 202a 2073 656c 662e 7863 616c 6962 7261   * self.xcalibra
+00015930: 7469 6f6e 202a 2073 656c 662e 7963 616c  tion * self.ycal
+00015940: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+00015950: 7a63 616c 6962 7261 7469 6f6e 2c20 312e  zcalibration, 1.
+00015960: 302f 332e 3029 200d 0a0d 0a20 2020 2020  0/3.0) ....     
+00015970: 2020 2020 2020 2064 6973 7461 6e63 655f         distance_
+00015980: 6365 6c6c 5f6d 6173 6b2c 206d 6173 6b63  cell_mask, maskc
+00015990: 656e 7472 6f69 6420 3d20 7365 6c66 2e5f  entroid = self._
+000159a0: 6765 745f 626f 756e 6461 7279 5f64 6973  get_boundary_dis
+000159b0: 7428 6672 616d 652c 206c 6f63 6174 696f  t(frame, locatio
+000159c0: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+000159d0: 6966 2064 6973 7420 3c3d 2032 202a 2076  if dist <= 2 * v
+000159e0: 6574 6f5f 7261 6469 7573 3a0d 0a20 2020  eto_radius:..   
+000159f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015a00: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
+00015a10: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015a20: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a40: 2020 2020 2020 2073 656c 662e 6365 6c6c         self.cell
+00015a50: 6964 5f6b 6579 3a20 696e 7428 6365 6c6c  id_key: int(cell
+00015a60: 5f69 6429 2c20 0d0a 2020 2020 2020 2020  _id), ..        
+00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a80: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00015a90: 203a 2069 6e74 2866 7261 6d65 292c 0d0a   : int(frame),..
+00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ab0: 2020 2020 2020 2020 7365 6c66 2e7a 706f          self.zpo
+00015ac0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
+00015ad0: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00015ae0: 5b30 5d2a 2073 656c 662e 7a63 616c 6962  [0]* self.zcalib
+00015af0: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
+00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b10: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+00015b20: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
+00015b30: 6964 735b 696e 6465 785d 5b31 5d2a 2073  ids[index][1]* s
+00015b40: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
+00015b50: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00015b60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015b70: 2e78 706f 7369 645f 6b65 7920 3a20 666c  .xposid_key : fl
+00015b80: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
+00015b90: 6465 785d 5b32 5d2a 2073 656c 662e 7863  dex][2]* self.xc
+00015ba0: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
+00015bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bc0: 2020 2020 2020 7365 6c66 2e74 7261 636b        self.track
+00015bd0: 6964 5f6b 6579 3a20 696e 7428 7472 6163  id_key: int(trac
+00015be0: 6b5f 6964 292c 0d0a 2020 2020 2020 2020  k_id),..        
+00015bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c00: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+00015c10: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
+00015c20: 7428 696e 7465 6e73 6974 795f 746f 7461  t(intensity_tota
+00015c30: 6c5b 696e 6465 785d 2929 2c0d 0a20 2020  l[index])),..   
+00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c50: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+00015c60: 6e74 656e 7369 7479 5f6b 6579 203a 2028  ntensity_key : (
+00015c70: 666c 6f61 7428 696e 7465 6e73 6974 795f  float(intensity_
+00015c80: 6d65 616e 5b69 6e64 6578 5d29 292c 0d0a  mean[index])),..
+00015c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ca0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+00015cb0: 6975 735f 6b65 7920 3a20 2866 6c6f 6174  ius_key : (float
+00015cc0: 2852 4144 4955 5329 292c 0d0a 2020 2020  (RADIUS)),..    
+00015cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ce0: 2020 2020 7365 6c66 2e71 7561 6c69 7479      self.quality
+00015cf0: 5f6b 6579 203a 2028 666c 6f61 7428 5155  _key : (float(QU
+00015d00: 414c 4954 5929 292c 0d0a 2020 2020 2020  ALITY)),..      
+00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d20: 2020 7365 6c66 2e64 6973 7461 6e63 655f    self.distance_
+00015d30: 6365 6c6c 5f6d 6173 6b5f 6b65 793a 2066  cell_mask_key: f
+00015d40: 6c6f 6174 2864 6973 7461 6e63 655f 6365  loat(distance_ce
+00015d50: 6c6c 5f6d 6173 6b29 2c0d 0a20 2020 2020  ll_mask),..     
+00015d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d70: 2020 2073 656c 662e 6d61 736b 6365 6e74     self.maskcent
+00015d80: 726f 6964 5f7a 5f6b 6579 3a20 666c 6f61  roid_z_key: floa
+00015d90: 7428 6d61 736b 6365 6e74 726f 6964 5b30  t(maskcentroid[0
+00015da0: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
+00015db0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015dc0: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
+00015dd0: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+00015de0: 6365 6e74 726f 6964 5b31 5d29 2c0d 0a20  centroid[1]),.. 
+00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e00: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
+00015e10: 6365 6e74 726f 6964 5f78 5f6b 6579 3a20  centroid_x_key: 
+00015e20: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
+00015e30: 6964 5b32 5d29 200d 0a0d 0a20 2020 2020  id[2]) ....     
+00015e40: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00015e50: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00015e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e70: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
+00015e80: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+00015e90: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+00015ea0: 5d20 3d20 7365 6c66 2e75 6e69 7175 655f  ] = self.unique_
+00015eb0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015ec0: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
+00015ed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015ee0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+00015ef0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015f00: 735b 6365 6c6c 5f69 645d 2e75 7064 6174  s[cell_id].updat
+00015f10: 6528 7b73 656c 662e 746f 7461 6c5f 696e  e({self.total_in
+00015f20: 7465 6e73 6974 795f 6b65 793a 202d 317d  tensity_key: -1}
+00015f30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00015f40: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+00015f50: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
+00015f60: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+00015f70: 6964 5d2e 7570 6461 7465 287b 7365 6c66  id].update({self
+00015f80: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
+00015f90: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
+00015fa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015fb0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+00015fc0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00015fd0: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
+00015fe0: 7465 287b 7365 6c66 2e72 6164 6975 735f  te({self.radius_
+00015ff0: 6b65 793a 202d 317d 290d 0a20 2020 2020  key: -1})..     
+00016000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016010: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+00016020: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00016030: 6573 5b63 656c 6c5f 6964 5d2e 7570 6461  es[cell_id].upda
+00016040: 7465 287b 7365 6c66 2e71 7561 6c69 7479  te({self.quality
+00016050: 5f6b 6579 3a20 2d31 7d29 0d0a 0d0a 0d0a  _key: -1})......
+00016060: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016080: 2020 200d 0a20 2020 2064 6566 205f 6469     ..    def _di
+00016090: 6374 5f75 7064 6174 6528 7365 6c66 2c20  ct_update(self, 
+000160a0: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+000160b0: 6964 733a 204c 6973 742c 2020 6365 6c6c  ids: List,  cell
+000160c0: 5f69 643a 2069 6e74 2c20 7472 6163 6b5f  _id: int, track_
+000160d0: 6964 3a20 696e 742c 2073 6f75 7263 655f  id: int, source_
+000160e0: 6964 3a20 696e 742c 2074 6172 6765 745f  id: int, target_
+000160f0: 6964 3a20 696e 7429 3a0d 0a0d 0a20 0d0a  id: int):.... ..
+00016100: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+00016110: 6f6e 5f69 6420 3d20 7365 6c66 2e67 656e  on_id = self.gen
+00016120: 6572 6174 696f 6e5f 6469 6374 5b63 656c  eration_dict[cel
+00016130: 6c5f 6964 5d0d 0a20 2020 2020 2020 2074  l_id]..        t
+00016140: 7261 636b 6c65 745f 6964 203d 2073 656c  racklet_id = sel
+00016150: 662e 7472 6163 6b6c 6574 5f64 6963 745b  f.tracklet_dict[
+00016160: 6365 6c6c 5f69 645d 0d0a 2020 2020 2020  cell_id]..      
+00016170: 200d 0a0d 0a20 2020 2020 2020 2075 6e69   ....        uni
+00016180: 7175 655f 6964 203d 2073 7472 2874 7261  que_id = str(tra
+00016190: 636b 5f69 6429 202b 2020 7374 7228 6765  ck_id) +  str(ge
+000161a0: 6e65 7261 7469 6f6e 5f69 6429 202b 2073  neration_id) + s
+000161b0: 7472 2874 7261 636b 6c65 745f 6964 290d  tr(tracklet_id).
+000161c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+000161d0: 2020 2076 6563 5f6d 6173 6b20 3d20 5b66     vec_mask = [f
+000161e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000161f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00016200: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
+00016210: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+00016220: 5f78 5f6b 6579 5d29 2c20 666c 6f61 7428  _x_key]), float(
+00016230: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00016240: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00016250: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00016260: 6173 6b63 656e 7472 6f69 645f 795f 6b65  askcentroid_y_ke
+00016270: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00016280: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016290: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000162a0: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+000162b0: 6e74 726f 6964 5f7a 5f6b 6579 5d29 205d  ntroid_z_key]) ]
+000162c0: 0d0a 0d0a 2020 2020 2020 2020 7665 635f  ....        vec_
+000162d0: 6365 6c6c 203d 205b 666c 6f61 7428 7365  cell = [float(se
+000162e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000162f0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00016300: 6c6c 5f69 6429 5d5b 7365 6c66 2e78 706f  ll_id)][self.xpo
+00016310: 7369 645f 6b65 795d 2920 2c20 0d0a 2020  sid_key]) , ..  
+00016320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016330: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00016340: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00016350: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00016360: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
+00016370: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
+00016380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016390: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+000163a0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+000163b0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+000163c0: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+000163d0: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a0d  zposid_key])]...
+000163e0: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+000163f0: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
+00016400: 7665 635f 6d61 736b 2c20 7665 635f 6365  vec_mask, vec_ce
+00016410: 6c6c 290d 0a0d 0a20 2020 2020 2020 2073  ll)....        s
+00016420: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016430: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00016440: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00016450: 7b73 656c 662e 7261 6469 616c 5f61 6e67  {self.radial_ang
+00016460: 6c65 5f6b 6579 203a 2061 6e67 6c65 7d29  le_key : angle})
+00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016480: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+00016490: 756e 6971 7565 5f74 7261 636b 6c65 745f  unique_tracklet_
+000164a0: 6964 732e 6170 7065 6e64 2873 7472 2875  ids.append(str(u
+000164b0: 6e69 7175 655f 6964 2929 0d0a 2020 2020  nique_id))..    
+000164c0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+000164d0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000164e0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+000164f0: 6461 7465 287b 7365 6c66 2e75 6e69 7175  date({self.uniqu
+00016500: 6569 645f 6b65 7920 3a20 7374 7228 756e  eid_key : str(un
+00016510: 6971 7565 5f69 6429 7d29 0d0a 2020 2020  ique_id)})..    
+00016520: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00016530: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016540: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00016550: 6461 7465 287b 7365 6c66 2e74 7261 636b  date({self.track
+00016560: 6c65 7469 645f 6b65 7920 3a20 7374 7228  letid_key : str(
+00016570: 7472 6163 6b6c 6574 5f69 6429 7d29 200d  tracklet_id)}) .
+00016580: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00016590: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000165a0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000165b0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000165c0: 6765 6e65 7261 7469 6f6e 6964 5f6b 6579  generationid_key
+000165d0: 203a 2073 7472 2867 656e 6572 6174 696f   : str(generatio
+000165e0: 6e5f 6964 297d 2920 0d0a 2020 2020 2020  n_id)}) ..      
+000165f0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00016600: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00016610: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00016620: 7465 287b 7365 6c66 2e74 7261 636b 6964  te({self.trackid
+00016630: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
+00016640: 5f69 6429 7d29 0d0a 2020 2020 2020 2020  _id)})..        
+00016650: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00016660: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00016670: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00016680: 287b 7365 6c66 2e6d 6f74 696f 6e5f 616e  ({self.motion_an
+00016690: 676c 655f 6b65 7920 3a20 302e 307d 290d  gle_key : 0.0}).
+000166a0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+000166b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000166c0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+000166d0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+000166e0: 7370 6565 645f 6b65 7920 3a20 302e 307d  speed_key : 0.0}
+000166f0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00016700: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016710: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016720: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00016730: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00016740: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
+00016750: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00016760: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016770: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00016780: 6461 7465 287b 7365 6c66 2e65 6363 656e  date({self.eccen
+00016790: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+000167a0: 7374 6b65 7920 3a20 2d31 7d29 0d0a 2020  stkey : -1})..  
+000167b0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000167c0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000167d0: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000167e0: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+000167f0: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00016800: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
+00016810: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00016820: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016830: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00016840: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00016850: 7375 7266 6163 655f 6172 6561 5f6b 6579  surface_area_key
+00016860: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
+00016870: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00016880: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00016890: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+000168a0: 6528 7b73 656c 662e 6365 6c6c 6178 6973  e({self.cellaxis
+000168b0: 5f6d 6173 6b5f 6b65 7920 3a20 2d31 7d29  _mask_key : -1})
+000168c0: 0d0a 0d0a 2020 2020 2020 2020 6966 2073  ....        if s
+000168d0: 6f75 7263 655f 6964 2069 7320 6e6f 7420  ource_id is not 
+000168e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000168f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00016900: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00016910: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00016920: 6174 6528 7b73 656c 662e 6265 666f 7265  ate({self.before
+00016930: 6964 5f6b 6579 203a 2069 6e74 2873 6f75  id_key : int(sou
+00016940: 7263 655f 6964 297d 290d 0a20 2020 2020  rce_id)})..     
+00016950: 2020 2020 2020 2076 6563 5f31 203d 205b         vec_1 = [
+00016960: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00016970: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016980: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00016990: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+000169a0: 2920 2d20 666c 6f61 7428 7365 6c66 2e75  ) - float(self.u
+000169b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000169c0: 7274 6965 735b 696e 7428 736f 7572 6365  rties[int(source
+000169d0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
+000169e0: 645f 6b65 795d 292c 200d 0a20 2020 2020  d_key]), ..     
+000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a00: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00016a10: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00016a20: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00016a30: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
+00016a40: 6964 5f6b 6579 5d29 202d 2066 6c6f 6174  id_key]) - float
+00016a50: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00016a60: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00016a70: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
+00016a80: 662e 7970 6f73 6964 5f6b 6579 5d29 2c20  f.yposid_key]), 
+00016a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+00016ab0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00016ac0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016ad0: 696e 7428 6365 6c6c 5f69 6429 5d5b 7365  int(cell_id)][se
+00016ae0: 6c66 2e7a 706f 7369 645f 6b65 795d 2920  lf.zposid_key]) 
+00016af0: 2d20 2066 6c6f 6174 2873 656c 662e 756e  -  float(self.un
+00016b00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016b10: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+00016b20: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+00016b30: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
+00016b40: 2020 2020 2073 7065 6564 203d 206e 702e       speed = np.
+00016b50: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
+00016b60: 312c 2076 6563 5f31 2929 2f73 656c 662e  1, vec_1))/self.
+00016b70: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
+00016b80: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00016b90: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00016ba0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00016bb0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00016bc0: 2e73 7065 6564 5f6b 6579 203a 2073 7065  .speed_key : spe
+00016bd0: 6564 7d29 0d0a 0d0a 2020 2020 2020 2020  ed})....        
+00016be0: 2020 2020 6d6f 7469 6f6e 5f61 6e67 6c65      motion_angle
+00016bf0: 203d 2061 6e67 756c 6172 5f63 6861 6e67   = angular_chang
+00016c00: 6528 7665 635f 6d61 736b 2c20 7665 635f  e(vec_mask, vec_
+00016c10: 3129 0d0a 0d0a 2020 2020 2020 2020 2020  1)....          
+00016c20: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00016c30: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00016c40: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00016c50: 7465 287b 7365 6c66 2e6d 6f74 696f 6e5f  te({self.motion_
+00016c60: 616e 676c 655f 6b65 7920 3a20 6d6f 7469  angle_key : moti
+00016c70: 6f6e 5f61 6e67 6c65 7d29 200d 0a0d 0a20  on_angle}) .... 
+00016c80: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+00016c90: 7572 6365 5f69 6420 696e 2073 656c 662e  urce_id in self.
+00016ca0: 6564 6765 5f73 6f75 7263 655f 6c6f 6f6b  edge_source_look
+00016cb0: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00016cc0: 2020 2020 2020 2020 2070 7265 5f73 6f75           pre_sou
+00016cd0: 7263 655f 6964 203d 2073 656c 662e 6564  rce_id = self.ed
+00016ce0: 6765 5f73 6f75 7263 655f 6c6f 6f6b 7570  ge_source_lookup
+00016cf0: 5b73 6f75 7263 655f 6964 5d0d 0a20 2020  [source_id]..   
+00016d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d10: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016d20: 2020 2020 2020 2076 6563 5f32 203d 205b         vec_2 = [
+00016d30: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00016d40: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016d50: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00016d60: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00016d70: 2920 2d20 3220 2a20 666c 6f61 7428 7365  ) - 2 * float(se
+00016d80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016d90: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00016da0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
+00016db0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
+00016dc0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00016dd0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016de0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
+00016df0: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
+00016e00: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e20: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00016e30: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016e40: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016e50: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+00016e60: 5f6b 6579 5d29 202d 2032 202a 2066 6c6f  _key]) - 2 * flo
+00016e70: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00016e80: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00016e90: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
+00016ea0: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00016eb0: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
+00016ec0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016ed0: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
+00016ee0: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
+00016ef0: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
+00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f10: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
+00016f20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00016f30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00016f40: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e7a  cell_id)][self.z
+00016f50: 706f 7369 645f 6b65 795d 2920 2d20 2032  posid_key]) -  2
+00016f60: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
+00016f70: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016f80: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+00016f90: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+00016fa0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
+00016fb0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00016fc0: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
+00016fd0: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
+00016fe0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00016ff0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017000: 2020 2020 2020 2061 6363 203d 206e 702e         acc = np.
+00017010: 7371 7274 286e 702e 646f 7428 7665 635f  sqrt(np.dot(vec_
+00017020: 322c 2076 6563 5f32 2929 2f73 656c 662e  2, vec_2))/self.
+00017030: 7463 616c 6962 7261 7469 6f6e 0d0a 2020  tcalibration..  
+00017040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017050: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00017060: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00017070: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00017080: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00017090: 5d2e 7570 6461 7465 287b 7365 6c66 2e61  ].update({self.a
+000170a0: 6363 656c 6572 6174 696f 6e5f 6b65 7920  cceleration_key 
+000170b0: 3a20 6163 637d 290d 0a20 2020 2020 2020  : acc})..       
+000170c0: 2065 6c69 6620 736f 7572 6365 5f69 6420   elif source_id 
+000170d0: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+000170e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000170f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00017100: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00017110: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
+00017120: 6f72 6569 645f 6b65 7920 3a20 4e6f 6e65  oreid_key : None
+00017130: 7d29 200d 0a20 2020 2020 2020 2020 2020  }) ..           
+00017140: 200d 0a0d 0a20 2020 2020 2020 2069 6620   ....        if 
+00017150: 7461 7267 6574 5f69 6420 6973 206e 6f74  target_id is not
+00017160: 204e 6f6e 653a 2020 2020 2020 200d 0a20   None:       .. 
+00017170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017180: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00017190: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+000171a0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+000171b0: 662e 6166 7465 7269 645f 6b65 7920 3a20  f.afterid_key : 
+000171c0: 696e 7428 7461 7267 6574 5f69 6429 7d29  int(target_id)})
+000171d0: 200d 0a20 2020 2020 2020 2065 6c69 6620   ..        elif 
+000171e0: 7461 7267 6574 5f69 6420 6973 204e 6f6e  target_id is Non
+000171f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00017200: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00017210: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00017220: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00017230: 287b 7365 6c66 2e61 6674 6572 6964 5f6b  ({self.afterid_k
+00017240: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
+00017250: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00017260: 2020 2073 656c 662e 5f73 6563 6f6e 645f     self._second_
+00017270: 6368 616e 6e65 6c5f 7570 6461 7465 2863  channel_update(c
+00017280: 656c 6c5f 6964 2c20 7472 6163 6b5f 6964  ell_id, track_id
+00017290: 2920 2020 200d 0a0d 0a0d 0a20 2020 2064  )    ......    d
+000172a0: 6566 205f 7465 6d70 6f72 616c 5f70 6c6f  ef _temporal_plo
+000172b0: 7473 5f74 7261 636b 6d61 7465 2873 656c  ts_trackmate(sel
+000172c0: 6629 3a0d 0a20 2020 200d 0a20 2020 200d  f):..    ..    .
+000172d0: 0a20 2020 200d 0a20 2020 2020 2020 2020  .    ..         
+000172e0: 2020 2020 2020 2073 656c 662e 4174 7472         self.Attr
+000172f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00017300: 2020 2020 2020 2073 7461 7274 7469 6d65         starttime
+00017310: 203d 2069 6e74 286d 696e 2873 656c 662e   = int(min(self.
+00017320: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
+00017330: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
+00017340: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017350: 6e64 7469 6d65 203d 2069 6e74 286d 6178  ndtime = int(max
+00017360: 2873 656c 662e 416c 6c56 616c 7565 735b  (self.AllValues[
+00017370: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00017380: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00017390: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000173a0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000173b0: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
+000173c0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+000173d0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
+000173e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000173f0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017400: 7469 635f 7661 725f 6469 7370 5f7a 203d  tic_var_disp_z =
+00017410: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00017420: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00017430: 7469 635f 6d65 616e 5f64 6973 705f 7920  tic_mean_disp_y 
+00017440: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017450: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017460: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
+00017470: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00017480: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00017490: 6963 5f6d 6561 6e5f 6469 7370 5f78 203d  ic_mean_disp_x =
+000174a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000174b0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000174c0: 635f 7661 725f 6469 7370 5f78 203d 205b  c_var_disp_x = [
+000174d0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000174e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000174f0: 635f 6d65 616e 5f72 6164 6975 7320 3d20  c_mean_radius = 
+00017500: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017510: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017520: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00017530: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017540: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00017550: 5f6d 6561 6e5f 7370 6565 6420 3d20 5b5d  _mean_speed = []
+00017560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017570: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00017580: 6172 5f73 7065 6564 203d 205b 5d0d 0a0d  ar_speed = []...
+00017590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175a0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+000175b0: 616e 5f61 6363 203d 205b 5d0d 0a20 2020  an_acc = []..   
+000175c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000175d0: 662e 6d69 746f 7469 635f 7661 725f 6163  f.mitotic_var_ac
+000175e0: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+000175f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00017600: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+00017610: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00017620: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017630: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00017640: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00017650: 6c5f 6368 616e 6765 203d 205b 5d0d 0a0d  l_change = []...
+00017660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017670: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00017680: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
+00017690: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+000176a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000176b0: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+000176c0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+000176d0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000176e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000176f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00017700: 7370 5f7a 203d 205b 5d0d 0a20 2020 2020  sp_z = []..     
+00017710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017720: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00017730: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
+00017740: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017750: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00017760: 6d65 616e 5f64 6973 705f 7920 3d20 5b5d  mean_disp_y = []
+00017770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017780: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00017790: 6963 5f76 6172 5f64 6973 705f 7920 3d20  ic_var_disp_y = 
+000177a0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+000177b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000177c0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+000177d0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+000177e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000177f0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00017800: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
+00017810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017820: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00017830: 616e 5f72 6164 6975 7320 3d20 5b5d 0d0a  an_radius = []..
+00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017850: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00017860: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00017870: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017880: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00017890: 6f74 6963 5f6d 6561 6e5f 7370 6565 6420  otic_mean_speed 
+000178a0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000178b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000178c0: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
+000178d0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000178e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000178f0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f61  n_mitotic_mean_a
+00017900: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+00017910: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00017920: 6e5f 6d69 746f 7469 635f 7661 725f 6163  n_mitotic_var_ac
+00017930: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+00017940: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00017950: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00017960: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00017970: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00017980: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00017990: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+000179a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000179b0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+000179c0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+000179d0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
+000179e0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+000179f0: 6b20 3d20 5b5d 0d0a 2020 2020 2020 2020  k = []..        
+00017a00: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00017a10: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00017a20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00017a30: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00017a40: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00017a50: 5f6d 6561 6e5f 6469 7370 5f7a 203d 205b  _mean_disp_z = [
+00017a60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017a70: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00017a80: 6469 7370 5f7a 203d 205b 5d0d 0a0d 0a20  disp_z = [].... 
+00017a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00017aa0: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00017ab0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00017ac0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017ad0: 6c6c 5f76 6172 5f64 6973 705f 7920 3d20  ll_var_disp_y = 
+00017ae0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00017af0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00017b00: 6561 6e5f 6469 7370 5f78 203d 205b 5d0d  ean_disp_x = [].
+00017b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b20: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00017b30: 7370 5f78 203d 205b 5d0d 0a0d 0a20 2020  sp_x = []....   
+00017b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017b50: 662e 616c 6c5f 6d65 616e 5f72 6164 6975  f.all_mean_radiu
+00017b60: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+00017b70: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00017b80: 5f76 6172 5f72 6164 6975 7320 3d20 5b5d  _var_radius = []
+00017b90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017ba0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00017bb0: 6e5f 7370 6565 6420 3d20 5b5d 0d0a 2020  n_speed = []..  
+00017bc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017bd0: 6c66 2e61 6c6c 5f76 6172 5f73 7065 6564  lf.all_var_speed
+00017be0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00017bf0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00017c00: 6c5f 6d65 616e 5f61 6363 203d 205b 5d0d  l_mean_acc = [].
+00017c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c20: 2073 656c 662e 616c 6c5f 7661 725f 6163   self.all_var_ac
+00017c30: 6320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  c = []....      
+00017c40: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00017c50: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
+00017c60: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+00017c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017c80: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00017c90: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00017ca0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+00017cb0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+00017cc0: 6c5f 6d65 616e 5f64 6973 7461 6e63 655f  l_mean_distance_
+00017cd0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
+00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cf0: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00017d00: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00017d10: 3d20 5b5d 0d0a 0d0a 0d0a 2020 2020 2020  = []......      
+00017d20: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
+00017d30: 6f74 735f 7472 6163 6b73 203d 207b 7d0d  ots_tracks = {}.
+00017d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d50: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
+00017d60: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00017d70: 726f 7065 7274 6965 732e 6974 656d 7328  roperties.items(
+00017d80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00017d90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017db0: 2020 616c 6c5f 7370 6f74 7320 3d20 7365    all_spots = se
+00017dc0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00017dd0: 726f 7065 7274 6965 735b 6b5d 0d0a 2020  roperties[k]..  
+00017de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017df0: 2020 2020 6966 2073 656c 662e 7472 6163      if self.trac
+00017e00: 6b69 645f 6b65 7920 696e 2061 6c6c 5f73  kid_key in all_s
+00017e10: 706f 7473 3a0d 0a20 2020 2020 2020 2020  pots:..         
+00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e30: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00017e40: 735b 6b5d 203d 2061 6c6c 5f73 706f 7473  s[k] = all_spots
+00017e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017e60: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00017e70: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00017e80: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
+00017e90: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017ea0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
+00017eb0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
+00017ec0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
+00017ed0: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
+00017ee0: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
+00017ef0: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
+00017f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f10: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00017f20: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00017f30: 6e20 7471 646d 2872 616e 6765 2873 7461  n tqdm(range(sta
+00017f40: 7274 7469 6d65 2c20 656e 6474 696d 6529  rttime, endtime)
+00017f50: 2c20 746f 7461 6c3d 656e 6474 696d 6520  , total=endtime 
+00017f60: 2d20 7374 6172 7474 696d 6529 3a0d 0a20  - starttime):.. 
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017fa0: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
+00017fb0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
+00017fc0: 6c66 2e5f 636f 6d70 7574 655f 7465 6d70  lf._compute_temp
+00017fd0: 6f72 616c 2c20 692c 2061 6c6c 5f73 706f  oral, i, all_spo
+00017fe0: 7473 5f74 7261 636b 7329 290d 0a20 0d0a  ts_tracks)).. ..
+00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018000: 2020 2020 5b72 2e72 6573 756c 7428 2920      [r.result() 
+00018010: 666f 7220 7220 696e 2063 6f6e 6375 7272  for r in concurr
+00018020: 656e 742e 6675 7475 7265 732e 6173 5f63  ent.futures.as_c
+00018030: 6f6d 706c 6574 6564 2866 7574 7572 6573  ompleted(futures
+00018040: 295d 0d0a 0d0a 0d0a 2020 2020 6465 6620  )]......    def 
+00018050: 5f63 6f6d 7075 7465 5f74 656d 706f 7261  _compute_tempora
+00018060: 6c28 7365 6c66 2c20 692c 2061 6c6c 5f73  l(self, i, all_s
+00018070: 706f 7473 5f74 7261 636b 7329 3a20 2020  pots_tracks):   
+00018080: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00018090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180a0: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+000180b0: 7a20 3d20 5b5d 0d0a 2020 2020 2020 2020  z = []..        
+000180c0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+000180d0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
+000180e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000180f0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00018100: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
+00018110: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00018120: 746f 7469 635f 7261 6469 7573 203d 205b  totic_radius = [
+00018130: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00018140: 2020 2020 2020 206d 6974 6f74 6963 5f73         mitotic_s
+00018150: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
+00018160: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00018170: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
+00018180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018190: 2020 2020 206d 6974 6f74 6963 5f64 6972       mitotic_dir
+000181a0: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
+000181b0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+000181c0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000181d0: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
+000181e0: 6d61 736b 203d 205b 5d0d 0a0d 0a20 2020  mask = []....   
+000181f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018200: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00018210: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
+00018220: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018230: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00018240: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018250: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00018260: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
+00018270: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00018280: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00018290: 7469 635f 7261 6469 7573 203d 205b 5d0d  tic_radius = [].
+000182a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000182b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000182c0: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182e0: 206e 6f6e 5f6d 6974 6f74 6963 5f61 6363   non_mitotic_acc
+000182f0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018300: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00018310: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+00018320: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018340: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00018350: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018360: 736b 203d 205b 5d0d 0a20 2020 2020 2020  sk = []..       
+00018370: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018390: 2020 2061 6c6c 5f64 6973 705f 7a20 3d20     all_disp_z = 
+000183a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000183b0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+000183c0: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
+000183d0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000183e0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
+000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018400: 2020 616c 6c5f 7261 6469 7573 203d 205b    all_radius = [
+00018410: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00018420: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
+00018430: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00018440: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
+00018450: 6363 203d 205b 5d0d 0a20 2020 2020 2020  cc = []..       
+00018460: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00018470: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018480: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
+00018490: 2020 2020 2020 2020 2020 2020 2020 616c                al
+000184a0: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
+000184b0: 6d61 736b 203d 205b 5d0d 0a0d 0a0d 0a0d  mask = [].......
+000184c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000184d0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+000184e0: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
+000184f0: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
+00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018510: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018530: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00018540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018550: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00018560: 7469 6d65 203d 2061 6c6c 5f73 706f 7473  time = all_spots
-00018570: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018580: 6672 616d 6569 645f 6b65 795d 0d0a 2020  frameid_key]..  
-00018590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185a0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
-000185b0: 6320 3d20 616c 6c5f 7370 6f74 735f 7472  c = all_spots_tr
-000185c0: 6163 6b73 5b6b 5d5b 7365 6c66 2e64 6976  acks[k][self.div
-000185d0: 6964 696e 675f 6b65 795d 0d0a 2020 2020  iding_key]..    
+00018530: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00018540: 5f74 696d 6520 3d20 616c 6c5f 7370 6f74  _time = all_spot
+00018550: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018560: 2e66 7261 6d65 6964 5f6b 6579 5d0d 0a20  .frameid_key].. 
+00018570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018580: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
+00018590: 6963 203d 2061 6c6c 5f73 706f 7473 5f74  ic = all_spots_t
+000185a0: 7261 636b 735b 6b5d 5b73 656c 662e 6469  racks[k][self.di
+000185b0: 7669 6469 6e67 5f6b 6579 5d0d 0a20 2020  viding_key]..   
+000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018610: 2020 2020 2069 6620 6920 3d3d 2069 6e74       if i == int
-00018620: 2863 7572 7265 6e74 5f74 696d 6529 3a0d  (current_time):.
-00018630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018650: 2020 2069 6620 6d69 746f 7469 633a 0d0a     if mitotic:..
-00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018680: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00018690: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-000186a0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000186b0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-000186c0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186e0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-000186f0: 6f74 6963 5f64 6973 705f 792e 6170 7065  otic_disp_y.appe
-00018700: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00018710: 636b 735b 6b5d 5b73 656c 662e 7970 6f73  cks[k][self.ypos
-00018720: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00018730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018750: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
-00018760: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018770: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018780: 2e78 706f 7369 645f 6b65 795d 290d 0a20  .xposid_key]).. 
-00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187b0: 2020 2020 2020 2069 6620 616c 6c5f 7370         if all_sp
-000187c0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-000187d0: 6c66 2e72 6164 6975 735f 6b65 795d 203e  lf.radius_key] >
-000187e0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
-000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018810: 6d69 746f 7469 635f 7261 6469 7573 2e61  mitotic_radius.a
-00018820: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018830: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
-00018840: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
-00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185f0: 2020 2020 2020 6966 2069 203d 3d20 696e        if i == in
+00018600: 7428 6375 7272 656e 745f 7469 6d65 293a  t(current_time):
+00018610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018630: 2020 2020 6966 206d 6974 6f74 6963 3a0d      if mitotic:.
+00018640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00018670: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
+00018680: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00018690: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
+000186a0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186c0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000186d0: 746f 7469 635f 6469 7370 5f79 2e61 7070  totic_disp_y.app
+000186e0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000186f0: 6163 6b73 5b6b 5d5b 7365 6c66 2e79 706f  acks[k][self.ypo
+00018700: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018730: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
+00018740: 782e 6170 7065 6e64 2861 6c6c 5f73 706f  x.append(all_spo
+00018750: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00018760: 662e 7870 6f73 6964 5f6b 6579 5d29 0d0a  f.xposid_key])..
+00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018790: 2020 2020 2020 2020 6966 2061 6c6c 5f73          if all_s
+000187a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000187b0: 656c 662e 7261 6469 7573 5f6b 6579 5d20  elf.radius_key] 
+000187c0: 3e20 303a 0d0a 2020 2020 2020 2020 2020  > 0:..          
+000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187f0: 206d 6974 6f74 6963 5f72 6164 6975 732e   mitotic_radius.
+00018800: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00018810: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00018820: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
+00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018850: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
 00018860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018870: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 2020 2020 2020 206d 6974 6f74 6963 5f72         mitotic_r
-000188b0: 6164 6975 732e 6170 7065 6e64 284e 6f6e  adius.append(Non
-000188c0: 6529 2020 2020 2020 200d 0a20 2020 2020  e)       ..     
-000188d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
-00018900: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018910: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018920: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018950: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
-00018960: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
-00018970: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00018980: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-00018990: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189b0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000189c0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-000189d0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-000189e0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-000189f0: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
-00018a00: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
-00018a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a30: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00018a40: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00018a50: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018a60: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018a70: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018a80: 736b 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020  sk_key])......  
-00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ab0: 6966 206e 6f74 206d 6974 6f74 6963 3a0d  if not mitotic:.
-00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ae0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00018af0: 6f74 6963 5f64 6973 705f 7a2e 6170 7065  otic_disp_z.appe
-00018b00: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00018b10: 636b 735b 6b5d 5b73 656c 662e 7a70 6f73  cks[k][self.zpos
-00018b20: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b50: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00018b60: 7370 5f79 2e61 7070 656e 6428 616c 6c5f  sp_y.append(all_
-00018b70: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00018b80: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-00018b90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bb0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018bc0: 6974 6f74 6963 5f64 6973 705f 782e 6170  itotic_disp_x.ap
-00018bd0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00018be0: 7261 636b 735b 6b5d 5b73 656c 662e 7870  racks[k][self.xp
-00018bf0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00018c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c20: 2020 2020 6966 2061 6c6c 5f73 706f 7473      if all_spots
-00018c30: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018c40: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
-00018c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c70: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00018c80: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
-00018c90: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00018ca0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00018cb0: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018880: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00018890: 7261 6469 7573 2e61 7070 656e 6428 4e6f  radius.append(No
+000188a0: 6e65 2920 2020 2020 2020 0d0a 2020 2020  ne)       ..    
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188d0: 2020 2020 6d69 746f 7469 635f 7370 6565      mitotic_spee
+000188e0: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
+000188f0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00018900: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
+00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018930: 2020 2020 2020 206d 6974 6f74 6963 5f61         mitotic_a
+00018940: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
+00018950: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00018960: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
+00018970: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000189a0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+000189b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
+000189c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+000189d0: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
+000189e0: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00018a20: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018a30: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00018a40: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018a50: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+00018a60: 6173 6b5f 6b65 795d 290d 0a0d 0a0d 0a20  ask_key])...... 
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a90: 2069 6620 6e6f 7420 6d69 746f 7469 633a   if not mitotic:
+00018aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ac0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00018ad0: 746f 7469 635f 6469 7370 5f7a 2e61 7070  totic_disp_z.app
+00018ae0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00018af0: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
+00018b00: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b30: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00018b40: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
+00018b50: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00018b60: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00018b70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b90: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00018ba0: 6d69 746f 7469 635f 6469 7370 5f78 2e61  mitotic_disp_x.a
+00018bb0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00018bc0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e78  tracks[k][self.x
+00018bd0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c00: 2020 2020 2069 6620 616c 6c5f 7370 6f74       if all_spot
+00018c10: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018c20: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
+00018c30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00018c60: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+00018c70: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
+00018c80: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00018c90: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
+00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cc0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00018d20: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
-00018d30: 656e 6428 4e6f 6e65 2920 2020 2020 2020  end(None)       
-00018d40: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d60: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00018d70: 5f6d 6974 6f74 6963 5f73 7065 6564 2e61  _mitotic_speed.a
-00018d80: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018d90: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e73  tracks[k][self.s
-00018da0: 7065 6564 5f6b 6579 5d29 0d0a 2020 2020  peed_key])..    
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00018de0: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
-00018df0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00018e00: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
-00018e10: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e40: 6e6f 6e5f 6d69 746f 7469 635f 6469 7265  non_mitotic_dire
-00018e50: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
-00018e60: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018e70: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
-00018e80: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
-00018e90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018eb0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00018ec0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-00018ed0: 6365 6c6c 5f6d 6173 6b2e 6170 7065 6e64  cell_mask.append
-00018ee0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00018ef0: 735b 6b5d 5b73 656c 662e 6469 7374 616e  s[k][self.distan
-00018f00: 6365 5f63 656c 6c5f 6d61 736b 5f6b 6579  ce_cell_mask_key
-00018f10: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f30: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-00018f40: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
-00018f50: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00018f60: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
-00018f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f90: 2020 2061 6c6c 5f64 6973 705f 792e 6170     all_disp_y.ap
-00018fa0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00018fb0: 7261 636b 735b 6b5d 5b73 656c 662e 7970  racks[k][self.yp
-00018fc0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
-00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fe0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018ff0: 6c5f 6469 7370 5f78 2e61 7070 656e 6428  l_disp_x.append(
-00019000: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00019010: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
-00019020: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019040: 2020 2020 2020 2020 2069 6620 616c 6c5f           if all_
-00019050: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00019060: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
-00019070: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019090: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000190a0: 5f72 6164 6975 732e 6170 7065 6e64 2861  _radius.append(a
-000190b0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000190c0: 6b5d 5b73 656c 662e 7261 6469 7573 5f6b  k][self.radius_k
-000190d0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cf0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+00018d00: 6974 6f74 6963 5f72 6164 6975 732e 6170  itotic_radius.ap
+00018d10: 7065 6e64 284e 6f6e 6529 2020 2020 2020  pend(None)      
+00018d20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d40: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018d50: 6e5f 6d69 746f 7469 635f 7370 6565 642e  n_mitotic_speed.
+00018d60: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00018d70: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00018d80: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
+00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018db0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00018dc0: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+00018dd0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00018de0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+00018df0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
+00018e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e20: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
+00018e30: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
+00018e40: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00018e50: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00018e60: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
+00018e70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00018e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e90: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00018ea0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+00018eb0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
+00018ec0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00018ed0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
+00018ee0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
+00018ef0: 795d 290d 0a0d 0a20 2020 2020 2020 2020  y])....         
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00018f20: 705f 7a2e 6170 7065 6e64 2861 6c6c 5f73  p_z.append(all_s
+00018f30: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00018f40: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
+00018f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f70: 2020 2020 616c 6c5f 6469 7370 5f79 2e61      all_disp_y.a
+00018f80: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00018f90: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e79  tracks[k][self.y
+00018fa0: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00018fd0: 6c6c 5f64 6973 705f 782e 6170 7065 6e64  ll_disp_x.append
+00018fe0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00018ff0: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
+00019000: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019020: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
+00019030: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00019040: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
+00019050: 5d20 3e20 303a 0d0a 2020 2020 2020 2020  ] > 0:..        
+00019060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019070: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00019080: 6c5f 7261 6469 7573 2e61 7070 656e 6428  l_radius.append(
+00019090: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000190a0: 5b6b 5d5b 7365 6c66 2e72 6164 6975 735f  [k][self.radius_
+000190b0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000190c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190d0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
 000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019120: 2020 2020 2061 6c6c 5f72 6164 6975 732e       all_radius.
-00019130: 6170 7065 6e64 284e 6f6e 6529 2020 2020  append(None)    
-00019140: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019160: 2020 2020 2020 2061 6c6c 5f73 7065 6564         all_speed
-00019170: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00019180: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00019190: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 616c 6c5f 6163 632e 6170 7065 6e64 2861  all_acc.append(a
-000191d0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000191e0: 6b5d 5b73 656c 662e 6163 6365 6c65 7261  k][self.accelera
-000191f0: 7469 6f6e 5f6b 6579 5d29 0d0a 2020 2020  tion_key])..    
-00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019210: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00019220: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
-00019230: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
-00019240: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00019250: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
-00019260: 655f 6b65 795d 2920 2020 0d0a 2020 2020  e_key])   ..    
-00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019280: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00019290: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-000192a0: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
-000192b0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-000192c0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-000192d0: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a20  ll_mask_key]).. 
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019300: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00019310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019320: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-00019330: 705f 7a20 3d20 6e70 2e61 6273 286e 702e  p_z = np.abs(np.
-00019340: 6469 6666 286d 6974 6f74 6963 5f64 6973  diff(mitotic_dis
-00019350: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-00019360: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00019370: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
-00019380: 6273 286e 702e 6469 6666 286d 6974 6f74  bs(np.diff(mitot
-00019390: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
-000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193b0: 206d 6974 6f74 6963 5f64 6973 705f 7820   mitotic_disp_x 
-000193c0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-000193d0: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
-000193e0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000193f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00019400: 6f74 6963 5f64 6973 705f 7a20 3d20 6e70  otic_disp_z = np
-00019410: 2e61 6273 286e 702e 6469 6666 286e 6f6e  .abs(np.diff(non
-00019420: 5f6d 6974 6f74 6963 5f64 6973 705f 7a29  _mitotic_disp_z)
-00019430: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019440: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00019450: 6963 5f64 6973 705f 7920 3d20 6e70 2e61  ic_disp_y = np.a
-00019460: 6273 286e 702e 6469 6666 286e 6f6e 5f6d  bs(np.diff(non_m
-00019470: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-00019480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019490: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000194a0: 5f64 6973 705f 7820 3d20 6e70 2e61 6273  _disp_x = np.abs
-000194b0: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
-000194c0: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-000194d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000194e0: 2020 2020 2061 6c6c 5f64 6973 705f 7a20       all_disp_z 
-000194f0: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00019500: 2861 6c6c 5f64 6973 705f 7a29 290d 0a20  (all_disp_z)).. 
-00019510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019520: 2020 2061 6c6c 5f64 6973 705f 7920 3d20     all_disp_y = 
-00019530: 6e70 2e61 6273 286e 702e 6469 6666 2861  np.abs(np.diff(a
-00019540: 6c6c 5f64 6973 705f 7929 290d 0a20 2020  ll_disp_y))..   
-00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019560: 2061 6c6c 5f64 6973 705f 7820 3d20 6e70   all_disp_x = np
-00019570: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
-00019580: 5f64 6973 705f 7829 290d 0a0d 0a0d 0a20  _disp_x))...... 
-00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000195c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000195d0: 662e 7469 6d65 2e61 7070 656e 6428 6920  f.time.append(i 
-000195e0: 2a20 7365 6c66 2e74 6361 6c69 6272 6174  * self.tcalibrat
-000195f0: 696f 6e29 0d0a 0d0a 0d0a 2020 2020 2020  ion)......      
-00019600: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019610: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00019620: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00019630: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00019640: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00019650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019660: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
-00019670: 705f 7a2e 6170 7065 6e64 286e 702e 7374  p_z.append(np.st
-00019680: 6428 6d69 746f 7469 635f 6469 7370 5f7a  d(mitotic_disp_z
-00019690: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000196a0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000196b0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-000196c0: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
-000196d0: 6e28 6d69 746f 7469 635f 6469 7370 5f79  n(mitotic_disp_y
-000196e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000196f0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00019700: 6f74 6963 5f76 6172 5f64 6973 705f 792e  otic_var_disp_y.
-00019710: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
-00019720: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
-00019730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019740: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00019750: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
-00019760: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
-00019770: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
-00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019790: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000197a0: 5f76 6172 5f64 6973 705f 782e 6170 7065  _var_disp_x.appe
-000197b0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-000197c0: 635f 6469 7370 5f78 2929 0d0a 0d0a 2020  c_disp_x))....  
-000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197e0: 2020 6669 6c74 6572 6564 5f76 616c 7565    filtered_value
-000197f0: 7320 3d20 5b76 616c 2066 6f72 2076 616c  s = [val for val
-00019800: 2069 6e20 6d69 746f 7469 635f 7261 6469   in mitotic_radi
-00019810: 7573 2069 6620 7661 6c20 6973 206e 6f74  us if val is not
-00019820: 204e 6f6e 655d 0d0a 2020 2020 2020 2020   None]..        
-00019830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019840: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7261  .mitotic_mean_ra
-00019850: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
-00019860: 6561 6e28 6669 6c74 6572 6564 5f76 616c  ean(filtered_val
-00019870: 7565 7329 290d 0a20 2020 2020 2020 2020  ues))..         
-00019880: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198a0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-000198b0: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
-000198c0: 6e70 2e73 7464 2866 696c 7465 7265 645f  np.std(filtered_
-000198d0: 7661 6c75 6573 2929 0d0a 2020 2020 2020  values))..      
-000198e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000198f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019900: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00019910: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
-00019920: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
-00019930: 6963 5f73 7065 6564 2929 0d0a 2020 2020  ic_speed))..    
-00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00019960: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
-00019970: 2e73 7464 286d 6974 6f74 6963 5f73 7065  .std(mitotic_spe
-00019980: 6564 2929 0d0a 0d0a 2020 2020 2020 2020  ed))....        
-00019990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000199a0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6163  .mitotic_mean_ac
-000199b0: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
-000199c0: 286d 6974 6f74 6963 5f61 6363 2929 0d0a  (mitotic_acc))..
-000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199e0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-000199f0: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
-00019a00: 6e70 2e73 7464 286d 6974 6f74 6963 5f61  np.std(mitotic_a
-00019a10: 6363 2929 0d0a 0d0a 2020 2020 2020 2020  cc))....        
-00019a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019a30: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-00019a40: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00019a50: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019a60: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
-00019a70: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
-00019a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00019aa0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00019ab0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00019ac0: 7374 6428 6d69 746f 7469 635f 6469 7265  std(mitotic_dire
-00019ad0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-00019ae0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019af0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00019b00: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
-00019b10: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00019b20: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00019b30: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
-00019b40: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-00019b50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019b60: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00019b70: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00019b80: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
-00019b90: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00019ba0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
-00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bc0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00019bd0: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
-00019be0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019bf0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00019c00: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
-00019c10: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00019c20: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-00019c30: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
-00019c40: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00019c50: 6469 7370 5f7a 2929 0d0a 0d0a 2020 2020  disp_z))....    
-00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c70: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00019c80: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
-00019c90: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
-00019ca0: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
-00019cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019cc0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00019cd0: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00019ce0: 792e 6170 7065 6e64 286e 702e 7374 6428  y.append(np.std(
-00019cf0: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00019d00: 5f79 2929 0d0a 0d0a 2020 2020 2020 2020  _y))....        
-00019d10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019d20: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00019d30: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
-00019d40: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-00019d50: 7469 635f 6469 7370 5f78 2929 0d0a 2020  tic_disp_x))..  
-00019d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d70: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00019d80: 6963 5f76 6172 5f64 6973 705f 782e 6170  ic_var_disp_x.ap
-00019d90: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00019da0: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-00019db0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019dc0: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
-00019dd0: 5f76 616c 7565 7320 3d20 5b76 616c 2066  _values = [val f
-00019de0: 6f72 2076 616c 2069 6e20 6e6f 6e5f 6d69  or val in non_mi
-00019df0: 746f 7469 635f 7261 6469 7573 2069 6620  totic_radius if 
-00019e00: 7661 6c20 6973 206e 6f74 204e 6f6e 655d  val is not None]
-00019e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019e20: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00019e30: 6974 6f74 6963 5f6d 6561 6e5f 7261 6469  itotic_mean_radi
-00019e40: 7573 2e61 7070 656e 6428 6e70 2e6d 6561  us.append(np.mea
-00019e50: 6e28 6669 6c74 6572 6564 5f76 616c 7565  n(filtered_value
-00019e60: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-00019e70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019e90: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00019ea0: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-00019eb0: 6428 6e70 2e73 7464 2866 696c 7465 7265  d(np.std(filtere
-00019ec0: 645f 7661 6c75 6573 2929 0d0a 0d0a 2020  d_values))....  
-00019ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ee0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00019ef0: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
-00019f00: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00019f10: 5f6d 6974 6f74 6963 5f73 7065 6564 2929  _mitotic_speed))
-00019f20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019f30: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00019f40: 6974 6f74 6963 5f76 6172 5f73 7065 6564  itotic_var_speed
-00019f50: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-00019f60: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
-00019f70: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00019f80: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00019f90: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00019fa0: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
-00019fb0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f61  an(non_mitotic_a
-00019fc0: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
-00019fd0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00019fe0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f61  on_mitotic_var_a
-00019ff0: 6363 2e61 7070 656e 6428 6e70 2e73 7464  cc.append(np.std
-0001a000: 286e 6f6e 5f6d 6974 6f74 6963 5f61 6363  (non_mitotic_acc
-0001a010: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-0001a020: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001a030: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-0001a040: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-0001a050: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-0001a060: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-0001a070: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-0001a080: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0001a090: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-0001a0a0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6972  _mitotic_var_dir
-0001a0b0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-0001a0c0: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-0001a0d0: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
-0001a0e0: 696f 6e61 6c5f 6368 616e 6765 2929 200d  ional_change)) .
-0001a0f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a100: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-0001a110: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-0001a120: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-0001a130: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
-0001a140: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
-0001a150: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
-0001a160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a170: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-0001a180: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-0001a190: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-0001a1a0: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
-0001a1b0: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
-0001a1c0: 6365 6c6c 5f6d 6173 6b29 290d 0a0d 0a0d  cell_mask)).....
-0001a1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a1e0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
-0001a1f0: 616e 5f64 6973 705f 7a2e 6170 7065 6e64  an_disp_z.append
-0001a200: 286e 702e 6d65 616e 2861 6c6c 5f64 6973  (np.mean(all_dis
-0001a210: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-0001a220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a230: 616c 6c5f 7661 725f 6469 7370 5f7a 2e61  all_var_disp_z.a
-0001a240: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-0001a250: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
-0001a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a270: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
-0001a280: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-0001a290: 6d65 616e 2861 6c6c 5f64 6973 705f 7929  mean(all_disp_y)
-0001a2a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a2b0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-0001a2c0: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
-0001a2d0: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
-0001a2e0: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-0001a2f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001a300: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
-0001a310: 782e 6170 7065 6e64 286e 702e 6d65 616e  x.append(np.mean
-0001a320: 2861 6c6c 5f64 6973 705f 7829 290d 0a20  (all_disp_x)).. 
-0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a340: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-0001a350: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-0001a360: 2e73 7464 2861 6c6c 5f64 6973 705f 7829  .std(all_disp_x)
-0001a370: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001a380: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
-0001a390: 645f 7661 6c75 6573 203d 205b 7661 6c20  d_values = [val 
-0001a3a0: 666f 7220 7661 6c20 696e 2061 6c6c 5f72  for val in all_r
-0001a3b0: 6164 6975 7320 6966 2076 616c 2069 7320  adius if val is 
-0001a3c0: 6e6f 7420 4e6f 6e65 5d0d 0a20 2020 2020  not None]..     
-0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a3e0: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
-0001a3f0: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
-0001a400: 616e 2866 696c 7465 7265 645f 7661 6c75  an(filtered_valu
-0001a410: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
-0001a420: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a440: 7365 6c66 2e61 6c6c 5f76 6172 5f72 6164  self.all_var_rad
-0001a450: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
-0001a460: 6428 6669 6c74 6572 6564 5f76 616c 7565  d(filtered_value
-0001a470: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
-0001a480: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a490: 616c 6c5f 6d65 616e 5f73 7065 6564 2e61  all_mean_speed.a
-0001a4a0: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-0001a4b0: 6c5f 7370 6565 6429 290d 0a20 2020 2020  l_speed))..     
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a4d0: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
-0001a4e0: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-0001a4f0: 616c 6c5f 7370 6565 6429 290d 0a0d 0a20  all_speed)).... 
-0001a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a510: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-0001a520: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-0001a530: 6561 6e28 616c 6c5f 6163 6329 290d 0a20  ean(all_acc)).. 
-0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a550: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-0001a560: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-0001a570: 6428 616c 6c5f 6163 6329 290d 0a0d 0a0d  d(all_acc)).....
-0001a580: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a590: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-0001a5a0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-0001a5b0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-0001a5c0: 702e 6d65 616e 2861 6c6c 5f64 6972 6563  p.mean(all_direc
-0001a5d0: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
-0001a5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a5f0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-0001a600: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
-0001a610: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
-0001a620: 7464 2861 6c6c 5f64 6972 6563 7469 6f6e  td(all_direction
-0001a630: 616c 5f63 6861 6e67 6529 290d 0a0d 0a20  al_change)).... 
-0001a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a650: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-0001a660: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-0001a670: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
-0001a680: 616e 2861 6c6c 5f64 6973 7461 6e63 655f  an(all_distance_
-0001a690: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
-0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-0001a6c0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0001a6d0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-0001a6e0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-0001a6f0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
-0001a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a710: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-0001a720: 0a64 6566 2062 6f75 6e64 6172 795f 706f  .def boundary_po
-0001a730: 696e 7473 286d 6173 6b2c 2078 6361 6c69  ints(mask, xcali
-0001a740: 6272 6174 696f 6e2c 2079 6361 6c69 6272  bration, ycalibr
-0001a750: 6174 696f 6e2c 207a 6361 6c69 6272 6174  ation, zcalibrat
-0001a760: 696f 6e29 3a0d 0a0d 0a20 2020 206e 6469  ion):....    ndi
-0001a770: 6d20 3d20 6c65 6e28 6d61 736b 2e73 6861  m = len(mask.sha
-0001a780: 7065 290d 0a20 2020 2074 696d 6564 5f6d  pe)..    timed_m
-0001a790: 6173 6b20 3d20 7b7d 0d0a 2020 2020 6d61  ask = {}..    ma
-0001a7a0: 736b 203d 206d 6173 6b20 3e20 300d 0a20  sk = mask > 0.. 
-0001a7b0: 2020 206d 6173 6b20 3d20 6d61 736b 2e61     mask = mask.a
-0001a7c0: 7374 7970 6528 2775 696e 7438 2729 0d0a  stype('uint8')..
-0001a7d0: 2020 2020 2320 5958 2073 6861 7065 6420      # YX shaped 
-0001a7e0: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
-0001a7f0: 6469 6d20 3d3d 2032 3a0d 0a20 2020 2020  dim == 2:..     
-0001a800: 2020 200d 0a20 2020 2020 2020 2062 6f75     ..        bou
-0001a810: 6e64 6172 7920 3d20 6669 6e64 5f62 6f75  ndary = find_bou
-0001a820: 6e64 6172 6965 7328 6d61 736b 290d 0a20  ndaries(mask).. 
-0001a830: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
-0001a840: 7472 6f69 6420 3d20 2830 2c29 202b 2063  troid = (0,) + c
-0001a850: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-0001a860: 626f 756e 6461 7279 2920 0d0a 2020 2020  boundary) ..    
-0001a870: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
-0001a880: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
-0001a890: 3e20 3029 0d0a 2020 2020 2020 2020 7265  > 0)..        re
-0001a8a0: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
-0001a8b0: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
-0001a8c0: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
-0001a8d0: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
-0001a8e0: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
-0001a8f0: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-0001a900: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
-0001a910: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
-0001a920: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-0001a930: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
-0001a940: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
-0001a950: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
-0001a960: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001a970: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
-0001a980: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-0001a990: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
-0001a9a0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 7472  on....        tr
-0001a9b0: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
-0001a9c0: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
-0001a9d0: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
-0001a9e0: 6973 206f 626a 6563 7420 636f 6e74 6169  is object contai
-0001a9f0: 6e73 206c 6973 7420 6f66 2061 6c6c 2074  ns list of all t
-0001aa00: 6865 2070 6f69 6e74 7320 666f 7220 616c  he points for al
-0001aa10: 6c20 7468 6520 6c61 6265 6c73 2069 6e20  l the labels in 
-0001aa20: 7468 6520 4d61 736b 2069 6d61 6765 2077  the Mask image w
-0001aa30: 6974 6820 7468 6520 6c61 6265 6c20 6964  ith the label id
-0001aa40: 2061 6e64 2076 6f6c 756d 6520 6f66 2065   and volume of e
-0001aa50: 6163 6820 6c61 6265 6c0d 0a20 2020 2020  ach label..     
-0001aa60: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
-0001aa70: 7228 3029 5d20 3d20 5b74 7265 652c 2069  r(0)] = [tree, i
-0001aa80: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
-0001aa90: 6e74 726f 6964 5d0d 0a0d 0a20 2020 2023  ntroid]....    #
-0001aaa0: 2054 5958 2073 6861 7065 6420 6f62 6a65   TYX shaped obje
-0001aab0: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
-0001aac0: 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020 2020  == 3:......     
-0001aad0: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
-0001aae0: 2872 616e 6765 2830 2c20 6d61 736b 2e73  (range(0, mask.s
-0001aaf0: 6861 7065 5b30 5d29 293a 0d0a 2020 2020  hape[0])):..    
-0001ab00: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0001ab10: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-0001ab20: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
-0001ab30: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
-0001ab40: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
-0001ab50: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-0001ab60: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
-0001ab70: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
-0001ab80: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
-0001ab90: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-0001aba0: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
-0001abb0: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
-0001abc0: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001abd0: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
-0001abe0: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
-0001abf0: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
-0001ac00: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
-0001ac10: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-0001ac20: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
-0001ac30: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
-0001ac40: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
-0001ac50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ac60: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-0001ac70: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
-0001ac80: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
-0001ac90: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acb0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-0001acc0: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
-0001acd0: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
-0001ace0: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
-0001acf0: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-0001ad00: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-0001ad10: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-0001ad20: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001ad30: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
-0001ad40: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
-0001ad50: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
-0001ad60: 656e 7472 6f69 645d 0d0a 2020 2020 2020  entroid]..      
-0001ad70: 2020 2020 2020 0d0a 2020 2020 2320 545a        ..    # TZ
-0001ad80: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-0001ad90: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-0001ada0: 2034 3a0d 0a20 2020 2020 2020 2070 7269   4:..        pri
-0001adb0: 6e74 2827 4d61 6b69 6e67 206d 6173 6b20  nt('Making mask 
-0001adc0: 696e 2034 4427 290d 0a20 2020 2020 2020  in 4D')..       
-0001add0: 2062 6f75 6e64 6172 7920 3d20 6e70 2e7a   boundary = np.z
-0001ade0: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
-0001adf0: 2020 205b 6d61 736b 2e73 6861 7065 5b30     [mask.shape[0
-0001ae00: 5d2c 206d 6173 6b2e 7368 6170 655b 315d  ], mask.shape[1]
-0001ae10: 2c20 6d61 736b 2e73 6861 7065 5b32 5d2c  , mask.shape[2],
-0001ae20: 206d 6173 6b2e 7368 6170 655b 335d 5d2c   mask.shape[3]],
-0001ae30: 2064 7479 7065 3d6e 702e 7569 6e74 380d   dtype=np.uint8.
-0001ae40: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-0001ae50: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0001ae60: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
-0001ae70: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
-0001ae80: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001ae90: 2062 6f75 6e64 6172 795b 692c 3a5d 203d   boundary[i,:] =
-0001aea0: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
-0001aeb0: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
-0001aec0: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
-0001aed0: 656e 7472 6f69 6420 3d20 636f 6d70 7574  entroid = comput
-0001aee0: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-0001aef0: 6172 795b 692c 3a5d 2920 0d0a 2020 2020  ary[i,:]) ..    
-0001af00: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-0001af10: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
-0001af20: 6172 795b 692c 3a5d 203e 2030 290d 0a20  ary[i,:] > 0).. 
-0001af30: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-0001af40: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
-0001af50: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
-0001af60: 7928 696e 6469 6365 732c 2064 7479 7065  y(indices, dtype
-0001af70: 3d6e 702e 666c 6f61 7433 3229 292e 636f  =np.float32)).co
-0001af80: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
-0001af90: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-0001afa0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
-0001afb0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
-0001afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afd0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-0001afe0: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
-0001aff0: 6573 5b6a 5d5b 305d 202a 207a 6361 6c69  es[j][0] * zcali
-0001b000: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-0001b010: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-0001b020: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-0001b030: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-0001b040: 5d5b 315d 202a 2079 6361 6c69 6272 6174  ][1] * ycalibrat
-0001b050: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-0001b060: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-0001b070: 6469 6365 735b 6a5d 5b32 5d20 3d20 7265  dices[j][2] = re
-0001b080: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
-0001b090: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
-0001b0a0: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
-0001b0b0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
-0001b0c0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
-0001b0d0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-0001b0e0: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
-0001b0f0: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
-0001b100: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
-0001b110: 726f 6964 5d0d 0a20 2020 2070 7269 6e74  roid]..    print
-0001b120: 2827 436f 6d70 7574 6564 2074 6865 2062  ('Computed the b
-0001b130: 6f75 6e64 6172 7920 706f 696e 7473 2729  oundary points')
-0001b140: 0d0a 0d0a 2020 2020 7265 7475 726e 2074  ....    return t
-0001b150: 696d 6564 5f6d 6173 6b2c 2062 6f75 6e64  imed_mask, bound
-0001b160: 6172 7920 2020 2020 2020 200d 0a0d 0a64  ary        ....d
-0001b170: 6566 2063 6f6d 7075 7465 5f63 656e 7472  ef compute_centr
-0001b180: 6f69 6428 6269 6e61 7279 5f69 6d61 6765  oid(binary_image
-0001b190: 293a 0d0a 2020 2020 2320 456e 7375 7265  ):..    # Ensure
-0001b1a0: 2062 696e 6172 7920 696d 6167 6520 6973   binary image is
-0001b1b0: 2061 204e 756d 5079 2061 7272 6179 0d0a   a NumPy array..
-0001b1c0: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
-0001b1d0: 203d 206e 702e 6172 7261 7928 6269 6e61   = np.array(bina
-0001b1e0: 7279 5f69 6d61 6765 290d 0a0d 0a20 2020  ry_image)....   
-0001b1f0: 2077 6869 7465 5f70 6978 656c 7320 3d20   white_pixels = 
-0001b200: 6e70 2e77 6865 7265 2862 696e 6172 795f  np.where(binary_
-0001b210: 696d 6167 6520 3d3d 2031 290d 0a20 2020  image == 1)..   
-0001b220: 206e 756d 5f70 6978 656c 7320 3d20 6c65   num_pixels = le
-0001b230: 6e28 7768 6974 655f 7069 7865 6c73 5b30  n(white_pixels[0
-0001b240: 5d29 0d0a 0d0a 2020 2020 2320 436f 6d70  ])....    # Comp
-0001b250: 7574 6520 7468 6520 6365 6e74 726f 6964  ute the centroid
-0001b260: 206f 6620 7468 6520 7768 6974 6520 7069   of the white pi
-0001b270: 7865 6c73 2069 6e20 7468 6520 626f 756e  xels in the boun
-0001b280: 6461 7279 2069 6d61 6765 0d0a 2020 2020  dary image..    
-0001b290: 6365 6e74 726f 6964 203d 206e 702e 7a65  centroid = np.ze
-0001b2a0: 726f 7328 6269 6e61 7279 5f69 6d61 6765  ros(binary_image
-0001b2b0: 2e6e 6469 6d29 0d0a 2020 2020 666f 7220  .ndim)..    for 
-0001b2c0: 6469 6d20 696e 2072 616e 6765 2862 696e  dim in range(bin
-0001b2d0: 6172 795f 696d 6167 652e 6e64 696d 293a  ary_image.ndim):
-0001b2e0: 0d0a 2020 2020 2020 2020 6365 6e74 726f  ..        centro
-0001b2f0: 6964 5b64 696d 5d20 3d20 7768 6974 655f  id[dim] = white_
-0001b300: 7069 7865 6c73 5b64 696d 5d2e 7375 6d28  pixels[dim].sum(
-0001b310: 2920 2f20 6e75 6d5f 7069 7865 6c73 0d0a  ) / num_pixels..
-0001b320: 0d0a 2020 2020 7265 7475 726e 2063 656e  ..    return cen
-0001b330: 7472 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a  troid........ ..
-0001b340: 0d0a 6465 6620 6765 745f 6373 765f 6461  ..def get_csv_da
-0001b350: 7461 2863 7376 293a 0d0a 0d0a 2020 2020  ta(csv):....    
-0001b360: 2020 2020 6461 7461 7365 7420 3d20 7064      dataset = pd
-0001b370: 2e72 6561 645f 6373 7628 0d0a 2020 2020  .read_csv(..    
-0001b380: 2020 2020 2020 2020 6373 762c 2064 656c          csv, del
-0001b390: 696d 6974 6572 3d22 2c22 2c20 656e 636f  imiter=",", enco
-0001b3a0: 6469 6e67 3d22 756e 6963 6f64 655f 6573  ding="unicode_es
-0001b3b0: 6361 7065 222c 206c 6f77 5f6d 656d 6f72  cape", low_memor
-0001b3c0: 793d 4661 6c73 650d 0a20 2020 2020 2020  y=False..       
-0001b3d0: 2029 5b33 3a5d 0d0a 2020 2020 2020 2020   )[3:]..        
-0001b3e0: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
-0001b3f0: 6461 7461 7365 742e 696e 6465 780d 0a20  dataset.index.. 
-0001b400: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-0001b410: 7461 7365 742c 2064 6174 6173 6574 5f69  taset, dataset_i
-0001b420: 6e64 6578 0d0a 2020 2020 0d0a 6465 6620  ndex..    ..def 
-0001b430: 6765 745f 7370 6f74 5f64 6174 6173 6574  get_spot_dataset
-0001b440: 2873 706f 745f 6461 7461 7365 742c 2074  (spot_dataset, t
-0001b450: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001b460: 6f74 5f6b 6579 732c 2078 6361 6c69 6272  ot_keys, xcalibr
-0001b470: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
-0001b480: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
-0001b490: 6e2c 2041 7474 7269 6275 7465 426f 786e  n, AttributeBoxn
-0001b4a0: 616d 652c 2064 6574 6563 7469 6f6e 6368  ame, detectionch
-0001b4b0: 616e 6e65 6c29 3a0d 0a20 2020 2020 2020  annel):..       
-0001b4c0: 2041 6c6c 5661 6c75 6573 203d 207b 7d0d   AllValues = {}.
-0001b4d0: 0a20 2020 2020 2020 2070 6f73 6978 203d  .        posix =
-0001b4e0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001b4f0: 7370 6f74 5f6b 6579 735b 2270 6f73 6978  spot_keys["posix
-0001b500: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
-0001b510: 7920 3d20 7472 6163 6b5f 616e 616c 7973  y = track_analys
-0001b520: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-0001b530: 7369 7922 5d0d 0a20 2020 2020 2020 2070  siy"]..        p
-0001b540: 6f73 697a 203d 2074 7261 636b 5f61 6e61  osiz = track_ana
-0001b550: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001b560: 2270 6f73 697a 225d 0d0a 2020 2020 2020  "posiz"]..      
-0001b570: 2020 6672 616d 6520 3d20 7472 6163 6b5f    frame = track_
-0001b580: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001b590: 7973 5b22 6672 616d 6522 5d0d 0a20 2020  ys["frame"]..   
-0001b5a0: 2020 2020 200d 0a20 2020 2020 2020 204c       ..        L
-0001b5b0: 6f63 6174 696f 6e58 203d 2028 0d0a 2020  ocationX = (..  
-0001b5c0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
-0001b5d0: 6174 6173 6574 5b70 6f73 6978 5d2e 6173  ataset[posix].as
-0001b5e0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
-0001b5f0: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
-0001b600: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
-0001b610: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
-0001b620: 6f63 6174 696f 6e59 203d 2028 0d0a 2020  ocationY = (..  
-0001b630: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
-0001b640: 6174 6173 6574 5b70 6f73 6979 5d2e 6173  ataset[posiy].as
-0001b650: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
-0001b660: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-0001b670: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
-0001b680: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
-0001b690: 6f63 6174 696f 6e5a 203d 2028 0d0a 2020  ocationZ = (..  
-0001b6a0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
-0001b6b0: 6174 6173 6574 5b70 6f73 697a 5d2e 6173  ataset[posiz].as
-0001b6c0: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
-0001b6d0: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
-0001b6e0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
-0001b6f0: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
-0001b700: 6f63 6174 696f 6e54 203d 2028 7370 6f74  ocationT = (spot
-0001b710: 5f64 6174 6173 6574 5b66 7261 6d65 5d2e  _dataset[frame].
-0001b720: 6173 7479 7065 2822 666c 6f61 7422 2929  astype("float"))
-0001b730: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
-0001b740: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-0001b750: 2020 2020 6967 6e6f 7265 5f76 616c 7565      ignore_value
-0001b760: 7320 3d20 5b74 7261 636b 5f61 6e61 6c79  s = [track_analy
-0001b770: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
-0001b780: 6561 6e5f 696e 7465 6e73 6974 7922 5d2c  ean_intensity"],
-0001b790: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001b7a0: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
-0001b7b0: 696e 7465 6e73 6974 7922 5d5d 0d0a 2020  intensity"]]..  
-0001b7c0: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
-0001b7d0: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001b7e0: 735f 7370 6f74 5f6b 6579 732e 6974 656d  s_spot_keys.item
-0001b7f0: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
-0001b800: 2020 2020 2020 2020 6966 2064 6574 6563          if detec
-0001b810: 7469 6f6e 6368 616e 6e65 6c20 3d3d 2031  tionchannel == 1
-0001b820: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b830: 2020 2020 2020 2020 6966 206b 203d 3d20          if k == 
-0001b840: 226d 6561 6e5f 696e 7465 6e73 6974 795f  "mean_intensity_
-0001b850: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
-0001b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b870: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
-0001b880: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001b890: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
-0001b8a0: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
-0001b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8c0: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
-0001b8d0: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
-0001b8e0: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-0001b8f0: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
-0001b900: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
-0001b910: 3d20 2274 6f74 616c 5f69 6e74 656e 7369  = "total_intensi
-0001b920: 7479 5f63 6832 223a 0d0a 2020 2020 2020  ty_ch2":..      
-0001b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b940: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
-0001b950: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001b960: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
-0001b970: 656e 7369 7479 225d 0d0a 2020 2020 2020  ensity"]..      
-0001b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b990: 2020 2020 2041 6c6c 5661 6c75 6573 5b76       AllValues[v
-0001b9a0: 616c 7565 5d20 3d20 7370 6f74 5f64 6174  alue] = spot_dat
-0001b9b0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001b9c0: 666c 6f61 7422 2920 2020 2020 2020 0d0a  float")       ..
-0001b9d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b9e0: 2020 6966 2076 206e 6f74 2069 6e20 6967    if v not in ig
-0001b9f0: 6e6f 7265 5f76 616c 7565 733a 0d0a 2020  nore_values:..  
-0001ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0001ba20: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001ba30: 6c56 616c 7565 735b 765d 203d 2073 706f  lValues[v] = spo
-0001ba40: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
-0001ba50: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba70: 200d 0a0d 0a20 2020 2020 2020 2041 6c6c   ....        All
-0001ba80: 5661 6c75 6573 5b70 6f73 6978 5d20 3d20  Values[posix] = 
-0001ba90: 726f 756e 6428 4c6f 6361 7469 6f6e 582c  round(LocationX,
-0001baa0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
-0001bab0: 616c 7565 735b 706f 7369 795d 203d 2072  alues[posiy] = r
-0001bac0: 6f75 6e64 284c 6f63 6174 696f 6e59 2c33  ound(LocationY,3
-0001bad0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
-0001bae0: 6c75 6573 5b70 6f73 697a 5d20 3d20 726f  lues[posiz] = ro
-0001baf0: 756e 6428 4c6f 6361 7469 6f6e 5a2c 3329  und(LocationZ,3)
-0001bb00: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
-0001bb10: 7565 735b 6672 616d 655d 203d 2072 6f75  ues[frame] = rou
-0001bb20: 6e64 284c 6f63 6174 696f 6e54 2c33 290d  nd(LocationT,3).
-0001bb30: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
-0001bb40: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
-0001bb50: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
-0001bb60: 2e61 7070 656e 6428 4174 7472 6962 7574  .append(Attribut
-0001bb70: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
-0001bb80: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
-0001bb90: 6e61 6d65 2069 6e20 416c 6c56 616c 7565  name in AllValue
-0001bba0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
-0001bbb0: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
-0001bbc0: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
-0001bbd0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
-0001bbe0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001bbf0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001bc00: 2072 6574 7572 6e20 4174 7472 6962 7574   return Attribut
-0001bc10: 6569 6473 2c20 416c 6c56 616c 7565 7320  eids, AllValues 
-0001bc20: 2020 2020 0d0a 2020 2020 0d0a 0d0a 6465      ..    ....de
-0001bc30: 6620 6765 745f 7472 6163 6b5f 6461 7461  f get_track_data
-0001bc40: 7365 7428 7472 6163 6b5f 6461 7461 7365  set(track_datase
-0001bc50: 742c 2074 7261 636b 5f61 6e61 6c79 7369  t, track_analysi
-0001bc60: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
-0001bc70: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
-0001bc80: 6b5f 6b65 7973 2c20 5472 6163 6b41 7474  k_keys, TrackAtt
-0001bc90: 7269 6275 7465 426f 786e 616d 6529 3a0d  ributeBoxname):.
-0001bca0: 0a0d 0a20 2020 2020 2020 2041 6c6c 5472  ...        AllTr
-0001bcb0: 6163 6b56 616c 7565 7320 3d20 7b7d 0d0a  ackValues = {}..
-0001bcc0: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0001bcd0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001bce0: 735f 7370 6f74 5f6b 6579 735b 2274 7261  s_spot_keys["tra
-0001bcf0: 636b 5f69 6422 5d0d 0a20 2020 2020 2020  ck_id"]..       
-0001bd00: 2054 6964 203d 2074 7261 636b 5f64 6174   Tid = track_dat
-0001bd10: 6173 6574 5b74 7261 636b 5f69 645d 2e61  aset[track_id].a
-0001bd20: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001bd30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001bd40: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
-0001bd50: 7472 6163 6b5f 6964 5d20 3d20 5469 640d  track_id] = Tid.
-0001bd60: 0a20 2020 2020 200d 0a20 2020 2020 2020  .      ..       
-0001bd70: 2066 6f72 2028 6b2c 2076 2920 696e 2074   for (k, v) in t
-0001bd80: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001bd90: 6163 6b5f 6b65 7973 2e69 7465 6d73 2829  ack_keys.items()
-0001bda0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001bdb0: 2020 2020 2078 203d 2074 7261 636b 5f64       x = track_d
-0001bdc0: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
-0001bdd0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001bde0: 2020 2020 2020 2020 2020 206d 696e 7661             minva
-0001bdf0: 6c20 3d20 6d69 6e28 7829 0d0a 2020 2020  l = min(x)..    
-0001be00: 2020 2020 2020 2020 2020 2020 6d61 7876              maxv
-0001be10: 616c 203d 206d 6178 2878 290d 0a0d 0a20  al = max(x).... 
-0001be20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001be30: 6620 6d69 6e76 616c 203e 2030 2061 6e64  f minval > 0 and
-0001be40: 206d 6178 7661 6c20 3c3d 2031 3a0d 0a0d   maxval <= 1:...
-0001be50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001be60: 2020 2020 2078 203d 2078 202b 2031 0d0a       x = x + 1..
-0001be70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001be80: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
-0001be90: 5b6b 5d20 3d20 726f 756e 6428 782c 2033  [k] = round(x, 3
-0001bea0: 290d 0a0d 0a20 2020 2020 2020 2054 7261  )....        Tra
-0001beb0: 636b 4174 7472 6962 7574 6569 6473 203d  ckAttributeids =
-0001bec0: 205b 5d0d 0a20 2020 2020 2020 2054 7261   []..        Tra
-0001bed0: 636b 4174 7472 6962 7574 6569 6473 2e61  ckAttributeids.a
-0001bee0: 7070 656e 6428 5472 6163 6b41 7474 7269  ppend(TrackAttri
-0001bef0: 6275 7465 426f 786e 616d 6529 0d0a 2020  buteBoxname)..  
-0001bf00: 2020 2020 2020 666f 7220 6174 7472 6962        for attrib
-0001bf10: 7574 656e 616d 6520 696e 2074 7261 636b  utename in track
-0001bf20: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
-0001bf30: 6b65 7973 2e6b 6579 7328 293a 0d0a 2020  keys.keys():..  
-0001bf40: 2020 2020 2020 2020 2020 5472 6163 6b41            TrackA
-0001bf50: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
-0001bf60: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
-0001bf70: 2920 2020 200d 0a20 2020 200d 0a20 2020  )    ..    ..   
-0001bf80: 2020 2020 2072 6574 7572 6e20 5472 6163       return Trac
-0001bf90: 6b41 7474 7269 6275 7465 6964 732c 2041  kAttributeids, A
-0001bfa0: 6c6c 5472 6163 6b56 616c 7565 730d 0a20  llTrackValues.. 
-0001bfb0: 2020 200d 0a64 6566 2067 6574 5f65 6467     ..def get_edg
-0001bfc0: 6573 5f64 6174 6173 6574 2865 6467 6573  es_dataset(edges
-0001bfd0: 5f64 6174 6173 6574 2c20 6564 6765 735f  _dataset, edges_
-0001bfe0: 6461 7461 7365 745f 696e 6465 782c 2074  dataset_index, t
-0001bff0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001c000: 6f74 5f6b 6579 732c 2074 7261 636b 5f61  ot_keys, track_a
-0001c010: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
-0001c020: 7973 293a 0d0a 0d0a 2020 2020 2020 2020  ys):....        
-0001c030: 416c 6c45 6467 6573 5661 6c75 6573 203d  AllEdgesValues =
-0001c040: 207b 7d0d 0a20 2020 2020 2020 2074 7261   {}..        tra
-0001c050: 636b 5f69 6420 3d20 7472 6163 6b5f 616e  ck_id = track_an
-0001c060: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001c070: 5b22 7472 6163 6b5f 6964 225d 0d0a 2020  ["track_id"]..  
-0001c080: 2020 2020 2020 5469 6420 3d20 6564 6765        Tid = edge
-0001c090: 735f 6461 7461 7365 745b 7472 6163 6b5f  s_dataset[track_
-0001c0a0: 6964 5d2e 6173 7479 7065 2822 666c 6f61  id].astype("floa
-0001c0b0: 7422 290d 0a20 2020 2020 2020 2069 6e64  t")..        ind
-0001c0c0: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
-0001c0d0: 5469 6420 3d3d 2030 290d 0a20 2020 2020  Tid == 0)..     
-0001c0e0: 2020 206d 6178 7472 6163 6b5f 6964 203d     maxtrack_id =
-0001c0f0: 206d 6178 2854 6964 290d 0a20 2020 2020   max(Tid)..     
-0001c100: 2020 2063 6f6e 6469 7469 6f6e 5f69 6e64     condition_ind
-0001c110: 6963 6573 203d 2065 6467 6573 5f64 6174  ices = edges_dat
-0001c120: 6173 6574 5f69 6e64 6578 5b69 6e64 6963  aset_index[indic
-0001c130: 6573 5d0d 0a20 2020 2020 2020 2054 6964  es]..        Tid
-0001c140: 5b63 6f6e 6469 7469 6f6e 5f69 6e64 6963  [condition_indic
-0001c150: 6573 5d20 3d20 6d61 7874 7261 636b 5f69  es] = maxtrack_i
-0001c160: 6420 2b20 310d 0a20 2020 2020 2020 2041  d + 1..        A
-0001c170: 6c6c 4564 6765 7356 616c 7565 735b 7472  llEdgesValues[tr
-0001c180: 6163 6b5f 6964 5d20 3d20 5469 640d 0a0d  ack_id] = Tid...
-0001c190: 0a20 2020 2020 2020 2066 6f72 206b 2069  .        for k i
-0001c1a0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
-0001c1b0: 5f65 6467 6573 5f6b 6579 732e 7661 6c75  _edges_keys.valu
-0001c1c0: 6573 2829 3a0d 0a0d 0a20 2020 2020 2020  es():....       
-0001c1d0: 2020 2020 2069 6620 6b20 213d 2074 7261       if k != tra
-0001c1e0: 636b 5f69 643a 0d0a 2020 2020 2020 2020  ck_id:..        
-0001c1f0: 2020 2020 2020 2020 7820 3d20 6564 6765          x = edge
-0001c200: 735f 6461 7461 7365 745b 6b5d 2e61 7374  s_dataset[k].ast
-0001c210: 7970 6528 2266 6c6f 6174 2229 0d0a 0d0a  ype("float")....
-0001c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c230: 416c 6c45 6467 6573 5661 6c75 6573 5b6b  AllEdgesValues[k
-0001c240: 5d20 3d20 7820 2020 0d0a 2020 2020 2020  ] = x   ..      
-0001c250: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001c260: 7572 6e20 416c 6c45 6467 6573 5661 6c75  urn AllEdgesValu
-0001c270: 6573 2020 200d 0a20 2020 200d 0a20 2020  es   ..    ..   
-0001c280: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
-0001c290: 7363 616c 655f 7661 6c75 6528 782c 2073  scale_value(x, s
-0001c2a0: 6361 6c65 203d 2032 3535 202a 2032 3535  cale = 255 * 255
-0001c2b0: 293a 0d0a 0d0a 0d0a 2020 2020 2072 6574  ):......     ret
-0001c2c0: 7572 6e20 7820 2a20 7363 616c 6520 2020  urn x * scale   
-0001c2d0: 0d0a 2020 2020 0d0a 0d0a 0d0a 6465 6620  ..    ......def 
-0001c2e0: 7072 6f62 5f73 6967 6d6f 6964 2878 293a  prob_sigmoid(x):
-0001c2f0: 0d0a 2020 2020 7265 7475 726e 2031 202d  ..    return 1 -
-0001c300: 206d 6174 682e 6578 7028 2d78 290d 0a0d   math.exp(-x)...
-0001c310: 0a0d 0a64 6566 2061 6e67 756c 6172 5f63  ...def angular_c
-0001c320: 6861 6e67 6528 7665 635f 302c 2076 6563  hange(vec_0, vec
-0001c330: 5f31 293a 0d0a 2020 2020 2020 2020 0d0a  _1):..        ..
-0001c340: 2020 2020 2020 2020 7665 635f 3020 3d20          vec_0 = 
-0001c350: 7665 635f 3020 2f20 6e70 2e6c 696e 616c  vec_0 / np.linal
-0001c360: 672e 6e6f 726d 2876 6563 5f30 290d 0a20  g.norm(vec_0).. 
-0001c370: 2020 2020 2020 2076 6563 5f31 203d 2076         vec_1 = v
-0001c380: 6563 5f31 202f 206e 702e 6c69 6e61 6c67  ec_1 / np.linalg
-0001c390: 2e6e 6f72 6d28 7665 635f 3129 0d0a 2020  .norm(vec_1)..  
-0001c3a0: 2020 2020 2020 616e 676c 6520 3d20 6e70        angle = np
-0001c3b0: 2e61 7263 636f 7328 6e70 2e63 6c69 7028  .arccos(np.clip(
-0001c3c0: 6e70 2e64 6f74 2876 6563 5f30 2c20 7665  np.dot(vec_0, ve
-0001c3d0: 635f 3129 2c20 2d31 2e30 2c20 312e 3029  c_1), -1.0, 1.0)
-0001c3e0: 290d 0a20 2020 2020 2020 2061 6e67 6c65  )..        angle
-0001c3f0: 203d 2061 6e67 6c65 202a 2031 3830 202f   = angle * 180 /
-0001c400: 206e 702e 7069 0d0a 2020 2020 2020 2020   np.pi..        
-0001c410: 7265 7475 726e 2061 6e67 6c65 0d0a 2020  return angle..  
-0001c420: 2020 200d 0a0d 0a64 6566 2065 7661 6c5f     ....def eval_
-0001c430: 626f 6f6c 2876 616c 7565 293a 0d0a 2020  bool(value):..  
-0001c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c450: 0d0a 2020 2020 2020 2020 6966 2076 616c  ..        if val
-0001c460: 7565 2020 3d3d 2027 5472 7565 273a 200d  ue  == 'True': .
-0001c470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c480: 2064 6976 5f6b 6579 203d 2054 7275 650d   div_key = True.
-0001c490: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0001c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4b0: 6469 765f 6b65 7920 3d20 4661 6c73 6520  div_key = False 
-0001c4c0: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-0001c4d0: 726e 2064 6976 5f6b 6579 2020 2020 2020  rn div_key      
-0001c4e0: 2020 2020 2020 2020 2020 0d0a 0d0a 6465            ....de
-0001c4f0: 6620 6368 6563 6b5f 616e 645f 7570 6461  f check_and_upda
-0001c500: 7465 5f6d 6173 6b28 6d61 736b 2c69 6d61  te_mask(mask,ima
-0001c510: 6765 293a 0d0a 2020 2020 2020 200d 0a20  ge):..       .. 
-0001c520: 2020 2020 2020 2069 6620 6c65 6e28 6d61         if len(ma
-0001c530: 736b 2e73 6861 7065 2920 3c20 6c65 6e28  sk.shape) < len(
-0001c540: 696d 6167 652e 7368 6170 6529 3a0d 0a20  image.shape):.. 
-0001c550: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-0001c560: 655f 6d61 736b 203d 206e 702e 7a65 726f  e_mask = np.zero
-0001c570: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
+000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019100: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
+00019110: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
+00019120: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019140: 2020 2020 2020 2020 616c 6c5f 7370 6565          all_spee
+00019150: 642e 6170 7065 6e64 2861 6c6c 5f73 706f  d.append(all_spo
+00019160: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00019170: 662e 7370 6565 645f 6b65 795d 290d 0a20  f.speed_key]).. 
+00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191a0: 2061 6c6c 5f61 6363 2e61 7070 656e 6428   all_acc.append(
+000191b0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+000191c0: 5b6b 5d5b 7365 6c66 2e61 6363 656c 6572  [k][self.acceler
+000191d0: 6174 696f 6e5f 6b65 795d 290d 0a20 2020  ation_key])..   
+000191e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019200: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
+00019210: 6861 6e67 652e 6170 7065 6e64 2861 6c6c  hange.append(all
+00019220: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00019230: 5b73 656c 662e 6d6f 7469 6f6e 5f61 6e67  [self.motion_ang
+00019240: 6c65 5f6b 6579 5d29 2020 200d 0a20 2020  le_key])   ..   
+00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019260: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00019270: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+00019280: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
+00019290: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000192a0: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+000192b0: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000192f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019300: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
+00019310: 7370 5f7a 203d 206e 702e 6162 7328 6e70  sp_z = np.abs(np
+00019320: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
+00019330: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+00019340: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00019350: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
+00019360: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
+00019370: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
+00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019390: 2020 6d69 746f 7469 635f 6469 7370 5f78    mitotic_disp_x
+000193a0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+000193b0: 6628 6d69 746f 7469 635f 6469 7370 5f78  f(mitotic_disp_x
+000193c0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000193d0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+000193e0: 746f 7469 635f 6469 7370 5f7a 203d 206e  totic_disp_z = n
+000193f0: 702e 6162 7328 6e70 2e64 6966 6628 6e6f  p.abs(np.diff(no
+00019400: 6e5f 6d69 746f 7469 635f 6469 7370 5f7a  n_mitotic_disp_z
+00019410: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00019420: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00019430: 7469 635f 6469 7370 5f79 203d 206e 702e  tic_disp_y = np.
+00019440: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
+00019450: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+00019460: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019470: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00019480: 635f 6469 7370 5f78 203d 206e 702e 6162  c_disp_x = np.ab
+00019490: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
+000194a0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+000194b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000194c0: 2020 2020 2020 616c 6c5f 6469 7370 5f7a        all_disp_z
+000194d0: 203d 206e 702e 6162 7328 6e70 2e64 6966   = np.abs(np.dif
+000194e0: 6628 616c 6c5f 6469 7370 5f7a 2929 0d0a  f(all_disp_z))..
+000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019500: 2020 2020 616c 6c5f 6469 7370 5f79 203d      all_disp_y =
+00019510: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00019520: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
+00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019540: 2020 616c 6c5f 6469 7370 5f78 203d 206e    all_disp_x = n
+00019550: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
+00019560: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 0d0a  l_disp_x))......
+00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019590: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000195a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000195b0: 6c66 2e74 696d 652e 6170 7065 6e64 2869  lf.time.append(i
+000195c0: 202a 2073 656c 662e 7463 616c 6962 7261   * self.tcalibra
+000195d0: 7469 6f6e 290d 0a0d 0a0d 0a20 2020 2020  tion)......     
+000195e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000195f0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00019600: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+00019610: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+00019620: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00019630: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019640: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00019650: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
+00019660: 7464 286d 6974 6f74 6963 5f64 6973 705f  td(mitotic_disp_
+00019670: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
+00019680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019690: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+000196a0: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
+000196b0: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+000196c0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+000196d0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+000196e0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
+000196f0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+00019700: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+00019710: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019720: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00019730: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
+00019740: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00019750: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00019760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019770: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00019780: 635f 7661 725f 6469 7370 5f78 2e61 7070  c_var_disp_x.app
+00019790: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+000197a0: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2066 696c 7465 7265 645f 7661 6c75     filtered_valu
+000197d0: 6573 203d 205b 7661 6c20 666f 7220 7661  es = [val for va
+000197e0: 6c20 696e 206d 6974 6f74 6963 5f72 6164  l in mitotic_rad
+000197f0: 6975 7320 6966 2076 616c 2069 7320 6e6f  ius if val is no
+00019800: 7420 4e6f 6e65 5d0d 0a20 2020 2020 2020  t None]..       
+00019810: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019820: 662e 6d69 746f 7469 635f 6d65 616e 5f72  f.mitotic_mean_r
+00019830: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
+00019840: 6d65 616e 2866 696c 7465 7265 645f 7661  mean(filtered_va
+00019850: 6c75 6573 2929 0d0a 2020 2020 2020 2020  lues))..        
+00019860: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00019870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019880: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00019890: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
+000198a0: 286e 702e 7374 6428 6669 6c74 6572 6564  (np.std(filtered
+000198b0: 5f76 616c 7565 7329 290d 0a20 2020 2020  _values))..     
+000198c0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000198d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000198e0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000198f0: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
+00019900: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00019910: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
+00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019930: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00019940: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
+00019950: 702e 7374 6428 6d69 746f 7469 635f 7370  p.std(mitotic_sp
+00019960: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
+00019970: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019980: 662e 6d69 746f 7469 635f 6d65 616e 5f61  f.mitotic_mean_a
+00019990: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
+000199a0: 6e28 6d69 746f 7469 635f 6163 6329 290d  n(mitotic_acc)).
+000199b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199c0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+000199d0: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
+000199e0: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+000199f0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
+00019a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019a10: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00019a20: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00019a30: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
+00019a40: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
+00019a50: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
+00019a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a70: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00019a80: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+00019a90: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
+00019aa0: 2e73 7464 286d 6974 6f74 6963 5f64 6972  .std(mitotic_dir
+00019ab0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+00019ac0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019ad0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00019ae0: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
+00019af0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00019b00: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
+00019b10: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00019b20: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
+00019b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019b40: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00019b50: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00019b60: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
+00019b70: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
+00019b80: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
+00019b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ba0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00019bb0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+00019bc0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
+00019bd0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00019be0: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
+00019bf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019c00: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019c10: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
+00019c20: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
+00019c30: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
+00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c50: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00019c60: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
+00019c70: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+00019c80: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
+00019c90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019ca0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00019cb0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00019cc0: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
+00019cd0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
+00019ce0: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
+00019cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019d00: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00019d10: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
+00019d20: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
+00019d30: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
+00019d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d50: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00019d60: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
+00019d70: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+00019d80: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
+00019d90: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019da0: 2020 2020 2020 2020 2066 696c 7465 7265           filtere
+00019db0: 645f 7661 6c75 6573 203d 205b 7661 6c20  d_values = [val 
+00019dc0: 666f 7220 7661 6c20 696e 206e 6f6e 5f6d  for val in non_m
+00019dd0: 6974 6f74 6963 5f72 6164 6975 7320 6966  itotic_radius if
+00019de0: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
+00019df0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00019e00: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00019e10: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
+00019e20: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
+00019e30: 616e 2866 696c 7465 7265 645f 7661 6c75  an(filtered_valu
+00019e40: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
+00019e50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00019e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e70: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00019e80: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00019e90: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
+00019ea0: 6564 5f76 616c 7565 7329 290d 0a0d 0a20  ed_values)).... 
+00019eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ec0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00019ed0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
+00019ee0: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00019ef0: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
+00019f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019f10: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00019f20: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
+00019f30: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
+00019f40: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
+00019f50: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
+00019f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019f70: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00019f80: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+00019f90: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00019fa0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
+00019fb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019fc0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019fd0: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
+00019fe0: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
+00019ff0: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
+0001a000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a010: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+0001a020: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+0001a030: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+0001a040: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+0001a050: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+0001a060: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+0001a070: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+0001a080: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+0001a090: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+0001a0a0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+0001a0b0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
+0001a0c0: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
+0001a0d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a0e0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+0001a0f0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+0001a100: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+0001a110: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+0001a120: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
+0001a130: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
+0001a140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a150: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+0001a160: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+0001a170: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+0001a180: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+0001a190: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
+0001a1a0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
+0001a1b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a1c0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+0001a1d0: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
+0001a1e0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+0001a1f0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+0001a200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a210: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
+0001a220: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+0001a230: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
+0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a250: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+0001a260: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+0001a270: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
+0001a280: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0001a290: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+0001a2a0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+0001a2b0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
+0001a2c0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
+0001a2d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a2e0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+0001a2f0: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
+0001a300: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
+0001a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a320: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+0001a330: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+0001a340: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
+0001a350: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+0001a360: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+0001a370: 6564 5f76 616c 7565 7320 3d20 5b76 616c  ed_values = [val
+0001a380: 2066 6f72 2076 616c 2069 6e20 616c 6c5f   for val in all_
+0001a390: 7261 6469 7573 2069 6620 7661 6c20 6973  radius if val is
+0001a3a0: 206e 6f74 204e 6f6e 655d 0d0a 2020 2020   not None]..    
+0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3c0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
+0001a3d0: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
+0001a3e0: 6561 6e28 6669 6c74 6572 6564 5f76 616c  ean(filtered_val
+0001a3f0: 7565 7329 290d 0a20 2020 2020 2020 2020  ues))..         
+0001a400: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a420: 2073 656c 662e 616c 6c5f 7661 725f 7261   self.all_var_ra
+0001a430: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+0001a440: 7464 2866 696c 7465 7265 645f 7661 6c75  td(filtered_valu
+0001a450: 6573 2929 0d0a 0d0a 2020 2020 2020 2020  es))....        
+0001a460: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a470: 2e61 6c6c 5f6d 6561 6e5f 7370 6565 642e  .all_mean_speed.
+0001a480: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+0001a490: 6c6c 5f73 7065 6564 2929 0d0a 2020 2020  ll_speed))..    
+0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4b0: 7365 6c66 2e61 6c6c 5f76 6172 5f73 7065  self.all_var_spe
+0001a4c0: 6564 2e61 7070 656e 6428 6e70 2e73 7464  ed.append(np.std
+0001a4d0: 2861 6c6c 5f73 7065 6564 2929 0d0a 0d0a  (all_speed))....
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4f0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+0001a500: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
+0001a510: 6d65 616e 2861 6c6c 5f61 6363 2929 0d0a  mean(all_acc))..
+0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a530: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+0001a540: 5f61 6363 2e61 7070 656e 6428 6e70 2e73  _acc.append(np.s
+0001a550: 7464 2861 6c6c 5f61 6363 2929 0d0a 0d0a  td(all_acc))....
+0001a560: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a570: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+0001a580: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
+0001a590: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+0001a5a0: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7265  np.mean(all_dire
+0001a5b0: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
+0001a5c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a5d0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+0001a5e0: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
+0001a5f0: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+0001a600: 7374 6428 616c 6c5f 6469 7265 6374 696f  std(all_directio
+0001a610: 6e61 6c5f 6368 616e 6765 2929 0d0a 0d0a  nal_change))....
+0001a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a630: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+0001a640: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+0001a650: 6d61 736b 2e61 7070 656e 6428 6e70 2e6d  mask.append(np.m
+0001a660: 6561 6e28 616c 6c5f 6469 7374 616e 6365  ean(all_distance
+0001a670: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
+0001a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a690: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
+0001a6a0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0001a6b0: 6b2e 6170 7065 6e64 286e 702e 7374 6428  k.append(np.std(
+0001a6c0: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
+0001a6d0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a700: 0d0a 6465 6620 626f 756e 6461 7279 5f70  ..def boundary_p
+0001a710: 6f69 6e74 7328 6d61 736b 2c20 7863 616c  oints(mask, xcal
+0001a720: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
+0001a730: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
+0001a740: 7469 6f6e 293a 0d0a 0d0a 2020 2020 6e64  tion):....    nd
+0001a750: 696d 203d 206c 656e 286d 6173 6b2e 7368  im = len(mask.sh
+0001a760: 6170 6529 0d0a 2020 2020 7469 6d65 645f  ape)..    timed_
+0001a770: 6d61 736b 203d 207b 7d0d 0a20 2020 206d  mask = {}..    m
+0001a780: 6173 6b20 3d20 6d61 736b 203e 2030 0d0a  ask = mask > 0..
+0001a790: 2020 2020 6d61 736b 203d 206d 6173 6b2e      mask = mask.
+0001a7a0: 6173 7479 7065 2827 7569 6e74 3827 290d  astype('uint8').
+0001a7b0: 0a20 2020 2023 2059 5820 7368 6170 6564  .    # YX shaped
+0001a7c0: 206f 626a 6563 740d 0a20 2020 2069 6620   object..    if 
+0001a7d0: 6e64 696d 203d 3d20 323a 0d0a 2020 2020  ndim == 2:..    
+0001a7e0: 2020 2020 0d0a 2020 2020 2020 2020 626f      ..        bo
+0001a7f0: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
+0001a800: 756e 6461 7269 6573 286d 6173 6b29 0d0a  undaries(mask)..
+0001a810: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
+0001a820: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
+0001a830: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
+0001a840: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
+0001a850: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
+0001a860: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
+0001a870: 203e 2030 290d 0a20 2020 2020 2020 2072   > 0)..        r
+0001a880: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
+0001a890: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
+0001a8a0: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
+0001a8b0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+0001a8c0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
+0001a8d0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0001a8e0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+0001a8f0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+0001a900: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+0001a910: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
+0001a920: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+0001a930: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+0001a940: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+0001a950: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+0001a960: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+0001a970: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
+0001a980: 696f 6e0d 0a0d 0a20 2020 2020 2020 2074  ion....        t
+0001a990: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+0001a9a0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+0001a9b0: 6573 290d 0a20 2020 2020 2020 2023 2054  es)..        # T
+0001a9c0: 6869 7320 6f62 6a65 6374 2063 6f6e 7461  his object conta
+0001a9d0: 696e 7320 6c69 7374 206f 6620 616c 6c20  ins list of all 
+0001a9e0: 7468 6520 706f 696e 7473 2066 6f72 2061  the points for a
+0001a9f0: 6c6c 2074 6865 206c 6162 656c 7320 696e  ll the labels in
+0001aa00: 2074 6865 204d 6173 6b20 696d 6167 6520   the Mask image 
+0001aa10: 7769 7468 2074 6865 206c 6162 656c 2069  with the label i
+0001aa20: 6420 616e 6420 766f 6c75 6d65 206f 6620  d and volume of 
+0001aa30: 6561 6368 206c 6162 656c 0d0a 2020 2020  each label..    
+0001aa40: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
+0001aa50: 7472 2830 295d 203d 205b 7472 6565 2c20  tr(0)] = [tree, 
+0001aa60: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
+0001aa70: 656e 7472 6f69 645d 0d0a 0d0a 2020 2020  entroid]....    
+0001aa80: 2320 5459 5820 7368 6170 6564 206f 626a  # TYX shaped obj
+0001aa90: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
+0001aaa0: 203d 3d20 333a 0d0a 0d0a 0d0a 2020 2020   == 3:......    
+0001aab0: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
+0001aac0: 6d28 7261 6e67 6528 302c 206d 6173 6b2e  m(range(0, mask.
+0001aad0: 7368 6170 655b 305d 2929 3a0d 0a20 2020  shape[0])):..   
+0001aae0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001ab00: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
+0001ab10: 6f75 6e64 6172 6965 7328 6d61 736b 5b69  oundaries(mask[i
+0001ab20: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
+0001ab30: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
+0001ab40: 726f 6964 203d 2028 302c 2920 2b20 636f  roid = (0,) + co
+0001ab50: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
+0001ab60: 6f75 6e64 6172 7929 200d 0a20 2020 2020  oundary) ..     
+0001ab70: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+0001ab80: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
+0001ab90: 756e 6461 7279 203e 2030 290d 0a20 2020  undary > 0)..   
+0001aba0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0001abb0: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
+0001abc0: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
+0001abd0: 7261 7928 696e 6469 6365 732c 2064 7479  ray(indices, dty
+0001abe0: 7065 3d6e 702e 666c 6f61 7433 3229 292e  pe=np.float32)).
+0001abf0: 636f 7079 2829 0d0a 0d0a 2020 2020 2020  copy()....      
+0001ac00: 2020 2020 2020 2020 2020 666f 7220 6a20            for j 
+0001ac10: 696e 2072 616e 6765 2830 2c20 6c65 6e28  in range(0, len(
+0001ac20: 7265 616c 5f69 6e64 6963 6573 2929 3a0d  real_indices)):.
+0001ac30: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001ac40: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+0001ac50: 6365 735b 6a5d 5b30 5d20 3d20 7265 616c  ces[j][0] = real
+0001ac60: 5f69 6e64 6963 6573 5b6a 5d5b 305d 202a  _indices[j][0] *
+0001ac70: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
+0001ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac90: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
+0001aca0: 6a5d 5b31 5d20 3d20 7265 616c 5f69 6e64  j][1] = real_ind
+0001acb0: 6963 6573 5b6a 5d5b 315d 202a 2078 6361  ices[j][1] * xca
+0001acc0: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
+0001acd0: 2020 2020 2020 2020 2020 2020 2074 7265               tre
+0001ace0: 6520 3d20 7370 6174 6961 6c2e 634b 4454  e = spatial.cKDT
+0001acf0: 7265 6528 7265 616c 5f69 6e64 6963 6573  ree(real_indices
+0001ad00: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001ad10: 2020 2020 2074 696d 6564 5f6d 6173 6b5b       timed_mask[
+0001ad20: 7374 7228 6929 5d20 3d20 5b74 7265 652c  str(i)] = [tree,
+0001ad30: 2069 6e64 6963 6573 2c20 7265 6769 6f6e   indices, region
+0001ad40: 6365 6e74 726f 6964 5d0d 0a20 2020 2020  centroid]..     
+0001ad50: 2020 2020 2020 200d 0a20 2020 2023 2054         ..    # T
+0001ad60: 5a59 5820 7368 6170 6564 206f 626a 6563  ZYX shaped objec
+0001ad70: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
+0001ad80: 3d20 343a 0d0a 2020 2020 2020 2020 7072  = 4:..        pr
+0001ad90: 696e 7428 274d 616b 696e 6720 6d61 736b  int('Making mask
+0001ada0: 2069 6e20 3444 2729 0d0a 2020 2020 2020   in 4D')..      
+0001adb0: 2020 626f 756e 6461 7279 203d 206e 702e    boundary = np.
+0001adc0: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
+0001add0: 2020 2020 5b6d 6173 6b2e 7368 6170 655b      [mask.shape[
+0001ade0: 305d 2c20 6d61 736b 2e73 6861 7065 5b31  0], mask.shape[1
+0001adf0: 5d2c 206d 6173 6b2e 7368 6170 655b 325d  ], mask.shape[2]
+0001ae00: 2c20 6d61 736b 2e73 6861 7065 5b33 5d5d  , mask.shape[3]]
+0001ae10: 2c20 6474 7970 653d 6e70 2e75 696e 7438  , dtype=np.uint8
+0001ae20: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0001ae30: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0001ae40: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
+0001ae50: 655b 305d 293a 0d0a 2020 2020 2020 2020  e[0]):..        
+0001ae60: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0001ae70: 2020 626f 756e 6461 7279 5b69 2c3a 5d20    boundary[i,:] 
+0001ae80: 3d20 6669 6e64 5f62 6f75 6e64 6172 6965  = find_boundarie
+0001ae90: 7328 6d61 736b 5b69 2c3a 5d29 0d0a 2020  s(mask[i,:])..  
+0001aea0: 2020 2020 2020 2020 2020 7265 6769 6f6e            region
+0001aeb0: 6365 6e74 726f 6964 203d 2063 6f6d 7075  centroid = compu
+0001aec0: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
+0001aed0: 6461 7279 5b69 2c3a 5d29 200d 0a20 2020  dary[i,:]) ..   
+0001aee0: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
+0001aef0: 203d 206e 702e 7768 6572 6528 626f 756e   = np.where(boun
+0001af00: 6461 7279 5b69 2c3a 5d20 3e20 3029 0d0a  dary[i,:] > 0)..
+0001af10: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001af20: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
+0001af30: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
+0001af40: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
+0001af50: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
+0001af60: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
+0001af70: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0001af80: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
+0001af90: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
+0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afb0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+0001afc0: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
+0001afd0: 6365 735b 6a5d 5b30 5d20 2a20 7a63 616c  ces[j][0] * zcal
+0001afe0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001aff0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001b000: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+0001b010: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+0001b020: 6a5d 5b31 5d20 2a20 7963 616c 6962 7261  j][1] * ycalibra
+0001b030: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+0001b040: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+0001b050: 6e64 6963 6573 5b6a 5d5b 325d 203d 2072  ndices[j][2] = r
+0001b060: 6561 6c5f 696e 6469 6365 735b 6a5d 5b32  eal_indices[j][2
+0001b070: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
+0001b080: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001b090: 7472 6565 203d 2073 7061 7469 616c 2e63  tree = spatial.c
+0001b0a0: 4b44 5472 6565 2872 6561 6c5f 696e 6469  KDTree(real_indi
+0001b0b0: 6365 7329 0d0a 2020 2020 2020 2020 2020  ces)..          
+0001b0c0: 2020 7469 6d65 645f 6d61 736b 5b73 7472    timed_mask[str
+0001b0d0: 2869 295d 203d 205b 7472 6565 2c20 696e  (i)] = [tree, in
+0001b0e0: 6469 6365 732c 2072 6567 696f 6e63 656e  dices, regioncen
+0001b0f0: 7472 6f69 645d 0d0a 2020 2020 7072 696e  troid]..    prin
+0001b100: 7428 2743 6f6d 7075 7465 6420 7468 6520  t('Computed the 
+0001b110: 626f 756e 6461 7279 2070 6f69 6e74 7327  boundary points'
+0001b120: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
+0001b130: 7469 6d65 645f 6d61 736b 2c20 626f 756e  timed_mask, boun
+0001b140: 6461 7279 2020 2020 2020 2020 0d0a 0d0a  dary        ....
+0001b150: 6465 6620 636f 6d70 7574 655f 6365 6e74  def compute_cent
+0001b160: 726f 6964 2862 696e 6172 795f 696d 6167  roid(binary_imag
+0001b170: 6529 3a0d 0a20 2020 2023 2045 6e73 7572  e):..    # Ensur
+0001b180: 6520 6269 6e61 7279 2069 6d61 6765 2069  e binary image i
+0001b190: 7320 6120 4e75 6d50 7920 6172 7261 790d  s a NumPy array.
+0001b1a0: 0a20 2020 2062 696e 6172 795f 696d 6167  .    binary_imag
+0001b1b0: 6520 3d20 6e70 2e61 7272 6179 2862 696e  e = np.array(bin
+0001b1c0: 6172 795f 696d 6167 6529 0d0a 0d0a 2020  ary_image)....  
+0001b1d0: 2020 7768 6974 655f 7069 7865 6c73 203d    white_pixels =
+0001b1e0: 206e 702e 7768 6572 6528 6269 6e61 7279   np.where(binary
+0001b1f0: 5f69 6d61 6765 203d 3d20 3129 0d0a 2020  _image == 1)..  
+0001b200: 2020 6e75 6d5f 7069 7865 6c73 203d 206c    num_pixels = l
+0001b210: 656e 2877 6869 7465 5f70 6978 656c 735b  en(white_pixels[
+0001b220: 305d 290d 0a0d 0a20 2020 2023 2043 6f6d  0])....    # Com
+0001b230: 7075 7465 2074 6865 2063 656e 7472 6f69  pute the centroi
+0001b240: 6420 6f66 2074 6865 2077 6869 7465 2070  d of the white p
+0001b250: 6978 656c 7320 696e 2074 6865 2062 6f75  ixels in the bou
+0001b260: 6e64 6172 7920 696d 6167 650d 0a20 2020  ndary image..   
+0001b270: 2063 656e 7472 6f69 6420 3d20 6e70 2e7a   centroid = np.z
+0001b280: 6572 6f73 2862 696e 6172 795f 696d 6167  eros(binary_imag
+0001b290: 652e 6e64 696d 290d 0a20 2020 2066 6f72  e.ndim)..    for
+0001b2a0: 2064 696d 2069 6e20 7261 6e67 6528 6269   dim in range(bi
+0001b2b0: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
+0001b2c0: 3a0d 0a20 2020 2020 2020 2063 656e 7472  :..        centr
+0001b2d0: 6f69 645b 6469 6d5d 203d 2077 6869 7465  oid[dim] = white
+0001b2e0: 5f70 6978 656c 735b 6469 6d5d 2e73 756d  _pixels[dim].sum
+0001b2f0: 2829 202f 206e 756d 5f70 6978 656c 730d  () / num_pixels.
+0001b300: 0a0d 0a20 2020 2072 6574 7572 6e20 6365  ...    return ce
+0001b310: 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a 200d  ntroid........ .
+0001b320: 0a0d 0a64 6566 2067 6574 5f63 7376 5f64  ...def get_csv_d
+0001b330: 6174 6128 6373 7629 3a0d 0a0d 0a20 2020  ata(csv):....   
+0001b340: 2020 2020 2064 6174 6173 6574 203d 2070       dataset = p
+0001b350: 642e 7265 6164 5f63 7376 280d 0a20 2020  d.read_csv(..   
+0001b360: 2020 2020 2020 2020 2063 7376 2c20 6465           csv, de
+0001b370: 6c69 6d69 7465 723d 222c 222c 2065 6e63  limiter=",", enc
+0001b380: 6f64 696e 673d 2275 6e69 636f 6465 5f65  oding="unicode_e
+0001b390: 7363 6170 6522 2c20 6c6f 775f 6d65 6d6f  scape", low_memo
+0001b3a0: 7279 3d46 616c 7365 0d0a 2020 2020 2020  ry=False..      
+0001b3b0: 2020 295b 333a 5d0d 0a20 2020 2020 2020    )[3:]..       
+0001b3c0: 2064 6174 6173 6574 5f69 6e64 6578 203d   dataset_index =
+0001b3d0: 2064 6174 6173 6574 2e69 6e64 6578 0d0a   dataset.index..
+0001b3e0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+0001b3f0: 6174 6173 6574 2c20 6461 7461 7365 745f  ataset, dataset_
+0001b400: 696e 6465 780d 0a20 2020 200d 0a64 6566  index..    ..def
+0001b410: 2067 6574 5f73 706f 745f 6461 7461 7365   get_spot_datase
+0001b420: 7428 7370 6f74 5f64 6174 6173 6574 2c20  t(spot_dataset, 
+0001b430: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001b440: 706f 745f 6b65 7973 2c20 7863 616c 6962  pot_keys, xcalib
+0001b450: 7261 7469 6f6e 2c20 7963 616c 6962 7261  ration, ycalibra
+0001b460: 7469 6f6e 2c20 7a63 616c 6962 7261 7469  tion, zcalibrati
+0001b470: 6f6e 2c20 4174 7472 6962 7574 6542 6f78  on, AttributeBox
+0001b480: 6e61 6d65 2c20 6465 7465 6374 696f 6e63  name, detectionc
+0001b490: 6861 6e6e 656c 293a 0d0a 2020 2020 2020  hannel):..      
+0001b4a0: 2020 416c 6c56 616c 7565 7320 3d20 7b7d    AllValues = {}
+0001b4b0: 0d0a 2020 2020 2020 2020 706f 7369 7820  ..        posix 
+0001b4c0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
+0001b4d0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
+0001b4e0: 7822 5d0d 0a20 2020 2020 2020 2070 6f73  x"]..        pos
+0001b4f0: 6979 203d 2074 7261 636b 5f61 6e61 6c79  iy = track_analy
+0001b500: 7369 735f 7370 6f74 5f6b 6579 735b 2270  sis_spot_keys["p
+0001b510: 6f73 6979 225d 0d0a 2020 2020 2020 2020  osiy"]..        
+0001b520: 706f 7369 7a20 3d20 7472 6163 6b5f 616e  posiz = track_an
+0001b530: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001b540: 5b22 706f 7369 7a22 5d0d 0a20 2020 2020  ["posiz"]..     
+0001b550: 2020 2066 7261 6d65 203d 2074 7261 636b     frame = track
+0001b560: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001b570: 6579 735b 2266 7261 6d65 225d 0d0a 2020  eys["frame"]..  
+0001b580: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001b590: 4c6f 6361 7469 6f6e 5820 3d20 280d 0a20  LocationX = (.. 
+0001b5a0: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+0001b5b0: 6461 7461 7365 745b 706f 7369 785d 2e61  dataset[posix].a
+0001b5c0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
+0001b5d0: 2078 6361 6c69 6272 6174 696f 6e0d 0a20   xcalibration.. 
+0001b5e0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
+0001b5f0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
+0001b600: 4c6f 6361 7469 6f6e 5920 3d20 280d 0a20  LocationY = (.. 
+0001b610: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+0001b620: 6461 7461 7365 745b 706f 7369 795d 2e61  dataset[posiy].a
+0001b630: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
+0001b640: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
+0001b650: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
+0001b660: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
+0001b670: 4c6f 6361 7469 6f6e 5a20 3d20 280d 0a20  LocationZ = (.. 
+0001b680: 2020 2020 2020 2020 2020 2073 706f 745f             spot_
+0001b690: 6461 7461 7365 745b 706f 7369 7a5d 2e61  dataset[posiz].a
+0001b6a0: 7374 7970 6528 2266 6c6f 6174 2229 202f  stype("float") /
+0001b6b0: 207a 6361 6c69 6272 6174 696f 6e0d 0a20   zcalibration.. 
+0001b6c0: 2020 2020 2020 2029 2e61 7374 7970 6528         ).astype(
+0001b6d0: 2269 6e74 2229 0d0a 2020 2020 2020 2020  "int")..        
+0001b6e0: 4c6f 6361 7469 6f6e 5420 3d20 2873 706f  LocationT = (spo
+0001b6f0: 745f 6461 7461 7365 745b 6672 616d 655d  t_dataset[frame]
+0001b700: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001b710: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
+0001b720: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
+0001b730: 2020 2020 2069 676e 6f72 655f 7661 6c75       ignore_valu
+0001b740: 6573 203d 205b 7472 6163 6b5f 616e 616c  es = [track_anal
+0001b750: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001b760: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
+0001b770: 2c74 7261 636b 5f61 6e61 6c79 7369 735f  ,track_analysis_
+0001b780: 7370 6f74 5f6b 6579 735b 2274 6f74 616c  spot_keys["total
+0001b790: 5f69 6e74 656e 7369 7479 225d 5d0d 0a20  _intensity"]].. 
+0001b7a0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+0001b7b0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
+0001b7c0: 6973 5f73 706f 745f 6b65 7973 2e69 7465  is_spot_keys.ite
+0001b7d0: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
+0001b7e0: 2020 2020 2020 2020 2069 6620 6465 7465           if dete
+0001b7f0: 6374 696f 6e63 6861 6e6e 656c 203d 3d20  ctionchannel == 
+0001b800: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+0001b810: 2020 2020 2020 2020 2069 6620 6b20 3d3d           if k ==
+0001b820: 2022 6d65 616e 5f69 6e74 656e 7369 7479   "mean_intensity
+0001b830: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
+0001b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b850: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
+0001b860: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001b870: 6579 735b 226d 6561 6e5f 696e 7465 6e73  eys["mean_intens
+0001b880: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
+0001b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8a0: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
+0001b8b0: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
+0001b8c0: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
+0001b8d0: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
+0001b8e0: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001b8f0: 3d3d 2022 746f 7461 6c5f 696e 7465 6e73  == "total_intens
+0001b900: 6974 795f 6368 3222 3a0d 0a20 2020 2020  ity_ch2":..     
+0001b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b920: 2020 2020 2020 7661 6c75 6520 3d20 7472        value = tr
+0001b930: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+0001b940: 745f 6b65 7973 5b22 746f 7461 6c5f 696e  t_keys["total_in
+0001b950: 7465 6e73 6974 7922 5d0d 0a20 2020 2020  tensity"]..     
+0001b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b970: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001b980: 7661 6c75 655d 203d 2073 706f 745f 6461  value] = spot_da
+0001b990: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001b9a0: 2266 6c6f 6174 2229 2020 2020 2020 200d  "float")       .
+0001b9b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b9c0: 2020 2069 6620 7620 6e6f 7420 696e 2069     if v not in i
+0001b9d0: 676e 6f72 655f 7661 6c75 6573 3a0d 0a20  gnore_values:.. 
+0001b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001ba00: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001ba10: 6c6c 5661 6c75 6573 5b76 5d20 3d20 7370  llValues[v] = sp
+0001ba20: 6f74 5f64 6174 6173 6574 5b76 5d2e 6173  ot_dataset[v].as
+0001ba30: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
+0001ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba50: 2020 0d0a 0d0a 2020 2020 2020 2020 416c    ....        Al
+0001ba60: 6c56 616c 7565 735b 706f 7369 785d 203d  lValues[posix] =
+0001ba70: 2072 6f75 6e64 284c 6f63 6174 696f 6e58   round(LocationX
+0001ba80: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
+0001ba90: 5661 6c75 6573 5b70 6f73 6979 5d20 3d20  Values[posiy] = 
+0001baa0: 726f 756e 6428 4c6f 6361 7469 6f6e 592c  round(LocationY,
+0001bab0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+0001bac0: 616c 7565 735b 706f 7369 7a5d 203d 2072  alues[posiz] = r
+0001bad0: 6f75 6e64 284c 6f63 6174 696f 6e5a 2c33  ound(LocationZ,3
+0001bae0: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
+0001baf0: 6c75 6573 5b66 7261 6d65 5d20 3d20 726f  lues[frame] = ro
+0001bb00: 756e 6428 4c6f 6361 7469 6f6e 542c 3329  und(LocationT,3)
+0001bb10: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
+0001bb20: 7574 6569 6473 203d 205b 5d0d 0a20 2020  uteids = []..   
+0001bb30: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001bb40: 732e 6170 7065 6e64 2841 7474 7269 6275  s.append(Attribu
+0001bb50: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
+0001bb60: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
+0001bb70: 656e 616d 6520 696e 2041 6c6c 5661 6c75  ename in AllValu
+0001bb80: 6573 2e6b 6579 7328 293a 0d0a 2020 2020  es.keys():..    
+0001bb90: 2020 2020 2020 2020 2020 4174 7472 6962            Attrib
+0001bba0: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
+0001bbb0: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
+0001bbc0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0001bbd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001bbe0: 2020 7265 7475 726e 2041 7474 7269 6275    return Attribu
+0001bbf0: 7465 6964 732c 2041 6c6c 5661 6c75 6573  teids, AllValues
+0001bc00: 2020 2020 200d 0a20 2020 200d 0a0d 0a64       ..    ....d
+0001bc10: 6566 2067 6574 5f74 7261 636b 5f64 6174  ef get_track_dat
+0001bc20: 6173 6574 2874 7261 636b 5f64 6174 6173  aset(track_datas
+0001bc30: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
+0001bc40: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
+0001bc50: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+0001bc60: 636b 5f6b 6579 732c 2054 7261 636b 4174  ck_keys, TrackAt
+0001bc70: 7472 6962 7574 6542 6f78 6e61 6d65 293a  tributeBoxname):
+0001bc80: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
+0001bc90: 7261 636b 5661 6c75 6573 203d 207b 7d0d  rackValues = {}.
+0001bca0: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
+0001bcb0: 6420 3d20 7472 6163 6b5f 616e 616c 7973  d = track_analys
+0001bcc0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
+0001bcd0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
+0001bce0: 2020 5469 6420 3d20 7472 6163 6b5f 6461    Tid = track_da
+0001bcf0: 7461 7365 745b 7472 6163 6b5f 6964 5d2e  taset[track_id].
+0001bd00: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001bd10: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
+0001bd20: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+0001bd30: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
+0001bd40: 0d0a 2020 2020 2020 0d0a 2020 2020 2020  ..      ..      
+0001bd50: 2020 666f 7220 286b 2c20 7629 2069 6e20    for (k, v) in 
+0001bd60: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
+0001bd70: 7261 636b 5f6b 6579 732e 6974 656d 7328  rack_keys.items(
+0001bd80: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001bd90: 2020 2020 2020 7820 3d20 7472 6163 6b5f        x = track_
+0001bda0: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+0001bdb0: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+0001bdc0: 2020 2020 2020 2020 2020 2020 6d69 6e76              minv
+0001bdd0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
+0001bde0: 2020 2020 2020 2020 2020 2020 206d 6178               max
+0001bdf0: 7661 6c20 3d20 6d61 7828 7829 0d0a 0d0a  val = max(x)....
+0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be10: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
+0001be20: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
+0001be30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001be40: 2020 2020 2020 7820 3d20 7820 2b20 310d        x = x + 1.
+0001be50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001be60: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
+0001be70: 735b 6b5d 203d 2072 6f75 6e64 2878 2c20  s[k] = round(x, 
+0001be80: 3329 0d0a 0d0a 2020 2020 2020 2020 5472  3)....        Tr
+0001be90: 6163 6b41 7474 7269 6275 7465 6964 7320  ackAttributeids 
+0001bea0: 3d20 5b5d 0d0a 2020 2020 2020 2020 5472  = []..        Tr
+0001beb0: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
+0001bec0: 6170 7065 6e64 2854 7261 636b 4174 7472  append(TrackAttr
+0001bed0: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
+0001bee0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
+0001bef0: 6275 7465 6e61 6d65 2069 6e20 7472 6163  butename in trac
+0001bf00: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
+0001bf10: 5f6b 6579 732e 6b65 7973 2829 3a0d 0a20  _keys.keys():.. 
+0001bf20: 2020 2020 2020 2020 2020 2054 7261 636b             Track
+0001bf30: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001bf40: 656e 6428 6174 7472 6962 7574 656e 616d  end(attributenam
+0001bf50: 6529 2020 2020 0d0a 2020 2020 0d0a 2020  e)    ..    ..  
+0001bf60: 2020 2020 2020 7265 7475 726e 2054 7261        return Tra
+0001bf70: 636b 4174 7472 6962 7574 6569 6473 2c20  ckAttributeids, 
+0001bf80: 416c 6c54 7261 636b 5661 6c75 6573 0d0a  AllTrackValues..
+0001bf90: 2020 2020 0d0a 6465 6620 6765 745f 6564      ..def get_ed
+0001bfa0: 6765 735f 6461 7461 7365 7428 6564 6765  ges_dataset(edge
+0001bfb0: 735f 6461 7461 7365 742c 2065 6467 6573  s_dataset, edges
+0001bfc0: 5f64 6174 6173 6574 5f69 6e64 6578 2c20  _dataset_index, 
+0001bfd0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001bfe0: 706f 745f 6b65 7973 2c20 7472 6163 6b5f  pot_keys, track_
+0001bff0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
+0001c000: 6579 7329 3a0d 0a0d 0a20 2020 2020 2020  eys):....       
+0001c010: 2041 6c6c 4564 6765 7356 616c 7565 7320   AllEdgesValues 
+0001c020: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
+0001c030: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
+0001c040: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001c050: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
+0001c060: 2020 2020 2020 2054 6964 203d 2065 6467         Tid = edg
+0001c070: 6573 5f64 6174 6173 6574 5b74 7261 636b  es_dataset[track
+0001c080: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
+0001c090: 6174 2229 0d0a 2020 2020 2020 2020 696e  at")..        in
+0001c0a0: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+0001c0b0: 2854 6964 203d 3d20 3029 0d0a 2020 2020  (Tid == 0)..    
+0001c0c0: 2020 2020 6d61 7874 7261 636b 5f69 6420      maxtrack_id 
+0001c0d0: 3d20 6d61 7828 5469 6429 0d0a 2020 2020  = max(Tid)..    
+0001c0e0: 2020 2020 636f 6e64 6974 696f 6e5f 696e      condition_in
+0001c0f0: 6469 6365 7320 3d20 6564 6765 735f 6461  dices = edges_da
+0001c100: 7461 7365 745f 696e 6465 785b 696e 6469  taset_index[indi
+0001c110: 6365 735d 0d0a 2020 2020 2020 2020 5469  ces]..        Ti
+0001c120: 645b 636f 6e64 6974 696f 6e5f 696e 6469  d[condition_indi
+0001c130: 6365 735d 203d 206d 6178 7472 6163 6b5f  ces] = maxtrack_
+0001c140: 6964 202b 2031 0d0a 2020 2020 2020 2020  id + 1..        
+0001c150: 416c 6c45 6467 6573 5661 6c75 6573 5b74  AllEdgesValues[t
+0001c160: 7261 636b 5f69 645d 203d 2054 6964 0d0a  rack_id] = Tid..
+0001c170: 0d0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
+0001c180: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001c190: 735f 6564 6765 735f 6b65 7973 2e76 616c  s_edges_keys.val
+0001c1a0: 7565 7328 293a 0d0a 0d0a 2020 2020 2020  ues():....      
+0001c1b0: 2020 2020 2020 6966 206b 2021 3d20 7472        if k != tr
+0001c1c0: 6163 6b5f 6964 3a0d 0a20 2020 2020 2020  ack_id:..       
+0001c1d0: 2020 2020 2020 2020 2078 203d 2065 6467           x = edg
+0001c1e0: 6573 5f64 6174 6173 6574 5b6b 5d2e 6173  es_dataset[k].as
+0001c1f0: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
+0001c200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c210: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
+0001c220: 6b5d 203d 2078 2020 200d 0a20 2020 2020  k] = x   ..     
+0001c230: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
+0001c240: 7475 726e 2041 6c6c 4564 6765 7356 616c  turn AllEdgesVal
+0001c250: 7565 7320 2020 0d0a 2020 2020 0d0a 2020  ues   ..    ..  
+0001c260: 2020 2020 200d 0a20 2020 200d 0a64 6566       ..    ..def
+0001c270: 2073 6361 6c65 5f76 616c 7565 2878 2c20   scale_value(x, 
+0001c280: 7363 616c 6520 3d20 3235 3520 2a20 3235  scale = 255 * 25
+0001c290: 3529 3a0d 0a0d 0a0d 0a20 2020 2020 7265  5):......     re
+0001c2a0: 7475 726e 2078 202a 2073 6361 6c65 2020  turn x * scale  
+0001c2b0: 200d 0a20 2020 200d 0a0d 0a0d 0a64 6566   ..    ......def
+0001c2c0: 2070 726f 625f 7369 676d 6f69 6428 7829   prob_sigmoid(x)
+0001c2d0: 3a0d 0a20 2020 2072 6574 7572 6e20 3120  :..    return 1 
+0001c2e0: 2d20 6d61 7468 2e65 7870 282d 7829 0d0a  - math.exp(-x)..
+0001c2f0: 0d0a 0d0a 6465 6620 616e 6775 6c61 725f  ....def angular_
+0001c300: 6368 616e 6765 2876 6563 5f30 2c20 7665  change(vec_0, ve
+0001c310: 635f 3129 3a0d 0a20 2020 2020 2020 200d  c_1):..        .
+0001c320: 0a20 2020 2020 2020 2076 6563 5f30 203d  .        vec_0 =
+0001c330: 2076 6563 5f30 202f 206e 702e 6c69 6e61   vec_0 / np.lina
+0001c340: 6c67 2e6e 6f72 6d28 7665 635f 3029 0d0a  lg.norm(vec_0)..
+0001c350: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
+0001c360: 7665 635f 3120 2f20 6e70 2e6c 696e 616c  vec_1 / np.linal
+0001c370: 672e 6e6f 726d 2876 6563 5f31 290d 0a20  g.norm(vec_1).. 
+0001c380: 2020 2020 2020 2061 6e67 6c65 203d 206e         angle = n
+0001c390: 702e 6172 6363 6f73 286e 702e 636c 6970  p.arccos(np.clip
+0001c3a0: 286e 702e 646f 7428 7665 635f 302c 2076  (np.dot(vec_0, v
+0001c3b0: 6563 5f31 292c 202d 312e 302c 2031 2e30  ec_1), -1.0, 1.0
+0001c3c0: 2929 0d0a 2020 2020 2020 2020 616e 676c  ))..        angl
+0001c3d0: 6520 3d20 616e 676c 6520 2a20 3138 3020  e = angle * 180 
+0001c3e0: 2f20 6e70 2e70 690d 0a20 2020 2020 2020  / np.pi..       
+0001c3f0: 2072 6574 7572 6e20 616e 676c 650d 0a20   return angle.. 
+0001c400: 2020 2020 0d0a 0d0a 6465 6620 6576 616c      ....def eval
+0001c410: 5f62 6f6f 6c28 7661 6c75 6529 3a0d 0a20  _bool(value):.. 
+0001c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c430: 200d 0a20 2020 2020 2020 2069 6620 7661   ..        if va
+0001c440: 6c75 6520 203d 3d20 2754 7275 6527 3a20  lue  == 'True': 
+0001c450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c460: 2020 6469 765f 6b65 7920 3d20 5472 7565    div_key = True
+0001c470: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0001c480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c490: 2064 6976 5f6b 6579 203d 2046 616c 7365   div_key = False
+0001c4a0: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
+0001c4b0: 7572 6e20 6469 765f 6b65 7920 2020 2020  urn div_key     
+0001c4c0: 2020 2020 2020 2020 2020 200d 0a0d 0a64             ....d
+0001c4d0: 6566 2063 6865 636b 5f61 6e64 5f75 7064  ef check_and_upd
+0001c4e0: 6174 655f 6d61 736b 286d 6173 6b2c 696d  ate_mask(mask,im
+0001c4f0: 6167 6529 3a0d 0a20 2020 2020 2020 0d0a  age):..       ..
+0001c500: 2020 2020 2020 2020 6966 206c 656e 286d          if len(m
+0001c510: 6173 6b2e 7368 6170 6529 203c 206c 656e  ask.shape) < len
+0001c520: 2869 6d61 6765 2e73 6861 7065 293a 0d0a  (image.shape):..
+0001c530: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001c540: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
+0001c550: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
+0001c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c570: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
 0001c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c590: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-0001c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5b0: 2020 2069 6d61 6765 2e73 6861 7065 5b30     image.shape[0
-0001c5c0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5e0: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
-0001c5f0: 315d 2c0d 0a20 2020 2020 2020 2020 2020  1],..           
-0001c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c610: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
-0001c620: 5b32 5d2c 0d0a 2020 2020 2020 2020 2020  [2],..          
-0001c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c640: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
-0001c650: 655b 335d 2c0d 0a20 2020 2020 2020 2020  e[3],..         
-0001c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c670: 2020 205d 2c20 6474 7970 653d 2275 696e     ], dtype="uin
-0001c680: 7438 220d 0a20 2020 2020 2020 2020 2020  t8"..           
-0001c690: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0001c6a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001c6b0: 6920 696e 2072 616e 6765 2830 2c20 7570  i in range(0, up
-0001c6c0: 6461 7465 5f6d 6173 6b2e 7368 6170 655b  date_mask.shape[
-0001c6d0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
-0001c6e0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-0001c6f0: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
-0001c700: 6173 6b2e 7368 6170 655b 315d 293a 0d0a  ask.shape[1]):..
-0001c710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001c720: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
-0001c730: 6b5b 692c 206a 2c20 3a2c 203a 5d20 3d20  k[i, j, :, :] = 
-0001c740: 6d61 736b 5b69 2c20 3a2c 203a 5d0d 0a20  mask[i, :, :].. 
-0001c750: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0001c760: 2020 2020 2020 2020 2020 2020 2020 7570                up
-0001c770: 6461 7465 5f6d 6173 6b20 3d20 6d61 736b  date_mask = mask
-0001c780: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-0001c790: 726e 2075 7064 6174 655f 6d61 736b 2020  rn update_mask  
-0001c7a0: 2020 2020 2020 0d0a 2020 2020 2020 200d        ..       .
-0001c7b0: 0a                                       .
+0001c590: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001c5a0: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+0001c5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c5c0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001c5d0: 5b31 5d2c 0d0a 2020 2020 2020 2020 2020  [1],..          
+0001c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c5f0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001c600: 655b 325d 2c0d 0a20 2020 2020 2020 2020  e[2],..         
+0001c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c620: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001c630: 7065 5b33 5d2c 0d0a 2020 2020 2020 2020  pe[3],..        
+0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c650: 2020 2020 5d2c 2064 7479 7065 3d22 7569      ], dtype="ui
+0001c660: 6e74 3822 0d0a 2020 2020 2020 2020 2020  nt8"..          
+0001c670: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001c680: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001c690: 2069 2069 6e20 7261 6e67 6528 302c 2075   i in range(0, u
+0001c6a0: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
+0001c6b0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+0001c6c0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0001c6d0: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
+0001c6e0: 6d61 736b 2e73 6861 7065 5b31 5d29 3a0d  mask.shape[1]):.
+0001c6f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001c700: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
+0001c710: 736b 5b69 2c20 6a2c 203a 2c20 3a5d 203d  sk[i, j, :, :] =
+0001c720: 206d 6173 6b5b 692c 203a 2c20 3a5d 0d0a   mask[i, :, :]..
+0001c730: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001c740: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0001c750: 7064 6174 655f 6d61 736b 203d 206d 6173  pdate_mask = mas
+0001c760: 6b0d 0a0d 0a20 2020 2020 2020 2072 6574  k....        ret
+0001c770: 7572 6e20 7570 6461 7465 5f6d 6173 6b20  urn update_mask 
+0001c780: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001c790: 0d0a                                     ..
```

### Comparing `napatrackmater-3.9.9/napatrackmater/Trackvector.py` & `napatrackmater-4.0.0/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/__init__.py` & `napatrackmater-4.0.0/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/clustering.py` & `napatrackmater-4.0.0/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/fast_radius_regression.py` & `napatrackmater-4.0.0/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/fate_mapping.py` & `napatrackmater-4.0.0/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater/pretrained.py` & `napatrackmater-4.0.0/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-4.0.0/napatrackmater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.9
+Version: 4.0.0
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.9/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-4.0.0/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.9/setup.py` & `napatrackmater-4.0.0/setup.py`

 * *Files identical despite different names*

