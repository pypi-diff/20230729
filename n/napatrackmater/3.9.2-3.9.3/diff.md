# Comparing `tmp/napatrackmater-3.9.2.tar.gz` & `tmp/napatrackmater-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.9.2.tar", last modified: Sat Jul 29 15:27:42 2023, max compression
+gzip compressed data, was "napatrackmater-3.9.3.tar", last modified: Sat Jul 29 16:04:00 2023, max compression
```

## Comparing `napatrackmater-3.9.2.tar` & `napatrackmater-3.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:27:42.524332 napatrackmater-3.9.2/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/LICENSE
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:27:42.524204 napatrackmater-3.9.2/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/README.md
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:27:42.523195 napatrackmater-3.9.2/napatrackmater/
--rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/CloudAutoEncoder.py
--rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/DeepEmbeddedClustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)   114234 2023-07-29 15:27:11.000000 napatrackmater-3.9.2/napatrackmater/Trackmate.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/Trackvector.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/__init__.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/clustering.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/fast_radius_regression.py
--rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/fate_mapping.py
--rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/napatrackmater/pretrained.py
--rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 15:26:54.000000 napatrackmater-3.9.2/napatrackmater/version.py
-drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 15:27:42.523937 napatrackmater-3.9.2/napatrackmater.egg-info/
--rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/PKG-INFO
--rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/SOURCES.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/dependency_links.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/entry_points.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/requires.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 15:27:42.000000 napatrackmater-3.9.2/napatrackmater.egg-info/top_level.txt
--rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 15:27:42.524374 napatrackmater-3.9.2/setup.cfg
--rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.2/setup.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.646534 napatrackmater-3.9.3/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1541 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/LICENSE
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:04:00.646434 napatrackmater-3.9.3/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2276 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/README.md
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.645413 napatrackmater-3.9.3/napatrackmater/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1261 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/CloudAutoEncoder.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)      887 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/DeepEmbeddedClustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)   114170 2023-07-29 16:02:33.000000 napatrackmater-3.9.3/napatrackmater/Trackmate.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    16426 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/Trackvector.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1723 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/__init__.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    14304 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/clustering.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     3675 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/fast_radius_regression.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)    13011 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/fate_mapping.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)     6008 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/napatrackmater/pretrained.py
+-rw-r--r--   0 vkapoor    (503) staff       (20)       25 2023-07-29 16:02:40.000000 napatrackmater-3.9.3/napatrackmater/version.py
+drwxr-xr-x   0 vkapoor    (503) staff       (20)        0 2023-07-29 16:04:00.646270 napatrackmater-3.9.3/napatrackmater.egg-info/
+-rw-r--r--   0 vkapoor    (503) staff       (20)     2833 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/PKG-INFO
+-rw-r--r--   0 vkapoor    (503) staff       (20)      573 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/SOURCES.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)        1 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/dependency_links.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       55 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/entry_points.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)      107 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/requires.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       15 2023-07-29 16:04:00.000000 napatrackmater-3.9.3/napatrackmater.egg-info/top_level.txt
+-rw-r--r--   0 vkapoor    (503) staff       (20)       38 2023-07-29 16:04:00.646569 napatrackmater-3.9.3/setup.cfg
+-rw-r--r--   0 vkapoor    (503) staff       (20)     1427 2023-07-21 10:29:04.000000 napatrackmater-3.9.3/setup.py
```

### Comparing `napatrackmater-3.9.2/LICENSE` & `napatrackmater-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/PKG-INFO` & `napatrackmater-3.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.2
+Version: 3.9.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.2/README.md` & `napatrackmater-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.9.3/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.9.3/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/Trackmate.py` & `napatrackmater-3.9.3/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -2457,4684 +2457,4680 @@
 00009980: 6b65 795d 290d 0a0d 0a20 2020 2020 2020  key])....       
 00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000099a0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
 000099b0: 7265 6e74 5f74 7261 636b 6c65 7473 2c20  rent_tracklets, 
 000099c0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
 000099d0: 735f 7072 6f70 6572 7469 6573 203d 2073  s_properties = s
 000099e0: 656c 662e 5f74 7261 636b 6c65 745f 616e  elf._tracklet_an
-000099f0: 645f 7072 6f70 6572 7469 6573 2861 6c6c  d_properties(all
-00009a00: 5f64 6963 745f 7661 6c75 6573 2c20 742c  _dict_values, t,
-00009a10: 207a 2c20 792c 2078 2c20 6b2c 2063 7572   z, y, x, k, cur
-00009a20: 7265 6e74 5f74 7261 636b 5f69 642c 2075  rent_track_id, u
-00009a30: 6e69 7175 655f 6964 2c20 6375 7272 656e  nique_id, curren
-00009a40: 745f 7472 6163 6b6c 6574 732c 2063 7572  t_tracklets, cur
-00009a50: 7265 6e74 5f74 7261 636b 6c65 7473 5f70  rent_tracklets_p
-00009a60: 726f 7065 7274 6965 7329 0d0a 2020 2020  roperties)..    
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099f0: 645f 7072 6f70 6572 7469 6573 2874 7261  d_properties(tra
+00009a00: 636b 5f69 642c 2061 6c6c 5f64 6963 745f  ck_id, all_dict_
+00009a10: 7661 6c75 6573 2c20 742c 207a 2c20 792c  values, t, z, y,
+00009a20: 2078 2c20 6b2c 2063 7572 7265 6e74 5f74   x, k, current_t
+00009a30: 7261 636b 5f69 642c 2075 6e69 7175 655f  rack_id, unique_
+00009a40: 6964 2c20 6375 7272 656e 745f 7472 6163  id, current_trac
+00009a50: 6b6c 6574 732c 2063 7572 7265 6e74 5f74  klets, current_t
+00009a60: 7261 636b 6c65 7473 5f70 726f 7065 7274  racklets_propert
+00009a70: 6965 7329 0d0a 2020 2020 2020 2020 2020  ies)..          
 00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00009a90: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
 00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009ac0: 7320 3d20 6e70 2e61 7361 7272 6179 2863  s = np.asarray(c
-00009ad0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
-00009ae0: 5b73 7472 2874 7261 636b 5f69 6429 5d2c  [str(track_id)],
-00009af0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00009b00: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00009ab0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009ac0: 745f 7472 6163 6b6c 6574 7320 3d20 6e70  t_tracklets = np
+00009ad0: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00009ae0: 5f74 7261 636b 6c65 7473 5b73 7472 2874  _tracklets[str(t
+00009af0: 7261 636b 5f69 6429 5d2c 2064 7479 7065  rack_id)], dtype
+00009b00: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
 00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b20: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009b30: 735f 7072 6f70 6572 7469 6573 203d 206e  s_properties = n
-00009b40: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00009b50: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
-00009b60: 6572 7469 6573 5b73 7472 2874 7261 636b  erties[str(track
-00009b70: 5f69 6429 5d2c 2064 7479 7065 3d6e 702e  _id)], dtype=np.
-00009b80: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
-00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ba0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bc0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00009bd0: 7472 6163 6b73 5b74 7261 636b 5f69 645d  tracks[track_id]
-00009be0: 203d 2063 7572 7265 6e74 5f74 7261 636b   = current_track
-00009bf0: 6c65 7473 2020 2020 200d 0a20 2020 2020  lets     ..     
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00009c20: 7565 5f74 7261 636b 5f70 726f 7065 7274  ue_track_propert
-00009c30: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00009c40: 6375 7272 656e 745f 7472 6163 6b6c 6574  current_tracklet
-00009c50: 735f 7072 6f70 6572 7469 6573 2020 2020  s_properties    
-00009c60: 0d0a 0d0a 2020 2020 6465 6620 5f74 7261  ....    def _tra
-00009c70: 636b 6c65 745f 616e 645f 7072 6f70 6572  cklet_and_proper
-00009c80: 7469 6573 2873 656c 662c 2061 6c6c 5f64  ties(self, all_d
-00009c90: 6963 745f 7661 6c75 6573 2c20 742c 207a  ict_values, t, z
-00009ca0: 2c20 792c 2078 2c20 6b2c 2063 7572 7265  , y, x, k, curre
-00009cb0: 6e74 5f74 7261 636b 5f69 642c 2075 6e69  nt_track_id, uni
-00009cc0: 7175 655f 6964 2c20 6375 7272 656e 745f  que_id, current_
-00009cd0: 7472 6163 6b6c 6574 732c 2063 7572 7265  tracklets, curre
-00009ce0: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-00009cf0: 7065 7274 6965 7329 3a0d 0a20 2020 2020  perties):..     
-00009d00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 2020 2020 2020 2020 2020 2020 6765 6e5f              gen_
-00009d30: 6964 203d 2069 6e74 2866 6c6f 6174 2861  id = int(float(a
-00009d40: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
-00009d50: 656c 662e 6765 6e65 7261 7469 6f6e 6964  elf.generationid
-00009d60: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00009d90: 6564 203d 2066 6c6f 6174 2861 6c6c 5f64  ed = float(all_d
-00009da0: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
-00009db0: 7370 6565 645f 6b65 795d 290d 0a20 2020  speed_key])..   
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2061 6363 656c 6572 6174 696f 6e20 3d20   acceleration = 
-00009df0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009e00: 616c 7565 735b 7365 6c66 2e61 6363 656c  alues[self.accel
-00009e10: 6572 6174 696f 6e5f 6b65 795d 290d 0a20  eration_key]).. 
-00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e40: 2020 206d 6f74 696f 6e5f 616e 676c 6520     motion_angle 
-00009e50: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-00009e60: 5f76 616c 7565 735b 7365 6c66 2e6d 6f74  _values[self.mot
-00009e70: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
-00009e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ea0: 2020 2020 2072 6164 6961 6c5f 616e 676c       radial_angl
-00009eb0: 6520 3d20 666c 6f61 7428 616c 6c5f 6469  e = float(all_di
-00009ec0: 6374 5f76 616c 7565 735b 7365 6c66 2e72  ct_values[self.r
-00009ed0: 6164 6961 6c5f 616e 676c 655f 6b65 795d  adial_angle_key]
-00009ee0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2020 2020 2020 2072 6164 6975 7320 3d20         radius = 
-00009f10: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
-00009f20: 616c 7565 735b 7365 6c66 2e72 6164 6975  alues[self.radiu
-00009f30: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
-00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f50: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
-00009f60: 756d 655f 7069 7865 6c73 203d 2069 6e74  ume_pixels = int
-00009f70: 2866 6c6f 6174 2861 6c6c 5f64 6963 745f  (float(all_dict_
-00009f80: 7661 6c75 6573 5b73 656c 662e 7175 616c  values[self.qual
-00009f90: 6974 795f 6b65 795d 2929 0d0a 2020 2020  ity_key]))..    
-00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00009b30: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009b40: 6572 7469 6573 203d 206e 702e 6173 6172  erties = np.asar
+00009b50: 7261 7928 6375 7272 656e 745f 7472 6163  ray(current_trac
+00009b60: 6b6c 6574 735f 7072 6f70 6572 7469 6573  klets_properties
+00009b70: 5b73 7472 2874 7261 636b 5f69 6429 5d2c  [str(track_id)],
+00009b80: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00009b90: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009bc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009bd0: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00009be0: 5b74 7261 636b 5f69 645d 203d 2063 7572  [track_id] = cur
+00009bf0: 7265 6e74 5f74 7261 636b 6c65 7473 2020  rent_tracklets  
+00009c00: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00009c30: 636b 5f70 726f 7065 7274 6965 735b 7472  ck_properties[tr
+00009c40: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
+00009c50: 745f 7472 6163 6b6c 6574 735f 7072 6f70  t_tracklets_prop
+00009c60: 6572 7469 6573 2020 2020 0d0a 0d0a 2020  erties    ....  
+00009c70: 2020 6465 6620 5f74 7261 636b 6c65 745f    def _tracklet_
+00009c80: 616e 645f 7072 6f70 6572 7469 6573 2873  and_properties(s
+00009c90: 656c 662c 2074 7261 636b 5f69 642c 2061  elf, track_id, a
+00009ca0: 6c6c 5f64 6963 745f 7661 6c75 6573 2c20  ll_dict_values, 
+00009cb0: 742c 207a 2c20 792c 2078 2c20 6b2c 2063  t, z, y, x, k, c
+00009cc0: 7572 7265 6e74 5f74 7261 636b 5f69 642c  urrent_track_id,
+00009cd0: 2075 6e69 7175 655f 6964 2c20 6375 7272   unique_id, curr
+00009ce0: 656e 745f 7472 6163 6b6c 6574 732c 2063  ent_tracklets, c
+00009cf0: 7572 7265 6e74 5f74 7261 636b 6c65 7473  urrent_tracklets
+00009d00: 5f70 726f 7065 7274 6965 7329 3a0d 0a20  _properties):.. 
+00009d10: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d40: 6765 6e5f 6964 203d 2069 6e74 2866 6c6f  gen_id = int(flo
+00009d50: 6174 2861 6c6c 5f64 6963 745f 7661 6c75  at(all_dict_valu
+00009d60: 6573 5b73 656c 662e 6765 6e65 7261 7469  es[self.generati
+00009d70: 6f6e 6964 5f6b 6579 5d29 290d 0a20 2020  onid_key]))..   
+00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009da0: 2073 7065 6564 203d 2066 6c6f 6174 2861   speed = float(a
+00009db0: 6c6c 5f64 6963 745f 7661 6c75 6573 5b73  ll_dict_values[s
+00009dc0: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
+00009dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
+00009e00: 6e20 3d20 666c 6f61 7428 616c 6c5f 6469  n = float(all_di
+00009e10: 6374 5f76 616c 7565 735b 7365 6c66 2e61  ct_values[self.a
+00009e20: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
+00009e30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
+00009e60: 676c 6520 3d20 666c 6f61 7428 616c 6c5f  gle = float(all_
+00009e70: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
+00009e80: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+00009e90: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00009ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009eb0: 2020 2020 2020 2020 2072 6164 6961 6c5f           radial_
+00009ec0: 616e 676c 6520 3d20 666c 6f61 7428 616c  angle = float(al
+00009ed0: 6c5f 6469 6374 5f76 616c 7565 735b 7365  l_dict_values[se
+00009ee0: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
+00009ef0: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f10: 2020 2020 2020 2020 2020 2072 6164 6975             radiu
+00009f20: 7320 3d20 666c 6f61 7428 616c 6c5f 6469  s = float(all_di
+00009f30: 6374 5f76 616c 7565 735b 7365 6c66 2e72  ct_values[self.r
+00009f40: 6164 6975 735f 6b65 795d 290d 0a20 2020  adius_key])..   
+00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2076 6f6c 756d 655f 7069 7865 6c73 203d   volume_pixels =
+00009f80: 2069 6e74 2866 6c6f 6174 2861 6c6c 5f64   int(float(all_d
+00009f90: 6963 745f 7661 6c75 6573 5b73 656c 662e  ict_values[self.
+00009fa0: 7175 616c 6974 795f 6b65 795d 2929 0d0a  quality_key]))..
 00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 746f 7461 6c5f 696e 7465 6e73 6974 7920  total_intensity 
-00009fd0: 3d20 2066 6c6f 6174 2861 6c6c 5f64 6963  =  float(all_dic
-00009fe0: 745f 7661 6c75 6573 5b73 656c 662e 746f  t_values[self.to
-00009ff0: 7461 6c5f 696e 7465 6e73 6974 795f 6b65  tal_intensity_ke
-0000a000: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a020: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a040: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0000a050: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000a060: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-0000a070: 745f 7661 6c75 6573 5b73 656c 662e 6469  t_values[self.di
-0000a080: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000a090: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-0000a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fd0: 2020 2020 746f 7461 6c5f 696e 7465 6e73      total_intens
+00009fe0: 6974 7920 3d20 2066 6c6f 6174 2861 6c6c  ity =  float(all
+00009ff0: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+0000a000: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
+0000a010: 795f 6b65 795d 290d 0a20 2020 2020 2020  y_key])..       
+0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a060: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
+0000a070: 6d61 736b 203d 2066 6c6f 6174 2861 6c6c  mask = float(all
+0000a080: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
+0000a090: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+0000a0a0: 6d61 736b 5f6b 6579 5d29 0d0a 2020 2020  mask_key])..    
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0e0: 2020 7472 6163 6b5f 6469 7370 6c61 6365    track_displace
-0000a0f0: 6d65 6e74 203d 2066 6c6f 6174 2861 6c6c  ment = float(all
-0000a100: 5f64 6963 745f 7661 6c75 6573 5b73 656c  _dict_values[sel
-0000a110: 662e 6469 7370 6c61 6365 6d65 6e74 5f6b  f.displacement_k
-0000a120: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
-0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a140: 2020 2020 2020 2020 2020 746f 7461 6c5f            total_
-0000a150: 7472 6163 6b5f 6469 7374 616e 6365 203d  track_distance =
-0000a160: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-0000a170: 7661 6c75 6573 5b73 656c 662e 746f 7461  values[self.tota
-0000a180: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
-0000a190: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1b0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
-0000a1c0: 7472 6163 6b5f 6469 7374 616e 6365 203d  track_distance =
-0000a1d0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-0000a1e0: 7661 6c75 6573 5b73 656c 662e 6d61 785f  values[self.max_
-0000a1f0: 6469 7374 616e 6365 5f74 7261 7665 6c65  distance_travele
-0000a200: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a220: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-0000a230: 636b 5f64 7572 6174 696f 6e20 3d20 666c  ck_duration = fl
-0000a240: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
-0000a250: 7565 735b 7365 6c66 2e74 7261 636b 5f64  ues[self.track_d
-0000a260: 7572 6174 696f 6e5f 6b65 795d 290d 0a0d  uration_key])...
-0000a270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000a2c0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
-0000a2d0: 5f6b 6579 2069 6e20 616c 6c5f 6469 6374  _key in all_dict
-0000a2e0: 5f76 616c 7565 732e 6b65 7973 2829 3a0d  _values.keys():.
-0000a2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a310: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
-0000a350: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-0000a360: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
-0000a370: 745f 7661 6c75 6573 5b73 656c 662e 6563  t_values[self.ec
-0000a380: 6365 6e74 7269 6369 7479 5f63 6f6d 705f  centricity_comp_
-0000a390: 6669 7273 746b 6579 5d29 0d0a 2020 2020  firstkey])..    
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3c0: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
-0000a3d0: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
-0000a3e0: 3d20 666c 6f61 7428 616c 6c5f 6469 6374  = float(all_dict
-0000a3f0: 5f76 616c 7565 735b 7365 6c66 2e65 6363  _values[self.ecc
-0000a400: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
-0000a410: 6563 6f6e 646b 6579 5d29 0d0a 2020 2020  econdkey])..    
-0000a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a440: 2020 2020 2020 2073 7572 6661 6365 5f61         surface_a
-0000a450: 7265 6120 3d20 666c 6f61 7428 616c 6c5f  rea = float(all_
-0000a460: 6469 6374 5f76 616c 7565 735b 7365 6c66  dict_values[self
-0000a470: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-0000a480: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4b0: 6365 6c6c 5f61 7869 735f 6d61 736b 203d  cell_axis_mask =
-0000a4c0: 2066 6c6f 6174 2861 6c6c 5f64 6963 745f   float(all_dict_
-0000a4d0: 7661 6c75 6573 5b73 656c 662e 6365 6c6c  values[self.cell
-0000a4e0: 6178 6973 5f6d 6173 6b5f 6b65 795d 290d  axis_mask_key]).
-0000a4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000a0d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0f0: 2020 2020 2020 7472 6163 6b5f 6469 7370        track_disp
+0000a100: 6c61 6365 6d65 6e74 203d 2066 6c6f 6174  lacement = float
+0000a110: 2873 656c 662e 416c 6c54 7261 636b 5661  (self.AllTrackVa
+0000a120: 6c75 6573 5b74 7261 636b 5f69 645d 5b73  lues[track_id][s
+0000a130: 656c 662e 6469 7370 6c61 6365 6d65 6e74  elf.displacement
+0000a140: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+0000a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a160: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+0000a170: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+0000a180: 203d 2066 6c6f 6174 2873 656c 662e 416c   = float(self.Al
+0000a190: 6c54 7261 636b 5661 6c75 6573 5b74 7261  lTrackValues[tra
+0000a1a0: 636b 5f69 645d 5b73 656c 662e 746f 7461  ck_id][self.tota
+0000a1b0: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
+0000a1c0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1e0: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000a1f0: 7472 6163 6b5f 6469 7374 616e 6365 203d  track_distance =
+0000a200: 2066 6c6f 6174 2873 656c 662e 416c 6c54   float(self.AllT
+0000a210: 7261 636b 5661 6c75 6573 5b74 7261 636b  rackValues[track
+0000a220: 5f69 645d 5b73 656c 662e 6d61 785f 6469  _id][self.max_di
+0000a230: 7374 616e 6365 5f74 7261 7665 6c65 645f  stance_traveled_
+0000a240: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 2020 2020 2020 2020 2074 7261 636b             track
+0000a270: 5f64 7572 6174 696f 6e20 3d20 666c 6f61  _duration = floa
+0000a280: 7428 7365 6c66 2e41 6c6c 5472 6163 6b56  t(self.AllTrackV
+0000a290: 616c 7565 735b 7472 6163 6b5f 6964 5d5b  alues[track_id][
+0000a2a0: 7365 6c66 2e74 7261 636b 5f64 7572 6174  self.track_durat
+0000a2b0: 696f 6e5f 6b65 795d 290d 0a0d 0a20 2020  ion_key])....   
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000a310: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
+0000a320: 7920 696e 2061 6c6c 5f64 6963 745f 7661  y in all_dict_va
+0000a330: 6c75 6573 2e6b 6579 7328 293a 0d0a 2020  lues.keys():..  
+0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a360: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
+0000a3a0: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
+0000a3b0: 666c 6f61 7428 616c 6c5f 6469 6374 5f76  float(all_dict_v
+0000a3c0: 616c 7565 735b 7365 6c66 2e65 6363 656e  alues[self.eccen
+0000a3d0: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
+0000a3e0: 7374 6b65 795d 290d 0a20 2020 2020 2020  stkey])..       
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
+0000a420: 5f63 6f6d 705f 7365 636f 6e64 203d 2066  _comp_second = f
+0000a430: 6c6f 6174 2861 6c6c 5f64 6963 745f 7661  loat(all_dict_va
+0000a440: 6c75 6573 5b73 656c 662e 6563 6365 6e74  lues[self.eccent
+0000a450: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+0000a460: 6e64 6b65 795d 290d 0a20 2020 2020 2020  ndkey])..       
+0000a470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+0000a4a0: 203d 2066 6c6f 6174 2861 6c6c 5f64 6963   = float(all_dic
+0000a4b0: 745f 7661 6c75 6573 5b73 656c 662e 7375  t_values[self.su
+0000a4c0: 7266 6163 655f 6172 6561 5f6b 6579 5d29  rface_area_key])
+0000a4d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4f0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000a500: 6c5f 6178 6973 5f6d 6173 6b20 3d20 666c  l_axis_mask = fl
+0000a510: 6f61 7428 616c 6c5f 6469 6374 5f76 616c  oat(all_dict_val
+0000a520: 7565 735b 7365 6c66 2e63 656c 6c61 7869  ues[self.cellaxi
+0000a530: 735f 6d61 736b 5f6b 6579 5d29 0d0a 2020  s_mask_key])..  
+0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000a560: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2020 2020 6563 6365 6e74 7269 6369        eccentrici
-0000a5b0: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
-0000a5c0: 2d31 0d0a 2020 2020 2020 2020 2020 2020  -1..            
+0000a590: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
 0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5f0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000a600: 705f 7365 636f 6e64 203d 202d 310d 0a20  p_second = -1.. 
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+0000a600: 636f 6d70 5f66 6972 7374 203d 202d 310d  comp_first = -1.
+0000a610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a630: 2020 2020 2020 2020 2020 2073 7572 6661             surfa
-0000a640: 6365 5f61 7265 6120 3d20 2d31 0d0a 2020  ce_area = -1..  
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 2020 2020 2020 2020 2020 2020 2065 6363               ecc
+0000a640: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+0000a650: 6563 6f6e 6420 3d20 2d31 0d0a 2020 2020  econd = -1..    
 0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a670: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
-0000a680: 7869 735f 6d61 736b 203d 202d 3120 2020  xis_mask = -1   
-0000a690: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 2020 2020 7375 7266 6163 655f          surface_
+0000a690: 6172 6561 203d 202d 310d 0a20 2020 2020  area = -1..     
 0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6b0: 2020 2020 2020 2020 2020 6672 616d 655f            frame_
-0000a6c0: 7370 6f74 5f63 656e 7472 6f69 6420 3d20  spot_centroid = 
-0000a6d0: 2874 2c72 6f75 6e64 287a 292f 7365 6c66  (t,round(z)/self
-0000a6e0: 2e7a 6361 6c69 6272 6174 696f 6e2c 2072  .zcalibration, r
-0000a6f0: 6f75 6e64 2879 292f 7365 6c66 2e79 6361  ound(y)/self.yca
-0000a700: 6c69 6272 6174 696f 6e2c 2072 6f75 6e64  libration, round
-0000a710: 2878 292f 7365 6c66 2e78 6361 6c69 6272  (x)/self.xcalibr
-0000a720: 6174 696f 6e29 200d 0a20 2020 2020 2020  ation) ..       
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000a750: 662e 756e 6971 7565 5f73 706f 745f 6365  f.unique_spot_ce
-0000a760: 6e74 726f 6964 5b66 7261 6d65 5f73 706f  ntroid[frame_spo
-0000a770: 745f 6365 6e74 726f 6964 5d20 3d20 6b0d  t_centroid] = k.
-0000a780: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7a0: 2020 2020 2020 2069 6620 6375 7272 656e         if curren
-0000a7b0: 745f 7472 6163 6b5f 6964 2069 6e20 6375  t_track_id in cu
-0000a7c0: 7272 656e 745f 7472 6163 6b6c 6574 733a  rrent_tracklets:
-0000a7d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+0000a6d0: 5f6d 6173 6b20 3d20 2d31 2020 2020 200d  _mask = -1     .
+0000a6e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 2066 7261 6d65 5f73 706f         frame_spo
+0000a710: 745f 6365 6e74 726f 6964 203d 2028 742c  t_centroid = (t,
+0000a720: 726f 756e 6428 7a29 2f73 656c 662e 7a63  round(z)/self.zc
+0000a730: 616c 6962 7261 7469 6f6e 2c20 726f 756e  alibration, roun
+0000a740: 6428 7929 2f73 656c 662e 7963 616c 6962  d(y)/self.ycalib
+0000a750: 7261 7469 6f6e 2c20 726f 756e 6428 7829  ration, round(x)
+0000a760: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
+0000a770: 6f6e 2920 0d0a 2020 2020 2020 2020 2020  on) ..          
+0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a790: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000a7a0: 6e69 7175 655f 7370 6f74 5f63 656e 7472  nique_spot_centr
+0000a7b0: 6f69 645b 6672 616d 655f 7370 6f74 5f63  oid[frame_spot_c
+0000a7c0: 656e 7472 6f69 645d 203d 206b 0d0a 0d0a  entroid] = k....
+0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7f0: 2020 2020 2020 2020 2020 7472 6163 6b6c            trackl
-0000a800: 6574 5f61 7272 6179 203d 2063 7572 7265  et_array = curre
-0000a810: 6e74 5f74 7261 636b 6c65 7473 5b63 7572  nt_tracklets[cur
-0000a820: 7265 6e74 5f74 7261 636b 5f69 645d 0d0a  rent_track_id]..
+0000a7f0: 2020 2020 6966 2063 7572 7265 6e74 5f74      if current_t
+0000a800: 7261 636b 5f69 6420 696e 2063 7572 7265  rack_id in curre
+0000a810: 6e74 5f74 7261 636b 6c65 7473 3a0d 0a20  nt_tracklets:.. 
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a850: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-0000a860: 7472 6163 6b6c 6574 5f61 7272 6179 203d  tracklet_array =
-0000a870: 206e 702e 6172 7261 7928 5b69 6e74 2866   np.array([int(f
-0000a880: 6c6f 6174 2875 6e69 7175 655f 6964 2929  loat(unique_id))
-0000a890: 2c20 742c 207a 2f73 656c 662e 7a63 616c  , t, z/self.zcal
-0000a8a0: 6962 7261 7469 6f6e 2c20 792f 7365 6c66  ibration, y/self
-0000a8b0: 2e79 6361 6c69 6272 6174 696f 6e2c 2078  .ycalibration, x
-0000a8c0: 2f73 656c 662e 7863 616c 6962 7261 7469  /self.xcalibrati
-0000a8d0: 6f6e 5d29 0d0a 2020 2020 2020 2020 2020  on])..          
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8f0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000a900: 7272 656e 745f 7472 6163 6b6c 6574 735b  rrent_tracklets[
-0000a910: 6375 7272 656e 745f 7472 6163 6b5f 6964  current_track_id
-0000a920: 5d20 3d20 6e70 2e76 7374 6163 6b28 2874  ] = np.vstack((t
-0000a930: 7261 636b 6c65 745f 6172 7261 792c 2063  racklet_array, c
-0000a940: 7572 7265 6e74 5f74 7261 636b 6c65 745f  urrent_tracklet_
-0000a950: 6172 7261 7929 290d 0a0d 0a20 2020 2020  array))....     
-0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a980: 2020 2076 616c 7565 5f61 7272 6179 203d     value_array =
-0000a990: 2063 7572 7265 6e74 5f74 7261 636b 6c65   current_trackle
-0000a9a0: 7473 5f70 726f 7065 7274 6965 735b 6375  ts_properties[cu
-0000a9b0: 7272 656e 745f 7472 6163 6b5f 6964 5d0d  rrent_track_id].
-0000a9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000a9f0: 5f76 616c 7565 5f61 7272 6179 203d 206e  _value_array = n
-0000aa00: 702e 6172 7261 7928 5b74 2c20 696e 7428  p.array([t, int(
-0000aa10: 666c 6f61 7428 756e 6971 7565 5f69 6429  float(unique_id)
-0000aa20: 292c 2067 656e 5f69 642c 2072 6164 6975  ), gen_id, radiu
-0000aa30: 732c 2076 6f6c 756d 655f 7069 7865 6c73  s, volume_pixels
-0000aa40: 2c20 6563 6365 6e74 7269 6369 7479 5f63  , eccentricity_c
-0000aa50: 6f6d 705f 6669 7273 742c 2065 6363 656e  omp_first, eccen
-0000aa60: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-0000aa70: 6f6e 642c 2073 7572 6661 6365 5f61 7265  ond, surface_are
-0000aa80: 612c 2074 6f74 616c 5f69 6e74 656e 7369  a, total_intensi
-0000aa90: 7479 2c20 7370 6565 642c 206d 6f74 696f  ty, speed, motio
-0000aaa0: 6e5f 616e 676c 652c 2061 6363 656c 6572  n_angle, acceler
-0000aab0: 6174 696f 6e2c 2064 6973 7461 6e63 655f  ation, distance_
-0000aac0: 6365 6c6c 5f6d 6173 6b2c 2072 6164 6961  cell_mask, radia
-0000aad0: 6c5f 616e 676c 652c 2063 656c 6c5f 6178  l_angle, cell_ax
-0000aae0: 6973 5f6d 6173 6b2c 2074 7261 636b 5f64  is_mask, track_d
-0000aaf0: 6973 706c 6163 656d 656e 742c 746f 7461  isplacement,tota
-0000ab00: 6c5f 7472 6163 6b5f 6469 7374 616e 6365  l_track_distance
-0000ab10: 2c6d 6178 5f74 7261 636b 5f64 6973 7461  ,max_track_dista
-0000ab20: 6e63 652c 2074 7261 636b 5f64 7572 6174  nce, track_durat
-0000ab30: 696f 6e5d 290d 0a20 2020 2020 2020 2020  ion])..         
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000ab60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-0000ab90: 5f74 7261 636b 6c65 7473 5f70 726f 7065  _tracklets_prope
-0000aba0: 7274 6965 735b 6375 7272 656e 745f 7472  rties[current_tr
-0000abb0: 6163 6b5f 6964 5d20 3d20 6e70 2e76 7374  ack_id] = np.vst
-0000abc0: 6163 6b28 2876 616c 7565 5f61 7272 6179  ack((value_array
-0000abd0: 2c20 6375 7272 656e 745f 7661 6c75 655f  , current_value_
-0000abe0: 6172 7261 7929 290d 0a0d 0a20 2020 2020  array))....     
-0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000ac10: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000ac40: 7272 656e 745f 7472 6163 6b6c 6574 5f61  rrent_tracklet_a
-0000ac50: 7272 6179 203d 206e 702e 6172 7261 7928  rray = np.array(
-0000ac60: 5b69 6e74 2866 6c6f 6174 2875 6e69 7175  [int(float(uniqu
-0000ac70: 655f 6964 2929 2c20 742c 207a 2f73 656c  e_id)), t, z/sel
-0000ac80: 662e 7a63 616c 6962 7261 7469 6f6e 2c20  f.zcalibration, 
-0000ac90: 792f 7365 6c66 2e79 6361 6c69 6272 6174  y/self.ycalibrat
-0000aca0: 696f 6e2c 2078 2f73 656c 662e 7863 616c  ion, x/self.xcal
-0000acb0: 6962 7261 7469 6f6e 5d29 0d0a 2020 2020  ibration])..    
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ace0: 2020 2020 6375 7272 656e 745f 7472 6163      current_trac
-0000acf0: 6b6c 6574 735b 6375 7272 656e 745f 7472  klets[current_tr
-0000ad00: 6163 6b5f 6964 5d20 3d20 6375 7272 656e  ack_id] = curren
-0000ad10: 745f 7472 6163 6b6c 6574 5f61 7272 6179  t_tracklet_array
-0000ad20: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-0000ad50: 7265 6e74 5f76 616c 7565 5f61 7272 6179  rent_value_array
-0000ad60: 203d 206e 702e 6172 7261 7928 5b74 2c20   = np.array([t, 
-0000ad70: 696e 7428 666c 6f61 7428 756e 6971 7565  int(float(unique
-0000ad80: 5f69 6429 292c 2067 656e 5f69 642c 2072  _id)), gen_id, r
-0000ad90: 6164 6975 732c 2076 6f6c 756d 655f 7069  adius, volume_pi
-0000ada0: 7865 6c73 2c20 2065 6363 656e 7472 6963  xels,  eccentric
-0000adb0: 6974 795f 636f 6d70 5f66 6972 7374 2c20  ity_comp_first, 
-0000adc0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000add0: 705f 7365 636f 6e64 2c20 7375 7266 6163  p_second, surfac
-0000ade0: 655f 6172 6561 2c20 2074 6f74 616c 5f69  e_area,  total_i
-0000adf0: 6e74 656e 7369 7479 2c20 7370 6565 642c  ntensity, speed,
-0000ae00: 206d 6f74 696f 6e5f 616e 676c 652c 2061   motion_angle, a
-0000ae10: 6363 656c 6572 6174 696f 6e2c 2064 6973  cceleration, dis
-0000ae20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
-0000ae30: 2072 6164 6961 6c5f 616e 676c 652c 2063   radial_angle, c
-0000ae40: 656c 6c5f 6178 6973 5f6d 6173 6b2c 2074  ell_axis_mask, t
-0000ae50: 7261 636b 5f64 6973 706c 6163 656d 656e  rack_displacemen
-0000ae60: 742c 746f 7461 6c5f 7472 6163 6b5f 6469  t,total_track_di
-0000ae70: 7374 616e 6365 2c6d 6178 5f74 7261 636b  stance,max_track
-0000ae80: 5f64 6973 7461 6e63 652c 2074 7261 636b  _distance, track
-0000ae90: 5f64 7572 6174 696f 6e5d 290d 0a20 2020  _duration])..   
-0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
-0000aed0: 636b 6c65 7473 5f70 726f 7065 7274 6965  cklets_propertie
-0000aee0: 735b 6375 7272 656e 745f 7472 6163 6b5f  s[current_track_
-0000aef0: 6964 5d20 3d20 6375 7272 656e 745f 7661  id] = current_va
-0000af00: 6c75 655f 6172 7261 790d 0a0d 0a20 2020  lue_array....   
-0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af30: 2072 6574 7572 6e20 6375 7272 656e 745f   return current_
-0000af40: 7472 6163 6b6c 6574 732c 2063 7572 7265  tracklets, curre
-0000af50: 6e74 5f74 7261 636b 6c65 7473 5f70 726f  nt_tracklets_pro
-0000af60: 7065 7274 6965 7320 2020 2020 0d0a 0d0a  perties     ....
-0000af70: 2020 2020 6465 6620 5f6d 6173 7465 725f      def _master_
-0000af80: 7370 6f74 5f63 6f6d 7075 7465 7228 7365  spot_computer(se
-0000af90: 6c66 2c20 6672 616d 6529 3a0d 0a20 2020  lf, frame):..   
-0000afa0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000afb0: 2020 2066 6f72 2053 706f 746f 626a 6563     for Spotobjec
-0000afc0: 7420 696e 2066 7261 6d65 2e66 696e 6461  t in frame.finda
-0000afd0: 6c6c 2827 5370 6f74 2729 3a0d 0a20 2020  ll('Spot'):..   
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b000: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-0000b010: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-0000b020: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b030: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
-0000b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b050: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000b060: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b070: 2073 656c 662e 756e 6971 7565 6964 5f6b   self.uniqueid_k
-0000b080: 6579 2069 6e20 5370 6f74 6f62 6a65 6374  ey in Spotobject
-0000b090: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0d0: 2020 2020 7261 6469 7573 203d 2066 6c6f      radius = flo
-0000b0e0: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000b0f0: 7428 7365 6c66 2e72 6164 6975 735f 6b65  t(self.radius_ke
-0000b100: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000a840: 2020 2020 2020 2074 7261 636b 6c65 745f         tracklet_
+0000a850: 6172 7261 7920 3d20 6375 7272 656e 745f  array = current_
+0000a860: 7472 6163 6b6c 6574 735b 6375 7272 656e  tracklets[curren
+0000a870: 745f 7472 6163 6b5f 6964 5d0d 0a20 2020  t_track_id]..   
+0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 2020 2063 7572 7265 6e74 5f74 7261       current_tra
+0000a8b0: 636b 6c65 745f 6172 7261 7920 3d20 6e70  cklet_array = np
+0000a8c0: 2e61 7272 6179 285b 696e 7428 666c 6f61  .array([int(floa
+0000a8d0: 7428 756e 6971 7565 5f69 6429 292c 2074  t(unique_id)), t
+0000a8e0: 2c20 7a2f 7365 6c66 2e7a 6361 6c69 6272  , z/self.zcalibr
+0000a8f0: 6174 696f 6e2c 2079 2f73 656c 662e 7963  ation, y/self.yc
+0000a900: 616c 6962 7261 7469 6f6e 2c20 782f 7365  alibration, x/se
+0000a910: 6c66 2e78 6361 6c69 6272 6174 696f 6e5d  lf.xcalibration]
+0000a920: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0000a950: 6e74 5f74 7261 636b 6c65 7473 5b63 7572  nt_tracklets[cur
+0000a960: 7265 6e74 5f74 7261 636b 5f69 645d 203d  rent_track_id] =
+0000a970: 206e 702e 7673 7461 636b 2828 7472 6163   np.vstack((trac
+0000a980: 6b6c 6574 5f61 7272 6179 2c20 6375 7272  klet_array, curr
+0000a990: 656e 745f 7472 6163 6b6c 6574 5f61 7272  ent_tracklet_arr
+0000a9a0: 6179 2929 0d0a 0d0a 2020 2020 2020 2020  ay))....        
+0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 7661 6c75 655f 6172 7261 7920 3d20 6375  value_array = cu
+0000a9e0: 7272 656e 745f 7472 6163 6b6c 6574 735f  rrent_tracklets_
+0000a9f0: 7072 6f70 6572 7469 6573 5b63 7572 7265  properties[curre
+0000aa00: 6e74 5f74 7261 636b 5f69 645d 0d0a 2020  nt_track_id]..  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa30: 2020 2020 2020 6375 7272 656e 745f 7661        current_va
+0000aa40: 6c75 655f 6172 7261 7920 3d20 6e70 2e61  lue_array = np.a
+0000aa50: 7272 6179 285b 742c 2069 6e74 2866 6c6f  rray([t, int(flo
+0000aa60: 6174 2875 6e69 7175 655f 6964 2929 2c20  at(unique_id)), 
+0000aa70: 6765 6e5f 6964 2c20 7261 6469 7573 2c20  gen_id, radius, 
+0000aa80: 766f 6c75 6d65 5f70 6978 656c 732c 2065  volume_pixels, e
+0000aa90: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+0000aaa0: 5f66 6972 7374 2c20 6563 6365 6e74 7269  _first, eccentri
+0000aab0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+0000aac0: 2c20 7375 7266 6163 655f 6172 6561 2c20  , surface_area, 
+0000aad0: 746f 7461 6c5f 696e 7465 6e73 6974 792c  total_intensity,
+0000aae0: 2073 7065 6564 2c20 6d6f 7469 6f6e 5f61   speed, motion_a
+0000aaf0: 6e67 6c65 2c20 6163 6365 6c65 7261 7469  ngle, accelerati
+0000ab00: 6f6e 2c20 6469 7374 616e 6365 5f63 656c  on, distance_cel
+0000ab10: 6c5f 6d61 736b 2c20 7261 6469 616c 5f61  l_mask, radial_a
+0000ab20: 6e67 6c65 2c20 6365 6c6c 5f61 7869 735f  ngle, cell_axis_
+0000ab30: 6d61 736b 2c74 7261 636b 5f64 6973 706c  mask,track_displ
+0000ab40: 6163 656d 656e 742c 2074 6f74 616c 5f74  acement, total_t
+0000ab50: 7261 636b 5f64 6973 7461 6e63 652c 206d  rack_distance, m
+0000ab60: 6178 5f74 7261 636b 5f64 6973 7461 6e63  ax_track_distanc
+0000ab70: 652c 2074 7261 636b 5f64 7572 6174 696f  e, track_duratio
+0000ab80: 6e20 5d29 0d0a 2020 2020 2020 2020 2020  n ])..          
+0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aba0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+0000abe0: 7472 6163 6b6c 6574 735f 7072 6f70 6572  tracklets_proper
+0000abf0: 7469 6573 5b63 7572 7265 6e74 5f74 7261  ties[current_tra
+0000ac00: 636b 5f69 645d 203d 206e 702e 7673 7461  ck_id] = np.vsta
+0000ac10: 636b 2828 7661 6c75 655f 6172 7261 792c  ck((value_array,
+0000ac20: 2063 7572 7265 6e74 5f76 616c 7565 5f61   current_value_a
+0000ac30: 7272 6179 2929 0d0a 0d0a 2020 2020 2020  rray))....      
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000ac60: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac80: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0000ac90: 7265 6e74 5f74 7261 636b 6c65 745f 6172  rent_tracklet_ar
+0000aca0: 7261 7920 3d20 6e70 2e61 7272 6179 285b  ray = np.array([
+0000acb0: 696e 7428 666c 6f61 7428 756e 6971 7565  int(float(unique
+0000acc0: 5f69 6429 292c 2074 2c20 7a2f 7365 6c66  _id)), t, z/self
+0000acd0: 2e7a 6361 6c69 6272 6174 696f 6e2c 2079  .zcalibration, y
+0000ace0: 2f73 656c 662e 7963 616c 6962 7261 7469  /self.ycalibrati
+0000acf0: 6f6e 2c20 782f 7365 6c66 2e78 6361 6c69  on, x/self.xcali
+0000ad00: 6272 6174 696f 6e5d 290d 0a20 2020 2020  bration])..     
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 2063 7572 7265 6e74 5f74 7261 636b     current_track
+0000ad40: 6c65 7473 5b63 7572 7265 6e74 5f74 7261  lets[current_tra
+0000ad50: 636b 5f69 645d 203d 2063 7572 7265 6e74  ck_id] = current
+0000ad60: 5f74 7261 636b 6c65 745f 6172 7261 7920  _tracklet_array 
+0000ad70: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad90: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+0000ada0: 656e 745f 7661 6c75 655f 6172 7261 7920  ent_value_array 
+0000adb0: 3d20 6e70 2e61 7272 6179 285b 742c 2069  = np.array([t, i
+0000adc0: 6e74 2866 6c6f 6174 2875 6e69 7175 655f  nt(float(unique_
+0000add0: 6964 2929 2c20 6765 6e5f 6964 2c20 7261  id)), gen_id, ra
+0000ade0: 6469 7573 2c20 766f 6c75 6d65 5f70 6978  dius, volume_pix
+0000adf0: 656c 732c 2020 6563 6365 6e74 7269 6369  els,  eccentrici
+0000ae00: 7479 5f63 6f6d 705f 6669 7273 742c 2065  ty_comp_first, e
+0000ae10: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
+0000ae20: 5f73 6563 6f6e 642c 2073 7572 6661 6365  _second, surface
+0000ae30: 5f61 7265 612c 2020 746f 7461 6c5f 696e  _area,  total_in
+0000ae40: 7465 6e73 6974 792c 2073 7065 6564 2c20  tensity, speed, 
+0000ae50: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6163  motion_angle, ac
+0000ae60: 6365 6c65 7261 7469 6f6e 2c20 6469 7374  celeration, dist
+0000ae70: 616e 6365 5f63 656c 6c5f 6d61 736b 2c20  ance_cell_mask, 
+0000ae80: 7261 6469 616c 5f61 6e67 6c65 2c20 6365  radial_angle, ce
+0000ae90: 6c6c 5f61 7869 735f 6d61 736b 2c74 7261  ll_axis_mask,tra
+0000aea0: 636b 5f64 6973 706c 6163 656d 656e 742c  ck_displacement,
+0000aeb0: 2074 6f74 616c 5f74 7261 636b 5f64 6973   total_track_dis
+0000aec0: 7461 6e63 652c 206d 6178 5f74 7261 636b  tance, max_track
+0000aed0: 5f64 6973 7461 6e63 652c 2074 7261 636b  _distance, track
+0000aee0: 5f64 7572 6174 696f 6e20 5d29 0d0a 2020  _duration ])..  
+0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 6375 7272 656e 745f 7472        current_tr
+0000af20: 6163 6b6c 6574 735f 7072 6f70 6572 7469  acklets_properti
+0000af30: 6573 5b63 7572 7265 6e74 5f74 7261 636b  es[current_track
+0000af40: 5f69 645d 203d 2063 7572 7265 6e74 5f76  _id] = current_v
+0000af50: 616c 7565 5f61 7272 6179 0d0a 0d0a 2020  alue_array....  
+0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af80: 2020 7265 7475 726e 2063 7572 7265 6e74    return current
+0000af90: 5f74 7261 636b 6c65 7473 2c20 6375 7272  _tracklets, curr
+0000afa0: 656e 745f 7472 6163 6b6c 6574 735f 7072  ent_tracklets_pr
+0000afb0: 6f70 6572 7469 6573 2020 2020 200d 0a0d  operties     ...
+0000afc0: 0a20 2020 2064 6566 205f 6d61 7374 6572  .    def _master
+0000afd0: 5f73 706f 745f 636f 6d70 7574 6572 2873  _spot_computer(s
+0000afe0: 656c 662c 2066 7261 6d65 293a 0d0a 2020  elf, frame):..  
+0000aff0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000b000: 2020 2020 666f 7220 5370 6f74 6f62 6a65      for Spotobje
+0000b010: 6374 2069 6e20 6672 616d 652e 6669 6e64  ct in frame.find
+0000b020: 616c 6c28 2753 706f 7427 293a 0d0a 2020  all('Spot'):..  
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b040: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000b060: 656c 6c5f 6964 203d 2069 6e74 2853 706f  ell_id = int(Spo
+0000b070: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b080: 2e73 706f 7469 645f 6b65 7929 290d 0a20  .spotid_key)).. 
+0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b0c0: 6620 7365 6c66 2e75 6e69 7175 6569 645f  f self.uniqueid_
+0000b0d0: 6b65 7920 696e 2053 706f 746f 626a 6563  key in Spotobjec
+0000b0e0: 742e 6b65 7973 2829 3a0d 0a20 2020 2020  t.keys():..     
+0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b100: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b120: 2020 2020 2071 7561 6c69 7479 203d 2066       quality = f
-0000b130: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000b140: 6765 7428 7365 6c66 2e71 7561 6c69 7479  get(self.quality
-0000b150: 5f6b 6579 2929 0d0a 2020 2020 2020 2020  _key))..        
+0000b120: 2020 2020 2072 6164 6975 7320 3d20 666c       radius = fl
+0000b130: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000b140: 6574 2873 656c 662e 7261 6469 7573 5f6b  et(self.radius_k
+0000b150: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b170: 2020 2020 2020 2020 746f 7461 6c5f 696e          total_in
-0000b180: 7465 6e73 6974 7920 3d20 666c 6f61 7428  tensity = float(
-0000b190: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000b1a0: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000b1b0: 6974 795f 6b65 7929 290d 0a20 2020 2020  ity_key))..     
-0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1d0: 2020 2020 2020 2020 2020 206d 6561 6e5f             mean_
-0000b1e0: 696e 7465 6e73 6974 7920 3d20 666c 6f61  intensity = floa
-0000b1f0: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000b200: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
-0000b210: 7369 7479 5f6b 6579 2929 0d0a 0d0a 2020  sity_key))....  
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b240: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-0000b250: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-0000b260: 645d 203d 207b 0d0a 2020 2020 2020 2020  d] = {..        
+0000b170: 2020 2020 2020 7175 616c 6974 7920 3d20        quality = 
+0000b180: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000b190: 2e67 6574 2873 656c 662e 7175 616c 6974  .get(self.qualit
+0000b1a0: 795f 6b65 7929 290d 0a20 2020 2020 2020  y_key))..       
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 2020 2020 2020 2020 2074 6f74 616c 5f69           total_i
+0000b1d0: 6e74 656e 7369 7479 203d 2066 6c6f 6174  ntensity = float
+0000b1e0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000b1f0: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000b200: 7369 7479 5f6b 6579 2929 0d0a 2020 2020  sity_key))..    
+0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2020 2020 2020 2020 2020 2020 6d65 616e              mean
+0000b230: 5f69 6e74 656e 7369 7479 203d 2066 6c6f  _intensity = flo
+0000b240: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000b250: 7428 7365 6c66 2e6d 6561 6e5f 696e 7465  t(self.mean_inte
+0000b260: 6e73 6974 795f 6b65 7929 290d 0a0d 0a20  nsity_key)).... 
 0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b280: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b290: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
-0000b2a0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000b2b0: 742e 6765 7428 7365 6c66 2e73 706f 7469  t.get(self.spoti
-0000b2c0: 645f 6b65 7929 2929 2c20 0d0a 2020 2020  d_key))), ..    
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
-0000b300: 203a 2069 6e74 2866 6c6f 6174 2853 706f   : int(float(Spo
-0000b310: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b320: 2e66 7261 6d65 6964 5f6b 6579 2929 292c  .frameid_key))),
-0000b330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b350: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-0000b360: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000b370: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b380: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-0000b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 2020 2073 656c 662e 7970 6f73 6964       self.yposid
-0000b3c0: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
-0000b3d0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b3e0: 2e79 706f 7369 645f 6b65 7929 292c 0d0a  .yposid_key)),..
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b290: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+0000b2a0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+0000b2b0: 6964 5d20 3d20 7b0d 0a20 2020 2020 2020  id] = {..       
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b2e0: 662e 6365 6c6c 6964 5f6b 6579 3a20 696e  f.cellid_key: in
+0000b2f0: 7428 666c 6f61 7428 5370 6f74 6f62 6a65  t(float(Spotobje
+0000b300: 6374 2e67 6574 2873 656c 662e 7370 6f74  ct.get(self.spot
+0000b310: 6964 5f6b 6579 2929 292c 200d 0a20 2020  id_key))), ..   
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2073 656c 662e 6672 616d 6569 645f 6b65   self.frameid_ke
+0000b350: 7920 3a20 696e 7428 666c 6f61 7428 5370  y : int(float(Sp
+0000b360: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b370: 662e 6672 616d 6569 645f 6b65 7929 2929  f.frameid_key)))
+0000b380: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
+0000b3b0: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
+0000b3c0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b3d0: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000b3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b410: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-0000b420: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000b430: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000b440: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
+0000b400: 2020 2020 2020 7365 6c66 2e79 706f 7369        self.yposi
+0000b410: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
+0000b420: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b430: 662e 7970 6f73 6964 5f6b 6579 2929 2c0d  f.yposid_key)),.
+0000b440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2073 656c 662e 746f 7461 6c5f 696e     self.total_in
-0000b480: 7465 6e73 6974 795f 6b65 7920 3a20 746f  tensity_key : to
-0000b490: 7461 6c5f 696e 7465 6e73 6974 792c 0d0a  tal_intensity,..
+0000b460: 2020 2020 2073 656c 662e 7870 6f73 6964       self.xposid
+0000b470: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000b480: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000b490: 2e78 706f 7369 645f 6b65 7929 292c 0d0a  .xposid_key)),..
 0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4c0: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-0000b4d0: 7465 6e73 6974 795f 6b65 7920 3a20 6d65  tensity_key : me
-0000b4e0: 616e 5f69 6e74 656e 7369 7479 2c0d 0a20  an_intensity,.. 
-0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4c0: 2020 2020 7365 6c66 2e74 6f74 616c 5f69      self.total_i
+0000b4d0: 6e74 656e 7369 7479 5f6b 6579 203a 2074  ntensity_key : t
+0000b4e0: 6f74 616c 5f69 6e74 656e 7369 7479 2c0d  otal_intensity,.
+0000b4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2073 656c 662e 7261 6469 7573 5f6b     self.radius_k
-0000b520: 6579 203a 2072 6164 6975 732c 0d0a 2020  ey : radius,..  
-0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b510: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+0000b520: 6e74 656e 7369 7479 5f6b 6579 203a 206d  ntensity_key : m
+0000b530: 6561 6e5f 696e 7465 6e73 6974 792c 0d0a  ean_intensity,..
 0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-0000b560: 6579 203a 2071 7561 6c69 7479 2c0d 0a20  ey : quality,.. 
-0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b560: 2020 2020 7365 6c66 2e72 6164 6975 735f      self.radius_
+0000b570: 6b65 7920 3a20 7261 6469 7573 2c0d 0a20  key : radius,.. 
 0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b590: 2020 2073 656c 662e 6469 7374 616e 6365     self.distance
-0000b5a0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 3a20  _cell_mask_key: 
-0000b5b0: 2866 6c6f 6174 2853 706f 746f 626a 6563  (float(Spotobjec
-0000b5c0: 742e 6765 7428 7365 6c66 2e64 6973 7461  t.get(self.dista
-0000b5d0: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-0000b5e0: 7929 2929 2c0d 0a20 2020 2020 2020 2020  y))),..         
-0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b610: 756e 6971 7565 6964 5f6b 6579 203a 2073  uniqueid_key : s
-0000b620: 7472 2853 706f 746f 626a 6563 742e 6765  tr(Spotobject.ge
-0000b630: 7428 7365 6c66 2e75 6e69 7175 6569 645f  t(self.uniqueid_
-0000b640: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b670: 2e74 7261 636b 6c65 7469 645f 6b65 7920  .trackletid_key 
-0000b680: 3a20 7374 7228 5370 6f74 6f62 6a65 6374  : str(Spotobject
-0000b690: 2e67 6574 2873 656c 662e 7472 6163 6b6c  .get(self.trackl
-0000b6a0: 6574 6964 5f6b 6579 2929 2c0d 0a20 2020  etid_key)),..   
-0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 2073 656c 662e 6765 6e65 7261 7469 6f6e   self.generation
-0000b6e0: 6964 5f6b 6579 203a 2073 7472 2853 706f  id_key : str(Spo
-0000b6f0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000b700: 2e67 656e 6572 6174 696f 6e69 645f 6b65  .generationid_ke
-0000b710: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b730: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0000b740: 7261 636b 6964 5f6b 6579 203a 2073 7472  rackid_key : str
-0000b750: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000b760: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-0000b770: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-0000b7a0: 7469 6f6e 5f61 6e67 6c65 5f6b 6579 203a  tion_angle_key :
-0000b7b0: 2028 666c 6f61 7428 5370 6f74 6f62 6a65   (float(Spotobje
-0000b7c0: 6374 2e67 6574 2873 656c 662e 6d6f 7469  ct.get(self.moti
-0000b7d0: 6f6e 5f61 6e67 6c65 5f6b 6579 2929 292c  on_angle_key))),
-0000b7e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
-0000b810: 5f6b 6579 203a 2028 666c 6f61 7428 5370  _key : (float(Sp
-0000b820: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000b830: 662e 7370 6565 645f 6b65 7929 2929 2c0d  f.speed_key))),.
-0000b840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2073 656c 662e 6163 6365 6c65       self.accele
-0000b870: 7261 7469 6f6e 5f6b 6579 203a 2028 666c  ration_key : (fl
-0000b880: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000b890: 6574 2873 656c 662e 6163 6365 6c65 7261  et(self.accelera
-0000b8a0: 7469 6f6e 5f6b 6579 2929 292c 0d0a 2020  tion_key))),..  
-0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8d0: 2020 7365 6c66 2e72 6164 6961 6c5f 616e    self.radial_an
-0000b8e0: 676c 655f 6b65 793a 2066 6c6f 6174 2853  gle_key: float(S
-0000b8f0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000b900: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
-0000b910: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b930: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b950: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000b960: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-0000b970: 6b65 7920 696e 2053 706f 746f 626a 6563  key in Spotobjec
-0000b980: 742e 6b65 7973 2829 3a0d 0a20 2020 2020  t.keys():..     
+0000b590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5a0: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+0000b5b0: 6b65 7920 3a20 7175 616c 6974 792c 0d0a  key : quality,..
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 2020 2020 7365 6c66 2e64 6973 7461 6e63      self.distanc
+0000b5f0: 655f 6365 6c6c 5f6d 6173 6b5f 6b65 793a  e_cell_mask_key:
+0000b600: 2028 666c 6f61 7428 5370 6f74 6f62 6a65   (float(Spotobje
+0000b610: 6374 2e67 6574 2873 656c 662e 6469 7374  ct.get(self.dist
+0000b620: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+0000b630: 6579 2929 292c 0d0a 2020 2020 2020 2020  ey))),..        
+0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b660: 2e75 6e69 7175 6569 645f 6b65 7920 3a20  .uniqueid_key : 
+0000b670: 7374 7228 5370 6f74 6f62 6a65 6374 2e67  str(Spotobject.g
+0000b680: 6574 2873 656c 662e 756e 6971 7565 6964  et(self.uniqueid
+0000b690: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b6c0: 662e 7472 6163 6b6c 6574 6964 5f6b 6579  f.trackletid_key
+0000b6d0: 203a 2073 7472 2853 706f 746f 626a 6563   : str(Spotobjec
+0000b6e0: 742e 6765 7428 7365 6c66 2e74 7261 636b  t.get(self.track
+0000b6f0: 6c65 7469 645f 6b65 7929 292c 0d0a 2020  letid_key)),..  
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 7365 6c66 2e67 656e 6572 6174 696f    self.generatio
+0000b730: 6e69 645f 6b65 7920 3a20 7374 7228 5370  nid_key : str(Sp
+0000b740: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000b750: 662e 6765 6e65 7261 7469 6f6e 6964 5f6b  f.generationid_k
+0000b760: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b790: 7472 6163 6b69 645f 6b65 7920 3a20 7374  trackid_key : st
+0000b7a0: 7228 5370 6f74 6f62 6a65 6374 2e67 6574  r(Spotobject.get
+0000b7b0: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
+0000b7c0: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000b7f0: 6f74 696f 6e5f 616e 676c 655f 6b65 7920  otion_angle_key 
+0000b800: 3a20 2866 6c6f 6174 2853 706f 746f 626a  : (float(Spotobj
+0000b810: 6563 742e 6765 7428 7365 6c66 2e6d 6f74  ect.get(self.mot
+0000b820: 696f 6e5f 616e 676c 655f 6b65 7929 2929  ion_angle_key)))
+0000b830: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b850: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
+0000b860: 645f 6b65 7920 3a20 2866 6c6f 6174 2853  d_key : (float(S
+0000b870: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000b880: 6c66 2e73 7065 6564 5f6b 6579 2929 292c  lf.speed_key))),
+0000b890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 2020 2020 7365 6c66 2e61 6363 656c        self.accel
+0000b8c0: 6572 6174 696f 6e5f 6b65 7920 3a20 2866  eration_key : (f
+0000b8d0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
+0000b8e0: 6765 7428 7365 6c66 2e61 6363 656c 6572  get(self.acceler
+0000b8f0: 6174 696f 6e5f 6b65 7929 2929 2c0d 0a20  ation_key))),.. 
+0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b920: 2020 2073 656c 662e 7261 6469 616c 5f61     self.radial_a
+0000b930: 6e67 6c65 5f6b 6579 3a20 666c 6f61 7428  ngle_key: float(
+0000b940: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000b950: 656c 662e 7261 6469 616c 5f61 6e67 6c65  elf.radial_angle
+0000b960: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
+0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b980: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
 0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b9b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-0000b9c0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-0000b9d0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-0000b9e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0000b9a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000b9b0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+0000b9c0: 5f6b 6579 2069 6e20 5370 6f74 6f62 6a65  _key in Spotobje
+0000b9d0: 6374 2e6b 6579 7328 293a 0d0a 2020 2020  ct.keys():..    
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ba40: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-0000ba50: 705f 6669 7273 746b 6579 203a 2066 6c6f  p_firstkey : flo
-0000ba60: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000ba70: 7428 7365 6c66 2e65 6363 656e 7472 6963  t(self.eccentric
-0000ba80: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
-0000ba90: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000baf0: 6c66 2e65 6363 656e 7472 6963 6974 795f  lf.eccentricity_
-0000bb00: 636f 6d70 5f73 6563 6f6e 646b 6579 203a  comp_secondkey :
-0000bb10: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000bb20: 742e 6765 7428 7365 6c66 2e65 6363 656e  t.get(self.eccen
-0000bb30: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-0000bb40: 6f6e 646b 6579 2929 2c0d 0a20 2020 2020  ondkey)),..     
-0000bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bba0: 2020 2073 656c 662e 7375 7266 6163 655f     self.surface_
-0000bbb0: 6172 6561 5f6b 6579 203a 2066 6c6f 6174  area_key : float
-0000bbc0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000bbd0: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
-0000bbe0: 615f 6b65 7929 292c 0d0a 2020 2020 2020  a_key)),..      
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 2020 7365 6c66 2e63 656c 6c61 7869 735f    self.cellaxis_
-0000bc50: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
-0000bc60: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000bc70: 656c 662e 6365 6c6c 6178 6973 5f6d 6173  elf.cellaxis_mas
-0000bc80: 6b5f 6b65 7929 290d 0a20 2020 2020 2020  k_key))..       
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2020 2020 207d 290d 0a20 2020 2020 2020       })..       
+0000ba00: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+0000ba10: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+0000ba20: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+0000ba30: 287b 0d0a 2020 2020 2020 2020 2020 2020  ({..            
+0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ba90: 2e65 6363 656e 7472 6963 6974 795f 636f  .eccentricity_co
+0000baa0: 6d70 5f66 6972 7374 6b65 7920 3a20 666c  mp_firstkey : fl
+0000bab0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
+0000bac0: 6574 2873 656c 662e 6563 6365 6e74 7269  et(self.eccentri
+0000bad0: 6369 7479 5f63 6f6d 705f 6669 7273 746b  city_comp_firstk
+0000bae0: 6579 2929 2c0d 0a20 2020 2020 2020 2020  ey)),..         
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000bb40: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+0000bb50: 5f63 6f6d 705f 7365 636f 6e64 6b65 7920  _comp_secondkey 
+0000bb60: 3a20 666c 6f61 7428 5370 6f74 6f62 6a65  : float(Spotobje
+0000bb70: 6374 2e67 6574 2873 656c 662e 6563 6365  ct.get(self.ecce
+0000bb80: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
+0000bb90: 636f 6e64 6b65 7929 292c 0d0a 2020 2020  condkey)),..    
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbf0: 2020 2020 7365 6c66 2e73 7572 6661 6365      self.surface
+0000bc00: 5f61 7265 615f 6b65 7920 3a20 666c 6f61  _area_key : floa
+0000bc10: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000bc20: 2873 656c 662e 7375 7266 6163 655f 6172  (self.surface_ar
+0000bc30: 6561 5f6b 6579 2929 2c0d 0a20 2020 2020  ea_key)),..     
+0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc90: 2020 2073 656c 662e 6365 6c6c 6178 6973     self.cellaxis
+0000bca0: 5f6d 6173 6b5f 6b65 793a 2066 6c6f 6174  _mask_key: float
+0000bcb0: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000bcc0: 7365 6c66 2e63 656c 6c61 7869 735f 6d61  self.cellaxis_ma
+0000bcd0: 736b 5f6b 6579 2929 0d0a 2020 2020 2020  sk_key))..      
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd40: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000bd30: 2020 2020 2020 7d29 0d0a 2020 2020 2020        })..      
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd60: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bd60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd80: 2020 656c 6966 2073 656c 662e 756e 6971    elif self.uniq
-0000bd90: 7565 6964 5f6b 6579 206e 6f74 2069 6e20  ueid_key not in 
-0000bda0: 5370 6f74 6f62 6a65 6374 2e6b 6579 7328  Spotobject.keys(
-0000bdb0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000be20: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
-0000be30: 6e65 6c20 3d3d 2031 3a0d 0a20 2020 2020  nel == 1:..     
-0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2020 2065 6c69 6620 7365 6c66 2e75 6e69     elif self.uni
+0000bde0: 7175 6569 645f 6b65 7920 6e6f 7420 696e  queid_key not in
+0000bdf0: 2053 706f 746f 626a 6563 742e 6b65 7973   Spotobject.keys
+0000be00: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be30: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000be40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000be70: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000be80: 2053 706f 746f 626a 6563 742e 6765 7428   Spotobject.get(
-0000be90: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
-0000bea0: 7369 7479 5f63 6832 5f6b 6579 290d 0a20  sity_ch2_key).. 
+0000be60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000be70: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
+0000be80: 6e6e 656c 203d 3d20 313a 0d0a 2020 2020  nnel == 1:..    
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 204d 4541 4e5f 494e 5445 4e53 4954     MEAN_INTENSIT
-0000bef0: 5920 3d20 5370 6f74 6f62 6a65 6374 2e67  Y = Spotobject.g
-0000bf00: 6574 2873 656c 662e 6d65 616e 5f69 6e74  et(self.mean_int
-0000bf10: 656e 7369 7479 5f63 6832 5f6b 6579 290d  ensity_ch2_key).
-0000bf20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf40: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000bf50: 653a 2020 2020 2020 2020 0d0a 2020 2020  e:        ..    
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000bed0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
+0000bee0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
+0000bef0: 6e73 6974 795f 6368 325f 6b65 7929 0d0a  nsity_ch2_key)..
+0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf30: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
+0000bf40: 5459 203d 2053 706f 746f 626a 6563 742e  TY = Spotobject.
+0000bf50: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
+0000bf60: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
+0000bf70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
-0000bfa0: 3d20 5370 6f74 6f62 6a65 6374 2e67 6574  = Spotobject.get
-0000bfb0: 2873 656c 662e 746f 7461 6c5f 696e 7465  (self.total_inte
-0000bfc0: 6e73 6974 795f 6368 315f 6b65 7929 0d0a  nsity_ch1_key)..
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000bfa0: 7365 3a20 2020 2020 2020 200d 0a20 2020  se:        ..   
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c000: 2020 2020 4d45 414e 5f49 4e54 454e 5349      MEAN_INTENSI
-0000c010: 5459 203d 2053 706f 746f 626a 6563 742e  TY = Spotobject.
-0000c020: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000c030: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000c040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 2020 2020 2020 2020 2020 5241                RA
-0000c070: 4449 5553 203d 2066 6c6f 6174 2853 706f  DIUS = float(Spo
-0000c080: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000c090: 2e72 6164 6975 735f 6b65 7929 290d 0a20  .radius_key)).. 
+0000bfe0: 2054 4f54 414c 5f49 4e54 454e 5349 5459   TOTAL_INTENSITY
+0000bff0: 203d 2053 706f 746f 626a 6563 742e 6765   = Spotobject.ge
+0000c000: 7428 7365 6c66 2e74 6f74 616c 5f69 6e74  t(self.total_int
+0000c010: 656e 7369 7479 5f63 6831 5f6b 6579 290d  ensity_ch1_key).
+0000c020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c050: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
+0000c060: 4954 5920 3d20 5370 6f74 6f62 6a65 6374  ITY = Spotobject
+0000c070: 2e67 6574 2873 656c 662e 6d65 616e 5f69  .get(self.mean_i
+0000c080: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
+0000c090: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 2020 2020 2051 5541 4c49             QUALI
-0000c0d0: 5459 203d 2066 6c6f 6174 2853 706f 746f  TY = float(Spoto
-0000c0e0: 626a 6563 742e 6765 7428 7365 6c66 2e71  bject.get(self.q
-0000c0f0: 7561 6c69 7479 5f6b 6579 2929 2020 2020  uality_key))    
-0000c100: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000c130: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000c140: 2066 6c6f 6174 2854 4f54 414c 5f49 4e54   float(TOTAL_INT
-0000c150: 454e 5349 5459 290d 0a20 2020 2020 2020  ENSITY)..       
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2052                 R
+0000c0c0: 4144 4955 5320 3d20 666c 6f61 7428 5370  ADIUS = float(Sp
+0000c0d0: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c0e0: 662e 7261 6469 7573 5f6b 6579 2929 0d0a  f.radius_key))..
+0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
+0000c120: 4954 5920 3d20 666c 6f61 7428 5370 6f74  ITY = float(Spot
+0000c130: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
+0000c140: 7175 616c 6974 795f 6b65 7929 2920 2020  quality_key))   
+0000c150: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2020 2020 204d 4541 4e5f 494e 5445 4e53       MEAN_INTENS
-0000c190: 4954 5920 3d20 666c 6f61 7428 4d45 414e  ITY = float(MEAN
-0000c1a0: 5f49 4e54 454e 5349 5459 290d 0a20 2020  _INTENSITY)..   
+0000c180: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000c190: 3d20 666c 6f61 7428 544f 5441 4c5f 494e  = float(TOTAL_IN
+0000c1a0: 5445 4e53 4954 5929 0d0a 2020 2020 2020  TENSITY)..      
 0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-0000c1e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000c1f0: 7469 6573 5b63 656c 6c5f 6964 5d20 3d20  ties[cell_id] = 
-0000c200: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+0000c1d0: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
+0000c1e0: 5349 5459 203d 2066 6c6f 6174 284d 4541  SITY = float(MEA
+0000c1f0: 4e5f 494e 5445 4e53 4954 5929 0d0a 2020  N_INTENSITY)..  
+0000c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c230: 656c 662e 6365 6c6c 6964 5f6b 6579 3a20  elf.cellid_key: 
-0000c240: 696e 7428 6365 6c6c 5f69 6429 2c20 0d0a  int(cell_id), ..
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c220: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0000c230: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000c240: 7274 6965 735b 6365 6c6c 5f69 645d 203d  rties[cell_id] =
+0000c250: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
 0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c280: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
-0000c290: 6e74 2866 6c6f 6174 2853 706f 746f 626a  nt(float(Spotobj
-0000c2a0: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
-0000c2b0: 6d65 6964 5f6b 6579 2929 292c 0d0a 2020  meid_key))),..  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
-0000c2f0: 706f 7369 645f 6b65 7920 3a20 666c 6f61  posid_key : floa
-0000c300: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
-0000c310: 2873 656c 662e 7a70 6f73 6964 5f6b 6579  (self.zposid_key
-0000c320: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
-0000c360: 203a 2066 6c6f 6174 2853 706f 746f 626a   : float(Spotobj
-0000c370: 6563 742e 6765 7428 7365 6c66 2e79 706f  ect.get(self.ypo
-0000c380: 7369 645f 6b65 7929 292c 0d0a 2020 2020  sid_key)),..    
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 7365 6c66 2e63 656c 6c69 645f 6b65 793a  self.cellid_key:
+0000c290: 2069 6e74 2863 656c 6c5f 6964 292c 200d   int(cell_id), .
+0000c2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c2d0: 662e 6672 616d 6569 645f 6b65 7920 3a20  f.frameid_key : 
+0000c2e0: 696e 7428 666c 6f61 7428 5370 6f74 6f62  int(float(Spotob
+0000c2f0: 6a65 6374 2e67 6574 2873 656c 662e 6672  ject.get(self.fr
+0000c300: 616d 6569 645f 6b65 7929 2929 2c0d 0a20  ameid_key))),.. 
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c340: 7a70 6f73 6964 5f6b 6579 203a 2066 6c6f  zposid_key : flo
+0000c350: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
+0000c360: 7428 7365 6c66 2e7a 706f 7369 645f 6b65  t(self.zposid_ke
+0000c370: 7929 292c 0d0a 2020 2020 2020 2020 2020  y)),..          
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
-0000c3c0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-0000c3d0: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
-0000c3e0: 656c 662e 7870 6f73 6964 5f6b 6579 2929  elf.xposid_key))
-0000c3f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c420: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
-0000c430: 6974 795f 6b65 7920 3a20 544f 5441 4c5f  ity_key : TOTAL_
-0000c440: 494e 5445 4e53 4954 592c 0d0a 2020 2020  INTENSITY,..    
+0000c3a0: 2020 7365 6c66 2e79 706f 7369 645f 6b65    self.yposid_ke
+0000c3b0: 7920 3a20 666c 6f61 7428 5370 6f74 6f62  y : float(Spotob
+0000c3c0: 6a65 6374 2e67 6574 2873 656c 662e 7970  ject.get(self.yp
+0000c3d0: 6f73 6964 5f6b 6579 2929 2c0d 0a20 2020  osid_key)),..   
+0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 2073 656c 662e 7870           self.xp
+0000c410: 6f73 6964 5f6b 6579 203a 2066 6c6f 6174  osid_key : float
+0000c420: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
+0000c430: 7365 6c66 2e78 706f 7369 645f 6b65 7929  self.xposid_key)
+0000c440: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c470: 2020 2020 2020 2020 7365 6c66 2e6d 6561          self.mea
-0000c480: 6e5f 696e 7465 6e73 6974 795f 6b65 7920  n_intensity_key 
-0000c490: 3a20 4d45 414e 5f49 4e54 454e 5349 5459  : MEAN_INTENSITY
-0000c4a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000c470: 7365 6c66 2e74 6f74 616c 5f69 6e74 656e  self.total_inten
+0000c480: 7369 7479 5f6b 6579 203a 2054 4f54 414c  sity_key : TOTAL
+0000c490: 5f49 4e54 454e 5349 5459 2c0d 0a20 2020  _INTENSITY,..   
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c4d0: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
-0000c4e0: 2052 4144 4955 532c 0d0a 2020 2020 2020   RADIUS,..      
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4c0: 2020 2020 2020 2020 2073 656c 662e 6d65           self.me
+0000c4d0: 616e 5f69 6e74 656e 7369 7479 5f6b 6579  an_intensity_key
+0000c4e0: 203a 204d 4541 4e5f 494e 5445 4e53 4954   : MEAN_INTENSIT
+0000c4f0: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
 0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 7365 6c66 2e71 7561 6c69        self.quali
-0000c520: 7479 5f6b 6579 203a 2051 5541 4c49 5459  ty_key : QUALITY
-0000c530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c520: 7365 6c66 2e72 6164 6975 735f 6b65 7920  self.radius_key 
+0000c530: 3a20 5241 4449 5553 2c0d 0a20 2020 2020  : RADIUS,..     
 0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
-0000c560: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000c570: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c5a0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
-0000c5b0: 2064 6566 205f 7370 6f74 5f63 6f6d 7075   def _spot_compu
-0000c5c0: 7465 7228 7365 6c66 2c20 6672 616d 6529  ter(self, frame)
-0000c5d0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2066  :....          f
-0000c5e0: 6f72 2053 706f 746f 626a 6563 7420 696e  or Spotobject in
-0000c5f0: 2066 7261 6d65 2e66 696e 6461 6c6c 2827   frame.findall('
-0000c600: 5370 6f74 2729 3a0d 0a20 2020 2020 2020  Spot'):..       
-0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2023 2043 7265 6174 6520 6f62 6a65 6374   # Create object
-0000c630: 2077 6974 6820 756e 6971 7565 2063 656c   with unique cel
-0000c640: 6c20 4944 0d0a 2020 2020 2020 2020 2020  l ID..          
-0000c650: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-0000c660: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-0000c670: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000c680: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6a0: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-0000c6b0: 545a 5958 206c 6f63 6174 696f 6e20 6f66  TZYX location of
-0000c6c0: 2074 6865 2063 656c 6c73 2069 6e20 7468   the cells in th
-0000c6d0: 6174 2066 7261 6d65 0d0a 2020 2020 2020  at frame..      
+0000c550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c560: 2020 2020 2020 2073 656c 662e 7175 616c         self.qual
+0000c570: 6974 795f 6b65 7920 3a20 5155 414c 4954  ity_key : QUALIT
+0000c580: 590d 0a20 2020 2020 2020 2020 2020 2020  Y..             
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+0000c5b0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000c5c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000c5f0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+0000c600: 2020 6465 6620 5f73 706f 745f 636f 6d70    def _spot_comp
+0000c610: 7574 6572 2873 656c 662c 2066 7261 6d65  uter(self, frame
+0000c620: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0000c630: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
+0000c640: 6e20 6672 616d 652e 6669 6e64 616c 6c28  n frame.findall(
+0000c650: 2753 706f 7427 293a 0d0a 2020 2020 2020  'Spot'):..      
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 2020 2320 4372 6561 7465 206f 626a 6563    # Create objec
+0000c680: 7420 7769 7468 2075 6e69 7175 6520 6365  t with unique ce
+0000c690: 6c6c 2049 440d 0a20 2020 2020 2020 2020  ll ID..         
+0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000c6b0: 656c 6c5f 6964 203d 2069 6e74 2853 706f  ell_id = int(Spo
+0000c6c0: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000c6d0: 2e73 706f 7469 645f 6b65 7929 290d 0a20  .spotid_key)).. 
 0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6f0: 2020 6966 2073 656c 662e 6465 7465 6374    if self.detect
-0000c700: 6f72 6368 616e 6e65 6c20 3d3d 2031 3a0d  orchannel == 1:.
-0000c710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c730: 2069 6620 5370 6f74 6f62 6a65 6374 2e67   if Spotobject.g
-0000c740: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000c750: 7465 6e73 6974 795f 6368 325f 6b65 7929  tensity_ch2_key)
-0000c760: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+0000c6f0: 2020 2020 2020 2023 2047 6574 2074 6865         # Get the
+0000c700: 2054 5a59 5820 6c6f 6361 7469 6f6e 206f   TZYX location o
+0000c710: 6620 7468 6520 6365 6c6c 7320 696e 2074  f the cells in t
+0000c720: 6861 7420 6672 616d 650d 0a20 2020 2020  hat frame..     
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c740: 2020 2069 6620 7365 6c66 2e64 6574 6563     if self.detec
+0000c750: 746f 7263 6861 6e6e 656c 203d 3d20 313a  torchannel == 1:
+0000c760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c790: 2020 2020 2020 2054 4f54 414c 5f49 4e54         TOTAL_INT
-0000c7a0: 454e 5349 5459 203d 2066 6c6f 6174 2853  ENSITY = float(S
-0000c7b0: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
-0000c7c0: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
-0000c7d0: 7479 5f63 6832 5f6b 6579 2929 0d0a 2020  ty_ch2_key))..  
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000c810: 5349 5459 203d 2066 6c6f 6174 2853 706f  SITY = float(Spo
-0000c820: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
-0000c830: 2e6d 6561 6e5f 696e 7465 6e73 6974 795f  .mean_intensity_
-0000c840: 6368 325f 6b65 7929 290d 0a20 2020 2020  ch2_key))..     
-0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c890: 2020 2020 2020 2020 2054 4f54 414c 5f49           TOTAL_I
-0000c8a0: 4e54 454e 5349 5459 203d 202d 310d 0a20  NTENSITY = -1.. 
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8d0: 2020 2020 2020 4d45 414e 5f49 4e54 454e        MEAN_INTEN
-0000c8e0: 5349 5459 203d 202d 3120 2020 2020 2020  SITY = -1       
-0000c8f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c900: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-0000c910: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c930: 2020 2020 2020 2020 2069 6620 5370 6f74           if Spot
-0000c940: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000c950: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000c960: 6368 315f 6b65 7929 2069 7320 6e6f 7420  ch1_key) is not 
-0000c970: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000c9a0: 4f54 414c 5f49 4e54 454e 5349 5459 203d  OTAL_INTENSITY =
-0000c9b0: 2066 6c6f 6174 2853 706f 746f 626a 6563   float(Spotobjec
-0000c9c0: 742e 6765 7428 7365 6c66 2e74 6f74 616c  t.get(self.total
-0000c9d0: 5f69 6e74 656e 7369 7479 5f63 6831 5f6b  _intensity_ch1_k
-0000c9e0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca00: 2020 2020 2020 2020 2020 2020 2020 4d45                ME
-0000ca10: 414e 5f49 4e54 454e 5349 5459 203d 2066  AN_INTENSITY = f
-0000ca20: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000ca30: 6765 7428 7365 6c66 2e6d 6561 6e5f 696e  get(self.mean_in
-0000ca40: 7465 6e73 6974 795f 6368 315f 6b65 7929  tensity_ch1_key)
-0000ca50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca70: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 2020 544f 5441 4c5f 494e 5445 4e53 4954    TOTAL_INTENSIT
-0000cab0: 5920 3d20 2d31 0d0a 2020 2020 2020 2020  Y = -1..        
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 6966 2053 706f 746f 626a 6563 742e    if Spotobject.
+0000c790: 6765 7428 7365 6c66 2e74 6f74 616c 5f69  get(self.total_i
+0000c7a0: 6e74 656e 7369 7479 5f63 6832 5f6b 6579  ntensity_ch2_key
+0000c7b0: 2920 6973 206e 6f74 204e 6f6e 653a 0d0a  ) is not None:..
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 2020 2020 2020 544f 5441 4c5f 494e          TOTAL_IN
+0000c7f0: 5445 4e53 4954 5920 3d20 666c 6f61 7428  TENSITY = float(
+0000c800: 5370 6f74 6f62 6a65 6374 2e67 6574 2873  Spotobject.get(s
+0000c810: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+0000c820: 6974 795f 6368 325f 6b65 7929 290d 0a20  ity_ch2_key)).. 
+0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c850: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
+0000c860: 4e53 4954 5920 3d20 666c 6f61 7428 5370  NSITY = float(Sp
+0000c870: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
+0000c880: 662e 6d65 616e 5f69 6e74 656e 7369 7479  f.mean_intensity
+0000c890: 5f63 6832 5f6b 6579 2929 0d0a 2020 2020  _ch2_key))..    
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000c8c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 2020 2020 2020 2020 2020 544f 5441 4c5f            TOTAL_
+0000c8f0: 494e 5445 4e53 4954 5920 3d20 2d31 0d0a  INTENSITY = -1..
+0000c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c920: 2020 2020 2020 204d 4541 4e5f 494e 5445         MEAN_INTE
+0000c930: 4e53 4954 5920 3d20 2d31 2020 2020 2020  NSITY = -1      
+0000c940: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000c950: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000c960: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000c970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c980: 2020 2020 2020 2020 2020 6966 2053 706f            if Spo
+0000c990: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000c9a0: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000c9b0: 5f63 6831 5f6b 6579 2920 6973 206e 6f74  _ch1_key) is not
+0000c9c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9f0: 544f 5441 4c5f 494e 5445 4e53 4954 5920  TOTAL_INTENSITY 
+0000ca00: 3d20 666c 6f61 7428 5370 6f74 6f62 6a65  = float(Spotobje
+0000ca10: 6374 2e67 6574 2873 656c 662e 746f 7461  ct.get(self.tota
+0000ca20: 6c5f 696e 7465 6e73 6974 795f 6368 315f  l_intensity_ch1_
+0000ca30: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+0000ca60: 4541 4e5f 494e 5445 4e53 4954 5920 3d20  EAN_INTENSITY = 
+0000ca70: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000ca80: 2e67 6574 2873 656c 662e 6d65 616e 5f69  .get(self.mean_i
+0000ca90: 6e74 656e 7369 7479 5f63 6831 5f6b 6579  ntensity_ch1_key
+0000caa0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cac0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
 0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 4d45 414e 5f49 4e54 454e 5349 5459 203d  MEAN_INTENSITY =
-0000caf0: 202d 3120 2020 2020 2020 2020 0d0a 0d0a   -1         ....
-0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caf0: 2020 2054 4f54 414c 5f49 4e54 454e 5349     TOTAL_INTENSI
+0000cb00: 5459 203d 202d 310d 0a20 2020 2020 2020  TY = -1..       
 0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cb30: 2020 2020 2020 2020 2020 5241 4449 5553            RADIUS
-0000cb40: 203d 2066 6c6f 6174 2853 706f 746f 626a   = float(Spotobj
-0000cb50: 6563 742e 6765 7428 7365 6c66 2e72 6164  ect.get(self.rad
-0000cb60: 6975 735f 6b65 7929 290d 0a20 2020 2020  ius_key))..     
-0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 2020 2051 5541 4c49 5459 203d 2066 6c6f     QUALITY = flo
-0000cb90: 6174 2853 706f 746f 626a 6563 742e 6765  at(Spotobject.ge
-0000cba0: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
-0000cbb0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0000cbd0: 7374 6c6f 6361 7469 6f6e 203d 2028 666c  stlocation = (fl
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb30: 204d 4541 4e5f 494e 5445 4e53 4954 5920   MEAN_INTENSITY 
+0000cb40: 3d20 2d31 2020 2020 2020 2020 200d 0a0d  = -1         ...
+0000cb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000cb80: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
+0000cb90: 5320 3d20 666c 6f61 7428 5370 6f74 6f62  S = float(Spotob
+0000cba0: 6a65 6374 2e67 6574 2873 656c 662e 7261  ject.get(self.ra
+0000cbb0: 6469 7573 5f6b 6579 2929 0d0a 2020 2020  dius_key))..    
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 2020 2020 5155 414c 4954 5920 3d20 666c      QUALITY = fl
 0000cbe0: 6f61 7428 5370 6f74 6f62 6a65 6374 2e67  oat(Spotobject.g
-0000cbf0: 6574 2873 656c 662e 7a70 6f73 6964 5f6b  et(self.zposid_k
-0000cc00: 6579 2929 2c20 666c 6f61 7428 5370 6f74  ey)), float(Spot
-0000cc10: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000cc20: 7970 6f73 6964 5f6b 6579 2929 2c20 2066  yposid_key)),  f
+0000cbf0: 6574 2873 656c 662e 7175 616c 6974 795f  et(self.quality_
+0000cc00: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+0000cc10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000cc20: 6573 746c 6f63 6174 696f 6e20 3d20 2866  estlocation = (f
 0000cc30: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000cc40: 6765 7428 7365 6c66 2e78 706f 7369 645f  get(self.xposid_
-0000cc50: 6b65 7929 2929 0d0a 2020 2020 2020 2020  key)))..        
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc70: 6672 616d 6520 3d20 5370 6f74 6f62 6a65  frame = Spotobje
-0000cc80: 6374 2e67 6574 2873 656c 662e 6672 616d  ct.get(self.fram
-0000cc90: 6569 645f 6b65 7929 0d0a 2020 2020 2020  eid_key)..      
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccb0: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
-0000ccc0: 6d61 736b 2c20 6d61 736b 6365 6e74 726f  mask, maskcentro
-0000ccd0: 6964 203d 2073 656c 662e 5f67 6574 5f62  id = self._get_b
-0000cce0: 6f75 6e64 6172 795f 6469 7374 2866 7261  oundary_dist(fra
-0000ccf0: 6d65 2c20 7465 7374 6c6f 6361 7469 6f6e  me, testlocation
-0000cd00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000cd10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd30: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000cd40: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000cd50: 5b63 656c 6c5f 6964 5d20 3d20 7b0d 0a20  [cell_id] = {.. 
-0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cd80: 6365 6c6c 6964 5f6b 6579 3a20 696e 7428  cellid_key: int(
-0000cd90: 6365 6c6c 5f69 6429 2c20 0d0a 2020 2020  cell_id), ..    
-0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdb0: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-0000cdc0: 6d65 6964 5f6b 6579 203a 2069 6e74 2866  meid_key : int(f
-0000cdd0: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000cde0: 6765 7428 7365 6c66 2e66 7261 6d65 6964  get(self.frameid
-0000cdf0: 5f6b 6579 2929 292c 0d0a 2020 2020 2020  _key))),..      
-0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce10: 2020 2020 2020 7365 6c66 2e7a 706f 7369        self.zposi
-0000ce20: 645f 6b65 7920 3a20 666c 6f61 7428 5370  d_key : float(Sp
-0000ce30: 6f74 6f62 6a65 6374 2e67 6574 2873 656c  otobject.get(sel
-0000ce40: 662e 7a70 6f73 6964 5f6b 6579 2929 2c0d  f.zposid_key)),.
-0000ce50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ce60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ce70: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
-0000ce80: 6c6f 6174 2853 706f 746f 626a 6563 742e  loat(Spotobject.
-0000ce90: 6765 7428 7365 6c66 2e79 706f 7369 645f  get(self.yposid_
-0000cea0: 6b65 7929 292c 0d0a 2020 2020 2020 2020  key)),..        
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 2020 2020 7365 6c66 2e78 706f 7369 645f      self.xposid_
-0000ced0: 6b65 7920 3a20 666c 6f61 7428 5370 6f74  key : float(Spot
-0000cee0: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-0000cef0: 7870 6f73 6964 5f6b 6579 2929 2c0d 0a20  xposid_key)),.. 
+0000cc40: 6765 7428 7365 6c66 2e7a 706f 7369 645f  get(self.zposid_
+0000cc50: 6b65 7929 292c 2066 6c6f 6174 2853 706f  key)), float(Spo
+0000cc60: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000cc70: 2e79 706f 7369 645f 6b65 7929 292c 2020  .yposid_key)),  
+0000cc80: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000cc90: 2e67 6574 2873 656c 662e 7870 6f73 6964  .get(self.xposid
+0000cca0: 5f6b 6579 2929 290d 0a20 2020 2020 2020  _key)))..       
+0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccc0: 2066 7261 6d65 203d 2053 706f 746f 626a   frame = Spotobj
+0000ccd0: 6563 742e 6765 7428 7365 6c66 2e66 7261  ect.get(self.fra
+0000cce0: 6d65 6964 5f6b 6579 290d 0a20 2020 2020  meid_key)..     
+0000ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd00: 2020 2064 6973 7461 6e63 655f 6365 6c6c     distance_cell
+0000cd10: 5f6d 6173 6b2c 206d 6173 6b63 656e 7472  _mask, maskcentr
+0000cd20: 6f69 6420 3d20 7365 6c66 2e5f 6765 745f  oid = self._get_
+0000cd30: 626f 756e 6461 7279 5f64 6973 7428 6672  boundary_dist(fr
+0000cd40: 616d 652c 2074 6573 746c 6f63 6174 696f  ame, testlocatio
+0000cd50: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
+0000cd60: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd80: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+0000cd90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000cda0: 735b 6365 6c6c 5f69 645d 203d 207b 0d0a  s[cell_id] = {..
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cdd0: 2e63 656c 6c69 645f 6b65 793a 2069 6e74  .cellid_key: int
+0000cde0: 2863 656c 6c5f 6964 292c 200d 0a20 2020  (cell_id), ..   
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 2020 2020 2073 656c 662e 6672           self.fr
+0000ce10: 616d 6569 645f 6b65 7920 3a20 696e 7428  ameid_key : int(
+0000ce20: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000ce30: 2e67 6574 2873 656c 662e 6672 616d 6569  .get(self.framei
+0000ce40: 645f 6b65 7929 2929 2c0d 0a20 2020 2020  d_key))),..     
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
+0000ce70: 6964 5f6b 6579 203a 2066 6c6f 6174 2853  id_key : float(S
+0000ce80: 706f 746f 626a 6563 742e 6765 7428 7365  potobject.get(se
+0000ce90: 6c66 2e7a 706f 7369 645f 6b65 7929 292c  lf.zposid_key)),
+0000cea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000cec0: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
+0000ced0: 666c 6f61 7428 5370 6f74 6f62 6a65 6374  float(Spotobject
+0000cee0: 2e67 6574 2873 656c 662e 7970 6f73 6964  .get(self.yposid
+0000cef0: 5f6b 6579 2929 2c0d 0a20 2020 2020 2020  _key)),..       
 0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cf20: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0000cf30: 6b65 7920 3a20 544f 5441 4c5f 494e 5445  key : TOTAL_INTE
-0000cf40: 4e53 4954 592c 0d0a 2020 2020 2020 2020  NSITY,..        
+0000cf10: 2020 2020 2073 656c 662e 7870 6f73 6964       self.xposid
+0000cf20: 5f6b 6579 203a 2066 6c6f 6174 2853 706f  _key : float(Spo
+0000cf30: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+0000cf40: 2e78 706f 7369 645f 6b65 7929 292c 0d0a  .xposid_key)),..
 0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
-0000cf70: 7465 6e73 6974 795f 6b65 7920 3a20 4d45  tensity_key : ME
-0000cf80: 414e 5f49 4e54 454e 5349 5459 2c0d 0a20  AN_INTENSITY,.. 
-0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cfb0: 7261 6469 7573 5f6b 6579 203a 2052 4144  radius_key : RAD
-0000cfc0: 4955 532c 0d0a 2020 2020 2020 2020 2020  IUS,..          
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-0000cff0: 6579 203a 2051 5541 4c49 5459 2c0d 0a20  ey : QUALITY,.. 
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d020: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-0000d030: 736b 5f6b 6579 3a20 666c 6f61 7428 6469  sk_key: float(di
-0000d040: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000d050: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d070: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-0000d080: 645f 7a5f 6b65 793a 2066 6c6f 6174 286d  d_z_key: float(m
-0000d090: 6173 6b63 656e 7472 6f69 645b 305d 292c  askcentroid[0]),
-0000d0a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d0c0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
-0000d0d0: 795f 6b65 793a 2066 6c6f 6174 286d 6173  y_key: float(mas
-0000d0e0: 6b63 656e 7472 6f69 645b 315d 292c 0d0a  kcentroid[1]),..
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d110: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
-0000d120: 6b65 793a 2066 6c6f 6174 286d 6173 6b63  key: float(maskc
-0000d130: 656e 7472 6f69 645b 325d 2920 0d0a 2020  entroid[2]) ..  
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-0000d160: 0d0a 2020 2020 6465 6620 5f67 6574 5f6d  ..    def _get_m
-0000d170: 6173 7465 725f 786d 6c5f 6461 7461 2873  aster_xml_data(s
-0000d180: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-0000d190: 2020 2069 6620 7365 6c66 2e63 6861 6e6e     if self.chann
-0000d1a0: 656c 5f73 6567 5f69 6d61 6765 2069 7320  el_seg_image is 
-0000d1b0: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1d0: 2073 656c 662e 6368 616e 6e65 6c5f 786d   self.channel_xm
-0000d1e0: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
-0000d1f0: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
-0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d210: 2020 2020 7365 6c66 2e78 6d6c 5f74 7265      self.xml_tre
-0000d220: 6520 3d20 6574 2e70 6172 7365 2873 656c  e = et.parse(sel
-0000d230: 662e 786d 6c5f 7061 7468 290d 0a20 2020  f.xml_path)..   
-0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d250: 2020 2073 656c 662e 786d 6c5f 726f 6f74     self.xml_root
-0000d260: 203d 2073 656c 662e 786d 6c5f 7472 6565   = self.xml_tree
-0000d270: 2e67 6574 726f 6f74 2829 0d0a 2020 2020  .getroot()..    
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
-0000d2a0: 6d6c 5f6e 616d 6520 3d20 2773 6563 6f6e  ml_name = 'secon
-0000d2b0: 645f 6368 616e 6e65 6c5f 2720 2b20 6f73  d_channel_' + os
-0000d2c0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
-0000d2d0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000d2e0: 7365 6c66 2e78 6d6c 5f70 6174 6829 295b  self.xml_path))[
-0000d2f0: 305d 202b 2027 2e78 6d6c 270d 0a20 2020  0] + '.xml'..   
-0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d310: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
-0000d320: 786d 6c5f 7061 7468 203d 206f 732e 7061  xml_path = os.pa
-0000d330: 7468 2e64 6972 6e61 6d65 2873 656c 662e  th.dirname(self.
-0000d340: 786d 6c5f 7061 7468 290d 0a20 2020 2020  xml_path)..     
+0000cf60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cf70: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
+0000cf80: 5f6b 6579 203a 2054 4f54 414c 5f49 4e54  _key : TOTAL_INT
+0000cf90: 454e 5349 5459 2c0d 0a20 2020 2020 2020  ENSITY,..       
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2020 2073 656c 662e 6d65 616e 5f69       self.mean_i
+0000cfc0: 6e74 656e 7369 7479 5f6b 6579 203a 204d  ntensity_key : M
+0000cfd0: 4541 4e5f 494e 5445 4e53 4954 592c 0d0a  EAN_INTENSITY,..
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d000: 2e72 6164 6975 735f 6b65 7920 3a20 5241  .radius_key : RA
+0000d010: 4449 5553 2c0d 0a20 2020 2020 2020 2020  DIUS,..         
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d030: 2020 2073 656c 662e 7175 616c 6974 795f     self.quality_
+0000d040: 6b65 7920 3a20 5155 414c 4954 592c 0d0a  key : QUALITY,..
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d070: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+0000d080: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
+0000d090: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000d0a0: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
+0000d0d0: 6964 5f7a 5f6b 6579 3a20 666c 6f61 7428  id_z_key: float(
+0000d0e0: 6d61 736b 6365 6e74 726f 6964 5b30 5d29  maskcentroid[0])
+0000d0f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0000d100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d110: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
+0000d120: 5f79 5f6b 6579 3a20 666c 6f61 7428 6d61  _y_key: float(ma
+0000d130: 736b 6365 6e74 726f 6964 5b31 5d29 2c0d  skcentroid[1]),.
+0000d140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d150: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000d160: 662e 6d61 736b 6365 6e74 726f 6964 5f78  f.maskcentroid_x
+0000d170: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
+0000d180: 6365 6e74 726f 6964 5b32 5d29 200d 0a20  centroid[2]) .. 
+0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1a0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+0000d1b0: 200d 0a20 2020 2064 6566 205f 6765 745f   ..    def _get_
+0000d1c0: 6d61 7374 6572 5f78 6d6c 5f64 6174 6128  master_xml_data(
+0000d1d0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0000d1e0: 2020 2020 6966 2073 656c 662e 6368 616e      if self.chan
+0000d1f0: 6e65 6c5f 7365 675f 696d 6167 6520 6973  nel_seg_image is
+0000d200: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d220: 2020 7365 6c66 2e63 6861 6e6e 656c 5f78    self.channel_x
+0000d230: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
+0000d240: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 2020 2073 656c 662e 786d 6c5f 7472       self.xml_tr
+0000d270: 6565 203d 2065 742e 7061 7273 6528 7365  ee = et.parse(se
+0000d280: 6c66 2e78 6d6c 5f70 6174 6829 0d0a 2020  lf.xml_path)..  
+0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2a0: 2020 2020 7365 6c66 2e78 6d6c 5f72 6f6f      self.xml_roo
+0000d2b0: 7420 3d20 7365 6c66 2e78 6d6c 5f74 7265  t = self.xml_tre
+0000d2c0: 652e 6765 7472 6f6f 7428 290d 0a20 2020  e.getroot()..   
+0000d2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2e0: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000d2f0: 786d 6c5f 6e61 6d65 203d 2027 7365 636f  xml_name = 'seco
+0000d300: 6e64 5f63 6861 6e6e 656c 5f27 202b 206f  nd_channel_' + o
+0000d310: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
+0000d320: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+0000d330: 2873 656c 662e 786d 6c5f 7061 7468 2929  (self.xml_path))
+0000d340: 5b30 5d20 2b20 272e 786d 6c27 0d0a 2020  [0] + '.xml'..  
 0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d360: 2073 656c 662e 5f63 7265 6174 655f 6368   self._create_ch
-0000d370: 616e 6e65 6c5f 7472 6565 2829 0d0a 0d0a  annel_tree()....
-0000d380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d390: 2e75 6e69 7175 655f 6f62 6a65 6374 7320  .unique_objects 
-0000d3a0: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
-0000d3b0: 2020 7365 6c66 2e75 6e69 7175 655f 7072    self.unique_pr
-0000d3c0: 6f70 6572 7469 6573 203d 207b 7d0d 0a20  operties = {}.. 
-0000d3d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d3e0: 416c 6c54 7261 636b 4964 7320 3d20 5b5d  AllTrackIds = []
-0000d3f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d400: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000d410: 4964 7320 3d20 5b5d 0d0a 2020 2020 2020  Ids = []..      
-0000d420: 2020 2020 2020 7365 6c66 2e4e 6f72 6d61        self.Norma
-0000d430: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
-0000d440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d450: 2e61 6c6c 5f74 7261 636b 5f70 726f 7065  .all_track_prope
-0000d460: 7274 6965 7320 3d20 5b5d 0d0a 2020 2020  rties = []..    
-0000d470: 2020 2020 2020 2020 7365 6c66 2e73 706c          self.spl
-0000d480: 6974 5f70 6f69 6e74 735f 7469 6d65 7320  it_points_times 
-0000d490: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-0000d4a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000d4b0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000d4c0: 7365 6c66 2e41 6c6c 5472 6163 6b49 6473  self.AllTrackIds
-0000d4d0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
-0000d4e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d4f0: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000d500: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
-0000d510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d520: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
-0000d530: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000d540: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000d550: 2020 2020 2020 2073 656c 662e 416c 6c54         self.AllT
-0000d560: 7261 636b 4964 732e 6170 7065 6e64 2873  rackIds.append(s
-0000d570: 656c 662e 5472 6163 6b69 6442 6f78 290d  elf.TrackidBox).
-0000d580: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d590: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
-0000d5a0: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
-0000d5b0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
-0000d5c0: 2020 2020 2020 2020 7365 6c66 2e4e 6f72          self.Nor
-0000d5d0: 6d61 6c54 7261 636b 4964 732e 6170 7065  malTrackIds.appe
-0000d5e0: 6e64 2873 656c 662e 5472 6163 6b69 6442  nd(self.TrackidB
-0000d5f0: 6f78 290d 0a20 2020 2020 2020 2020 2020  ox)..           
-0000d600: 200d 0a20 2020 2020 2020 2020 2020 200d   ..            .
-0000d610: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d620: 662e 5370 6f74 6f62 6a65 6374 7320 3d20  f.Spotobjects = 
-0000d630: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
-0000d640: 2e66 696e 6428 274d 6f64 656c 2729 2e66  .find('Model').f
-0000d650: 696e 6428 2741 6c6c 5370 6f74 7327 290d  ind('AllSpots').
-0000d660: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
-0000d670: 7874 7261 6374 2074 6865 2074 7261 636b  xtract the track
-0000d680: 7320 6672 6f6d 2078 6d6c 0d0a 2020 2020  s from xml..    
-0000d690: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
-0000d6a0: 636b 7320 3d20 7365 6c66 2e78 6d6c 5f63  cks = self.xml_c
-0000d6b0: 6f6e 7465 6e74 2e66 696e 6428 224d 6f64  ontent.find("Mod
-0000d6c0: 656c 2229 2e66 696e 6428 2241 6c6c 5472  el").find("AllTr
-0000d6d0: 6163 6b73 2229 0d0a 2020 2020 2020 2020  acks")..        
-0000d6e0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000d6f0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000d700: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
-0000d710: 6e67 7322 292e 6669 6e64 2822 496d 6167  ngs").find("Imag
-0000d720: 6544 6174 6122 290d 0a20 2020 2020 2020  eData")..       
-0000d730: 2020 2020 2073 656c 662e 7863 616c 6962       self.xcalib
-0000d740: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
-0000d750: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000d760: 2822 7069 7865 6c77 6964 7468 2229 290d  ("pixelwidth")).
-0000d770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d780: 662e 7963 616c 6962 7261 7469 6f6e 203d  f.ycalibration =
-0000d790: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
-0000d7a0: 696e 6773 2e67 6574 2822 7069 7865 6c68  ings.get("pixelh
-0000d7b0: 6569 6768 7422 2929 0d0a 2020 2020 2020  eight"))..      
-0000d7c0: 2020 2020 2020 7365 6c66 2e7a 6361 6c69        self.zcali
-0000d7d0: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000d7e0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000d7f0: 7428 2276 6f78 656c 6465 7074 6822 2929  t("voxeldepth"))
-0000d800: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000d810: 6c66 2e74 6361 6c69 6272 6174 696f 6e20  lf.tcalibration 
-0000d820: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
-0000d830: 2e73 6574 7469 6e67 732e 6765 7428 2274  .settings.get("t
-0000d840: 696d 6569 6e74 6572 7661 6c22 2929 290d  imeinterval"))).
-0000d850: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d860: 662e 6465 7465 6374 6f72 7365 7474 696e  f.detectorsettin
-0000d870: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
-0000d880: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
-0000d890: 696e 6773 2229 2e66 696e 6428 2244 6574  ings").find("Det
-0000d8a0: 6563 746f 7253 6574 7469 6e67 7322 290d  ectorSettings").
-0000d8b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d8c0: 662e 6261 7369 6373 6574 7469 6e67 7320  f.basicsettings 
-0000d8d0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
-0000d8e0: 6e74 2e66 696e 6428 2253 6574 7469 6e67  nt.find("Setting
-0000d8f0: 7322 292e 6669 6e64 2822 4261 7369 6353  s").find("BasicS
-0000d900: 6574 7469 6e67 7322 290d 0a20 2020 2020  ettings")..     
-0000d910: 2020 2020 2020 2073 656c 662e 6465 7465         self.dete
-0000d920: 6374 6f72 6368 616e 6e65 6c20 3d20 696e  ctorchannel = in
-0000d930: 7428 666c 6f61 7428 7365 6c66 2e64 6574  t(float(self.det
-0000d940: 6563 746f 7273 6574 7469 6e67 732e 6765  ectorsettings.ge
-0000d950: 7428 2254 4152 4745 545f 4348 414e 4e45  t("TARGET_CHANNE
-0000d960: 4c22 2929 290d 0a20 2020 2020 2020 2020  L")))..         
-0000d970: 2020 2073 656c 662e 7473 7461 7274 203d     self.tstart =
-0000d980: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
-0000d990: 6261 7369 6373 6574 7469 6e67 732e 6765  basicsettings.ge
-0000d9a0: 7428 2274 7374 6172 7422 2929 290d 0a20  t("tstart"))).. 
-0000d9b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d9c0: 7465 6e64 203d 2069 6e74 2866 6c6f 6174  tend = int(float
-0000d9d0: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
-0000d9e0: 6e67 732e 6765 7428 2274 656e 6422 2929  ngs.get("tend"))
-0000d9f0: 2920 2020 2020 200d 0a0d 0a20 2020 2020  )      ....     
-0000da00: 2020 2020 2020 2070 7269 6e74 2827 4974         print('It
-0000da10: 6572 6174 696e 6720 6f76 6572 2073 706f  erating over spo
-0000da20: 7473 2069 6e20 6672 616d 6527 290d 0a20  ts in frame').. 
-0000da30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000da40: 636f 756e 7420 3d20 300d 0a20 2020 2020  count = 0..     
-0000da50: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
-0000da60: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-0000da70: 2020 2077 6974 6820 636f 6e63 7572 7265     with concurre
-0000da80: 6e74 2e66 7574 7572 6573 2e54 6872 6561  nt.futures.Threa
-0000da90: 6450 6f6f 6c45 7865 6375 746f 7228 6d61  dPoolExecutor(ma
-0000daa0: 785f 776f 726b 6572 7320 3d20 6f73 2e63  x_workers = os.c
-0000dab0: 7075 5f63 6f75 6e74 2829 2920 6173 2065  pu_count()) as e
-0000dac0: 7865 6375 746f 723a 0d0a 2020 2020 2020  xecutor:..      
-0000dad0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000dae0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000daf0: 6672 616d 6520 696e 2073 656c 662e 5370  frame in self.Sp
-0000db00: 6f74 6f62 6a65 6374 732e 6669 6e64 616c  otobjects.findal
-0000db10: 6c28 2753 706f 7473 496e 4672 616d 6527  l('SpotsInFrame'
-0000db20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db40: 6675 7475 7265 732e 6170 7065 6e64 2865  futures.append(e
-0000db50: 7865 6375 746f 722e 7375 626d 6974 2873  xecutor.submit(s
-0000db60: 656c 662e 5f6d 6173 7465 725f 7370 6f74  elf._master_spot
-0000db70: 5f63 6f6d 7075 7465 722c 2066 7261 6d65  _computer, frame
-0000db80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000db90: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
-0000dba0: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
-0000dbb0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbd0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbf0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000dc00: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
-0000dc10: 203d 2022 436f 6c6c 6563 7469 6e67 2053   = "Collecting S
-0000dc20: 706f 7473 220d 0a20 2020 2020 2020 2020  pots"..         
+0000d360: 2020 2020 7365 6c66 2e63 6861 6e6e 656c      self.channel
+0000d370: 5f78 6d6c 5f70 6174 6820 3d20 6f73 2e70  _xml_path = os.p
+0000d380: 6174 682e 6469 726e 616d 6528 7365 6c66  ath.dirname(self
+0000d390: 2e78 6d6c 5f70 6174 6829 0d0a 2020 2020  .xml_path)..    
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 7365 6c66 2e5f 6372 6561 7465 5f63    self._create_c
+0000d3c0: 6861 6e6e 656c 5f74 7265 6528 290d 0a0d  hannel_tree()...
+0000d3d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d3e0: 662e 756e 6971 7565 5f6f 626a 6563 7473  f.unique_objects
+0000d3f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+0000d400: 2020 2073 656c 662e 756e 6971 7565 5f70     self.unique_p
+0000d410: 726f 7065 7274 6965 7320 3d20 7b7d 0d0a  roperties = {}..
+0000d420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d430: 2e41 6c6c 5472 6163 6b49 6473 203d 205b  .AllTrackIds = [
+0000d440: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+0000d450: 656c 662e 4469 7669 6469 6e67 5472 6163  elf.DividingTrac
+0000d460: 6b49 6473 203d 205b 5d0d 0a20 2020 2020  kIds = []..     
+0000d470: 2020 2020 2020 2073 656c 662e 4e6f 726d         self.Norm
+0000d480: 616c 5472 6163 6b49 6473 203d 205b 5d0d  alTrackIds = [].
+0000d490: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d4a0: 662e 616c 6c5f 7472 6163 6b5f 7072 6f70  f.all_track_prop
+0000d4b0: 6572 7469 6573 203d 205b 5d0d 0a20 2020  erties = []..   
+0000d4c0: 2020 2020 2020 2020 2073 656c 662e 7370           self.sp
+0000d4d0: 6c69 745f 706f 696e 7473 5f74 696d 6573  lit_points_times
+0000d4e0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+0000d4f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000d500: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d510: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
+0000d520: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000d530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d540: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
+0000d550: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000d560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d570: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
+0000d580: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
+0000d590: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000d5a0: 2020 2020 2020 2020 7365 6c66 2e41 6c6c          self.All
+0000d5b0: 5472 6163 6b49 6473 2e61 7070 656e 6428  TrackIds.append(
+0000d5c0: 7365 6c66 2e54 7261 636b 6964 426f 7829  self.TrackidBox)
+0000d5d0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d5e0: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
+0000d5f0: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
+0000d600: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
+0000d610: 2020 2020 2020 2020 2073 656c 662e 4e6f           self.No
+0000d620: 726d 616c 5472 6163 6b49 6473 2e61 7070  rmalTrackIds.app
+0000d630: 656e 6428 7365 6c66 2e54 7261 636b 6964  end(self.Trackid
+0000d640: 426f 7829 0d0a 2020 2020 2020 2020 2020  Box)..          
+0000d650: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000d660: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d670: 6c66 2e53 706f 746f 626a 6563 7473 203d  lf.Spotobjects =
+0000d680: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
+0000d690: 742e 6669 6e64 2827 4d6f 6465 6c27 292e  t.find('Model').
+0000d6a0: 6669 6e64 2827 416c 6c53 706f 7473 2729  find('AllSpots')
+0000d6b0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000d6c0: 4578 7472 6163 7420 7468 6520 7472 6163  Extract the trac
+0000d6d0: 6b73 2066 726f 6d20 786d 6c0d 0a20 2020  ks from xml..   
+0000d6e0: 2020 2020 2020 2020 2073 656c 662e 7472           self.tr
+0000d6f0: 6163 6b73 203d 2073 656c 662e 786d 6c5f  acks = self.xml_
+0000d700: 636f 6e74 656e 742e 6669 6e64 2822 4d6f  content.find("Mo
+0000d710: 6465 6c22 292e 6669 6e64 2822 416c 6c54  del").find("AllT
+0000d720: 7261 636b 7322 290d 0a20 2020 2020 2020  racks")..       
+0000d730: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+0000d740: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000d750: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000d760: 696e 6773 2229 2e66 696e 6428 2249 6d61  ings").find("Ima
+0000d770: 6765 4461 7461 2229 0d0a 2020 2020 2020  geData")..      
+0000d780: 2020 2020 2020 7365 6c66 2e78 6361 6c69        self.xcali
+0000d790: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
+0000d7a0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000d7b0: 7428 2270 6978 656c 7769 6474 6822 2929  t("pixelwidth"))
+0000d7c0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d7d0: 6c66 2e79 6361 6c69 6272 6174 696f 6e20  lf.ycalibration 
+0000d7e0: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000d7f0: 7469 6e67 732e 6765 7428 2270 6978 656c  tings.get("pixel
+0000d800: 6865 6967 6874 2229 290d 0a20 2020 2020  height"))..     
+0000d810: 2020 2020 2020 2073 656c 662e 7a63 616c         self.zcal
+0000d820: 6962 7261 7469 6f6e 203d 2066 6c6f 6174  ibration = float
+0000d830: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
+0000d840: 6574 2822 766f 7865 6c64 6570 7468 2229  et("voxeldepth")
+0000d850: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000d860: 656c 662e 7463 616c 6962 7261 7469 6f6e  elf.tcalibration
+0000d870: 203d 2069 6e74 2866 6c6f 6174 2873 656c   = int(float(sel
+0000d880: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
+0000d890: 7469 6d65 696e 7465 7276 616c 2229 2929  timeinterval")))
+0000d8a0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d8b0: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
+0000d8c0: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
+0000d8d0: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
+0000d8e0: 7469 6e67 7322 292e 6669 6e64 2822 4465  tings").find("De
+0000d8f0: 7465 6374 6f72 5365 7474 696e 6773 2229  tectorSettings")
+0000d900: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000d910: 6c66 2e62 6173 6963 7365 7474 696e 6773  lf.basicsettings
+0000d920: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
+0000d930: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
+0000d940: 6773 2229 2e66 696e 6428 2242 6173 6963  gs").find("Basic
+0000d950: 5365 7474 696e 6773 2229 0d0a 2020 2020  Settings")..    
+0000d960: 2020 2020 2020 2020 7365 6c66 2e64 6574          self.det
+0000d970: 6563 746f 7263 6861 6e6e 656c 203d 2069  ectorchannel = i
+0000d980: 6e74 2866 6c6f 6174 2873 656c 662e 6465  nt(float(self.de
+0000d990: 7465 6374 6f72 7365 7474 696e 6773 2e67  tectorsettings.g
+0000d9a0: 6574 2822 5441 5247 4554 5f43 4841 4e4e  et("TARGET_CHANN
+0000d9b0: 454c 2229 2929 0d0a 2020 2020 2020 2020  EL")))..        
+0000d9c0: 2020 2020 7365 6c66 2e74 7374 6172 7420      self.tstart 
+0000d9d0: 3d20 696e 7428 666c 6f61 7428 7365 6c66  = int(float(self
+0000d9e0: 2e62 6173 6963 7365 7474 696e 6773 2e67  .basicsettings.g
+0000d9f0: 6574 2822 7473 7461 7274 2229 2929 0d0a  et("tstart")))..
+0000da00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000da10: 2e74 656e 6420 3d20 696e 7428 666c 6f61  .tend = int(floa
+0000da20: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
+0000da30: 696e 6773 2e67 6574 2822 7465 6e64 2229  ings.get("tend")
+0000da40: 2929 2020 2020 2020 0d0a 0d0a 2020 2020  ))      ....    
+0000da50: 2020 2020 2020 2020 7072 696e 7428 2749          print('I
+0000da60: 7465 7261 7469 6e67 206f 7665 7220 7370  terating over sp
+0000da70: 6f74 7320 696e 2066 7261 6d65 2729 0d0a  ots in frame')..
+0000da80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000da90: 2e63 6f75 6e74 203d 2030 0d0a 2020 2020  .count = 0..    
+0000daa0: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
+0000dab0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000dac0: 2020 2020 7769 7468 2063 6f6e 6375 7272      with concurr
+0000dad0: 656e 742e 6675 7475 7265 732e 5468 7265  ent.futures.Thre
+0000dae0: 6164 506f 6f6c 4578 6563 7574 6f72 286d  adPoolExecutor(m
+0000daf0: 6178 5f77 6f72 6b65 7273 203d 206f 732e  ax_workers = os.
+0000db00: 6370 755f 636f 756e 7428 2929 2061 7320  cpu_count()) as 
+0000db10: 6578 6563 7574 6f72 3a0d 0a20 2020 2020  executor:..     
+0000db20: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000db30: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000db40: 2066 7261 6d65 2069 6e20 7365 6c66 2e53   frame in self.S
+0000db50: 706f 746f 626a 6563 7473 2e66 696e 6461  potobjects.finda
+0000db60: 6c6c 2827 5370 6f74 7349 6e46 7261 6d65  ll('SpotsInFrame
+0000db70: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db90: 2066 7574 7572 6573 2e61 7070 656e 6428   futures.append(
+0000dba0: 6578 6563 7574 6f72 2e73 7562 6d69 7428  executor.submit(
+0000dbb0: 7365 6c66 2e5f 6d61 7374 6572 5f73 706f  self._master_spo
+0000dbc0: 745f 636f 6d70 7574 6572 2c20 6672 616d  t_computer, fram
+0000dbd0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+0000dbe0: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
+0000dbf0: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
+0000dc00: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 0000dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc40: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-0000dc50: 7265 7373 5f62 6172 2e72 616e 6765 203d  ress_bar.range =
-0000dc60: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-0000dc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc80: 2020 2020 2020 2020 302c 0d0a 2020 2020          0,..    
-0000dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 6c65 6e28 6675 7475 7265 7329 2c0d 0a20  len(futures),.. 
+0000dc40: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0000dc50: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
+0000dc60: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
+0000dc70: 5370 6f74 7322 0d0a 2020 2020 2020 2020  Spots"..        
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc90: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+0000dca0: 6772 6573 735f 6261 722e 7261 6e67 6520  gress_bar.range 
+0000dcb0: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
 0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000dce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dcd0: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
+0000dce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd00: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000dd10: 6261 722e 7368 6f77 2829 0d0a 0d0a 2020  bar.show()....  
-0000dd20: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000dd30: 7220 7220 696e 2063 6f6e 6375 7272 656e  r r in concurren
-0000dd40: 742e 6675 7475 7265 732e 6173 5f63 6f6d  t.futures.as_com
-0000dd50: 706c 6574 6564 2866 7574 7572 6573 293a  pleted(futures):
-0000dd60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd80: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000dd90: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
-0000dda0: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000ddd0: 726f 6772 6573 735f 6261 7220 6973 206e  rogress_bar is n
-0000dde0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 206c 656e 2866 7574 7572 6573 292c 0d0a   len(futures),..
+0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd50: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000dd60: 5f62 6172 2e73 686f 7728 290d 0a0d 0a20  _bar.show().... 
+0000dd70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000dd80: 6f72 2072 2069 6e20 636f 6e63 7572 7265  or r in concurre
+0000dd90: 6e74 2e66 7574 7572 6573 2e61 735f 636f  nt.futures.as_co
+0000dda0: 6d70 6c65 7465 6428 6675 7475 7265 7329  mpleted(futures)
+0000ddb0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000dde0: 7420 3d20 7365 6c66 2e63 6f75 6e74 202b  t = self.count +
+0000ddf0: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
 0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000de20: 6261 722e 7661 6c75 6520 3d20 2073 656c  bar.value =  sel
-0000de30: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+0000de10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000de20: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+0000de30: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2020 2020 2020 2020 2020 2020 2072 2e72               r.r
-0000de60: 6573 756c 7428 2920 2020 200d 0a0d 0a20  esult()    .... 
-0000de70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000de80: 2866 2749 7465 7261 7469 6e67 206f 7665  (f'Iterating ove
-0000de90: 7220 7472 6163 6b73 207b 6c65 6e28 7365  r tracks {len(se
-0000dea0: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-0000deb0: 6b5f 6964 7329 7d27 2920 200d 0a20 2020  k_ids)}')  ..   
-0000dec0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000ded0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0000dee0: 2020 2020 2066 7574 7572 6573 203d 205b       futures = [
-0000def0: 5d0d 0a20 2020 2020 2020 2020 2020 2069  ]..            i
-0000df00: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
-0000df10: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
-0000df20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000df30: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
-0000df40: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
-0000df50: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
-0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df70: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-0000df80: 6172 2e72 616e 6765 203d 2028 302c 206c  ar.range = (0, l
-0000df90: 656e 2873 656c 662e 6669 6c74 6572 6564  en(self.filtered
-0000dfa0: 5f74 7261 636b 5f69 6473 2929 0d0a 2020  _track_ids))..  
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000dfc0: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000dfd0: 7368 6f77 2829 0d0a 0d0a 2020 2020 2020  show()....      
-0000dfe0: 2020 2020 2020 666f 7220 7472 6163 6b20        for track 
-0000dff0: 696e 2073 656c 662e 7472 6163 6b73 2e66  in self.tracks.f
-0000e000: 696e 6461 6c6c 2827 5472 6163 6b27 293a  indall('Track'):
-0000e010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e020: 2020 7472 6163 6b5f 6964 203d 2069 6e74    track_id = int
-0000e030: 2874 7261 636b 2e67 6574 2873 656c 662e  (track.get(self.
-0000e040: 7472 6163 6b69 645f 6b65 7929 290d 0a20  trackid_key)).. 
-0000e050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e060: 6620 7472 6163 6b5f 6964 2069 6e20 7365  f track_id in se
-0000e070: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
-0000e080: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
-0000e090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e0a0: 2e5f 6d61 7374 6572 5f74 7261 636b 5f63  ._master_track_c
-0000e0b0: 6f6d 7075 7465 7228 7472 6163 6b2c 2074  omputer(track, t
-0000e0c0: 7261 636b 5f69 6429 0d0a 2020 2020 2020  rack_id)..      
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e0e0: 6c66 2e63 6f75 6e74 202b 3d20 310d 0a20  lf.count += 1.. 
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e100: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-0000e110: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-0000e120: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000e130: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e140: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
-0000e150: 7661 6c75 6520 3d20 7365 6c66 2e63 6f75  value = self.cou
-0000e160: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-0000e170: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-0000e180: 7365 675f 696d 6167 6520 6973 206e 6f74  seg_image is not
-0000e190: 204e 6f6e 653a 2020 0d0a 2020 2020 2020   None:  ..      
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000e1c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0000e1d0: 6372 6561 7465 5f73 6563 6f6e 645f 6368  create_second_ch
-0000e1e0: 616e 6e65 6c5f 786d 6c28 290d 0a20 2020  annel_xml()..   
+0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de60: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000de70: 5f62 6172 2e76 616c 7565 203d 2020 7365  _bar.value =  se
+0000de80: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+0000de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dea0: 2020 2020 2020 2020 2020 2020 2020 722e                r.
+0000deb0: 7265 7375 6c74 2829 2020 2020 0d0a 0d0a  result()    ....
+0000dec0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000ded0: 7428 6627 4974 6572 6174 696e 6720 6f76  t(f'Iterating ov
+0000dee0: 6572 2074 7261 636b 7320 7b6c 656e 2873  er tracks {len(s
+0000def0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000df00: 636b 5f69 6473 297d 2729 2020 0d0a 2020  ck_ids)}')  ..  
+0000df10: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000df20: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+0000df30: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
+0000df40: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+0000df50: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+0000df60: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+0000df70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000df80: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
+0000df90: 5f62 6172 2e6c 6162 656c 203d 2022 436f  _bar.label = "Co
+0000dfa0: 6c6c 6563 7469 6e67 2054 7261 636b 7322  llecting Tracks"
+0000dfb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000dfc0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+0000dfd0: 6261 722e 7261 6e67 6520 3d20 2830 2c20  bar.range = (0, 
+0000dfe0: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
+0000dff0: 645f 7472 6163 6b5f 6964 7329 290d 0a20  d_track_ids)).. 
+0000e000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e010: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000e020: 2e73 686f 7728 290d 0a0d 0a20 2020 2020  .show()....     
+0000e030: 2020 2020 2020 2066 6f72 2074 7261 636b         for track
+0000e040: 2069 6e20 7365 6c66 2e74 7261 636b 732e   in self.tracks.
+0000e050: 6669 6e64 616c 6c28 2754 7261 636b 2729  findall('Track')
+0000e060: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000e070: 2020 2074 7261 636b 5f69 6420 3d20 696e     track_id = in
+0000e080: 7428 7472 6163 6b2e 6765 7428 7365 6c66  t(track.get(self
+0000e090: 2e74 7261 636b 6964 5f6b 6579 2929 0d0a  .trackid_key))..
+0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0b0: 6966 2074 7261 636b 5f69 6420 696e 2073  if track_id in s
+0000e0c0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
+0000e0d0: 636b 5f69 6473 3a0d 0a20 2020 2020 2020  ck_ids:..       
+0000e0e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e0f0: 662e 5f6d 6173 7465 725f 7472 6163 6b5f  f._master_track_
+0000e100: 636f 6d70 7574 6572 2874 7261 636b 2c20  computer(track, 
+0000e110: 7472 6163 6b5f 6964 290d 0a20 2020 2020  track_id)..     
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e130: 656c 662e 636f 756e 7420 2b3d 2031 0d0a  elf.count += 1..
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e150: 2020 2020 6966 2073 656c 662e 7072 6f67      if self.prog
+0000e160: 7265 7373 5f62 6172 2069 7320 6e6f 7420  ress_bar is not 
+0000e170: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000e180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e190: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+0000e1a0: 2e76 616c 7565 203d 2073 656c 662e 636f  .value = self.co
+0000e1b0: 756e 740d 0a20 2020 2020 2020 2020 2020  unt..           
+0000e1c0: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000e1d0: 5f73 6567 5f69 6d61 6765 2069 7320 6e6f  _seg_image is no
+0000e1e0: 7420 4e6f 6e65 3a20 200d 0a20 2020 2020  t None:  ..     
 0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e200: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
-0000e210: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-0000e220: 2069 6e20 7365 6c66 2e67 7261 7068 5f73   in self.graph_s
-0000e230: 706c 6974 2e69 7465 6d73 2829 3a0d 0a20  plit.items():.. 
+0000e200: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000e210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e220: 5f63 7265 6174 655f 7365 636f 6e64 5f63  _create_second_c
+0000e230: 6861 6e6e 656c 5f78 6d6c 2829 0d0a 2020  hannel_xml()..  
 0000e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e250: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e270: 2020 2020 2020 2020 6461 7567 6874 6572          daughter
-0000e280: 5f74 7261 636b 5f69 6420 3d20 2069 6e74  _track_id =  int
-0000e290: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
-0000e2a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000e2b0: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
-0000e2c0: 286b 2929 5d5b 7365 6c66 2e75 6e69 7175  (k))][self.uniqu
-0000e2d0: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
-0000e300: 7472 6163 6b5f 6964 203d 2069 6e74 2866  track_id = int(f
-0000e310: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
-0000e320: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000e330: 7469 6573 5b69 6e74 2866 6c6f 6174 2876  ties[int(float(v
-0000e340: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
-0000e350: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
-0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e370: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
-0000e380: 685f 7472 6163 6b73 5b64 6175 6768 7465  h_tracks[daughte
-0000e390: 725f 7472 6163 6b5f 6964 5d20 3d20 7061  r_track_id] = pa
-0000e3a0: 7265 6e74 5f74 7261 636b 5f69 640d 0a0d  rent_track_id...
-0000e3b0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000e3c0: 6e74 2827 6765 7474 696e 6720 6174 7472  nt('getting attr
-0000e3d0: 6962 7574 6573 2729 2020 2020 2020 2020  ibutes')        
-0000e3e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000e3f0: 2020 2020 2020 7365 6c66 2e5f 6765 745f        self._get_
-0000e400: 6174 7472 6962 7574 6573 2829 0d0a 2020  attributes()..  
-0000e410: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000e420: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
-0000e430: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
-0000e440: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
-0000e450: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-0000e460: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
-0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e490: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-0000e4a0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-0000e4b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+0000e250: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000e260: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
+0000e270: 2920 696e 2073 656c 662e 6772 6170 685f  ) in self.graph_
+0000e280: 7370 6c69 742e 6974 656d 7328 293a 0d0a  split.items():..
+0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2c0: 2020 2020 2020 2020 2064 6175 6768 7465           daughte
+0000e2d0: 725f 7472 6163 6b5f 6964 203d 2020 696e  r_track_id =  in
+0000e2e0: 7428 666c 6f61 7428 7374 7228 7365 6c66  t(float(str(self
+0000e2f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+0000e300: 7065 7274 6965 735b 696e 7428 666c 6f61  perties[int(floa
+0000e310: 7428 6b29 295d 5b73 656c 662e 756e 6971  t(k))][self.uniq
+0000e320: 7565 6964 5f6b 6579 5d29 2929 0d0a 2020  ueid_key])))..  
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
+0000e350: 5f74 7261 636b 5f69 6420 3d20 696e 7428  _track_id = int(
+0000e360: 666c 6f61 7428 7374 7228 7365 6c66 2e75  float(str(self.u
+0000e370: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000e380: 7274 6965 735b 696e 7428 666c 6f61 7428  rties[int(float(
+0000e390: 7629 295d 5b73 656c 662e 756e 6971 7565  v))][self.unique
+0000e3a0: 6964 5f6b 6579 5d29 2929 0d0a 2020 2020  id_key])))..    
+0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3c0: 2020 2020 2020 2020 7365 6c66 2e67 7261          self.gra
+0000e3d0: 7068 5f74 7261 636b 735b 6461 7567 6874  ph_tracks[daught
+0000e3e0: 6572 5f74 7261 636b 5f69 645d 203d 2070  er_track_id] = p
+0000e3f0: 6172 656e 745f 7472 6163 6b5f 6964 0d0a  arent_track_id..
+0000e400: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000e410: 696e 7428 2767 6574 7469 6e67 2061 7474  int('getting att
+0000e420: 7269 6275 7465 7327 2920 2020 2020 2020  ributes')       
+0000e430: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000e440: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
+0000e450: 5f61 7474 7269 6275 7465 7328 290d 0a20  _attributes().. 
+0000e460: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000e470: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+0000e480: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+0000e490: 2020 2020 666f 7220 7472 6163 6b5f 6964      for track_id
+0000e4a0: 2069 6e20 7365 6c66 2e66 696c 7465 7265   in self.filtere
+0000e4b0: 645f 7472 6163 6b5f 6964 733a 0d0a 2020  d_track_ids:..  
 0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e4e0: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-0000e4f0: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-0000e500: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
+0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4e0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+0000e4f0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+0000e500: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
 0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e530: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-0000e540: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-0000e550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e520: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e530: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
+0000e540: 6162 656c 203d 2022 4a75 7374 206f 6e65  abel = "Just one
+0000e550: 206d 6f72 6520 7468 696e 6722 0d0a 2020   more thing"..  
 0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-0000e5c0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-0000e5d0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+0000e580: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+0000e590: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
+0000e5a0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5d0: 2020 2030 2c0d 0a20 2020 2020 2020 2020     0,..         
 0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e620: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e630: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-0000e640: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e670: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-0000e680: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e600: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
+0000e610: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+0000e620: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e670: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e680: 662e 7072 6f67 7265 7373 5f62 6172 2e73  f.progress_bar.s
+0000e690: 686f 7728 290d 0a20 2020 2020 2020 2020  how()..         
 0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-0000e6c0: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-0000e6d0: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e6c0: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
+0000e6d0: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
 0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e700: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
-0000e710: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-0000e720: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000e730: 662e 666f 7572 6965 723a 0d0a 2020 2020  f.fourier:..    
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000e750: 7269 6e74 2827 636f 6d70 7574 696e 6720  rint('computing 
-0000e760: 466f 7572 6965 7227 290d 0a20 2020 2020  Fourier')..     
-0000e770: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e780: 6c66 2e5f 636f 6d70 7574 655f 7068 656e  lf._compute_phen
-0000e790: 6f74 7970 6573 2829 2020 2020 2020 2020  otypes()        
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000e7c0: 6c66 2e5f 7465 6d70 6f72 616c 5f70 6c6f  lf._temporal_plo
-0000e7d0: 7473 5f74 7261 636b 6d61 7465 2829 2020  ts_trackmate()  
-0000e7e0: 2020 2020 2020 0d0a 0d0a 0d0a 2020 2020        ......    
-0000e7f0: 6465 6620 5f63 7265 6174 655f 7365 636f  def _create_seco
-0000e800: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2873  nd_channel_xml(s
-0000e810: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
-0000e820: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000e830: 2020 2020 2020 2020 7072 696e 7428 2754          print('T
-0000e840: 7261 6e73 6665 7272 696e 6720 584d 4c27  ransferring XML'
-0000e850: 2920 2020 0d0a 2020 2020 2020 2020 2020  )   ..          
-0000e860: 2020 2020 2020 2020 2020 6368 616e 6e65            channe
-0000e870: 6c5f 6669 6c74 6572 6564 5f74 7261 636b  l_filtered_track
-0000e880: 7320 3d20 5b5d 2020 2020 2020 2020 2020  s = []          
-0000e890: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000e8a0: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
-0000e8b0: 6f62 6a65 6374 2069 6e20 7365 6c66 2e78  object in self.x
-0000e8c0: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-0000e8d0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2020 2063 656c 6c5f 6964 203d 2069 6e74     cell_id = int
-0000e900: 2853 706f 746f 626a 6563 742e 6765 7428  (Spotobject.get(
-0000e910: 7365 6c66 2e73 706f 7469 645f 6b65 7929  self.spotid_key)
-0000e920: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e940: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
-0000e950: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000e960: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000e970: 2e6b 6579 7328 293a 2020 2020 2020 2020  .keys():        
-0000e980: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e990: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9c0: 2020 2020 6e65 775f 706f 7369 7469 6f6e      new_position
-0000e9d0: 7820 3d20 2073 656c 662e 6368 616e 6e65  x =  self.channe
-0000e9e0: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
-0000e9f0: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
-0000ea00: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-0000ea10: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 2020 2020 6e65 775f 706f 7369          new_posi
-0000ea40: 7469 6f6e 7920 3d20 2073 656c 662e 6368  tiony =  self.ch
-0000ea50: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000ea60: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000ea70: 6c5f 6964 5d5b 7365 6c66 2e79 706f 7369  l_id][self.yposi
-0000ea80: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-0000eab0: 706f 7369 7469 6f6e 7a20 3d20 2073 656c  positionz =  sel
-0000eac0: 662e 6368 616e 6e65 6c5f 756e 6971 7565  f.channel_unique
-0000ead0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-0000eae0: 5b63 656c 6c5f 6964 5d5b 7365 6c66 2e7a  [cell_id][self.z
-0000eaf0: 706f 7369 645f 6b65 795d 0d0a 0d0a 2020  posid_key]....  
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb20: 2020 6e65 775f 746f 7461 6c5f 696e 7465    new_total_inte
-0000eb30: 6e73 6974 7920 3d20 7365 6c66 2e63 6861  nsity = self.cha
-0000eb40: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-0000eb50: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-0000eb60: 5f69 645d 5b73 656c 662e 746f 7461 6c5f  _id][self.total_
-0000eb70: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 2020 2020 6e65 775f 6d65 616e 5f69 6e74      new_mean_int
-0000ebb0: 656e 7369 7479 203d 2073 656c 662e 6368  ensity = self.ch
-0000ebc0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-0000ebd0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-0000ebe0: 6c5f 6964 5d5b 7365 6c66 2e6d 6561 6e5f  l_id][self.mean_
-0000ebf0: 696e 7465 6e73 6974 795f 6b65 795d 0d0a  intensity_key]..
-0000ec00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec20: 2020 2020 2020 6e65 775f 7261 6469 7573        new_radius
-0000ec30: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
-0000ec40: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000ec50: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-0000ec60: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
-0000ec70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec90: 2020 2020 2020 6e65 775f 7175 616c 6974        new_qualit
-0000eca0: 7920 3d20 7365 6c66 2e63 6861 6e6e 656c  y = self.channel
-0000ecb0: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
-0000ecc0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
-0000ecd0: 5b73 656c 662e 7175 616c 6974 795f 6b65  [self.quality_ke
-0000ece0: 795d 0d0a 2020 2020 2020 2020 2020 2020  y]..            
-0000ecf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed00: 2020 2020 2020 2020 6e65 775f 6469 7374          new_dist
-0000ed10: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-0000ed20: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-0000ed30: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-0000ed40: 7469 6573 5b63 656c 6c5f 6964 5d5b 7365  ties[cell_id][se
-0000ed50: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
-0000ed60: 5f6d 6173 6b5f 6b65 795d 0d0a 0d0a 2020  _mask_key]....  
-0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000eda0: 2873 656c 662e 7870 6f73 6964 5f6b 6579  (self.xposid_key
-0000edb0: 2c20 7374 7228 6e65 775f 706f 7369 7469  , str(new_positi
-0000edc0: 6f6e 7829 2920 2020 2020 0d0a 2020 2020  onx))     ..    
+0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e700: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+0000e710: 735f 6261 722e 7661 6c75 6520 3d20 7365  s_bar.value = se
+0000e720: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e740: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e750: 6c66 2e5f 6669 6e61 6c5f 7472 6163 6b73  lf._final_tracks
+0000e760: 2874 7261 636b 5f69 6429 200d 0a0d 0a20  (track_id) .... 
+0000e770: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000e780: 6c66 2e66 6f75 7269 6572 3a0d 0a20 2020  lf.fourier:..   
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7a0: 7072 696e 7428 2763 6f6d 7075 7469 6e67  print('computing
+0000e7b0: 2046 6f75 7269 6572 2729 0d0a 2020 2020   Fourier')..    
+0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e7d0: 656c 662e 5f63 6f6d 7075 7465 5f70 6865  elf._compute_phe
+0000e7e0: 6e6f 7479 7065 7328 2920 2020 2020 2020  notypes()       
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+0000e810: 656c 662e 5f74 656d 706f 7261 6c5f 706c  elf._temporal_pl
+0000e820: 6f74 735f 7472 6163 6b6d 6174 6528 2920  ots_trackmate() 
+0000e830: 2020 2020 2020 200d 0a0d 0a0d 0a20 2020         ......   
+0000e840: 2064 6566 205f 6372 6561 7465 5f73 6563   def _create_sec
+0000e850: 6f6e 645f 6368 616e 6e65 6c5f 786d 6c28  ond_channel_xml(
+0000e860: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+0000e870: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e880: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0000e890: 5472 616e 7366 6572 7269 6e67 2058 4d4c  Transferring XML
+0000e8a0: 2729 2020 200d 0a20 2020 2020 2020 2020  ')   ..         
+0000e8b0: 2020 2020 2020 2020 2020 2063 6861 6e6e             chann
+0000e8c0: 656c 5f66 696c 7465 7265 645f 7472 6163  el_filtered_trac
+0000e8d0: 6b73 203d 205b 5d20 2020 2020 2020 2020  ks = []         
+0000e8e0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000e8f0: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
+0000e900: 746f 626a 6563 7420 696e 2073 656c 662e  tobject in self.
+0000e910: 786d 6c5f 726f 6f74 2e69 7465 7228 2753  xml_root.iter('S
+0000e920: 706f 7427 293a 0d0a 2020 2020 2020 2020  pot'):..        
+0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e940: 2020 2020 6365 6c6c 5f69 6420 3d20 696e      cell_id = in
+0000e950: 7428 5370 6f74 6f62 6a65 6374 2e67 6574  t(Spotobject.get
+0000e960: 2873 656c 662e 7370 6f74 6964 5f6b 6579  (self.spotid_key
+0000e970: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 6966 2063 656c 6c5f 6964 2069 6e20 7365  if cell_id in se
+0000e9a0: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000e9b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000e9c0: 732e 6b65 7973 2829 3a20 2020 2020 2020  s.keys():       
+0000e9d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000e9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea10: 2020 2020 206e 6577 5f70 6f73 6974 696f       new_positio
+0000ea20: 6e78 203d 2020 7365 6c66 2e63 6861 6e6e  nx =  self.chann
+0000ea30: 656c 5f75 6e69 7175 655f 7370 6f74 5f70  el_unique_spot_p
+0000ea40: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
+0000ea50: 645d 5b73 656c 662e 7870 6f73 6964 5f6b  d][self.xposid_k
+0000ea60: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea80: 2020 2020 2020 2020 206e 6577 5f70 6f73           new_pos
+0000ea90: 6974 696f 6e79 203d 2020 7365 6c66 2e63  itiony =  self.c
+0000eaa0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000eab0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000eac0: 6c6c 5f69 645d 5b73 656c 662e 7970 6f73  ll_id][self.ypos
+0000ead0: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
+0000eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaf0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000eb00: 5f70 6f73 6974 696f 6e7a 203d 2020 7365  _positionz =  se
+0000eb10: 6c66 2e63 6861 6e6e 656c 5f75 6e69 7175  lf.channel_uniqu
+0000eb20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+0000eb30: 735b 6365 6c6c 5f69 645d 5b73 656c 662e  s[cell_id][self.
+0000eb40: 7a70 6f73 6964 5f6b 6579 5d0d 0a0d 0a20  zposid_key].... 
+0000eb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2020 206e 6577 5f74 6f74 616c 5f69 6e74     new_total_int
+0000eb80: 656e 7369 7479 203d 2073 656c 662e 6368  ensity = self.ch
+0000eb90: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+0000eba0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+0000ebb0: 6c5f 6964 5d5b 7365 6c66 2e74 6f74 616c  l_id][self.total
+0000ebc0: 5f69 6e74 656e 7369 7479 5f6b 6579 5d0d  _intensity_key].
+0000ebd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebf0: 2020 2020 206e 6577 5f6d 6561 6e5f 696e       new_mean_in
+0000ec00: 7465 6e73 6974 7920 3d20 7365 6c66 2e63  tensity = self.c
+0000ec10: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+0000ec20: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+0000ec30: 6c6c 5f69 645d 5b73 656c 662e 6d65 616e  ll_id][self.mean
+0000ec40: 5f69 6e74 656e 7369 7479 5f6b 6579 5d0d  _intensity_key].
+0000ec50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec70: 2020 2020 2020 206e 6577 5f72 6164 6975         new_radiu
+0000ec80: 7320 3d20 7365 6c66 2e63 6861 6e6e 656c  s = self.channel
+0000ec90: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000eca0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+0000ecb0: 5b73 656c 662e 7261 6469 7573 5f6b 6579  [self.radius_key
+0000ecc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ece0: 2020 2020 2020 206e 6577 5f71 7561 6c69         new_quali
+0000ecf0: 7479 203d 2073 656c 662e 6368 616e 6e65  ty = self.channe
+0000ed00: 6c5f 756e 6971 7565 5f73 706f 745f 7072  l_unique_spot_pr
+0000ed10: 6f70 6572 7469 6573 5b63 656c 6c5f 6964  operties[cell_id
+0000ed20: 5d5b 7365 6c66 2e71 7561 6c69 7479 5f6b  ][self.quality_k
+0000ed30: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+0000ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed50: 2020 2020 2020 2020 206e 6577 5f64 6973           new_dis
+0000ed60: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+0000ed70: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f75  = self.channel_u
+0000ed80: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+0000ed90: 7274 6965 735b 6365 6c6c 5f69 645d 5b73  rties[cell_id][s
+0000eda0: 656c 662e 6469 7374 616e 6365 5f63 656c  elf.distance_cel
+0000edb0: 6c5f 6d61 736b 5f6b 6579 5d0d 0a0d 0a20  l_mask_key].... 
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000edf0: 5370 6f74 6f62 6a65 6374 2e73 6574 2873  Spotobject.set(s
-0000ee00: 656c 662e 7970 6f73 6964 5f6b 6579 2c20  elf.yposid_key, 
-0000ee10: 7374 7228 6e65 775f 706f 7369 7469 6f6e  str(new_position
-0000ee20: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+0000ede0: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000edf0: 7428 7365 6c66 2e78 706f 7369 645f 6b65  t(self.xposid_ke
+0000ee00: 792c 2073 7472 286e 6577 5f70 6f73 6974  y, str(new_posit
+0000ee10: 696f 6e78 2929 2020 2020 200d 0a20 2020  ionx))     ..   
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ee30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee40: 2020 2020 2020 2020 2053 706f 746f 626a           Spotobj
-0000ee50: 6563 742e 7365 7428 7365 6c66 2e7a 706f  ect.set(self.zpo
-0000ee60: 7369 645f 6b65 792c 2073 7472 286e 6577  sid_key, str(new
-0000ee70: 5f70 6f73 6974 696f 6e7a 2929 0d0a 0d0a  _positionz))....
+0000ee40: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
+0000ee50: 7365 6c66 2e79 706f 7369 645f 6b65 792c  self.yposid_key,
+0000ee60: 2073 7472 286e 6577 5f70 6f73 6974 696f   str(new_positio
+0000ee70: 6e79 2929 0d0a 2020 2020 2020 2020 2020  ny))..          
 0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 2020 2020 5370 6f74 6f62 6a65 6374 2e73      Spotobject.s
-0000eeb0: 6574 2873 656c 662e 746f 7461 6c5f 696e  et(self.total_in
-0000eec0: 7465 6e73 6974 795f 6b65 792c 2073 7472  tensity_key, str
-0000eed0: 286e 6577 5f74 6f74 616c 5f69 6e74 656e  (new_total_inten
-0000eee0: 7369 7479 2929 2020 2020 200d 0a20 2020  sity))     ..   
-0000eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef10: 2053 706f 746f 626a 6563 742e 7365 7428   Spotobject.set(
-0000ef20: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
-0000ef30: 6974 795f 6b65 792c 2073 7472 286e 6577  ity_key, str(new
-0000ef40: 5f6d 6561 6e5f 696e 7465 6e73 6974 7929  _mean_intensity)
-0000ef50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef70: 2020 2020 2020 2053 706f 746f 626a 6563         Spotobjec
-0000ef80: 742e 7365 7428 7365 6c66 2e72 6164 6975  t.set(self.radiu
-0000ef90: 735f 6b65 792c 2073 7472 286e 6577 5f72  s_key, str(new_r
-0000efa0: 6164 6975 7329 2920 2020 2020 0d0a 2020  adius))     ..  
+0000ee90: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
+0000eea0: 6a65 6374 2e73 6574 2873 656c 662e 7a70  ject.set(self.zp
+0000eeb0: 6f73 6964 5f6b 6579 2c20 7374 7228 6e65  osid_key, str(ne
+0000eec0: 775f 706f 7369 7469 6f6e 7a29 290d 0a0d  w_positionz))...
+0000eed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eef0: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
+0000ef00: 7365 7428 7365 6c66 2e74 6f74 616c 5f69  set(self.total_i
+0000ef10: 6e74 656e 7369 7479 5f6b 6579 2c20 7374  ntensity_key, st
+0000ef20: 7228 6e65 775f 746f 7461 6c5f 696e 7465  r(new_total_inte
+0000ef30: 6e73 6974 7929 2920 2020 2020 0d0a 2020  nsity))     ..  
+0000ef40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
+0000ef70: 2873 656c 662e 6d65 616e 5f69 6e74 656e  (self.mean_inten
+0000ef80: 7369 7479 5f6b 6579 2c20 7374 7228 6e65  sity_key, str(ne
+0000ef90: 775f 6d65 616e 5f69 6e74 656e 7369 7479  w_mean_intensity
+0000efa0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
 0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 2020 5370 6f74 6f62 6a65 6374 2e73 6574    Spotobject.set
-0000efe0: 2873 656c 662e 7175 616c 6974 795f 6b65  (self.quality_ke
-0000eff0: 792c 2073 7472 286e 6577 5f71 7561 6c69  y, str(new_quali
-0000f000: 7479 2929 0d0a 2020 2020 2020 2020 2020  ty))..          
+0000efc0: 2020 2020 2020 2020 5370 6f74 6f62 6a65          Spotobje
+0000efd0: 6374 2e73 6574 2873 656c 662e 7261 6469  ct.set(self.radi
+0000efe0: 7573 5f6b 6579 2c20 7374 7228 6e65 775f  us_key, str(new_
+0000eff0: 7261 6469 7573 2929 2020 2020 200d 0a20  radius))     .. 
+0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 2020 2020 2020 5370 6f74 6f62            Spotob
-0000f030: 6a65 6374 2e73 6574 2873 656c 662e 6469  ject.set(self.di
-0000f040: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000f050: 5f6b 6579 2c20 7374 7228 6e65 775f 6469  _key, str(new_di
-0000f060: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-0000f070: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000f080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f090: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0000f0a0: 203d 2073 656c 662e 6368 616e 6e65 6c5f   = self.channel_
-0000f0b0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-0000f0c0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-0000f0d0: 6964 295d 5b73 656c 662e 7472 6163 6b69  id)][self.tracki
-0000f0e0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f100: 2020 2020 2020 2020 2020 2020 6368 616e              chan
-0000f110: 6e65 6c5f 6669 6c74 6572 6564 5f74 7261  nel_filtered_tra
-0000f120: 636b 732e 6170 7065 6e64 2874 7261 636b  cks.append(track
-0000f130: 5f69 6429 0d0a 2020 2020 2020 2020 2020  _id)..          
+0000f020: 2020 2053 706f 746f 626a 6563 742e 7365     Spotobject.se
+0000f030: 7428 7365 6c66 2e71 7561 6c69 7479 5f6b  t(self.quality_k
+0000f040: 6579 2c20 7374 7228 6e65 775f 7175 616c  ey, str(new_qual
+0000f050: 6974 7929 290d 0a20 2020 2020 2020 2020  ity))..         
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f070: 2020 2020 2020 2020 2020 2053 706f 746f             Spoto
+0000f080: 626a 6563 742e 7365 7428 7365 6c66 2e64  bject.set(self.d
+0000f090: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000f0a0: 6b5f 6b65 792c 2073 7472 286e 6577 5f64  k_key, str(new_d
+0000f0b0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+0000f0c0: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0e0: 2020 2020 2020 2020 2074 7261 636b 5f69           track_i
+0000f0f0: 6420 3d20 7365 6c66 2e63 6861 6e6e 656c  d = self.channel
+0000f100: 5f75 6e69 7175 655f 7370 6f74 5f70 726f  _unique_spot_pro
+0000f110: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+0000f120: 5f69 6429 5d5b 7365 6c66 2e74 7261 636b  _id)][self.track
+0000f130: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
 0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f150: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000f160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f170: 7365 6c66 2e78 6d6c 5f74 7265 652e 7772  self.xml_tree.wr
-0000f180: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
-0000f190: 2873 656c 662e 6368 616e 6e65 6c5f 786d  (self.channel_xm
-0000f1a0: 6c5f 7061 7468 2c20 7365 6c66 2e63 6861  l_path, self.cha
-0000f1b0: 6e6e 656c 5f78 6d6c 5f6e 616d 6529 2920  nnel_xml_name)) 
-0000f1c0: 0d0a 0d0a 2020 2020 6465 6620 5f67 6574  ....    def _get
-0000f1d0: 5f78 6d6c 5f64 6174 6128 7365 6c66 293a  _xml_data(self):
-0000f1e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0000f1f0: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000f200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f210: 6368 616e 6e65 6c5f 7365 675f 696d 6167  channel_seg_imag
-0000f220: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
-0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f240: 2020 2020 2020 7365 6c66 2e63 6861 6e6e        self.chann
-0000f250: 656c 5f78 6d6c 5f63 6f6e 7465 6e74 203d  el_xml_content =
-0000f260: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000f270: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-0000f280: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
-0000f290: 6c5f 7472 6565 203d 2065 742e 7061 7273  l_tree = et.pars
-0000f2a0: 6528 7365 6c66 2e78 6d6c 5f70 6174 6829  e(self.xml_path)
-0000f2b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f2c0: 2020 2020 2020 2020 7365 6c66 2e78 6d6c          self.xml
-0000f2d0: 5f72 6f6f 7420 3d20 7365 6c66 2e78 6d6c  _root = self.xml
-0000f2e0: 5f74 7265 652e 6765 7472 6f6f 7428 290d  _tree.getroot().
-0000f2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f300: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-0000f310: 6e65 6c5f 786d 6c5f 6e61 6d65 203d 2027  nel_xml_name = '
-0000f320: 7365 636f 6e64 5f63 6861 6e6e 656c 5f27  second_channel_'
-0000f330: 202b 206f 732e 7061 7468 2e73 706c 6974   + os.path.split
-0000f340: 6578 7428 6f73 2e70 6174 682e 6261 7365  ext(os.path.base
-0000f350: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
-0000f360: 7468 2929 5b30 5d20 2b20 272e 786d 6c27  th))[0] + '.xml'
-0000f370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f380: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-0000f390: 6e6e 656c 5f78 6d6c 5f70 6174 6820 3d20  nnel_xml_path = 
-0000f3a0: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0000f3b0: 7365 6c66 2e78 6d6c 5f70 6174 6829 0d0a  self.xml_path)..
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3d0: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
-0000f3e0: 7465 5f63 6861 6e6e 656c 5f74 7265 6528  te_channel_tree(
-0000f3f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000f400: 2020 2069 6620 7365 6c66 2e61 7574 6f65     if self.autoe
-0000f410: 6e63 6f64 6572 5f6d 6f64 656c 2069 7320  ncoder_model is 
-0000f420: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-0000f430: 662e 7365 675f 696d 6167 6520 6973 206e  f.seg_image is n
-0000f440: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f460: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
-0000f470: 5f63 6f6e 7465 6e74 203d 2073 656c 662e  _content = self.
-0000f480: 786d 6c5f 636f 6e74 656e 740d 0a20 2020  xml_content..   
-0000f490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4a0: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000f4b0: 786d 6c5f 7472 6565 203d 2065 742e 7061  xml_tree = et.pa
-0000f4c0: 7273 6528 7365 6c66 2e78 6d6c 5f70 6174  rse(self.xml_pat
-0000f4d0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
-0000f4e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f4f0: 6d61 7374 6572 5f78 6d6c 5f72 6f6f 7420  master_xml_root 
-0000f500: 3d20 7365 6c66 2e6d 6173 7465 725f 786d  = self.master_xm
-0000f510: 6c5f 7472 6565 2e67 6574 726f 6f74 2829  l_tree.getroot()
-0000f520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f530: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-0000f540: 7374 6572 5f78 6d6c 5f6e 616d 6520 3d20  ster_xml_name = 
-0000f550: 276d 6173 7465 725f 2720 2b20 7365 6c66  'master_' + self
-0000f560: 2e6d 6173 7465 725f 6578 7472 615f 6e61  .master_extra_na
-0000f570: 6d65 2020 2b20 6f73 2e70 6174 682e 7370  me  + os.path.sp
-0000f580: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
-0000f590: 6173 656e 616d 6528 7365 6c66 2e78 6d6c  asename(self.xml
-0000f5a0: 5f70 6174 6829 295b 305d 202b 2027 2e78  _path))[0] + '.x
-0000f5b0: 6d6c 270d 0a20 2020 2020 2020 2020 2020  ml'..           
-0000f5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f5d0: 2e6d 6173 7465 725f 786d 6c5f 7061 7468  .master_xml_path
-0000f5e0: 203d 206f 732e 7061 7468 2e64 6972 6e61   = os.path.dirna
-0000f5f0: 6d65 2873 656c 662e 786d 6c5f 7061 7468  me(self.xml_path
-0000f600: 2920 2020 2020 200d 0a20 2020 2020 2020  )      ..       
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f630: 2020 7365 6c66 2e75 6e69 7175 655f 6f62    self.unique_ob
-0000f640: 6a65 6374 7320 3d20 7b7d 0d0a 2020 2020  jects = {}..    
-0000f650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f660: 2e75 6e69 7175 655f 7072 6f70 6572 7469  .unique_properti
-0000f670: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0000f680: 2020 2020 2020 2020 2073 656c 662e 416c           self.Al
-0000f690: 6c54 7261 636b 4964 7320 3d20 5b5d 0d0a  lTrackIds = []..
-0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6b0: 7365 6c66 2e44 6976 6964 696e 6754 7261  self.DividingTra
-0000f6c0: 636b 4964 7320 3d20 5b5d 0d0a 2020 2020  ckIds = []..    
-0000f6d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f6e0: 2e4e 6f72 6d61 6c54 7261 636b 4964 7320  .NormalTrackIds 
-0000f6f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000f700: 2020 2020 2020 7365 6c66 2e61 6c6c 5f74        self.all_t
-0000f710: 7261 636b 5f70 726f 7065 7274 6965 7320  rack_properties 
-0000f720: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0000f730: 2020 2020 2020 7365 6c66 2e73 706c 6974        self.split
-0000f740: 5f70 6f69 6e74 735f 7469 6d65 7320 3d20  _points_times = 
-0000f750: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-0000f760: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000f770: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000f780: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-0000f790: 6c6c 5472 6163 6b49 6473 2e61 7070 656e  llTrackIds.appen
-0000f7a0: 6428 4e6f 6e65 290d 0a20 2020 2020 2020  d(None)..       
-0000f7b0: 2020 2020 2020 2020 2073 656c 662e 4469           self.Di
-0000f7c0: 7669 6469 6e67 5472 6163 6b49 6473 2e61  vidingTrackIds.a
-0000f7d0: 7070 656e 6428 4e6f 6e65 290d 0a20 2020  ppend(None)..   
-0000f7e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f7f0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-0000f800: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
-0000f810: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f830: 2073 656c 662e 416c 6c54 7261 636b 4964   self.AllTrackId
-0000f840: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
-0000f850: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
-0000f860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f870: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
-0000f880: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000f890: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000f8a0: 2020 2020 2020 2020 2020 7365 6c66 2e4e            self.N
-0000f8b0: 6f72 6d61 6c54 7261 636b 4964 732e 6170  ormalTrackIds.ap
-0000f8c0: 7065 6e64 2873 656c 662e 5472 6163 6b69  pend(self.Tracki
-0000f8d0: 6442 6f78 290d 0a20 2020 2020 2020 2020  dBox)..         
-0000f8e0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000f8f0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000f900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f910: 5370 6f74 6f62 6a65 6374 7320 3d20 7365  Spotobjects = se
-0000f920: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000f930: 696e 6428 274d 6f64 656c 2729 2e66 696e  ind('Model').fin
-0000f940: 6428 2741 6c6c 5370 6f74 7327 290d 0a20  d('AllSpots').. 
-0000f950: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f960: 2045 7874 7261 6374 2074 6865 2074 7261   Extract the tra
-0000f970: 636b 7320 6672 6f6d 2078 6d6c 0d0a 2020  cks from xml..  
-0000f980: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f990: 6c66 2e74 7261 636b 7320 3d20 7365 6c66  lf.tracks = self
-0000f9a0: 2e78 6d6c 5f63 6f6e 7465 6e74 2e66 696e  .xml_content.fin
-0000f9b0: 6428 224d 6f64 656c 2229 2e66 696e 6428  d("Model").find(
-0000f9c0: 2241 6c6c 5472 6163 6b73 2229 0d0a 2020  "AllTracks")..  
-0000f9d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f9e0: 6c66 2e73 6574 7469 6e67 7320 3d20 7365  lf.settings = se
-0000f9f0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
-0000fa00: 696e 6428 2253 6574 7469 6e67 7322 292e  ind("Settings").
-0000fa10: 6669 6e64 2822 496d 6167 6544 6174 6122  find("ImageData"
-0000fa20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fa30: 2020 2073 656c 662e 696d 6167 6573 697a     self.imagesiz
-0000fa40: 6520 3d20 2869 6e74 2866 6c6f 6174 2873  e = (int(float(s
-0000fa50: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
-0000fa60: 2822 6e66 7261 6d65 7322 2929 292c 696e  ("nframes"))),in
-0000fa70: 7428 666c 6f61 7428 7365 6c66 2e73 6574  t(float(self.set
-0000fa80: 7469 6e67 732e 6765 7428 226e 736c 6963  tings.get("nslic
-0000fa90: 6573 2229 2929 2c69 6e74 2866 6c6f 6174  es"))),int(float
-0000faa0: 2873 656c 662e 7365 7474 696e 6773 2e67  (self.settings.g
-0000fab0: 6574 2822 6865 6967 6874 2229 2929 2c20  et("height"))), 
-0000fac0: 2069 6e74 2866 6c6f 6174 2873 656c 662e   int(float(self.
-0000fad0: 7365 7474 696e 6773 2e67 6574 2822 7769  settings.get("wi
-0000fae0: 6474 6822 2929 2929 0d0a 2020 2020 2020  dth"))))..      
-0000faf0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000fb00: 6627 584d 4c20 6669 6c65 206d 6164 6520  f'XML file made 
-0000fb10: 7573 696e 6720 696d 6167 6520 6f66 207b  using image of {
-0000fb20: 7365 6c66 2e69 6d61 6765 7369 7a65 7d27  self.imagesize}'
-0000fb30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fb40: 2020 2073 656c 662e 7863 616c 6962 7261     self.xcalibra
-0000fb50: 7469 6f6e 203d 2066 6c6f 6174 2873 656c  tion = float(sel
-0000fb60: 662e 7365 7474 696e 6773 2e67 6574 2822  f.settings.get("
-0000fb70: 7069 7865 6c77 6964 7468 2229 290d 0a20  pixelwidth")).. 
-0000fb80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fb90: 656c 662e 7963 616c 6962 7261 7469 6f6e  elf.ycalibration
-0000fba0: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
-0000fbb0: 7474 696e 6773 2e67 6574 2822 7069 7865  ttings.get("pixe
-0000fbc0: 6c68 6569 6768 7422 2929 0d0a 2020 2020  lheight"))..    
-0000fbd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fbe0: 2e7a 6361 6c69 6272 6174 696f 6e20 3d20  .zcalibration = 
-0000fbf0: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000fc00: 6e67 732e 6765 7428 2276 6f78 656c 6465  ngs.get("voxelde
-0000fc10: 7074 6822 2929 0d0a 2020 2020 2020 2020  pth"))..        
-0000fc20: 2020 2020 2020 2020 7365 6c66 2e74 6361          self.tca
-0000fc30: 6c69 6272 6174 696f 6e20 3d20 696e 7428  libration = int(
-0000fc40: 666c 6f61 7428 7365 6c66 2e73 6574 7469  float(self.setti
-0000fc50: 6e67 732e 6765 7428 2274 696d 6569 6e74  ngs.get("timeint
-0000fc60: 6572 7661 6c22 2929 290d 0a20 2020 2020  erval")))..     
-0000fc70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fc80: 6465 7465 6374 6f72 7365 7474 696e 6773  detectorsettings
-0000fc90: 203d 2073 656c 662e 786d 6c5f 636f 6e74   = self.xml_cont
-0000fca0: 656e 742e 6669 6e64 2822 5365 7474 696e  ent.find("Settin
-0000fcb0: 6773 2229 2e66 696e 6428 2244 6574 6563  gs").find("Detec
-0000fcc0: 746f 7253 6574 7469 6e67 7322 290d 0a20  torSettings").. 
-0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fce0: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
-0000fcf0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
-0000fd00: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
-0000fd10: 6e67 7322 292e 6669 6e64 2822 4261 7369  ngs").find("Basi
-0000fd20: 6353 6574 7469 6e67 7322 290d 0a20 2020  cSettings")..   
-0000fd30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fd40: 662e 6465 7465 6374 6f72 6368 616e 6e65  f.detectorchanne
-0000fd50: 6c20 3d20 696e 7428 666c 6f61 7428 7365  l = int(float(se
-0000fd60: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000fd70: 6e67 732e 6765 7428 2254 4152 4745 545f  ngs.get("TARGET_
-0000fd80: 4348 414e 4e45 4c22 2929 290d 0a20 2020  CHANNEL")))..   
-0000fd90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fda0: 662e 7473 7461 7274 203d 2069 6e74 2866  f.tstart = int(f
-0000fdb0: 6c6f 6174 2873 656c 662e 6261 7369 6373  loat(self.basics
-0000fdc0: 6574 7469 6e67 732e 6765 7428 2274 7374  ettings.get("tst
-0000fdd0: 6172 7422 2929 290d 0a20 2020 2020 2020  art")))..       
-0000fde0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-0000fdf0: 6e64 203d 2069 6e74 2866 6c6f 6174 2873  nd = int(float(s
-0000fe00: 656c 662e 6261 7369 6373 6574 7469 6e67  elf.basicsetting
-0000fe10: 732e 6765 7428 2274 656e 6422 2929 290d  s.get("tend"))).
-0000fe20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe30: 2073 656c 662e 5f67 6574 5f62 6f75 6e64   self._get_bound
-0000fe40: 6172 795f 706f 696e 7473 2829 0d0a 2020  ary_points()..  
-0000fe50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000fe60: 696e 7428 2749 7465 7261 7469 6e67 206f  int('Iterating o
-0000fe70: 7665 7220 7370 6f74 7320 696e 2066 7261  ver spots in fra
-0000fe80: 6d65 2729 0d0a 2020 2020 2020 2020 2020  me')..          
-0000fe90: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
-0000fea0: 203d 2030 0d0a 2020 2020 2020 2020 2020   = 0..          
-0000feb0: 2020 2020 2020 6675 7475 7265 7320 3d20        futures = 
-0000fec0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
-0000fed0: 2020 2020 2020 7769 7468 2063 6f6e 6375        with concu
-0000fee0: 7272 656e 742e 6675 7475 7265 732e 5468  rrent.futures.Th
-0000fef0: 7265 6164 506f 6f6c 4578 6563 7574 6f72  readPoolExecutor
-0000ff00: 286d 6178 5f77 6f72 6b65 7273 203d 206f  (max_workers = o
-0000ff10: 732e 6370 755f 636f 756e 7428 2929 2061  s.cpu_count()) a
-0000ff20: 7320 6578 6563 7574 6f72 3a0d 0a20 2020  s executor:..   
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000ff50: 2020 2020 2020 2066 6f72 2066 7261 6d65         for frame
-0000ff60: 2069 6e20 7365 6c66 2e53 706f 746f 626a   in self.Spotobj
-0000ff70: 6563 7473 2e66 696e 6461 6c6c 2827 5370  ects.findall('Sp
-0000ff80: 6f74 7349 6e46 7261 6d65 2729 3a0d 0a20  otsInFrame'):.. 
-0000ff90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ffa0: 2020 2020 2020 2020 2020 2020 6675 7475              futu
-0000ffb0: 7265 732e 6170 7065 6e64 2865 7865 6375  res.append(execu
-0000ffc0: 746f 722e 7375 626d 6974 2873 656c 662e  tor.submit(self.
-0000ffd0: 5f73 706f 745f 636f 6d70 7574 6572 2c20  _spot_computer, 
-0000ffe0: 6672 616d 6529 290d 0a20 2020 2020 2020  frame))..       
-0000fff0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00010000: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00010010: 7220 6973 206e 6f74 204e 6f6e 653a 0d0a  r is not None:..
-00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010040: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010060: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00010070: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-00010080: 2022 436f 6c6c 6563 7469 6e67 2053 706f   "Collecting Spo
-00010090: 7473 220d 0a20 2020 2020 2020 2020 2020  ts"..           
+0000f150: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+0000f160: 6e6e 656c 5f66 696c 7465 7265 645f 7472  nnel_filtered_tr
+0000f170: 6163 6b73 2e61 7070 656e 6428 7472 6163  acks.append(trac
+0000f180: 6b5f 6964 290d 0a20 2020 2020 2020 2020  k_id)..         
+0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1c0: 2073 656c 662e 786d 6c5f 7472 6565 2e77   self.xml_tree.w
+0000f1d0: 7269 7465 286f 732e 7061 7468 2e6a 6f69  rite(os.path.joi
+0000f1e0: 6e28 7365 6c66 2e63 6861 6e6e 656c 5f78  n(self.channel_x
+0000f1f0: 6d6c 5f70 6174 682c 2073 656c 662e 6368  ml_path, self.ch
+0000f200: 616e 6e65 6c5f 786d 6c5f 6e61 6d65 2929  annel_xml_name))
+0000f210: 200d 0a0d 0a20 2020 2064 6566 205f 6765   ....    def _ge
+0000f220: 745f 786d 6c5f 6461 7461 2873 656c 6629  t_xml_data(self)
+0000f230: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+0000f240: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0000f250: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000f260: 2e63 6861 6e6e 656c 5f73 6567 5f69 6d61  .channel_seg_ima
+0000f270: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
+0000f280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f290: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+0000f2a0: 6e65 6c5f 786d 6c5f 636f 6e74 656e 7420  nel_xml_content 
+0000f2b0: 3d20 7365 6c66 2e78 6d6c 5f63 6f6e 7465  = self.xml_conte
+0000f2c0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+0000f2d0: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+0000f2e0: 6d6c 5f74 7265 6520 3d20 6574 2e70 6172  ml_tree = et.par
+0000f2f0: 7365 2873 656c 662e 786d 6c5f 7061 7468  se(self.xml_path
+0000f300: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f310: 2020 2020 2020 2020 2073 656c 662e 786d           self.xm
+0000f320: 6c5f 726f 6f74 203d 2073 656c 662e 786d  l_root = self.xm
+0000f330: 6c5f 7472 6565 2e67 6574 726f 6f74 2829  l_tree.getroot()
+0000f340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f350: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+0000f360: 6e6e 656c 5f78 6d6c 5f6e 616d 6520 3d20  nnel_xml_name = 
+0000f370: 2773 6563 6f6e 645f 6368 616e 6e65 6c5f  'second_channel_
+0000f380: 2720 2b20 6f73 2e70 6174 682e 7370 6c69  ' + os.path.spli
+0000f390: 7465 7874 286f 732e 7061 7468 2e62 6173  text(os.path.bas
+0000f3a0: 656e 616d 6528 7365 6c66 2e78 6d6c 5f70  ename(self.xml_p
+0000f3b0: 6174 6829 295b 305d 202b 2027 2e78 6d6c  ath))[0] + '.xml
+0000f3c0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
+0000f3d0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+0000f3e0: 616e 6e65 6c5f 786d 6c5f 7061 7468 203d  annel_xml_path =
+0000f3f0: 206f 732e 7061 7468 2e64 6972 6e61 6d65   os.path.dirname
+0000f400: 2873 656c 662e 786d 6c5f 7061 7468 290d  (self.xml_path).
+0000f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f420: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
+0000f430: 6174 655f 6368 616e 6e65 6c5f 7472 6565  ate_channel_tree
+0000f440: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000f450: 2020 2020 6966 2073 656c 662e 6175 746f      if self.auto
+0000f460: 656e 636f 6465 725f 6d6f 6465 6c20 6973  encoder_model is
+0000f470: 206e 6f74 204e 6f6e 6520 616e 6420 7365   not None and se
+0000f480: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
+0000f490: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4b0: 2020 7365 6c66 2e6d 6173 7465 725f 786d    self.master_xm
+0000f4c0: 6c5f 636f 6e74 656e 7420 3d20 7365 6c66  l_content = self
+0000f4d0: 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a 2020  .xml_content..  
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4f0: 2020 2020 2073 656c 662e 6d61 7374 6572       self.master
+0000f500: 5f78 6d6c 5f74 7265 6520 3d20 6574 2e70  _xml_tree = et.p
+0000f510: 6172 7365 2873 656c 662e 786d 6c5f 7061  arse(self.xml_pa
+0000f520: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
+0000f530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f540: 2e6d 6173 7465 725f 786d 6c5f 726f 6f74  .master_xml_root
+0000f550: 203d 2073 656c 662e 6d61 7374 6572 5f78   = self.master_x
+0000f560: 6d6c 5f74 7265 652e 6765 7472 6f6f 7428  ml_tree.getroot(
+0000f570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f580: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0000f590: 6173 7465 725f 786d 6c5f 6e61 6d65 203d  aster_xml_name =
+0000f5a0: 2027 6d61 7374 6572 5f27 202b 2073 656c   'master_' + sel
+0000f5b0: 662e 6d61 7374 6572 5f65 7874 7261 5f6e  f.master_extra_n
+0000f5c0: 616d 6520 202b 206f 732e 7061 7468 2e73  ame  + os.path.s
+0000f5d0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
+0000f5e0: 6261 7365 6e61 6d65 2873 656c 662e 786d  basename(self.xm
+0000f5f0: 6c5f 7061 7468 2929 5b30 5d20 2b20 272e  l_path))[0] + '.
+0000f600: 786d 6c27 0d0a 2020 2020 2020 2020 2020  xml'..          
+0000f610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f620: 662e 6d61 7374 6572 5f78 6d6c 5f70 6174  f.master_xml_pat
+0000f630: 6820 3d20 6f73 2e70 6174 682e 6469 726e  h = os.path.dirn
+0000f640: 616d 6528 7365 6c66 2e78 6d6c 5f70 6174  ame(self.xml_pat
+0000f650: 6829 2020 2020 2020 0d0a 2020 2020 2020  h)      ..      
+0000f660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f670: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f680: 2020 2073 656c 662e 756e 6971 7565 5f6f     self.unique_o
+0000f690: 626a 6563 7473 203d 207b 7d0d 0a20 2020  bjects = {}..   
+0000f6a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f6b0: 662e 756e 6971 7565 5f70 726f 7065 7274  f.unique_propert
+0000f6c0: 6965 7320 3d20 7b7d 0d0a 2020 2020 2020  ies = {}..      
+0000f6d0: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
+0000f6e0: 6c6c 5472 6163 6b49 6473 203d 205b 5d0d  llTrackIds = [].
+0000f6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f700: 2073 656c 662e 4469 7669 6469 6e67 5472   self.DividingTr
+0000f710: 6163 6b49 6473 203d 205b 5d0d 0a20 2020  ackIds = []..   
+0000f720: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f730: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
+0000f740: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000f750: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+0000f760: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
+0000f770: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+0000f780: 2020 2020 2020 2073 656c 662e 7370 6c69         self.spli
+0000f790: 745f 706f 696e 7473 5f74 696d 6573 203d  t_points_times =
+0000f7a0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+0000f7b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000f7c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000f7d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f7e0: 416c 6c54 7261 636b 4964 732e 6170 7065  AllTrackIds.appe
+0000f7f0: 6e64 284e 6f6e 6529 0d0a 2020 2020 2020  nd(None)..      
+0000f800: 2020 2020 2020 2020 2020 7365 6c66 2e44            self.D
+0000f810: 6976 6964 696e 6754 7261 636b 4964 732e  ividingTrackIds.
+0000f820: 6170 7065 6e64 284e 6f6e 6529 0d0a 2020  append(None)..  
+0000f830: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f840: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000f850: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
+0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f880: 2020 7365 6c66 2e41 6c6c 5472 6163 6b49    self.AllTrackI
+0000f890: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000f8a0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000f8b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f8c0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
+0000f8d0: 732e 6170 7065 6e64 2873 656c 662e 5472  s.append(self.Tr
+0000f8e0: 6163 6b69 6442 6f78 290d 0a20 2020 2020  ackidBox)..     
+0000f8f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f900: 4e6f 726d 616c 5472 6163 6b49 6473 2e61  NormalTrackIds.a
+0000f910: 7070 656e 6428 7365 6c66 2e54 7261 636b  ppend(self.Track
+0000f920: 6964 426f 7829 0d0a 2020 2020 2020 2020  idBox)..        
+0000f930: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000f940: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f960: 2e53 706f 746f 626a 6563 7473 203d 2073  .Spotobjects = s
+0000f970: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000f980: 6669 6e64 2827 4d6f 6465 6c27 292e 6669  find('Model').fi
+0000f990: 6e64 2827 416c 6c53 706f 7473 2729 0d0a  nd('AllSpots')..
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9b0: 2320 4578 7472 6163 7420 7468 6520 7472  # Extract the tr
+0000f9c0: 6163 6b73 2066 726f 6d20 786d 6c0d 0a20  acks from xml.. 
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f9e0: 656c 662e 7472 6163 6b73 203d 2073 656c  elf.tracks = sel
+0000f9f0: 662e 786d 6c5f 636f 6e74 656e 742e 6669  f.xml_content.fi
+0000fa00: 6e64 2822 4d6f 6465 6c22 292e 6669 6e64  nd("Model").find
+0000fa10: 2822 416c 6c54 7261 636b 7322 290d 0a20  ("AllTracks").. 
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fa30: 656c 662e 7365 7474 696e 6773 203d 2073  elf.settings = s
+0000fa40: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
+0000fa50: 6669 6e64 2822 5365 7474 696e 6773 2229  find("Settings")
+0000fa60: 2e66 696e 6428 2249 6d61 6765 4461 7461  .find("ImageData
+0000fa70: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000fa80: 2020 2020 7365 6c66 2e69 6d61 6765 7369      self.imagesi
+0000fa90: 7a65 203d 2028 696e 7428 666c 6f61 7428  ze = (int(float(
+0000faa0: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
+0000fab0: 7428 226e 6672 616d 6573 2229 2929 2c69  t("nframes"))),i
+0000fac0: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
+0000fad0: 7474 696e 6773 2e67 6574 2822 6e73 6c69  ttings.get("nsli
+0000fae0: 6365 7322 2929 292c 696e 7428 666c 6f61  ces"))),int(floa
+0000faf0: 7428 7365 6c66 2e73 6574 7469 6e67 732e  t(self.settings.
+0000fb00: 6765 7428 2268 6569 6768 7422 2929 292c  get("height"))),
+0000fb10: 2020 696e 7428 666c 6f61 7428 7365 6c66    int(float(self
+0000fb20: 2e73 6574 7469 6e67 732e 6765 7428 2277  .settings.get("w
+0000fb30: 6964 7468 2229 2929 290d 0a20 2020 2020  idth"))))..     
+0000fb40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000fb50: 2866 2758 4d4c 2066 696c 6520 6d61 6465  (f'XML file made
+0000fb60: 2075 7369 6e67 2069 6d61 6765 206f 6620   using image of 
+0000fb70: 7b73 656c 662e 696d 6167 6573 697a 657d  {self.imagesize}
+0000fb80: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+0000fb90: 2020 2020 7365 6c66 2e78 6361 6c69 6272      self.xcalibr
+0000fba0: 6174 696f 6e20 3d20 666c 6f61 7428 7365  ation = float(se
+0000fbb0: 6c66 2e73 6574 7469 6e67 732e 6765 7428  lf.settings.get(
+0000fbc0: 2270 6978 656c 7769 6474 6822 2929 0d0a  "pixelwidth"))..
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 7365 6c66 2e79 6361 6c69 6272 6174 696f  self.ycalibratio
+0000fbf0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e73  n = float(self.s
+0000fc00: 6574 7469 6e67 732e 6765 7428 2270 6978  ettings.get("pix
+0000fc10: 656c 6865 6967 6874 2229 290d 0a20 2020  elheight"))..   
+0000fc20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fc30: 662e 7a63 616c 6962 7261 7469 6f6e 203d  f.zcalibration =
+0000fc40: 2066 6c6f 6174 2873 656c 662e 7365 7474   float(self.sett
+0000fc50: 696e 6773 2e67 6574 2822 766f 7865 6c64  ings.get("voxeld
+0000fc60: 6570 7468 2229 290d 0a20 2020 2020 2020  epth"))..       
+0000fc70: 2020 2020 2020 2020 2073 656c 662e 7463           self.tc
+0000fc80: 616c 6962 7261 7469 6f6e 203d 2069 6e74  alibration = int
+0000fc90: 2866 6c6f 6174 2873 656c 662e 7365 7474  (float(self.sett
+0000fca0: 696e 6773 2e67 6574 2822 7469 6d65 696e  ings.get("timein
+0000fcb0: 7465 7276 616c 2229 2929 0d0a 2020 2020  terval")))..    
+0000fcc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fcd0: 2e64 6574 6563 746f 7273 6574 7469 6e67  .detectorsetting
+0000fce0: 7320 3d20 7365 6c66 2e78 6d6c 5f63 6f6e  s = self.xml_con
+0000fcf0: 7465 6e74 2e66 696e 6428 2253 6574 7469  tent.find("Setti
+0000fd00: 6e67 7322 292e 6669 6e64 2822 4465 7465  ngs").find("Dete
+0000fd10: 6374 6f72 5365 7474 696e 6773 2229 0d0a  ctorSettings")..
+0000fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd30: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000fd40: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000fd50: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000fd60: 696e 6773 2229 2e66 696e 6428 2242 6173  ings").find("Bas
+0000fd70: 6963 5365 7474 696e 6773 2229 0d0a 2020  icSettings")..  
+0000fd80: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fd90: 6c66 2e64 6574 6563 746f 7263 6861 6e6e  lf.detectorchann
+0000fda0: 656c 203d 2069 6e74 2866 6c6f 6174 2873  el = int(float(s
+0000fdb0: 656c 662e 6465 7465 6374 6f72 7365 7474  elf.detectorsett
+0000fdc0: 696e 6773 2e67 6574 2822 5441 5247 4554  ings.get("TARGET
+0000fdd0: 5f43 4841 4e4e 454c 2229 2929 0d0a 2020  _CHANNEL")))..  
+0000fde0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fdf0: 6c66 2e74 7374 6172 7420 3d20 696e 7428  lf.tstart = int(
+0000fe00: 666c 6f61 7428 7365 6c66 2e62 6173 6963  float(self.basic
+0000fe10: 7365 7474 696e 6773 2e67 6574 2822 7473  settings.get("ts
+0000fe20: 7461 7274 2229 2929 0d0a 2020 2020 2020  tart")))..      
+0000fe30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000fe40: 656e 6420 3d20 696e 7428 666c 6f61 7428  end = int(float(
+0000fe50: 7365 6c66 2e62 6173 6963 7365 7474 696e  self.basicsettin
+0000fe60: 6773 2e67 6574 2822 7465 6e64 2229 2929  gs.get("tend")))
+0000fe70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000fe80: 2020 7365 6c66 2e5f 6765 745f 626f 756e    self._get_boun
+0000fe90: 6461 7279 5f70 6f69 6e74 7328 290d 0a20  dary_points().. 
+0000fea0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000feb0: 7269 6e74 2827 4974 6572 6174 696e 6720  rint('Iterating 
+0000fec0: 6f76 6572 2073 706f 7473 2069 6e20 6672  over spots in fr
+0000fed0: 616d 6527 290d 0a20 2020 2020 2020 2020  ame')..         
+0000fee0: 2020 2020 2020 2073 656c 662e 636f 756e         self.coun
+0000fef0: 7420 3d20 300d 0a20 2020 2020 2020 2020  t = 0..         
+0000ff00: 2020 2020 2020 2066 7574 7572 6573 203d         futures =
+0000ff10: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+0000ff20: 2020 2020 2020 2077 6974 6820 636f 6e63         with conc
+0000ff30: 7572 7265 6e74 2e66 7574 7572 6573 2e54  urrent.futures.T
+0000ff40: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+0000ff50: 7228 6d61 785f 776f 726b 6572 7320 3d20  r(max_workers = 
+0000ff60: 6f73 2e63 7075 5f63 6f75 6e74 2829 2920  os.cpu_count()) 
+0000ff70: 6173 2065 7865 6375 746f 723a 0d0a 2020  as executor:..  
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000ffa0: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
+0000ffb0: 6520 696e 2073 656c 662e 5370 6f74 6f62  e in self.Spotob
+0000ffc0: 6a65 6374 732e 6669 6e64 616c 6c28 2753  jects.findall('S
+0000ffd0: 706f 7473 496e 4672 616d 6527 293a 0d0a  potsInFrame'):..
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fff0: 2020 2020 2020 2020 2020 2020 2066 7574               fut
+00010000: 7572 6573 2e61 7070 656e 6428 6578 6563  ures.append(exec
+00010010: 7574 6f72 2e73 7562 6d69 7428 7365 6c66  utor.submit(self
+00010020: 2e5f 7370 6f74 5f63 6f6d 7075 7465 722c  ._spot_computer,
+00010030: 2066 7261 6d65 2929 0d0a 2020 2020 2020   frame))..      
+00010040: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010050: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+00010060: 6172 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ar is not None:.
+00010070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010090: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000100c0: 6f67 7265 7373 5f62 6172 2e72 616e 6765  ogress_bar.range
-000100d0: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00010100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 2020 2020 2020 6c65 6e28 6675            len(fu
-00010130: 7475 7265 7329 2c0d 0a20 2020 2020 2020  tures),..       
-00010140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010150: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+000100b0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+000100c0: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
+000100d0: 3d20 2243 6f6c 6c65 6374 696e 6720 5370  = "Collecting Sp
+000100e0: 6f74 7322 0d0a 2020 2020 2020 2020 2020  ots"..          
+000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010100: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00010110: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
+00010120: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
+00010130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010140: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00010150: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
 00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010180: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
-00010190: 735f 6261 722e 7368 6f77 2829 0d0a 0d0a  s_bar.show()....
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 2020 2020 666f 7220 7220 696e 2063 6f6e      for r in con
-000101c0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
-000101d0: 6173 5f63 6f6d 706c 6574 6564 2866 7574  as_completed(fut
-000101e0: 7572 6573 293a 0d0a 2020 2020 2020 2020  ures):..        
-000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 7365 6c66 2e63 6f75 6e74 203d 2073 656c  self.count = sel
-00010220: 662e 636f 756e 7420 2b20 310d 0a20 2020  f.count + 1..   
-00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010170: 2020 2020 2020 2020 2020 206c 656e 2866             len(f
+00010180: 7574 7572 6573 292c 0d0a 2020 2020 2020  utures),..      
+00010190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101a0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+000101b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101d0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+000101e0: 7373 5f62 6172 2e73 686f 7728 290d 0a0d  ss_bar.show()...
+000101f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010200: 2020 2020 2066 6f72 2072 2069 6e20 636f       for r in co
+00010210: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
+00010220: 2e61 735f 636f 6d70 6c65 7465 6428 6675  .as_completed(fu
+00010230: 7475 7265 7329 3a0d 0a20 2020 2020 2020  tures):..       
 00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2020 2069 6620 7365 6c66 2e70 726f       if self.pro
-00010260: 6772 6573 735f 6261 7220 6973 206e 6f74  gress_bar is not
-00010270: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 2073 656c 662e 636f 756e 7420 3d20 7365   self.count = se
+00010270: 6c66 2e63 6f75 6e74 202b 2031 0d0a 2020  lf.count + 1..  
 00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000102b0: 5f62 6172 2e76 616c 7565 203d 2020 7365  _bar.value =  se
-000102c0: 6c66 2e63 6f75 6e74 0d0a 2020 2020 2020  lf.count..      
+000102a0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+000102b0: 6f67 7265 7373 5f62 6172 2069 7320 6e6f  ogress_bar is no
+000102c0: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
 000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 722e 7265 7375 6c74 2829 0d0a 2020    r.result()..  
-00010300: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00010310: 696e 7428 6627 4974 6572 6174 696e 6720  int(f'Iterating 
-00010320: 6f76 6572 2074 7261 636b 7320 7b6c 656e  over tracks {len
-00010330: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-00010340: 7261 636b 5f69 6473 297d 2729 2020 0d0a  rack_ids)}')  ..
-00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010360: 7365 6c66 2e63 6f75 6e74 203d 2030 0d0a  self.count = 0..
-00010370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010380: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00010390: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-000103a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000103b0: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000103c0: 7265 7373 5f62 6172 2e6c 6162 656c 203d  ress_bar.label =
-000103d0: 2022 436f 6c6c 6563 7469 6e67 2054 7261   "Collecting Tra
-000103e0: 636b 7322 0d0a 2020 2020 2020 2020 2020  cks"..          
-000103f0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010400: 726f 6772 6573 735f 6261 722e 7261 6e67  rogress_bar.rang
-00010410: 6520 3d20 2830 2c20 6c65 6e28 7365 6c66  e = (0, len(self
-00010420: 2e66 696c 7465 7265 645f 7472 6163 6b5f  .filtered_track_
-00010430: 6964 7329 290d 0a20 2020 2020 2020 2020  ids))..         
+000102f0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010300: 735f 6261 722e 7661 6c75 6520 3d20 2073  s_bar.value =  s
+00010310: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
+00010320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2020 2072 2e72 6573 756c 7428 290d 0a20     r.result().. 
+00010350: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00010360: 7269 6e74 2866 2749 7465 7261 7469 6e67  rint(f'Iterating
+00010370: 206f 7665 7220 7472 6163 6b73 207b 6c65   over tracks {le
+00010380: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
+00010390: 7472 6163 6b5f 6964 7329 7d27 2920 200d  track_ids)}')  .
+000103a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000103b0: 2073 656c 662e 636f 756e 7420 3d20 300d   self.count = 0.
+000103c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000103d0: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
+000103e0: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
+000103f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00010400: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+00010410: 6772 6573 735f 6261 722e 6c61 6265 6c20  gress_bar.label 
+00010420: 3d20 2243 6f6c 6c65 6374 696e 6720 5472  = "Collecting Tr
+00010430: 6163 6b73 220d 0a20 2020 2020 2020 2020  acks"..         
 00010440: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010450: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
-00010460: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-00010470: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00010480: 2020 2020 2020 2020 206d 6178 5f6c 656e           max_len
-00010490: 6774 6820 3d20 3020 2020 200d 0a20 2020  gth = 0    ..   
-000104a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000104b0: 2074 7261 636b 2069 6e20 7365 6c66 2e74   track in self.t
-000104c0: 7261 636b 732e 6669 6e64 616c 6c28 2754  racks.findall('T
-000104d0: 7261 636b 2729 3a0d 0a20 2020 2020 2020  rack'):..       
-000104e0: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-000104f0: 636b 5f69 6420 3d20 696e 7428 7472 6163  ck_id = int(trac
-00010500: 6b2e 6765 7428 7365 6c66 2e74 7261 636b  k.get(self.track
-00010510: 6964 5f6b 6579 2929 0d0a 2020 2020 2020  id_key))..      
-00010520: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010530: 2074 7261 636b 5f69 6420 696e 2073 656c   track_id in sel
-00010540: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
-00010550: 5f69 6473 3a0d 0a20 2020 2020 2020 2020  _ids:..         
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010570: 2020 2064 6967 6974 5f6c 656e 6774 6820     digit_length 
-00010580: 3d20 6c65 6e28 7374 7228 7472 6163 6b5f  = len(str(track_
-00010590: 6964 2929 0d0a 2020 2020 2020 2020 2020  id))..          
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 2020 6966 2064 6967 6974 5f6c 656e 6774    if digit_lengt
-000105c0: 6820 3e20 6d61 785f 6c65 6e67 7468 3a0d  h > max_length:.
-000105d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105f0: 206d 6178 5f6c 656e 6774 6820 3d20 6469   max_length = di
-00010600: 6769 745f 6c65 6e67 7468 0d0a 2020 2020  git_length..    
-00010610: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010620: 2e6d 6178 5f74 7261 636b 5f64 6967 6974  .max_track_digit
-00010630: 203d 206d 6178 5f6c 656e 6774 6820 2020   = max_length   
-00010640: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00010650: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010660: 6f72 2074 7261 636b 2069 6e20 7365 6c66  or track in self
-00010670: 2e74 7261 636b 732e 6669 6e64 616c 6c28  .tracks.findall(
-00010680: 2754 7261 636b 2729 3a0d 0a20 2020 2020  'Track'):..     
-00010690: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000106a0: 7261 636b 5f69 6420 3d20 696e 7428 7472  rack_id = int(tr
-000106b0: 6163 6b2e 6765 7428 7365 6c66 2e74 7261  ack.get(self.tra
-000106c0: 636b 6964 5f6b 6579 2929 0d0a 2020 2020  ckid_key))..    
-000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 6966 2074 7261 636b 5f69 6420 696e 2073  if track_id in s
-000106f0: 656c 662e 6669 6c74 6572 6564 5f74 7261  elf.filtered_tra
-00010700: 636b 5f69 6473 3a0d 0a20 2020 2020 2020  ck_ids:..       
-00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010720: 2073 656c 662e 5f74 7261 636b 5f63 6f6d   self._track_com
-00010730: 7075 7465 7228 7472 6163 6b2c 2074 7261  puter(track, tra
-00010740: 636b 5f69 6429 0d0a 2020 2020 2020 2020  ck_id)..        
-00010750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010760: 7365 6c66 2e63 6f75 6e74 202b 3d20 310d  self.count += 1.
-00010770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010780: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010790: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-000107a0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107c0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
-000107d0: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
-000107e0: 3d20 7365 6c66 2e63 6f75 6e74 0d0a 2020  = self.count..  
-000107f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010800: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
-00010810: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
-00010820: 6f6e 653a 2020 0d0a 2020 2020 2020 2020  one:  ..        
-00010830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010840: 656c 662e 5f63 7265 6174 655f 7365 636f  elf._create_seco
-00010850: 6e64 5f63 6861 6e6e 656c 5f78 6d6c 2829  nd_channel_xml()
-00010860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010870: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
-00010880: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
-00010890: 696e 2073 656c 662e 6772 6170 685f 7370  in self.graph_sp
-000108a0: 6c69 742e 6974 656d 7328 293a 0d0a 2020  lit.items():..  
-000108b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2020 2020 2064 6175 6768 7465 725f         daughter_
-000108f0: 7472 6163 6b5f 6964 203d 2020 696e 7428  track_id =  int(
-00010900: 666c 6f61 7428 7374 7228 7365 6c66 2e75  float(str(self.u
-00010910: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00010920: 7274 6965 735b 696e 7428 666c 6f61 7428  rties[int(float(
-00010930: 6b29 295d 5b73 656c 662e 756e 6971 7565  k))][self.unique
-00010940: 6964 5f6b 6579 5d29 2929 0d0a 2020 2020  id_key])))..    
-00010950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010960: 2020 2020 2020 2020 7061 7265 6e74 5f74          parent_t
-00010970: 7261 636b 5f69 6420 3d20 696e 7428 666c  rack_id = int(fl
-00010980: 6f61 7428 7374 7228 7365 6c66 2e75 6e69  oat(str(self.uni
-00010990: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000109a0: 6965 735b 696e 7428 666c 6f61 7428 7629  ies[int(float(v)
-000109b0: 295d 5b73 656c 662e 756e 6971 7565 6964  )][self.uniqueid
-000109c0: 5f6b 6579 5d29 2929 0d0a 2020 2020 2020  _key])))..      
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 2020 7365 6c66 2e67 7261 7068        self.graph
-000109f0: 5f74 7261 636b 735b 6461 7567 6874 6572  _tracks[daughter
-00010a00: 5f74 7261 636b 5f69 645d 203d 2070 6172  _track_id] = par
-00010a10: 656e 745f 7472 6163 6b5f 6964 0d0a 2020  ent_track_id..  
-00010a20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010a30: 6c66 2e5f 6765 745f 6174 7472 6962 7574  lf._get_attribut
-00010a40: 6573 2829 0d0a 2020 2020 2020 2020 2020  es()..          
-00010a50: 2020 2020 2020 6966 2073 656c 662e 6175        if self.au
-00010a60: 746f 656e 636f 6465 725f 6d6f 6465 6c20  toencoder_model 
-00010a70: 616e 6420 7365 6c66 2e73 6567 5f69 6d61  and self.seg_ima
-00010a80: 6765 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ge is not None:.
-00010a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010aa0: 2020 2020 2020 2020 7072 696e 7428 2747          print('G
-00010ab0: 6574 7469 6e67 2061 7574 6f65 6e63 6f64  etting autoencod
-00010ac0: 6572 2063 6c6f 7564 7327 290d 0a20 2020  er clouds')..   
-00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ae0: 2020 2020 7365 6c66 2e5f 6173 7369 676e      self._assign
-00010af0: 5f63 6c75 7374 6572 5f63 6c61 7373 2829  _cluster_class()
-00010b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010b10: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00010b20: 4372 6561 7469 6e67 206d 6173 7465 7220  Creating master 
-00010b30: 786d 6c27 290d 0a20 2020 2020 2020 2020  xml')..         
-00010b40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010b50: 6c66 2e5f 6372 6561 7465 5f6d 6173 7465  lf._create_maste
-00010b60: 725f 786d 6c28 290d 0a20 2020 2020 2020  r_xml()..       
-00010b70: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010b80: 756e 7420 3d20 3020 0d0a 2020 2020 2020  unt = 0 ..      
-00010b90: 2020 2020 2020 2020 2020 666f 7220 7472            for tr
-00010ba0: 6163 6b5f 6964 2069 6e20 7365 6c66 2e66  ack_id in self.f
-00010bb0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-00010bc0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00010bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010be0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00010bf0: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
-00010c00: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010450: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+00010460: 6765 203d 2028 302c 206c 656e 2873 656c  ge = (0, len(sel
+00010470: 662e 6669 6c74 6572 6564 5f74 7261 636b  f.filtered_track
+00010480: 5f69 6473 2929 0d0a 2020 2020 2020 2020  _ids))..        
+00010490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000104a0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
+000104b0: 6f77 2829 0d0a 0d0a 2020 2020 2020 2020  ow()....        
+000104c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000104d0: 2020 2020 2020 2020 2020 6d61 785f 6c65            max_le
+000104e0: 6e67 7468 203d 2030 2020 2020 0d0a 2020  ngth = 0    ..  
+000104f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010500: 7220 7472 6163 6b20 696e 2073 656c 662e  r track in self.
+00010510: 7472 6163 6b73 2e66 696e 6461 6c6c 2827  tracks.findall('
+00010520: 5472 6163 6b27 293a 0d0a 2020 2020 2020  Track'):..      
+00010530: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00010540: 6163 6b5f 6964 203d 2069 6e74 2874 7261  ack_id = int(tra
+00010550: 636b 2e67 6574 2873 656c 662e 7472 6163  ck.get(self.trac
+00010560: 6b69 645f 6b65 7929 290d 0a20 2020 2020  kid_key))..     
+00010570: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010580: 6620 7472 6163 6b5f 6964 2069 6e20 7365  f track_id in se
+00010590: 6c66 2e66 696c 7465 7265 645f 7472 6163  lf.filtered_trac
+000105a0: 6b5f 6964 733a 0d0a 2020 2020 2020 2020  k_ids:..        
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 2020 2020 6469 6769 745f 6c65 6e67 7468      digit_length
+000105d0: 203d 206c 656e 2873 7472 2874 7261 636b   = len(str(track
+000105e0: 5f69 6429 290d 0a20 2020 2020 2020 2020  _id))..         
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2069 6620 6469 6769 745f 6c65 6e67     if digit_leng
+00010610: 7468 203e 206d 6178 5f6c 656e 6774 683a  th > max_length:
+00010620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010640: 2020 6d61 785f 6c65 6e67 7468 203d 2064    max_length = d
+00010650: 6967 6974 5f6c 656e 6774 680d 0a20 2020  igit_length..   
+00010660: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010670: 662e 6d61 785f 7472 6163 6b5f 6469 6769  f.max_track_digi
+00010680: 7420 3d20 6d61 785f 6c65 6e67 7468 2020  t = max_length  
+00010690: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106b0: 666f 7220 7472 6163 6b20 696e 2073 656c  for track in sel
+000106c0: 662e 7472 6163 6b73 2e66 696e 6461 6c6c  f.tracks.findall
+000106d0: 2827 5472 6163 6b27 293a 0d0a 2020 2020  ('Track'):..    
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 7472 6163 6b5f 6964 203d 2069 6e74 2874  track_id = int(t
+00010700: 7261 636b 2e67 6574 2873 656c 662e 7472  rack.get(self.tr
+00010710: 6163 6b69 645f 6b65 7929 290d 0a20 2020  ackid_key))..   
+00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010730: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
+00010740: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+00010750: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
+00010760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010770: 2020 7365 6c66 2e5f 7472 6163 6b5f 636f    self._track_co
+00010780: 6d70 7574 6572 2874 7261 636b 2c20 7472  mputer(track, tr
+00010790: 6163 6b5f 6964 290d 0a20 2020 2020 2020  ack_id)..       
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 2073 656c 662e 636f 756e 7420 2b3d 2031   self.count += 1
+000107c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000107d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000107e0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
+000107f0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010810: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010820: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
+00010830: 203d 2073 656c 662e 636f 756e 740d 0a20   = self.count.. 
+00010840: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010850: 6620 7365 6c66 2e63 6861 6e6e 656c 5f73  f self.channel_s
+00010860: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
+00010870: 4e6f 6e65 3a20 200d 0a20 2020 2020 2020  None:  ..       
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 7365 6c66 2e5f 6372 6561 7465 5f73 6563  self._create_sec
+000108a0: 6f6e 645f 6368 616e 6e65 6c5f 786d 6c28  ond_channel_xml(
+000108b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000108c0: 2020 200d 0a0d 0a20 2020 2020 2020 2020     ....         
+000108d0: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
+000108e0: 2069 6e20 7365 6c66 2e67 7261 7068 5f73   in self.graph_s
+000108f0: 706c 6974 2e69 7465 6d73 2829 3a0d 0a20  plit.items():.. 
+00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010910: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00010920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010930: 2020 2020 2020 2020 6461 7567 6874 6572          daughter
+00010940: 5f74 7261 636b 5f69 6420 3d20 2069 6e74  _track_id =  int
+00010950: 2866 6c6f 6174 2873 7472 2873 656c 662e  (float(str(self.
+00010960: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00010970: 6572 7469 6573 5b69 6e74 2866 6c6f 6174  erties[int(float
+00010980: 286b 2929 5d5b 7365 6c66 2e75 6e69 7175  (k))][self.uniqu
+00010990: 6569 645f 6b65 795d 2929 290d 0a20 2020  eid_key])))..   
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 2020 2020 2020 2020 2070 6172 656e 745f           parent_
+000109c0: 7472 6163 6b5f 6964 203d 2069 6e74 2866  track_id = int(f
+000109d0: 6c6f 6174 2873 7472 2873 656c 662e 756e  loat(str(self.un
+000109e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000109f0: 7469 6573 5b69 6e74 2866 6c6f 6174 2876  ties[int(float(v
+00010a00: 2929 5d5b 7365 6c66 2e75 6e69 7175 6569  ))][self.uniquei
+00010a10: 645f 6b65 795d 2929 290d 0a20 2020 2020  d_key])))..     
+00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a30: 2020 2020 2020 2073 656c 662e 6772 6170         self.grap
+00010a40: 685f 7472 6163 6b73 5b64 6175 6768 7465  h_tracks[daughte
+00010a50: 725f 7472 6163 6b5f 6964 5d20 3d20 7061  r_track_id] = pa
+00010a60: 7265 6e74 5f74 7261 636b 5f69 640d 0a20  rent_track_id.. 
+00010a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010a80: 656c 662e 5f67 6574 5f61 7474 7269 6275  elf._get_attribu
+00010a90: 7465 7328 290d 0a20 2020 2020 2020 2020  tes()..         
+00010aa0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+00010ab0: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
+00010ac0: 2061 6e64 2073 656c 662e 7365 675f 696d   and self.seg_im
+00010ad0: 6167 6520 6973 206e 6f74 204e 6f6e 653a  age is not None:
+00010ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010af0: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00010b00: 4765 7474 696e 6720 6175 746f 656e 636f  Getting autoenco
+00010b10: 6465 7220 636c 6f75 6473 2729 0d0a 2020  der clouds')..  
+00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b30: 2020 2020 2073 656c 662e 5f61 7373 6967       self._assig
+00010b40: 6e5f 636c 7573 7465 725f 636c 6173 7328  n_cluster_class(
+00010b50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010b60: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00010b70: 2743 7265 6174 696e 6720 6d61 7374 6572  'Creating master
+00010b80: 2078 6d6c 2729 0d0a 2020 2020 2020 2020   xml')..        
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010ba0: 656c 662e 5f63 7265 6174 655f 6d61 7374  elf._create_mast
+00010bb0: 6572 5f78 6d6c 2829 0d0a 2020 2020 2020  er_xml()..      
+00010bc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00010bd0: 6f75 6e74 203d 2030 200d 0a20 2020 2020  ount = 0 ..     
+00010be0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00010bf0: 7261 636b 5f69 6420 696e 2073 656c 662e  rack_id in self.
+00010c00: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
+00010c10: 6473 3a0d 0a20 2020 2020 2020 2020 2020  ds:..           
 00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c30: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00010c40: 5f62 6172 2e6c 6162 656c 203d 2022 4a75  _bar.label = "Ju
-00010c50: 7374 206f 6e65 206d 6f72 6520 7468 696e  st one more thin
-00010c60: 6722 0d0a 2020 2020 2020 2020 2020 2020  g"..            
+00010c30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010c40: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
+00010c50: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010c90: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-00010ca0: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
-00010cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c80: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010c90: 735f 6261 722e 6c61 6265 6c20 3d20 224a  s_bar.label = "J
+00010ca0: 7573 7420 6f6e 6520 6d6f 7265 2074 6869  ust one more thi
+00010cb0: 6e67 220d 0a20 2020 2020 2020 2020 2020  ng"..           
 00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2020 2020 2020 2020 2030 2c0d 0a20 2020           0,..   
-00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00010d10: 2873 656c 662e 6669 6c74 6572 6564 5f74  (self.filtered_t
-00010d20: 7261 636b 5f69 6473 292c 0d0a 2020 2020  rack_ids),..    
+00010cd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010ce0: 662e 7072 6f67 7265 7373 5f62 6172 2e72  f.progress_bar.r
+00010cf0: 616e 6765 203d 2028 0d0a 2020 2020 2020  ange = (..      
+00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d20: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
 00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d80: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00010d90: 5f62 6172 2e73 686f 7728 290d 0a20 2020  _bar.show()..   
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d50: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00010d60: 6e28 7365 6c66 2e66 696c 7465 7265 645f  n(self.filtered_
+00010d70: 7472 6163 6b5f 6964 7329 2c0d 0a20 2020  track_ids),..   
+00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010da0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
 00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 2020 2073 656c 662e 636f 756e 7420       self.count 
-00010dd0: 3d20 7365 6c66 2e63 6f75 6e74 202b 2031  = self.count + 1
-00010de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010dd0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010de0: 735f 6261 722e 7368 6f77 2829 0d0a 2020  s_bar.show()..  
 00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010e10: 726f 6772 6573 735f 6261 722e 7661 6c75  rogress_bar.valu
-00010e20: 6520 3d20 7365 6c66 2e63 6f75 6e74 0d0a  e = self.count..
-00010e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e10: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+00010e20: 203d 2073 656c 662e 636f 756e 7420 2b20   = self.count + 
+00010e30: 310d 0a20 2020 2020 2020 2020 2020 2020  1..             
 00010e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e50: 2020 2020 7365 6c66 2e5f 6669 6e61 6c5f      self._final_
-00010e60: 7472 6163 6b73 2874 7261 636b 5f69 6429  tracks(track_id)
-00010e70: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00010e80: 2020 2020 2069 6620 7365 6c66 2e66 6f75       if self.fou
-00010e90: 7269 6572 3a0d 0a20 2020 2020 2020 2020  rier:..         
-00010ea0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00010eb0: 2763 6f6d 7075 7469 6e67 2046 6f75 7269  'computing Fouri
-00010ec0: 6572 2729 0d0a 2020 2020 2020 2020 2020  er')..          
-00010ed0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
-00010ee0: 6f6d 7075 7465 5f70 6865 6e6f 7479 7065  ompute_phenotype
-00010ef0: 7328 2920 2020 2020 2020 2020 2020 2020  s()             
-00010f00: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00010f10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010f20: 662e 5f74 656d 706f 7261 6c5f 706c 6f74  f._temporal_plot
-00010f30: 735f 7472 6163 6b6d 6174 6528 290d 0a20  s_trackmate().. 
-00010f40: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00010f50: 0a0d 0a20 2020 2064 6566 205f 6372 6561  ...    def _crea
-00010f60: 7465 5f6d 6173 7465 725f 786d 6c28 7365  te_master_xml(se
-00010f70: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-00010f80: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00010f90: 2020 2020 2020 2020 666f 7220 5370 6f74          for Spot
-00010fa0: 6f62 6a65 6374 2069 6e20 7365 6c66 2e6d  object in self.m
-00010fb0: 6173 7465 725f 786d 6c5f 726f 6f74 2e69  aster_xml_root.i
-00010fc0: 7465 7228 2753 706f 7427 293a 0d0a 2020  ter('Spot'):..  
-00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fe0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00010ff0: 6c6c 5f69 6420 3d20 696e 7428 5370 6f74  ll_id = int(Spot
-00011000: 6f62 6a65 6374 2e67 6574 2873 656c 662e  object.get(self.
-00011010: 7370 6f74 6964 5f6b 6579 2929 0d0a 2020  spotid_key))..  
+00010e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010e60: 7072 6f67 7265 7373 5f62 6172 2e76 616c  progress_bar.val
+00010e70: 7565 203d 2073 656c 662e 636f 756e 740d  ue = self.count.
+00010e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ea0: 2020 2020 2073 656c 662e 5f66 696e 616c       self._final
+00010eb0: 5f74 7261 636b 7328 7472 6163 6b5f 6964  _tracks(track_id
+00010ec0: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
+00010ed0: 2020 2020 2020 6966 2073 656c 662e 666f        if self.fo
+00010ee0: 7572 6965 723a 0d0a 2020 2020 2020 2020  urier:..        
+00010ef0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00010f00: 2827 636f 6d70 7574 696e 6720 466f 7572  ('computing Four
+00010f10: 6965 7227 290d 0a20 2020 2020 2020 2020  ier')..         
+00010f20: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00010f30: 636f 6d70 7574 655f 7068 656e 6f74 7970  compute_phenotyp
+00010f40: 6573 2829 2020 2020 2020 2020 2020 2020  es()            
+00010f50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00010f60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010f70: 6c66 2e5f 7465 6d70 6f72 616c 5f70 6c6f  lf._temporal_plo
+00010f80: 7473 5f74 7261 636b 6d61 7465 2829 0d0a  ts_trackmate()..
+00010f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fa0: 0d0a 0d0a 2020 2020 6465 6620 5f63 7265  ....    def _cre
+00010fb0: 6174 655f 6d61 7374 6572 5f78 6d6c 2873  ate_master_xml(s
+00010fc0: 656c 6629 3a0d 0a20 2020 2020 2020 2020  elf):..         
+00010fd0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+00010fe0: 2020 2020 2020 2020 2066 6f72 2053 706f           for Spo
+00010ff0: 746f 626a 6563 7420 696e 2073 656c 662e  tobject in self.
+00011000: 6d61 7374 6572 5f78 6d6c 5f72 6f6f 742e  master_xml_root.
+00011010: 6974 6572 2827 5370 6f74 2729 3a0d 0a20  iter('Spot'):.. 
 00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011040: 2063 656c 6c5f 6964 2069 6e20 7365 6c66   cell_id in self
-00011050: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00011060: 7065 7274 6965 732e 6b65 7973 2829 3a0d  perties.keys():.
-00011070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110c0: 2066 6f72 206b 2069 6e20 7365 6c66 2e75   for k in self.u
-000110d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000110e0: 7274 6965 735b 6365 6c6c 5f69 645d 2e6b  rties[cell_id].k
-000110f0: 6579 7328 293a 0d0a 0d0a 2020 2020 2020  eys():....      
+00011030: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011040: 656c 6c5f 6964 203d 2069 6e74 2853 706f  ell_id = int(Spo
+00011050: 746f 626a 6563 742e 6765 7428 7365 6c66  tobject.get(self
+00011060: 2e73 706f 7469 645f 6b65 7929 290d 0a20  .spotid_key)).. 
+00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011090: 6620 6365 6c6c 5f69 6420 696e 2073 656c  f cell_id in sel
+000110a0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000110b0: 6f70 6572 7469 6573 2e6b 6579 7328 293a  operties.keys():
+000110c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000110d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000110e0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000110f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 2020 2020 2053 706f 746f 626a 6563 742e       Spotobject.
-00011130: 7365 7428 6b2c 2073 7472 2873 656c 662e  set(k, str(self.
-00011140: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00011150: 6572 7469 6573 5b63 656c 6c5f 6964 5d5b  erties[cell_id][
-00011160: 6b5d 2929 2020 200d 0a0d 0a20 2020 2020  k]))   ....     
-00011170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-000111a0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
-000111b0: 7472 6565 2e77 7269 7465 286f 732e 7061  tree.write(os.pa
-000111c0: 7468 2e6a 6f69 6e28 7365 6c66 2e6d 6173  th.join(self.mas
-000111d0: 7465 725f 786d 6c5f 7061 7468 2c20 7365  ter_xml_path, se
-000111e0: 6c66 2e6d 6173 7465 725f 786d 6c5f 6e61  lf.master_xml_na
-000111f0: 6d65 2929 0d0a 2020 2020 2020 2020 2020  me))..          
-00011200: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00011210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011220: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011250: 2020 200d 0a0d 0a20 2020 2064 6566 205f     ....    def _
-00011260: 6173 7369 676e 5f63 6c75 7374 6572 5f63  assign_cluster_c
-00011270: 6c61 7373 2873 656c 6629 3a0d 0a20 2020  lass(self):..   
-00011280: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00011290: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000112a0: 6c66 2e61 7865 7320 3d20 7365 6c66 2e61  lf.axes = self.a
-000112b0: 7865 732e 7265 706c 6163 6528 2254 222c  xes.replace("T",
-000112c0: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
-000112d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 666f 7220 636f 756e 742c 2074 696d 655f  for count, time_
-00011300: 6b65 7920 696e 2065 6e75 6d65 7261 7465  key in enumerate
-00011310: 2873 656c 662e 5f74 696d 6564 5f63 656e  (self._timed_cen
-00011320: 7472 6f69 642e 6b65 7973 2829 293a 0d0a  troid.keys()):..
+00011110: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
+00011120: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00011130: 6572 7469 6573 5b63 656c 6c5f 6964 5d2e  erties[cell_id].
+00011140: 6b65 7973 2829 3a0d 0a0d 0a20 2020 2020  keys():....     
+00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011170: 2020 2020 2020 5370 6f74 6f62 6a65 6374        Spotobject
+00011180: 2e73 6574 286b 2c20 7374 7228 7365 6c66  .set(k, str(self
+00011190: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000111a0: 7065 7274 6965 735b 6365 6c6c 5f69 645d  perties[cell_id]
+000111b0: 5b6b 5d29 2920 2020 0d0a 0d0a 2020 2020  [k]))   ....    
+000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111e0: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+000111f0: 2073 656c 662e 6d61 7374 6572 5f78 6d6c   self.master_xml
+00011200: 5f74 7265 652e 7772 6974 6528 6f73 2e70  _tree.write(os.p
+00011210: 6174 682e 6a6f 696e 2873 656c 662e 6d61  ath.join(self.ma
+00011220: 7374 6572 5f78 6d6c 5f70 6174 682c 2073  ster_xml_path, s
+00011230: 656c 662e 6d61 7374 6572 5f78 6d6c 5f6e  elf.master_xml_n
+00011240: 616d 6529 290d 0a20 2020 2020 2020 2020  ame))..         
+00011250: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00011260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011270: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00011280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112a0: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
+000112b0: 5f61 7373 6967 6e5f 636c 7573 7465 725f  _assign_cluster_
+000112c0: 636c 6173 7328 7365 6c66 293a 0d0a 2020  class(self):..  
+000112d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000112f0: 656c 662e 6178 6573 203d 2073 656c 662e  elf.axes = self.
+00011300: 6178 6573 2e72 6570 6c61 6365 2822 5422  axes.replace("T"
+00011310: 2c20 2222 290d 0a20 2020 2020 2020 2020  , "")..         
+00011320: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
 00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011340: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 2020 2020 7472 6565 2c20 7370          tree, sp
-00011370: 6f74 5f63 656e 7472 6f69 6473 203d 2073  ot_centroids = s
-00011380: 656c 662e 5f74 696d 6564 5f63 656e 7472  elf._timed_centr
-00011390: 6f69 645b 7469 6d65 5f6b 6579 5d0d 0a20  oid[time_key].. 
+00011340: 2066 6f72 2063 6f75 6e74 2c20 7469 6d65   for count, time
+00011350: 5f6b 6579 2069 6e20 656e 756d 6572 6174  _key in enumerat
+00011360: 6528 7365 6c66 2e5f 7469 6d65 645f 6365  e(self._timed_ce
+00011370: 6e74 726f 6964 2e6b 6579 7328 2929 3a0d  ntroid.keys()):.
+00011380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011390: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000113c0: 662e 7072 6f67 7265 7373 5f62 6172 2069  f.progress_bar i
-000113d0: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011400: 662e 7072 6f67 7265 7373 5f62 6172 2e6c  f.progress_bar.l
-00011410: 6162 656c 203d 2022 4175 746f 656e 636f  abel = "Autoenco
-00011420: 6465 7220 666f 7220 7265 6669 6e69 6e67  der for refining
-00011430: 2070 6f69 6e74 2063 6c6f 7564 7322 0d0a   point clouds"..
-00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011470: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
-00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2020 2020 2020 2020 2074 7265 652c 2073           tree, s
+000113c0: 706f 745f 6365 6e74 726f 6964 7320 3d20  pot_centroids = 
+000113d0: 7365 6c66 2e5f 7469 6d65 645f 6365 6e74  self._timed_cent
+000113e0: 726f 6964 5b74 696d 655f 6b65 795d 0d0a  roid[time_key]..
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00011410: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+00011420: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011450: 6c66 2e70 726f 6772 6573 735f 6261 722e  lf.progress_bar.
+00011460: 6c61 6265 6c20 3d20 2241 7574 6f65 6e63  label = "Autoenc
+00011470: 6f64 6572 2066 6f72 2072 6566 696e 696e  oder for refinin
+00011480: 6720 706f 696e 7420 636c 6f75 6473 220d  g point clouds".
+00011490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
-000114c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114b0: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
+000114c0: 6172 2e72 616e 6765 203d 2028 0d0a 2020  ar.range = (..  
 000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011500: 206c 656e 2873 656c 662e 5f74 696d 6564   len(self._timed
-00011510: 5f63 656e 7472 6f69 642e 6b65 7973 2829  _centroid.keys()
-00011520: 2920 2b20 312c 0d0a 2020 2020 2020 2020  ) + 1,..        
+00011500: 2020 2020 2020 2020 2020 2020 2020 302c                0,
+00011510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011560: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-00011590: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-000115a0: 2020 636f 756e 7420 0d0a 2020 2020 2020    count ..      
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000115d0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-000115e0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011600: 2063 6c75 7374 6572 5f65 7661 6c20 3d20   cluster_eval = 
-00011610: 436c 7573 7465 7269 6e67 2873 656c 662e  Clustering(self.
-00011620: 6163 6365 6c65 7261 746f 722c 2073 656c  accelerator, sel
-00011630: 662e 6465 7669 6365 732c 2073 656c 662e  f.devices, self.
-00011640: 7365 675f 696d 6167 655b 696e 7428 7469  seg_image[int(ti
-00011650: 6d65 5f6b 6579 292c 3a5d 2c20 2073 656c  me_key),:],  sel
-00011660: 662e 6178 6573 2c20 7365 6c66 2e6e 756d  f.axes, self.num
-00011670: 5f70 6f69 6e74 732c 2073 656c 662e 6175  _points, self.au
-00011680: 746f 656e 636f 6465 725f 6d6f 6465 6c2c  toencoder_model,
-00011690: 206b 6579 203d 2074 696d 655f 6b65 792c   key = time_key,
-000116a0: 2070 726f 6772 6573 735f 6261 723d 7365   progress_bar=se
-000116b0: 6c66 2e70 726f 6772 6573 735f 6261 722c  lf.progress_bar,
-000116c0: 2062 6174 6368 5f73 697a 6520 3d20 7365   batch_size = se
-000116d0: 6c66 2e62 6174 6368 5f73 697a 652c 2073  lf.batch_size, s
-000116e0: 6361 6c65 5f7a 3d73 656c 662e 7363 616c  cale_z=self.scal
-000116f0: 655f 7a2c 2073 6361 6c65 5f78 793d 2073  e_z, scale_xy= s
-00011700: 656c 662e 7363 616c 655f 7879 2c20 6365  elf.scale_xy, ce
-00011710: 6e74 6572 203d 2073 656c 662e 6365 6e74  nter = self.cent
-00011720: 6572 2920 2020 2020 2020 0d0a 2020 2020  er)       ..    
-00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011740: 2020 2020 2020 2063 6c75 7374 6572 5f65         cluster_e
-00011750: 7661 6c2e 5f63 7265 6174 655f 636c 7573  val._create_clus
-00011760: 7465 725f 6c61 6265 6c73 2829 0d0a 2020  ter_labels()..  
-00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 2020 2020 2074 696d 6564 5f63           timed_c
-00011790: 6c75 7374 6572 5f6c 6162 656c 203d 2063  luster_label = c
-000117a0: 6c75 7374 6572 5f65 7661 6c2e 7469 6d65  luster_eval.time
-000117b0: 645f 636c 7573 7465 725f 6c61 6265 6c20  d_cluster_label 
-000117c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000117d0: 2020 2020 2020 2020 2020 2020 206f 7574               out
-000117e0: 7075 745f 6c61 6265 6c73 2c20 206f 7574  put_labels,  out
-000117f0: 7075 745f 636c 7573 7465 725f 6365 6e74  put_cluster_cent
-00011800: 726f 6964 2c20 6f75 7470 7574 5f63 6c6f  roid, output_clo
-00011810: 7564 5f65 6363 656e 7472 6963 6974 792c  ud_eccentricity,
-00011820: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
-00011830: 6569 6765 6e76 6563 746f 722c 206f 7574  eigenvector, out
-00011840: 7075 745f 6c61 7267 6573 745f 6569 6765  put_largest_eige
-00011850: 6e76 616c 7565 2c20 6f75 7470 7574 5f64  nvalue, output_d
-00011860: 696d 656e 7369 6f6e 732c 206f 7574 7075  imensions, outpu
-00011870: 745f 636c 6f75 645f 7375 7266 6163 655f  t_cloud_surface_
-00011880: 6172 6561 203d 2074 696d 6564 5f63 6c75  area = timed_clu
-00011890: 7374 6572 5f6c 6162 656c 5b74 696d 655f  ster_label[time_
-000118a0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
-000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118c0: 2073 6361 6c65 5f31 203d 2031 0d0a 2020   scale_1 = 1..  
-000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118e0: 2020 2020 2020 2020 2073 6361 6c65 5f32           scale_2
-000118f0: 203d 2031 0d0a 2020 2020 2020 2020 2020   = 1..          
+00011550: 2020 6c65 6e28 7365 6c66 2e5f 7469 6d65    len(self._time
+00011560: 645f 6365 6e74 726f 6964 2e6b 6579 7328  d_centroid.keys(
+00011570: 2929 202b 2031 2c0d 0a20 2020 2020 2020  )) + 1,..       
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115b0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115d0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+000115e0: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+000115f0: 3d20 2063 6f75 6e74 200d 0a20 2020 2020  =  count ..     
+00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011610: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011620: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+00011630: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
+00011640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011650: 2020 636c 7573 7465 725f 6576 616c 203d    cluster_eval =
+00011660: 2043 6c75 7374 6572 696e 6728 7365 6c66   Clustering(self
+00011670: 2e61 6363 656c 6572 6174 6f72 2c20 7365  .accelerator, se
+00011680: 6c66 2e64 6576 6963 6573 2c20 7365 6c66  lf.devices, self
+00011690: 2e73 6567 5f69 6d61 6765 5b69 6e74 2874  .seg_image[int(t
+000116a0: 696d 655f 6b65 7929 2c3a 5d2c 2020 7365  ime_key),:],  se
+000116b0: 6c66 2e61 7865 732c 2073 656c 662e 6e75  lf.axes, self.nu
+000116c0: 6d5f 706f 696e 7473 2c20 7365 6c66 2e61  m_points, self.a
+000116d0: 7574 6f65 6e63 6f64 6572 5f6d 6f64 656c  utoencoder_model
+000116e0: 2c20 6b65 7920 3d20 7469 6d65 5f6b 6579  , key = time_key
+000116f0: 2c20 7072 6f67 7265 7373 5f62 6172 3d73  , progress_bar=s
+00011700: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00011710: 2c20 6261 7463 685f 7369 7a65 203d 2073  , batch_size = s
+00011720: 656c 662e 6261 7463 685f 7369 7a65 2c20  elf.batch_size, 
+00011730: 7363 616c 655f 7a3d 7365 6c66 2e73 6361  scale_z=self.sca
+00011740: 6c65 5f7a 2c20 7363 616c 655f 7879 3d20  le_z, scale_xy= 
+00011750: 7365 6c66 2e73 6361 6c65 5f78 792c 2063  self.scale_xy, c
+00011760: 656e 7465 7220 3d20 7365 6c66 2e63 656e  enter = self.cen
+00011770: 7465 7229 2020 2020 2020 200d 0a20 2020  ter)       ..   
+00011780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011790: 2020 2020 2020 2020 636c 7573 7465 725f          cluster_
+000117a0: 6576 616c 2e5f 6372 6561 7465 5f63 6c75  eval._create_clu
+000117b0: 7374 6572 5f6c 6162 656c 7328 290d 0a20  ster_labels().. 
+000117c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117d0: 2020 2020 2020 2020 2020 7469 6d65 645f            timed_
+000117e0: 636c 7573 7465 725f 6c61 6265 6c20 3d20  cluster_label = 
+000117f0: 636c 7573 7465 725f 6576 616c 2e74 696d  cluster_eval.tim
+00011800: 6564 5f63 6c75 7374 6572 5f6c 6162 656c  ed_cluster_label
+00011810: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00011820: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00011830: 7470 7574 5f6c 6162 656c 732c 2020 6f75  tput_labels,  ou
+00011840: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+00011850: 7472 6f69 642c 206f 7574 7075 745f 636c  troid, output_cl
+00011860: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
+00011870: 2c20 6f75 7470 7574 5f6c 6172 6765 7374  , output_largest
+00011880: 5f65 6967 656e 7665 6374 6f72 2c20 6f75  _eigenvector, ou
+00011890: 7470 7574 5f6c 6172 6765 7374 5f65 6967  tput_largest_eig
+000118a0: 656e 7661 6c75 652c 206f 7574 7075 745f  envalue, output_
+000118b0: 6469 6d65 6e73 696f 6e73 2c20 6f75 7470  dimensions, outp
+000118c0: 7574 5f63 6c6f 7564 5f73 7572 6661 6365  ut_cloud_surface
+000118d0: 5f61 7265 6120 3d20 7469 6d65 645f 636c  _area = timed_cl
+000118e0: 7573 7465 725f 6c61 6265 6c5b 7469 6d65  uster_label[time
+000118f0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
 00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00011920: 6c65 6e28 6f75 7470 7574 5f63 6c75 7374  len(output_clust
-00011930: 6572 5f63 656e 7472 6f69 6429 293a 0d0a  er_centroid)):..
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011910: 2020 7363 616c 655f 3120 3d20 310d 0a20    scale_1 = 1.. 
+00011920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011930: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
+00011940: 3220 3d20 310d 0a20 2020 2020 2020 2020  2 = 1..         
 00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 2020 2020 6365 6e74 726f 6964 203d 206f      centroid = o
-00011970: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
-00011980: 6e74 726f 6964 5b69 5d0d 0a20 2020 2020  ntroid[i]..     
-00011990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119a0: 2020 2020 2020 2020 2020 2020 2020 2071                 q
-000119b0: 7561 6c69 7479 203d 206f 7574 7075 745f  uality = output_
-000119c0: 6c61 7267 6573 745f 6569 6765 6e76 616c  largest_eigenval
-000119d0: 7565 5b69 5d0d 0a20 2020 2020 2020 2020  ue[i]..         
+00011960: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00011970: 286c 656e 286f 7574 7075 745f 636c 7573  (len(output_clus
+00011980: 7465 725f 6365 6e74 726f 6964 2929 3a0d  ter_centroid)):.
+00011990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119b0: 2020 2020 2063 656e 7472 6f69 6420 3d20       centroid = 
+000119c0: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
+000119d0: 656e 7472 6f69 645b 695d 0d0a 2020 2020  entroid[i]..    
 000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 2020 2020 2020 2020 2020 2065 6363 656e             eccen
-00011a00: 7472 6963 6974 795f 636f 6d70 5f66 6972  tricity_comp_fir
-00011a10: 7374 797a 203d 206f 7574 7075 745f 636c  styz = output_cl
-00011a20: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
-00011a30: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
-00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 2020 2020 2020 2065 7373 656e 7472           essentr
-00011a60: 6963 6974 795f 6469 6d65 6e73 696f 6e20  icity_dimension 
-00011a70: 3d20 6f75 7470 7574 5f64 696d 656e 7369  = output_dimensi
-00011a80: 6f6e 735b 695d 200d 0a20 2020 2020 2020  ons[i] ..       
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 7175 616c 6974 7920 3d20 6f75 7470 7574  quality = output
+00011a10: 5f6c 6172 6765 7374 5f65 6967 656e 7661  _largest_eigenva
+00011a20: 6c75 655b 695d 0d0a 2020 2020 2020 2020  lue[i]..        
+00011a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a40: 2020 2020 2020 2020 2020 2020 6563 6365              ecce
+00011a50: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
+00011a60: 7273 7479 7a20 3d20 6f75 7470 7574 5f63  rstyz = output_c
+00011a70: 6c6f 7564 5f65 6363 656e 7472 6963 6974  loud_eccentricit
+00011a80: 795b 695d 0d0a 2020 2020 2020 2020 2020  y[i]..          
 00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011aa0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011ab0: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011ac0: 656e 7369 6f6e 5b30 5d20 3d3d 2032 3a0d  ension[0] == 2:.
-00011ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011aa0: 2020 2020 2020 2020 2020 6573 7365 6e74            essent
+00011ab0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
+00011ac0: 203d 206f 7574 7075 745f 6469 6d65 6e73   = output_dimens
+00011ad0: 696f 6e73 5b69 5d20 0d0a 2020 2020 2020  ions[i] ..      
 00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-00011b00: 655f 3120 3d20 7365 6c66 2e7a 6361 6c69  e_1 = self.zcali
-00011b10: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011b00: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011b10: 6d65 6e73 696f 6e5b 305d 203d 3d20 323a  mension[0] == 2:
+00011b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
-00011b50: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
-00011b60: 203d 3d20 313a 0d0a 2020 2020 2020 2020   == 1:..        
+00011b40: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011b50: 6c65 5f31 203d 2073 656c 662e 7a63 616c  le_1 = self.zcal
+00011b60: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
 00011b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00011ba0: 3220 3d20 7365 6c66 2e79 6361 6c69 6272  2 = self.ycalibr
-00011bb0: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
+00011b90: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00011ba0: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
+00011bb0: 5d20 3d3d 2031 3a0d 0a20 2020 2020 2020  ] == 1:..       
 00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011be0: 6573 7365 6e74 7269 6369 7479 5f64 696d  essentricity_dim
-00011bf0: 656e 7369 6f6e 5b30 5d20 3d3d 2032 3a0d  ension[0] == 2:.
-00011c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011bf0: 5f32 203d 2073 656c 662e 7963 616c 6962  _2 = self.ycalib
+00011c00: 7261 7469 6f6e 0d0a 0d0a 2020 2020 2020  ration....      
 00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c20: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-00011c30: 655f 3120 3d20 7365 6c66 2e7a 6361 6c69  e_1 = self.zcali
-00011c40: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011c30: 2065 7373 656e 7472 6963 6974 795f 6469   essentricity_di
+00011c40: 6d65 6e73 696f 6e5b 305d 203d 3d20 323a  mension[0] == 2:
+00011c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2020 6966 2065 7373 656e 7472 6963      if essentric
-00011c80: 6974 795f 6469 6d65 6e73 696f 6e5b 315d  ity_dimension[1]
-00011c90: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00011c70: 2020 2020 2020 2020 2020 2020 2073 6361               sca
+00011c80: 6c65 5f31 203d 2073 656c 662e 7a63 616c  le_1 = self.zcal
+00011c90: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
 00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cc0: 2020 2020 2020 2020 2020 7363 616c 655f            scale_
-00011cd0: 3220 3d20 7365 6c66 2e78 6361 6c69 6272  2 = self.xcalibr
-00011ce0: 6174 696f 6e20 2020 0d0a 0d0a 2020 2020  ation   ....    
+00011cc0: 2020 2020 2069 6620 6573 7365 6e74 7269       if essentri
+00011cd0: 6369 7479 5f64 696d 656e 7369 6f6e 5b31  city_dimension[1
+00011ce0: 5d20 3d3d 2030 3a0d 0a20 2020 2020 2020  ] == 0:..       
 00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d10: 6966 2065 7373 656e 7472 6963 6974 795f  if essentricity_
-00011d20: 6469 6d65 6e73 696f 6e5b 305d 203d 3d20  dimension[0] == 
-00011d30: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00011d10: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+00011d20: 5f32 203d 2073 656c 662e 7863 616c 6962  _2 = self.xcalib
+00011d30: 7261 7469 6f6e 2020 200d 0a0d 0a20 2020  ration   ....   
 00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011d60: 6361 6c65 5f31 203d 2073 656c 662e 7963  cale_1 = self.yc
-00011d70: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d60: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
+00011d70: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
+00011d80: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
 00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2020 2069 6620 6573 7365 6e74         if essent
-00011db0: 7269 6369 7479 5f64 696d 656e 7369 6f6e  ricity_dimension
-00011dc0: 5b31 5d20 3d3d 2030 3a0d 0a20 2020 2020  [1] == 0:..     
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 7363 616c 655f 3120 3d20 7365 6c66 2e79  scale_1 = self.y
+00011dc0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
 00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00011e00: 6c65 5f32 203d 2073 656c 662e 7863 616c  le_2 = self.xcal
-00011e10: 6962 7261 7469 6f6e 2020 0d0a 0d0a 2020  ibration  ....  
+00011df0: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
+00011e00: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
+00011e10: 6e5b 315d 203d 3d20 303a 0d0a 2020 2020  n[1] == 0:..    
 00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e40: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
-00011e50: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
-00011e60: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+00011e40: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00011e50: 616c 655f 3220 3d20 7365 6c66 2e78 6361  ale_2 = self.xca
+00011e60: 6c69 6272 6174 696f 6e20 200d 0a0d 0a20  libration  .... 
 00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
-00011ea0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e90: 2020 2069 6620 6573 7365 6e74 7269 6369     if essentrici
+00011ea0: 7479 5f64 696d 656e 7369 6f6e 5b30 5d20  ty_dimension[0] 
+00011eb0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
 00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ed0: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
-00011ee0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
-00011ef0: 6f6e 5b31 5d20 3d3d 2032 3a0d 0a20 2020  on[1] == 2:..   
+00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ee0: 2020 7363 616c 655f 3120 3d20 7365 6c66    scale_1 = self
+00011ef0: 2e79 6361 6c69 6272 6174 696f 6e0d 0a20  .ycalibration.. 
 00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011f30: 6361 6c65 5f32 203d 2073 656c 662e 7a63  cale_2 = self.zc
-00011f40: 616c 6962 7261 7469 6f6e 2020 2020 2020  alibration      
-00011f50: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00011f20: 2020 2020 2020 2020 2020 6966 2065 7373            if ess
+00011f30: 656e 7472 6963 6974 795f 6469 6d65 6e73  entricity_dimens
+00011f40: 696f 6e5b 315d 203d 3d20 323a 0d0a 2020  ion[1] == 2:..  
+00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-00011f90: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
-00011fa0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00011f80: 7363 616c 655f 3220 3d20 7365 6c66 2e7a  scale_2 = self.z
+00011f90: 6361 6c69 6272 6174 696f 6e20 2020 2020  calibration     
+00011fa0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
 00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 7363 616c 655f 3120 3d20 7365 6c66 2e78  scale_1 = self.x
-00011fe0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00011ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fd0: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00011fe0: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
+00011ff0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
 00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012010: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
-00012020: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
-00012030: 6e5b 315d 203d 3d20 313a 0d0a 2020 2020  n[1] == 1:..    
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
+00012030: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
 00012040: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012060: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00012070: 616c 655f 3220 3d20 7365 6c66 2e79 6361  ale_2 = self.yca
-00012080: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
+00012060: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+00012070: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+00012080: 6f6e 5b31 5d20 3d3d 2031 3a0d 0a20 2020  on[1] == 1:..   
 00012090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2069 6620 6573 7365 6e74 7269 6369 7479   if essentricity
-000120c0: 5f64 696d 656e 7369 6f6e 5b30 5d20 3d3d  _dimension[0] ==
-000120d0: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+000120b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000120c0: 6361 6c65 5f32 203d 2073 656c 662e 7963  cale_2 = self.yc
+000120d0: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
 000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 7363 616c 655f 3120 3d20 7365 6c66 2e78  scale_1 = self.x
-00012110: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 6966 2065 7373 656e 7472 6963 6974    if essentricit
+00012110: 795f 6469 6d65 6e73 696f 6e5b 305d 203d  y_dimension[0] =
+00012120: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
 00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 2020 2020 2020 6966 2065 7373 656e          if essen
-00012150: 7472 6963 6974 795f 6469 6d65 6e73 696f  tricity_dimensio
-00012160: 6e5b 315d 203d 3d20 323a 0d0a 2020 2020  n[1] == 2:..    
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2073 6361 6c65 5f31 203d 2073 656c 662e   scale_1 = self.
+00012160: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
 00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000121a0: 616c 655f 3220 3d20 7365 6c66 2e7a 6361  ale_2 = self.zca
-000121b0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00012190: 2020 2020 2020 2020 2069 6620 6573 7365           if esse
+000121a0: 6e74 7269 6369 7479 5f64 696d 656e 7369  ntricity_dimensi
+000121b0: 6f6e 5b31 5d20 3d3d 2032 3a0d 0a20 2020  on[1] == 2:..   
 000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000121f0: 6361 6c65 5f32 203d 2073 656c 662e 7a63  cale_2 = self.zc
+00012200: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
 00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012220: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012240: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 6365 6c6c 5f61 7869 7320 3d20      cell_axis = 
-00012280: 6f75 7470 7574 5f6c 6172 6765 7374 5f65  output_largest_e
-00012290: 6967 656e 7665 6374 6f72 5b69 5d0d 0a20  igenvector[i].. 
-000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012270: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012290: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000122a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 2020 2073 7572 6661 6365 5f61 7265 6120     surface_area 
-000122d0: 3d20 6f75 7470 7574 5f63 6c6f 7564 5f73  = output_cloud_s
-000122e0: 7572 6661 6365 5f61 7265 615b 695d 202a  urface_area[i] *
-000122f0: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00012300: 6f6e 202a 2073 656c 662e 7963 616c 6962  on * self.ycalib
-00012310: 7261 7469 6f6e 202a 2073 656c 662e 7863  ration * self.xc
-00012320: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 6469 7374 2c20 696e 6465 7820 3d20 7472  dist, index = tr
-00012360: 6565 2e71 7565 7279 2863 656e 7472 6f69  ee.query(centroi
-00012370: 6429 0d0a 2020 2020 2020 2020 2020 2020  d)..            
+000122c0: 2020 2020 2063 656c 6c5f 6178 6973 203d       cell_axis =
+000122d0: 206f 7574 7075 745f 6c61 7267 6573 745f   output_largest_
+000122e0: 6569 6765 6e76 6563 746f 725b 695d 0d0a  eigenvector[i]..
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 2020 2020 7375 7266 6163 655f 6172 6561      surface_area
+00012320: 203d 206f 7574 7075 745f 636c 6f75 645f   = output_cloud_
+00012330: 7375 7266 6163 655f 6172 6561 5b69 5d20  surface_area[i] 
+00012340: 2a20 7365 6c66 2e7a 6361 6c69 6272 6174  * self.zcalibrat
+00012350: 696f 6e20 2a20 7365 6c66 2e79 6361 6c69  ion * self.ycali
+00012360: 6272 6174 696f 6e20 2a20 7365 6c66 2e78  bration * self.x
+00012370: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012390: 2020 2020 2020 2020 7261 6469 7573 203d          radius =
-000123a0: 2071 7561 6c69 7479 202a 206d 6174 682e   quality * math.
-000123b0: 706f 7728 7365 6c66 2e7a 6361 6c69 6272  pow(self.zcalibr
-000123c0: 6174 696f 6e20 2a20 7365 6c66 2e78 6361  ation * self.xca
-000123d0: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
-000123e0: 2e79 6361 6c69 6272 6174 696f 6e2c 2031  .ycalibration, 1
-000123f0: 2e30 2f33 2e30 290d 0a20 2020 2020 2020  .0/3.0)..       
-00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012410: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012420: 6469 7374 203c 2071 7561 6c69 7479 3a0d  dist < quality:.
-00012430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012450: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
-00012460: 7365 7374 5f63 656e 7472 6f69 6420 3d20  sest_centroid = 
-00012470: 7370 6f74 5f63 656e 7472 6f69 6473 5b69  spot_centroids[i
-00012480: 6e64 6578 5d0d 0a20 2020 2020 2020 2020  ndex]..         
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 2064 6973 742c 2069 6e64 6578 203d 2074   dist, index = t
+000123b0: 7265 652e 7175 6572 7928 6365 6e74 726f  ree.query(centro
+000123c0: 6964 290d 0a20 2020 2020 2020 2020 2020  id)..           
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123e0: 2020 2020 2020 2020 2072 6164 6975 7320           radius 
+000123f0: 3d20 7175 616c 6974 7920 2a20 6d61 7468  = quality * math
+00012400: 2e70 6f77 2873 656c 662e 7a63 616c 6962  .pow(self.zcalib
+00012410: 7261 7469 6f6e 202a 2073 656c 662e 7863  ration * self.xc
+00012420: 616c 6962 7261 7469 6f6e 202a 2073 656c  alibration * sel
+00012430: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+00012440: 312e 302f 332e 3029 0d0a 2020 2020 2020  1.0/3.0)..      
+00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012460: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012470: 2064 6973 7420 3c20 7175 616c 6974 793a   dist < quality:
+00012480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124b0: 2020 2066 7261 6d65 5f73 706f 745f 6365     frame_spot_ce
-000124c0: 6e74 726f 6964 203d 2028 696e 7428 7469  ntroid = (int(ti
-000124d0: 6d65 5f6b 6579 292c 636c 6f73 6573 745f  me_key),closest_
-000124e0: 6365 6e74 726f 6964 5b30 5d2c 2063 6c6f  centroid[0], clo
-000124f0: 7365 7374 5f63 656e 7472 6f69 645b 315d  sest_centroid[1]
-00012500: 2c20 636c 6f73 6573 745f 6365 6e74 726f  , closest_centro
-00012510: 6964 5b32 5d29 0d0a 2020 2020 2020 2020  id[2])..        
-00012520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012540: 2020 2020 636c 6f73 6573 745f 6365 6c6c      closest_cell
-00012550: 5f69 6420 3d20 7365 6c66 2e75 6e69 7175  _id = self.uniqu
-00012560: 655f 7370 6f74 5f63 656e 7472 6f69 645b  e_spot_centroid[
-00012570: 6672 616d 655f 7370 6f74 5f63 656e 7472  frame_spot_centr
-00012580: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 6d61 736b 5f76 6563 746f 7220 3d20    mask_vector = 
-000125c0: 5b20 666c 6f61 7428 7365 6c66 2e75 6e69  [ float(self.uni
-000125d0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000125e0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-000125f0: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
-00012600: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
-00012610: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
-00012620: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00012630: 6572 7469 6573 5b69 6e74 2863 6c6f 7365  erties[int(close
-00012640: 7374 5f63 656c 6c5f 6964 295d 5b73 656c  st_cell_id)][sel
-00012650: 662e 6d61 736b 6365 6e74 726f 6964 5f79  f.maskcentroid_y
-00012660: 5f6b 6579 5d29 2c20 666c 6f61 7428 7365  _key]), float(se
-00012670: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00012680: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
-00012690: 6f73 6573 745f 6365 6c6c 5f69 6429 5d5b  osest_cell_id)][
-000126a0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
-000126b0: 645f 7a5f 6b65 795d 2920 5d0d 0a20 2020  d_z_key]) ]..   
-000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000126e0: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-000126f0: 6973 5f6d 6173 6b20 3d20 616e 6775 6c61  is_mask = angula
-00012700: 725f 6368 616e 6765 2863 656c 6c5f 6178  r_change(cell_ax
-00012710: 6973 2c20 6d61 736b 5f76 6563 746f 7229  is, mask_vector)
-00012720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012780: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00012790: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
-000127a0: 6573 745f 6365 6c6c 5f69 6429 5d2e 7570  est_cell_id)].up
-000127b0: 6461 7465 287b 7365 6c66 2e63 656c 6c61  date({self.cella
-000127c0: 7869 735f 6d61 736b 5f6b 6579 203a 2063  xis_mask_key : c
-000127d0: 656c 6c5f 6178 6973 5f6d 6173 6b7d 290d  ell_axis_mask}).
-000127e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012800: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012810: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012820: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00012830: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012840: 5d5b 7365 6c66 2e72 6164 6975 735f 6b65  ][self.radius_ke
-00012850: 795d 203e 2030 3a0d 0a20 2020 2020 2020  y] > 0:..       
-00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012890: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000128a0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-000128b0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-000128c0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-000128d0: 6e74 7269 6369 7479 5f63 6f6d 705f 6669  ntricity_comp_fi
-000128e0: 7273 746b 6579 203a 2065 6363 656e 7472  rstkey : eccentr
-000128f0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00012900: 797a 5b30 5d20 2a20 7363 616c 655f 317d  yz[0] * scale_1}
-00012910: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012950: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012960: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012970: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012980: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-00012990: 7479 5f63 6f6d 705f 7365 636f 6e64 6b65  ty_comp_secondke
-000129a0: 7920 3a20 6563 6365 6e74 7269 6369 7479  y : eccentricity
-000129b0: 5f63 6f6d 705f 6669 7273 7479 7a5b 315d  _comp_firstyz[1]
-000129c0: 202a 2073 6361 6c65 5f32 7d29 0d0a 2020   * scale_2})..  
-000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a00: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00012a10: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00012a20: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
-00012a30: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00012a40: 2e73 7572 6661 6365 5f61 7265 615f 6b65  .surface_area_ke
-00012a50: 7920 3a20 7375 7266 6163 655f 6172 6561  y : surface_area
-00012a60: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012aa0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00012ab0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00012ac0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00012ad0: 287b 7365 6c66 2e71 7561 6c69 7479 5f6b  ({self.quality_k
-00012ae0: 6579 203a 2071 7561 6c69 7479 7d29 0d0a  ey : quality})..
-00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b20: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012b30: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012b40: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012b50: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00012b60: 6c66 2e72 6164 6975 735f 6b65 7920 3a20  lf.radius_key : 
-00012b70: 7261 6469 7573 207d 290d 0a20 2020 2020  radius })..     
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ba0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00012bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124a0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+000124b0: 6f73 6573 745f 6365 6e74 726f 6964 203d  osest_centroid =
+000124c0: 2073 706f 745f 6365 6e74 726f 6964 735b   spot_centroids[
+000124d0: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012500: 2020 2020 6672 616d 655f 7370 6f74 5f63      frame_spot_c
+00012510: 656e 7472 6f69 6420 3d20 2869 6e74 2874  entroid = (int(t
+00012520: 696d 655f 6b65 7929 2c63 6c6f 7365 7374  ime_key),closest
+00012530: 5f63 656e 7472 6f69 645b 305d 2c20 636c  _centroid[0], cl
+00012540: 6f73 6573 745f 6365 6e74 726f 6964 5b31  osest_centroid[1
+00012550: 5d2c 2063 6c6f 7365 7374 5f63 656e 7472  ], closest_centr
+00012560: 6f69 645b 325d 290d 0a20 2020 2020 2020  oid[2])..       
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012590: 2020 2020 2063 6c6f 7365 7374 5f63 656c       closest_cel
+000125a0: 6c5f 6964 203d 2073 656c 662e 756e 6971  l_id = self.uniq
+000125b0: 7565 5f73 706f 745f 6365 6e74 726f 6964  ue_spot_centroid
+000125c0: 5b66 7261 6d65 5f73 706f 745f 6365 6e74  [frame_spot_cent
+000125d0: 726f 6964 5d0d 0a20 2020 2020 2020 2020  roid]..         
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012600: 2020 206d 6173 6b5f 7665 6374 6f72 203d     mask_vector =
+00012610: 205b 2066 6c6f 6174 2873 656c 662e 756e   [ float(self.un
+00012620: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00012630: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00012640: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
+00012650: 6d61 736b 6365 6e74 726f 6964 5f78 5f6b  maskcentroid_x_k
+00012660: 6579 5d29 2c20 666c 6f61 7428 7365 6c66  ey]), float(self
+00012670: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00012680: 7065 7274 6965 735b 696e 7428 636c 6f73  perties[int(clos
+00012690: 6573 745f 6365 6c6c 5f69 6429 5d5b 7365  est_cell_id)][se
+000126a0: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+000126b0: 795f 6b65 795d 292c 2066 6c6f 6174 2873  y_key]), float(s
+000126c0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000126d0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000126e0: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
+000126f0: 5b73 656c 662e 6d61 736b 6365 6e74 726f  [self.maskcentro
+00012700: 6964 5f7a 5f6b 6579 5d29 205d 0d0a 2020  id_z_key]) ]..  
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012730: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
+00012740: 7869 735f 6d61 736b 203d 2061 6e67 756c  xis_mask = angul
+00012750: 6172 5f63 6861 6e67 6528 6365 6c6c 5f61  ar_change(cell_a
+00012760: 7869 732c 206d 6173 6b5f 7665 6374 6f72  xis, mask_vector
+00012770: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012790: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000127a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000127d0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+000127e0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
+000127f0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
+00012800: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
+00012810: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
+00012820: 6365 6c6c 5f61 7869 735f 6d61 736b 7d29  cell_axis_mask})
+00012830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012860: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012870: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012880: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012890: 295d 5b73 656c 662e 7261 6469 7573 5f6b  )][self.radius_k
+000128a0: 6579 5d20 3e20 303a 0d0a 2020 2020 2020  ey] > 0:..      
+000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000128e0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000128f0: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012900: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00012910: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+00012920: 656e 7472 6963 6974 795f 636f 6d70 5f66  entricity_comp_f
+00012930: 6972 7374 6b65 7920 3a20 6563 6365 6e74  irstkey : eccent
+00012940: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
+00012950: 7479 7a5b 305d 202a 2073 6361 6c65 5f31  tyz[0] * scale_1
+00012960: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012990: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+000129a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+000129b0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+000129c0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000129d0: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
+000129e0: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
+000129f0: 6579 203a 2065 6363 656e 7472 6963 6974  ey : eccentricit
+00012a00: 795f 636f 6d70 5f66 6972 7374 797a 5b31  y_comp_firstyz[1
+00012a10: 5d20 2a20 7363 616c 655f 327d 290d 0a20  ] * scale_2}).. 
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00012a60: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00012a70: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
+00012a80: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00012a90: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+00012aa0: 6579 203a 2073 7572 6661 6365 5f61 7265  ey : surface_are
+00012ab0: 617d 290d 0a20 2020 2020 2020 2020 2020  a})..           
+00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00012af0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00012b00: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
+00012b10: 5f63 656c 6c5f 6964 295d 2e75 7064 6174  _cell_id)].updat
+00012b20: 6528 7b73 656c 662e 7175 616c 6974 795f  e({self.quality_
+00012b30: 6b65 7920 3a20 7175 616c 6974 797d 290d  key : quality}).
+00012b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b70: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012b80: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00012b90: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00012ba0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00012bb0: 656c 662e 7261 6469 7573 5f6b 6579 203a  elf.radius_key :
+00012bc0: 2072 6164 6975 7320 7d29 0d0a 2020 2020   radius })..    
 00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012be0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
 00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c10: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012c20: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012c30: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012c40: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012c50: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-00012c60: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-00012c70: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00012cb0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00012cc0: 6f70 6572 7469 6573 5b69 6e74 2863 6c6f  operties[int(clo
-00012cd0: 7365 7374 5f63 656c 6c5f 6964 295d 2e75  sest_cell_id)].u
-00012ce0: 7064 6174 6528 7b73 656c 662e 6563 6365  pdate({self.ecce
-00012cf0: 6e74 7269 6369 7479 5f63 6f6d 705f 7365  ntricity_comp_se
-00012d00: 636f 6e64 6b65 7920 3a20 2d31 7d29 0d0a  condkey : -1})..
-00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012d50: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00012d60: 696e 7428 636c 6f73 6573 745f 6365 6c6c  int(closest_cell
-00012d70: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00012d80: 6c66 2e73 7572 6661 6365 5f61 7265 615f  lf.surface_area_
-00012d90: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012dd0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00012de0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00012df0: 636c 6f73 6573 745f 6365 6c6c 5f69 6429  closest_cell_id)
-00012e00: 5d2e 7570 6461 7465 287b 7365 6c66 2e71  ].update({self.q
-00012e10: 7561 6c69 7479 5f6b 6579 203a 202d 317d  uality_key : -1}
-00012e20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-00012e60: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00012e70: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-00012e80: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012e90: 7b73 656c 662e 7261 6469 7573 5f6b 6579  {self.radius_key
-00012ea0: 203a 202d 3120 7d29 0d0a 2020 2020 2020   : -1 })..      
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-00012ee0: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2020  .......         
-00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f00: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c60: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00012c70: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012c80: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012c90: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00012ca0: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
+00012cb0: 6974 795f 636f 6d70 5f66 6972 7374 6b65  ity_comp_firstke
+00012cc0: 7920 3a20 2d31 7d29 0d0a 2020 2020 2020  y : -1})..      
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012d00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00012d10: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00012d20: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00012d30: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+00012d40: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00012d50: 6563 6f6e 646b 6579 203a 202d 317d 290d  econdkey : -1}).
+00012d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012da0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00012db0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00012dc0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00012dd0: 656c 662e 7375 7266 6163 655f 6172 6561  elf.surface_area
+00012de0: 5f6b 6579 203a 202d 317d 290d 0a20 2020  _key : -1})..   
+00012df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e20: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00012e30: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00012e40: 2863 6c6f 7365 7374 5f63 656c 6c5f 6964  (closest_cell_id
+00012e50: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00012e60: 7175 616c 6974 795f 6b65 7920 3a20 2d31  quality_key : -1
+00012e70: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ea0: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00012eb0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00012ec0: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00012ed0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00012ee0: 287b 7365 6c66 2e72 6164 6975 735f 6b65  ({self.radius_ke
+00012ef0: 7920 3a20 2d31 207d 290d 0a20 2020 2020  y : -1 })..     
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 2020 2020 666f 7220 286b 2c76          for (k,v
-00012f30: 2920 696e 2073 656c 662e 726f 6f74 5f73  ) in self.root_s
-00012f40: 706f 7473 2e69 7465 6d73 2829 3a0d 0a20  pots.items():.. 
-00012f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012f30: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f70: 2073 656c 662e 726f 6f74 5f73 706f 7473   self.root_spots
-00012f80: 5b6b 5d20 3d20 7365 6c66 2e75 6e69 7175  [k] = self.uniqu
-00012f90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012fa0: 735b 6b5d 2020 2020 2020 2020 200d 0a20  s[k]         .. 
-00012fb0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00012fc0: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
-00012fd0: 655f 7068 656e 6f74 7970 6573 2873 656c  e_phenotypes(sel
-00012fe0: 6629 3a0d 0a0d 0a20 2020 2020 2020 2020  f):....         
-00012ff0: 2066 6f72 2028 6b2c 7629 2069 6e20 7365   for (k,v) in se
-00013000: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
-00013010: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00013020: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00013030: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00013040: 636b 5f69 6420 3d20 6b0d 0a20 2020 2020  ck_id = k..     
-00013050: 2020 2020 2020 2020 2020 2074 7261 636b             track
-00013060: 6c65 745f 7072 6f70 6572 7469 6573 203d  let_properties =
-00013070: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
-00013080: 636b 5f70 726f 7065 7274 6965 735b 6b5d  ck_properties[k]
-00013090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000130a0: 2020 7472 6163 6b73 203d 2073 656c 662e    tracks = self.
-000130b0: 756e 6971 7565 5f74 7261 636b 735b 6b5d  unique_tracks[k]
-000130c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000130d0: 2020 5a20 3d20 7472 6163 6b73 5b3a 2c32    Z = tracks[:,2
+00012f70: 2020 2020 2020 2020 2066 6f72 2028 6b2c           for (k,
+00012f80: 7629 2069 6e20 7365 6c66 2e72 6f6f 745f  v) in self.root_
+00012f90: 7370 6f74 732e 6974 656d 7328 293a 0d0a  spots.items():..
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fc0: 2020 7365 6c66 2e72 6f6f 745f 7370 6f74    self.root_spot
+00012fd0: 735b 6b5d 203d 2073 656c 662e 756e 6971  s[k] = self.uniq
+00012fe0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00012ff0: 6573 5b6b 5d20 2020 2020 2020 2020 0d0a  es[k]         ..
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013010: 0d0a 2020 2020 6465 6620 5f63 6f6d 7075  ..    def _compu
+00013020: 7465 5f70 6865 6e6f 7479 7065 7328 7365  te_phenotypes(se
+00013030: 6c66 293a 0d0a 0d0a 2020 2020 2020 2020  lf):....        
+00013040: 2020 666f 7220 286b 2c76 2920 696e 2073    for (k,v) in s
+00013050: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
+00013060: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+00013070: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00013080: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00013090: 6163 6b5f 6964 203d 206b 0d0a 2020 2020  ack_id = k..    
+000130a0: 2020 2020 2020 2020 2020 2020 7472 6163              trac
+000130b0: 6b6c 6574 5f70 726f 7065 7274 6965 7320  klet_properties 
+000130c0: 3d20 7365 6c66 2e75 6e69 7175 655f 7472  = self.unique_tr
+000130d0: 6163 6b5f 7072 6f70 6572 7469 6573 5b6b  ack_properties[k
 000130e0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000130f0: 2020 2059 203d 2074 7261 636b 735b 3a2c     Y = tracks[:,
-00013100: 335d 0d0a 2020 2020 2020 2020 2020 2020  3]..            
-00013110: 2020 2020 5820 3d20 7472 6163 6b73 5b3a      X = tracks[:
-00013120: 2c34 5d0d 0a20 2020 2020 2020 2020 2020  ,4]..           
-00013130: 2020 2020 2074 696d 6520 3d20 7472 6163       time = trac
-00013140: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00013150: 3a2c 305d 0d0a 2020 2020 2020 2020 2020  :,0]..          
-00013160: 2020 2020 2020 756e 6971 7565 5f69 6473        unique_ids
-00013170: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013180: 6572 7469 6573 5b3a 2c31 5d0d 0a20 2020  erties[:,1]..   
-00013190: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
-000131a0: 7175 655f 6964 735f 7365 7420 3d20 7365  que_ids_set = se
-000131b0: 7428 756e 6971 7565 5f69 6473 290d 0a20  t(unique_ids).. 
-000131c0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000131d0: 656e 6572 6174 696f 6e5f 6964 7320 3d20  eneration_ids = 
-000131e0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-000131f0: 6965 735b 3a2c 325d 0d0a 2020 2020 2020  ies[:,2]..      
-00013200: 2020 2020 2020 2020 2020 7261 6469 7573            radius
-00013210: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00013220: 6572 7469 6573 5b3a 2c33 5d0d 0a20 2020  erties[:,3]..   
-00013230: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
-00013240: 756d 6520 3d20 7472 6163 6b6c 6574 5f70  ume = tracklet_p
-00013250: 726f 7065 7274 6965 735b 3a2c 345d 0d0a  roperties[:,4]..
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00013280: 705f 6669 7273 7420 3d20 7472 6163 6b6c  p_first = trackl
-00013290: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000132a0: 355d 0d0a 2020 2020 2020 2020 2020 2020  5]..            
-000132b0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-000132c0: 5f63 6f6d 705f 7365 636f 6e64 203d 2074  _comp_second = t
-000132d0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000132e0: 6573 5b3a 2c36 5d0d 0a20 2020 2020 2020  es[:,6]..       
-000132f0: 2020 2020 2020 2020 2073 7572 6661 6365           surface
-00013300: 5f61 7265 6120 3d20 7472 6163 6b6c 6574  _area = tracklet
-00013310: 5f70 726f 7065 7274 6965 735b 3a2c 375d  _properties[:,7]
-00013320: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013330: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00013340: 2020 2069 6e74 656e 7369 7479 203d 2074     intensity = t
-00013350: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00013360: 6573 5b3a 2c38 5d0d 0a20 2020 2020 2020  es[:,8]..       
-00013370: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
-00013380: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
-00013390: 7469 6573 5b3a 2c39 5d0d 0a20 2020 2020  ties[:,9]..     
-000133a0: 2020 2020 2020 2020 2020 206d 6f74 696f             motio
-000133b0: 6e5f 616e 676c 6520 3d20 7472 6163 6b6c  n_angle = trackl
-000133c0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000133d0: 3130 5d0d 0a20 2020 2020 2020 2020 2020  10]..           
-000133e0: 2020 2020 2061 6363 656c 6572 6174 696f       acceleratio
-000133f0: 6e20 3d20 7472 6163 6b6c 6574 5f70 726f  n = tracklet_pro
-00013400: 7065 7274 6965 735b 3a2c 3131 5d0d 0a20  perties[:,11].. 
-00013410: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00013420: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00013430: 6b20 3d20 7472 6163 6b6c 6574 5f70 726f  k = tracklet_pro
-00013440: 7065 7274 6965 735b 3a2c 3132 5d0d 0a20  perties[:,12].. 
-00013450: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00013460: 6164 6961 6c5f 616e 676c 6520 3d20 7472  adial_angle = tr
-00013470: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-00013480: 735b 3a2c 3133 5d0d 0a20 2020 2020 2020  s[:,13]..       
-00013490: 2020 2020 2020 2020 2063 656c 6c5f 6178           cell_ax
-000134a0: 6973 5f6d 6173 6b20 3d20 7472 6163 6b6c  is_mask = trackl
-000134b0: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000134c0: 3134 5d0d 0a0d 0a0d 0a20 2020 2020 2020  14]......       
-000134d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000134e0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-000134f0: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00013500: 5f74 7261 636b 6c65 7420 3d20 7b7d 0d0a  _tracklet = {}..
-00013510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013520: 756e 6971 7565 5f63 6c75 7374 6572 5f70  unique_cluster_p
-00013530: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
-00013540: 6574 203d 207b 7d0d 0a20 2020 2020 2020  et = {}..       
-00013550: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00013560: 6971 7565 5f66 6674 5f70 726f 7065 7274  ique_fft_propert
-00013570: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
-00013580: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-00013590: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-000135a0: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
-000135b0: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-000135c0: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
-000135d0: 2020 2020 2075 6e69 7175 655f 7368 6170       unique_shap
-000135e0: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
-000135f0: 636b 6c65 7420 3d20 7b7d 0d0a 2020 2020  cklet = {}..    
-00013600: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-00013610: 7565 5f64 796e 616d 6963 5f70 726f 7065  ue_dynamic_prope
-00013620: 7274 6965 735f 7472 6163 6b6c 6574 203d  rties_tracklet =
-00013630: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
-00013640: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00013650: 5f73 6861 7065 5f70 726f 7065 7274 6965  _shape_propertie
-00013660: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
-00013670: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013680: 2020 7365 6c66 2e75 6e69 7175 655f 6479    self.unique_dy
-00013690: 6e61 6d69 635f 7072 6f70 6572 7469 6573  namic_properties
-000136a0: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
-000136b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000136c0: 2065 7870 616e 6465 645f 7469 6d65 203d   expanded_time =
-000136d0: 206e 702e 7a65 726f 7328 7365 6c66 2e74   np.zeros(self.t
-000136e0: 656e 6420 2d20 7365 6c66 2e74 7374 6172  end - self.tstar
-000136f0: 7420 2b20 3129 0d0a 2020 2020 2020 2020  t + 1)..        
-00013700: 2020 2020 2020 2020 706f 696e 745f 7361          point_sa
-00013710: 6d70 6c65 203d 2065 7870 616e 6465 645f  mple = expanded_
-00013720: 7469 6d65 2e73 6861 7065 5b30 5d0d 0a20  time.shape[0].. 
-00013730: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013740: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00013750: 6e28 6578 7061 6e64 6564 5f74 696d 6529  n(expanded_time)
-00013760: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00013770: 2020 2020 2020 2020 2020 2065 7870 616e             expan
-00013780: 6465 645f 7469 6d65 5b69 5d20 3d20 6920  ded_time[i] = i 
-00013790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000137a0: 2020 666f 7220 6375 7272 656e 745f 756e    for current_un
-000137b0: 6971 7565 5f69 6420 696e 2075 6e69 7175  ique_id in uniqu
-000137c0: 655f 6964 735f 7365 743a 0d0a 2020 2020  e_ids_set:..    
-000137d0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000137e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137f0: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
-00013800: 656e 7369 7479 203d 206e 702e 7a65 726f  ensity = np.zero
-00013810: 7328 7365 6c66 2e74 656e 6420 2d20 7365  s(self.tend - se
-00013820: 6c66 2e74 7374 6172 7420 2b20 3129 0d0a  lf.tstart + 1)..
-00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00013850: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00013860: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013870: 7265 6e74 5f74 696d 6520 3d20 5b5d 0d0a  rent_time = []..
-00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013890: 2020 2063 7572 7265 6e74 5f7a 203d 205b     current_z = [
-000138a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000138b0: 2020 2020 2020 6375 7272 656e 745f 7920        current_y 
-000138c0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000138d0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000138e0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
-000138f0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00013900: 656e 745f 696e 7465 6e73 6974 7920 3d20  ent_intensity = 
-00013910: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013920: 2020 2020 2020 2063 7572 7265 6e74 5f72         current_r
-00013930: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
-00013940: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013950: 7572 7265 6e74 5f76 6f6c 756d 6520 3d20  urrent_volume = 
-00013960: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013970: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
-00013980: 7065 6564 203d 205b 5d0d 0a20 2020 2020  peed = []..     
-00013990: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000139a0: 7272 656e 745f 6d6f 7469 6f6e 5f61 6e67  rrent_motion_ang
-000139b0: 6c65 203d 205b 5d0d 0a20 2020 2020 2020  le = []..       
-000139c0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000139d0: 656e 745f 6163 6365 6c65 7261 7469 6f6e  ent_acceleration
-000139e0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-000139f0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013a00: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-00013a10: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-00013a20: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013a30: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00013a40: 7479 5f63 6f6d 705f 6669 7273 7420 3d20  ty_comp_first = 
-00013a50: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00013a60: 2020 2020 2020 2063 7572 7265 6e74 5f65         current_e
-00013a70: 6363 656e 7472 6963 6974 795f 636f 6d70  ccentricity_comp
-00013a80: 5f73 6563 6f6e 6420 3d20 5b5d 0d0a 2020  _second = []..  
-00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013aa0: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
-00013ab0: 5f61 7265 6120 3d20 5b5d 0d0a 0d0a 2020  _area = []....  
-00013ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ad0: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
-00013ae0: 616e 676c 6520 3d20 5b5d 0d0a 2020 2020  angle = []..    
-00013af0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013b00: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
-00013b10: 5f6d 6173 6b20 3d20 5b5d 200d 0a20 2020  _mask = [] ..   
-00013b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013b40: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00013b50: 6e67 6528 7469 6d65 2e73 6861 7065 5b30  nge(time.shape[0
-00013b60: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
-00013b70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00013b80: 6620 6375 7272 656e 745f 756e 6971 7565  f current_unique
-00013b90: 5f69 6420 3d3d 2075 6e69 7175 655f 6964  _id == unique_id
-00013ba0: 735b 6a5d 3a0d 0a20 2020 2020 2020 2020  s[j]:..         
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013bd0: 7469 6d65 2e61 7070 656e 6428 7469 6d65  time.append(time
-00013be0: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
-00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c00: 2020 2020 2020 2063 7572 7265 6e74 5f7a         current_z
-00013c10: 2e61 7070 656e 6428 5a5b 6a5d 290d 0a20  .append(Z[j]).. 
-00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c40: 6375 7272 656e 745f 792e 6170 7065 6e64  current_y.append
-00013c50: 2859 5b6a 5d29 0d0a 2020 2020 2020 2020  (Y[j])..        
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013c80: 5f78 2e61 7070 656e 6428 585b 6a5d 290d  _x.append(X[j]).
-00013c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
-00013cc0: 7369 7479 5b69 6e74 2874 696d 655b 6a5d  sity[int(time[j]
-00013cd0: 295d 203d 2069 6e74 656e 7369 7479 5b6a  )] = intensity[j
-00013ce0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000130f0: 2020 2074 7261 636b 7320 3d20 7365 6c66     tracks = self
+00013100: 2e75 6e69 7175 655f 7472 6163 6b73 5b6b  .unique_tracks[k
+00013110: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013120: 2020 205a 203d 2074 7261 636b 735b 3a2c     Z = tracks[:,
+00013130: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
+00013140: 2020 2020 5920 3d20 7472 6163 6b73 5b3a      Y = tracks[:
+00013150: 2c33 5d0d 0a20 2020 2020 2020 2020 2020  ,3]..           
+00013160: 2020 2020 2058 203d 2074 7261 636b 735b       X = tracks[
+00013170: 3a2c 345d 0d0a 2020 2020 2020 2020 2020  :,4]..          
+00013180: 2020 2020 2020 7469 6d65 203d 2074 7261        time = tra
+00013190: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000131a0: 5b3a 2c30 5d0d 0a20 2020 2020 2020 2020  [:,0]..         
+000131b0: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
+000131c0: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
+000131d0: 7065 7274 6965 735b 3a2c 315d 0d0a 2020  perties[:,1]..  
+000131e0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000131f0: 6971 7565 5f69 6473 5f73 6574 203d 2073  ique_ids_set = s
+00013200: 6574 2875 6e69 7175 655f 6964 7329 0d0a  et(unique_ids)..
+00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013220: 6765 6e65 7261 7469 6f6e 5f69 6473 203d  generation_ids =
+00013230: 2074 7261 636b 6c65 745f 7072 6f70 6572   tracklet_proper
+00013240: 7469 6573 5b3a 2c32 5d0d 0a20 2020 2020  ties[:,2]..     
+00013250: 2020 2020 2020 2020 2020 2072 6164 6975             radiu
+00013260: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
+00013270: 7065 7274 6965 735b 3a2c 335d 0d0a 2020  perties[:,3]..  
+00013280: 2020 2020 2020 2020 2020 2020 2020 766f                vo
+00013290: 6c75 6d65 203d 2074 7261 636b 6c65 745f  lume = tracklet_
+000132a0: 7072 6f70 6572 7469 6573 5b3a 2c34 5d0d  properties[:,4].
+000132b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132c0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+000132d0: 6d70 5f66 6972 7374 203d 2074 7261 636b  mp_first = track
+000132e0: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+000132f0: 2c35 5d0d 0a20 2020 2020 2020 2020 2020  ,5]..           
+00013300: 2020 2020 2065 6363 656e 7472 6963 6974       eccentricit
+00013310: 795f 636f 6d70 5f73 6563 6f6e 6420 3d20  y_comp_second = 
+00013320: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+00013330: 6965 735b 3a2c 365d 0d0a 2020 2020 2020  ies[:,6]..      
+00013340: 2020 2020 2020 2020 2020 7375 7266 6163            surfac
+00013350: 655f 6172 6561 203d 2074 7261 636b 6c65  e_area = trackle
+00013360: 745f 7072 6f70 6572 7469 6573 5b3a 2c37  t_properties[:,7
+00013370: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00013380: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00013390: 2020 2020 696e 7465 6e73 6974 7920 3d20      intensity = 
+000133a0: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
+000133b0: 6965 735b 3a2c 385d 0d0a 2020 2020 2020  ies[:,8]..      
+000133c0: 2020 2020 2020 2020 2020 7370 6565 6420            speed 
+000133d0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+000133e0: 7274 6965 735b 3a2c 395d 0d0a 2020 2020  rties[:,9]..    
+000133f0: 2020 2020 2020 2020 2020 2020 6d6f 7469              moti
+00013400: 6f6e 5f61 6e67 6c65 203d 2074 7261 636b  on_angle = track
+00013410: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00013420: 2c31 305d 0d0a 2020 2020 2020 2020 2020  ,10]..          
+00013430: 2020 2020 2020 6163 6365 6c65 7261 7469        accelerati
+00013440: 6f6e 203d 2074 7261 636b 6c65 745f 7072  on = tracklet_pr
+00013450: 6f70 6572 7469 6573 5b3a 2c31 315d 0d0a  operties[:,11]..
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00013480: 736b 203d 2074 7261 636b 6c65 745f 7072  sk = tracklet_pr
+00013490: 6f70 6572 7469 6573 5b3a 2c31 325d 0d0a  operties[:,12]..
+000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134b0: 7261 6469 616c 5f61 6e67 6c65 203d 2074  radial_angle = t
+000134c0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+000134d0: 6573 5b3a 2c31 335d 0d0a 2020 2020 2020  es[:,13]..      
+000134e0: 2020 2020 2020 2020 2020 6365 6c6c 5f61            cell_a
+000134f0: 7869 735f 6d61 736b 203d 2074 7261 636b  xis_mask = track
+00013500: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00013510: 2c31 345d 0d0a 0d0a 0d0a 2020 2020 2020  ,14]......      
+00013520: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00013530: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
+00013540: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00013550: 735f 7472 6163 6b6c 6574 203d 207b 7d0d  s_tracklet = {}.
+00013560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013570: 2075 6e69 7175 655f 636c 7573 7465 725f   unique_cluster_
+00013580: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00013590: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
+000135a0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000135b0: 6e69 7175 655f 6666 745f 7072 6f70 6572  nique_fft_proper
+000135c0: 7469 6573 5b74 7261 636b 5f69 645d 203d  ties[track_id] =
+000135d0: 207b 7d0d 0a20 2020 2020 2020 2020 2020   {}..           
+000135e0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000135f0: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+00013600: 6965 735b 7472 6163 6b5f 6964 5d20 3d20  ies[track_id] = 
+00013610: 7b7d 0d0a 0d0a 2020 2020 2020 2020 2020  {}....          
+00013620: 2020 2020 2020 756e 6971 7565 5f73 6861        unique_sha
+00013630: 7065 5f70 726f 7065 7274 6965 735f 7472  pe_properties_tr
+00013640: 6163 6b6c 6574 203d 207b 7d0d 0a20 2020  acklet = {}..   
+00013650: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00013660: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+00013670: 6572 7469 6573 5f74 7261 636b 6c65 7420  erties_tracklet 
+00013680: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+00013690: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000136a0: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
+000136b0: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+000136c0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+000136d0: 2020 2073 656c 662e 756e 6971 7565 5f64     self.unique_d
+000136e0: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
+000136f0: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+00013700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013710: 2020 6578 7061 6e64 6564 5f74 696d 6520    expanded_time 
+00013720: 3d20 6e70 2e7a 6572 6f73 2873 656c 662e  = np.zeros(self.
+00013730: 7465 6e64 202d 2073 656c 662e 7473 7461  tend - self.tsta
+00013740: 7274 202b 2031 290d 0a20 2020 2020 2020  rt + 1)..       
+00013750: 2020 2020 2020 2020 2070 6f69 6e74 5f73           point_s
+00013760: 616d 706c 6520 3d20 6578 7061 6e64 6564  ample = expanded
+00013770: 5f74 696d 652e 7368 6170 655b 305d 0d0a  _time.shape[0]..
+00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013790: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+000137a0: 656e 2865 7870 616e 6465 645f 7469 6d65  en(expanded_time
+000137b0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+000137c0: 2020 2020 2020 2020 2020 2020 6578 7061              expa
+000137d0: 6e64 6564 5f74 696d 655b 695d 203d 2069  nded_time[i] = i
+000137e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000137f0: 2020 2066 6f72 2063 7572 7265 6e74 5f75     for current_u
+00013800: 6e69 7175 655f 6964 2069 6e20 756e 6971  nique_id in uniq
+00013810: 7565 5f69 6473 5f73 6574 3a0d 0a20 2020  ue_ids_set:..   
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013840: 2020 2020 2065 7870 616e 6465 645f 696e       expanded_in
+00013850: 7465 6e73 6974 7920 3d20 6e70 2e7a 6572  tensity = np.zer
+00013860: 6f73 2873 656c 662e 7465 6e64 202d 2073  os(self.tend - s
+00013870: 656c 662e 7473 7461 7274 202b 2031 290d  elf.tstart + 1).
+00013880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013890: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000138a0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000138b0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+000138c0: 7272 656e 745f 7469 6d65 203d 205b 5d0d  rrent_time = [].
+000138d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138e0: 2020 2020 6375 7272 656e 745f 7a20 3d20      current_z = 
+000138f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00013900: 2020 2020 2020 2063 7572 7265 6e74 5f79         current_y
+00013910: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00013920: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013930: 745f 7820 3d20 5b5d 0d0a 2020 2020 2020  t_x = []..      
+00013940: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013950: 7265 6e74 5f69 6e74 656e 7369 7479 203d  rent_intensity =
+00013960: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00013970: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013980: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139a0: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
+000139b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000139c0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000139d0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+000139e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000139f0: 7572 7265 6e74 5f6d 6f74 696f 6e5f 616e  urrent_motion_an
+00013a00: 676c 6520 3d20 5b5d 0d0a 2020 2020 2020  gle = []..      
+00013a10: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013a20: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
+00013a30: 6e20 3d20 5b5d 0d0a 2020 2020 2020 2020  n = []..        
+00013a40: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00013a50: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+00013a60: 5f6d 6173 6b20 3d20 5b5d 0d0a 2020 2020  _mask = []..    
+00013a70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013a80: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013a90: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+00013aa0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00013ab0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013ac0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
+00013ad0: 705f 7365 636f 6e64 203d 205b 5d0d 0a20  p_second = [].. 
+00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013af0: 2020 6375 7272 656e 745f 7375 7266 6163    current_surfac
+00013b00: 655f 6172 6561 203d 205b 5d0d 0a0d 0a20  e_area = [].... 
+00013b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b20: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
+00013b30: 5f61 6e67 6c65 203d 205b 5d0d 0a20 2020  _angle = []..   
+00013b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b50: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
+00013b60: 735f 6d61 736b 203d 205b 5d20 0d0a 2020  s_mask = [] ..  
+00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00013b90: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+00013ba0: 616e 6765 2874 696d 652e 7368 6170 655b  ange(time.shape[
+00013bb0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 6966 2063 7572 7265 6e74 5f75 6e69 7175  if current_uniqu
+00013be0: 655f 6964 203d 3d20 756e 6971 7565 5f69  e_id == unique_i
+00013bf0: 6473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ds[j]:..        
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013c20: 5f74 696d 652e 6170 7065 6e64 2874 696d  _time.append(tim
+00013c30: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c50: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+00013c60: 7a2e 6170 7065 6e64 285a 5b6a 5d29 0d0a  z.append(Z[j])..
+00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c90: 2063 7572 7265 6e74 5f79 2e61 7070 656e   current_y.appen
+00013ca0: 6428 595b 6a5d 290d 0a20 2020 2020 2020  d(Y[j])..       
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00013cd0: 745f 782e 6170 7065 6e64 2858 5b6a 5d29  t_x.append(X[j])
+00013ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 2020 2020 6375 7272 656e 745f 696e 7465      current_inte
-00013d10: 6e73 6974 792e 6170 7065 6e64 2869 6e74  nsity.append(int
-00013d20: 656e 7369 7479 5b6a 5d29 0d0a 2020 2020  ensity[j])..    
-00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013d50: 7265 6e74 5f72 6164 6975 732e 6170 7065  rent_radius.appe
-00013d60: 6e64 2872 6164 6975 735b 6a5d 290d 0a20  nd(radius[j]).. 
-00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d00: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
+00013d10: 6e73 6974 795b 696e 7428 7469 6d65 5b6a  nsity[int(time[j
+00013d20: 5d29 5d20 3d20 696e 7465 6e73 6974 795b  ])] = intensity[
+00013d30: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 2020 2020 2063 7572 7265 6e74 5f69 6e74       current_int
+00013d60: 656e 7369 7479 2e61 7070 656e 6428 696e  ensity.append(in
+00013d70: 7465 6e73 6974 795b 6a5d 290d 0a20 2020  tensity[j])..   
 00013d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d90: 6375 7272 656e 745f 766f 6c75 6d65 2e61  current_volume.a
-00013da0: 7070 656e 6428 766f 6c75 6d65 5b6a 5d29  ppend(volume[j])
-00013db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013d90: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013da0: 7272 656e 745f 7261 6469 7573 2e61 7070  rrent_radius.app
+00013db0: 656e 6428 7261 6469 7573 5b6a 5d29 0d0a  end(radius[j])..
 00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
-00013de0: 2e61 7070 656e 6428 7370 6565 645b 6a5d  .append(speed[j]
-00013df0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00013e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e10: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
-00013e20: 6f6e 5f61 6e67 6c65 2e61 7070 656e 6428  on_angle.append(
-00013e30: 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a 5d29  motion_angle[j])
-00013e40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013de0: 2063 7572 7265 6e74 5f76 6f6c 756d 652e   current_volume.
+00013df0: 6170 7065 6e64 2876 6f6c 756d 655b 6a5d  append(volume[j]
+00013e00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e20: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
+00013e30: 642e 6170 7065 6e64 2873 7065 6564 5b6a  d.append(speed[j
+00013e40: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
-00013e70: 6572 6174 696f 6e2e 6170 7065 6e64 2861  eration.append(a
-00013e80: 6363 656c 6572 6174 696f 6e5b 6a5d 290d  cceleration[j]).
-00013e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013e60: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
+00013e70: 696f 6e5f 616e 676c 652e 6170 7065 6e64  ion_angle.append
+00013e80: 286d 6f74 696f 6e5f 616e 676c 655b 6a5d  (motion_angle[j]
+00013e90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013eb0: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
-00013ec0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00013ed0: 656e 6428 6469 7374 616e 6365 5f63 656c  end(distance_cel
-00013ee0: 6c5f 6d61 736b 5b6a 5d29 0d0a 2020 2020  l_mask[j])..    
+00013eb0: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
+00013ec0: 6c65 7261 7469 6f6e 2e61 7070 656e 6428  leration.append(
+00013ed0: 6163 6365 6c65 7261 7469 6f6e 5b6a 5d29  acceleration[j])
+00013ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013f10: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013f20: 795f 636f 6d70 5f66 6972 7374 2e61 7070  y_comp_first.app
-00013f30: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
-00013f40: 5f63 6f6d 705f 6669 7273 745b 6a5d 290d  _comp_first[j]).
-00013f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f70: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-00013f80: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00013f90: 6e64 2e61 7070 656e 6428 6563 6365 6e74  nd.append(eccent
-00013fa0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00013fb0: 6e64 5b6a 5d29 0d0a 2020 2020 2020 2020  nd[j])..        
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00013fe0: 5f73 7572 6661 6365 5f61 7265 612e 6170  _surface_area.ap
-00013ff0: 7065 6e64 2873 7572 6661 6365 5f61 7265  pend(surface_are
-00014000: 615b 6a5d 290d 0a20 2020 2020 2020 2020  a[j])..         
+00013f00: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
+00013f10: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00013f20: 7065 6e64 2864 6973 7461 6e63 655f 6365  pend(distance_ce
+00013f30: 6c6c 5f6d 6173 6b5b 6a5d 290d 0a20 2020  ll_mask[j])..   
+00013f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f50: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00013f60: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013f70: 7479 5f63 6f6d 705f 6669 7273 742e 6170  ty_comp_first.ap
+00013f80: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
+00013f90: 795f 636f 6d70 5f66 6972 7374 5b6a 5d29  y_comp_first[j])
+00013fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fc0: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
+00013fd0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00013fe0: 6f6e 642e 6170 7065 6e64 2865 6363 656e  ond.append(eccen
+00013ff0: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
+00014000: 6f6e 645b 6a5d 290d 0a20 2020 2020 2020  ond[j])..       
 00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014030: 7261 6469 616c 5f61 6e67 6c65 2e61 7070  radial_angle.app
-00014040: 656e 6428 7261 6469 616c 5f61 6e67 6c65  end(radial_angle
-00014050: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
+00014020: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00014030: 745f 7375 7266 6163 655f 6172 6561 2e61  t_surface_area.a
+00014040: 7070 656e 6428 7375 7266 6163 655f 6172  ppend(surface_ar
+00014050: 6561 5b6a 5d29 0d0a 2020 2020 2020 2020  ea[j])..        
 00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014070: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
-00014080: 656c 6c5f 6178 6973 5f6d 6173 6b2e 6170  ell_axis_mask.ap
-00014090: 7065 6e64 2863 656c 6c5f 6178 6973 5f6d  pend(cell_axis_m
-000140a0: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
-000140b0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000140c0: 656e 745f 7469 6d65 203d 206e 702e 6173  ent_time = np.as
-000140d0: 6172 7261 7928 6375 7272 656e 745f 7469  array(current_ti
-000140e0: 6d65 2c20 6474 7970 653d 6e70 2e66 6c6f  me, dtype=np.flo
-000140f0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014100: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014110: 745f 696e 7465 6e73 6974 7920 3d20 6e70  t_intensity = np
-00014120: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00014130: 5f69 6e74 656e 7369 7479 2c20 6474 7970  _intensity, dtyp
-00014140: 653d 6e70 2e66 6c6f 6174 3332 290d 0a0d  e=np.float32)...
-00014150: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00014160: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00014170: 7261 6469 7573 203d 206e 702e 6173 6172  radius = np.asar
-00014180: 7261 7928 6375 7272 656e 745f 7261 6469  ray(current_radi
-00014190: 7573 2c20 6474 7970 653d 6e70 2e66 6c6f  us, dtype=np.flo
-000141a0: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-000141b0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000141c0: 745f 766f 6c75 6d65 203d 206e 702e 6173  t_volume = np.as
-000141d0: 6172 7261 7928 6375 7272 656e 745f 766f  array(current_vo
-000141e0: 6c75 6d65 2c20 6474 7970 653d 6e70 2e66  lume, dtype=np.f
-000141f0: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-00014200: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00014210: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
-00014220: 5f63 6f6d 705f 6669 7273 7420 3d20 6e70  _comp_first = np
-00014230: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
-00014240: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00014250: 6d70 5f66 6972 7374 2c20 6474 7970 653d  mp_first, dtype=
-00014260: 6e70 2e66 6c6f 6174 3332 290d 0a20 2020  np.float32)..   
-00014270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014280: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00014290: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000142a0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-000142b0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-000142c0: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
-000142d0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-000142e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000142f0: 2020 2020 2020 6375 7272 656e 745f 7375        current_su
-00014300: 7266 6163 655f 6172 6561 203d 206e 702e  rface_area = np.
-00014310: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00014320: 7375 7266 6163 655f 6172 6561 2c20 6474  surface_area, dt
-00014330: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-00014340: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00014350: 2020 2020 2020 6375 7272 656e 745f 7370        current_sp
-00014360: 6565 6420 3d20 6e70 2e61 7361 7272 6179  eed = np.asarray
-00014370: 2863 7572 7265 6e74 5f73 7065 6564 2c20  (current_speed, 
-00014380: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00014390: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000143a0: 2020 2020 2020 6375 7272 656e 745f 6d6f        current_mo
-000143b0: 7469 6f6e 5f61 6e67 6c65 203d 206e 702e  tion_angle = np.
-000143c0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-000143d0: 6d6f 7469 6f6e 5f61 6e67 6c65 2c20 6474  motion_angle, dt
-000143e0: 7970 653d 6e70 2e66 6c6f 6174 3332 290d  ype=np.float32).
-000143f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014400: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00014410: 6c65 7261 7469 6f6e 203d 206e 702e 6173  leration = np.as
-00014420: 6172 7261 7928 6375 7272 656e 745f 6163  array(current_ac
-00014430: 6365 6c65 7261 7469 6f6e 2c20 6474 7970  celeration, dtyp
-00014440: 653d 6e70 2e66 6c6f 6174 3332 290d 0a20  e=np.float32).. 
-00014450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014460: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
-00014470: 6365 5f63 656c 6c5f 6d61 736b 203d 206e  ce_cell_mask = n
-00014480: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00014490: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-000144a0: 6d61 736b 2c20 6474 7970 653d 6e70 2e66  mask, dtype=np.f
-000144b0: 6c6f 6174 3332 290d 0a20 2020 2020 2020  loat32)..       
-000144c0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-000144d0: 656e 745f 7261 6469 616c 5f61 6e67 6c65  ent_radial_angle
-000144e0: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-000144f0: 7272 656e 745f 7261 6469 616c 5f61 6e67  rrent_radial_ang
-00014500: 6c65 2c20 6474 7970 653d 6e70 2e66 6c6f  le, dtype=np.flo
-00014510: 6174 3332 290d 0a20 2020 2020 2020 2020  at32)..         
-00014520: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00014530: 745f 6365 6c6c 5f61 7869 735f 6d61 736b  t_cell_axis_mask
-00014540: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
-00014550: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
-00014560: 6d61 736b 2c20 6474 7970 653d 6e70 2e66  mask, dtype=np.f
-00014570: 6c6f 6174 3332 290d 0a0d 0a0d 0a20 2020  loat32)......   
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000145a0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-000145b0: 2020 2020 2020 2020 2020 6966 2070 6f69            if poi
-000145c0: 6e74 5f73 616d 706c 6520 3e20 303a 0d0a  nt_sample > 0:..
+00014070: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00014080: 5f72 6164 6961 6c5f 616e 676c 652e 6170  _radial_angle.ap
+00014090: 7065 6e64 2872 6164 6961 6c5f 616e 676c  pend(radial_angl
+000140a0: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000140d0: 6365 6c6c 5f61 7869 735f 6d61 736b 2e61  cell_axis_mask.a
+000140e0: 7070 656e 6428 6365 6c6c 5f61 7869 735f  ppend(cell_axis_
+000140f0: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
+00014100: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00014110: 7265 6e74 5f74 696d 6520 3d20 6e70 2e61  rent_time = np.a
+00014120: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
+00014130: 696d 652c 2064 7479 7065 3d6e 702e 666c  ime, dtype=np.fl
+00014140: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014150: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014160: 6e74 5f69 6e74 656e 7369 7479 203d 206e  nt_intensity = n
+00014170: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00014180: 745f 696e 7465 6e73 6974 792c 2064 7479  t_intensity, dty
+00014190: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+000141a0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+000141b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000141c0: 5f72 6164 6975 7320 3d20 6e70 2e61 7361  _radius = np.asa
+000141d0: 7272 6179 2863 7572 7265 6e74 5f72 6164  rray(current_rad
+000141e0: 6975 732c 2064 7479 7065 3d6e 702e 666c  ius, dtype=np.fl
+000141f0: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014200: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014210: 6e74 5f76 6f6c 756d 6520 3d20 6e70 2e61  nt_volume = np.a
+00014220: 7361 7272 6179 2863 7572 7265 6e74 5f76  sarray(current_v
+00014230: 6f6c 756d 652c 2064 7479 7065 3d6e 702e  olume, dtype=np.
+00014240: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00014250: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00014260: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00014270: 795f 636f 6d70 5f66 6972 7374 203d 206e  y_comp_first = n
+00014280: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
+00014290: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+000142a0: 6f6d 705f 6669 7273 742c 2064 7479 7065  omp_first, dtype
+000142b0: 3d6e 702e 666c 6f61 7433 3229 0d0a 2020  =np.float32)..  
+000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142d0: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+000142e0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000142f0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
+00014300: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00014310: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
+00014320: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00014330: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+00014340: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+00014350: 7572 6661 6365 5f61 7265 6120 3d20 6e70  urface_area = np
+00014360: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00014370: 5f73 7572 6661 6365 5f61 7265 612c 2064  _surface_area, d
+00014380: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014390: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000143a0: 2020 2020 2020 2063 7572 7265 6e74 5f73         current_s
+000143b0: 7065 6564 203d 206e 702e 6173 6172 7261  peed = np.asarra
+000143c0: 7928 6375 7272 656e 745f 7370 6565 642c  y(current_speed,
+000143d0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000143e0: 3229 0d0a 2020 2020 2020 2020 2020 2020  2)..            
+000143f0: 2020 2020 2020 2063 7572 7265 6e74 5f6d         current_m
+00014400: 6f74 696f 6e5f 616e 676c 6520 3d20 6e70  otion_angle = np
+00014410: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00014420: 5f6d 6f74 696f 6e5f 616e 676c 652c 2064  _motion_angle, d
+00014430: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00014440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014450: 2020 2020 2063 7572 7265 6e74 5f61 6363       current_acc
+00014460: 656c 6572 6174 696f 6e20 3d20 6e70 2e61  eleration = np.a
+00014470: 7361 7272 6179 2863 7572 7265 6e74 5f61  sarray(current_a
+00014480: 6363 656c 6572 6174 696f 6e2c 2064 7479  cceleration, dty
+00014490: 7065 3d6e 702e 666c 6f61 7433 3229 0d0a  pe=np.float32)..
+000144a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144b0: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
+000144c0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+000144d0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000144e0: 6e74 5f64 6973 7461 6e63 655f 6365 6c6c  nt_distance_cell
+000144f0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
+00014500: 666c 6f61 7433 3229 0d0a 2020 2020 2020  float32)..      
+00014510: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00014520: 7265 6e74 5f72 6164 6961 6c5f 616e 676c  rent_radial_angl
+00014530: 6520 3d20 6e70 2e61 7361 7272 6179 2863  e = np.asarray(c
+00014540: 7572 7265 6e74 5f72 6164 6961 6c5f 616e  urrent_radial_an
+00014550: 676c 652c 2064 7479 7065 3d6e 702e 666c  gle, dtype=np.fl
+00014560: 6f61 7433 3229 0d0a 2020 2020 2020 2020  oat32)..        
+00014570: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00014580: 6e74 5f63 656c 6c5f 6178 6973 5f6d 6173  nt_cell_axis_mas
+00014590: 6b20 3d20 6e70 2e61 7361 7272 6179 2863  k = np.asarray(c
+000145a0: 7572 7265 6e74 5f63 656c 6c5f 6178 6973  urrent_cell_axis
+000145b0: 5f6d 6173 6b2c 2064 7479 7065 3d6e 702e  _mask, dtype=np.
+000145c0: 666c 6f61 7433 3229 0d0a 0d0a 0d0a 2020  float32)......  
 000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145f0: 7866 5f73 616d 706c 6520 3d20 6666 7466  xf_sample = fftf
-00014600: 7265 7128 706f 696e 745f 7361 6d70 6c65  req(point_sample
-00014610: 2c20 7365 6c66 2e74 6361 6c69 6272 6174  , self.tcalibrat
-00014620: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+000145e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000145f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00014600: 2020 2020 2020 2020 2020 2069 6620 706f             if po
+00014610: 696e 745f 7361 6d70 6c65 203e 2030 3a0d  int_sample > 0:.
+00014620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 2020 2020 2020 6666 7473 7472 6970 5f73        fftstrip_s
-00014650: 616d 706c 6520 3d20 6666 7428 6578 7061  ample = fft(expa
-00014660: 6e64 6564 5f69 6e74 656e 7369 7479 290d  nded_intensity).
-00014670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014640: 2078 665f 7361 6d70 6c65 203d 2066 6674   xf_sample = fft
+00014650: 6672 6571 2870 6f69 6e74 5f73 616d 706c  freq(point_sampl
+00014660: 652c 2073 656c 662e 7463 616c 6962 7261  e, self.tcalibra
+00014670: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
 00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014690: 2066 6674 746f 7461 6c5f 7361 6d70 6c65   ffttotal_sample
-000146a0: 203d 206e 702e 6162 7328 6666 7473 7472   = np.abs(fftstr
-000146b0: 6970 5f73 616d 706c 6529 0d0a 2020 2020  ip_sample)..    
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2020 2020 2020 2020 2020 2020 7866 5f73              xf_s
-000146e0: 616d 706c 6520 3d20 7866 5f73 616d 706c  ample = xf_sampl
-000146f0: 655b 3020 3a20 6c65 6e28 7866 5f73 616d  e[0 : len(xf_sam
-00014700: 706c 6529 202f 2f20 325d 0d0a 2020 2020  ple) // 2]..    
+00014690: 2020 2020 2020 2066 6674 7374 7269 705f         fftstrip_
+000146a0: 7361 6d70 6c65 203d 2066 6674 2865 7870  sample = fft(exp
+000146b0: 616e 6465 645f 696e 7465 6e73 6974 7929  anded_intensity)
+000146c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146e0: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
+000146f0: 6520 3d20 6e70 2e61 6273 2866 6674 7374  e = np.abs(fftst
+00014700: 7269 705f 7361 6d70 6c65 290d 0a20 2020  rip_sample)..   
 00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2020 2020 2020 2020 6666 7474              fftt
-00014730: 6f74 616c 5f73 616d 706c 6520 3d20 6666  otal_sample = ff
-00014740: 7474 6f74 616c 5f73 616d 706c 655b 3020  ttotal_sample[0 
-00014750: 3a20 6c65 6e28 6666 7474 6f74 616c 5f73  : len(ffttotal_s
-00014760: 616d 706c 6529 202f 2f20 325d 0d0a 0d0a  ample) // 2]....
-00014770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014780: 2020 2075 6e69 7175 655f 6666 745f 7072     unique_fft_pr
-00014790: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-000147a0: 745b 6375 7272 656e 745f 756e 6971 7565  t[current_unique
-000147b0: 5f69 645d 203d 2065 7870 616e 6465 645f  _id] = expanded_
-000147c0: 7469 6d65 2c20 6578 7061 6e64 6564 5f69  time, expanded_i
-000147d0: 6e74 656e 7369 7479 2c20 7866 5f73 616d  ntensity, xf_sam
-000147e0: 706c 652c 2066 6674 746f 7461 6c5f 7361  ple, ffttotal_sa
-000147f0: 6d70 6c65 0d0a 2020 2020 2020 2020 2020  mple..          
-00014800: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00014810: 636c 7573 7465 725f 7072 6f70 6572 7469  cluster_properti
-00014820: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00014830: 656e 745f 756e 6971 7565 5f69 645d 203d  ent_unique_id] =
-00014840: 2020 6375 7272 656e 745f 7469 6d65 0d0a    current_time..
-00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014860: 2020 2075 6e69 7175 655f 7368 6170 655f     unique_shape_
-00014870: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00014880: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00014890: 7565 5f69 645d 203d 2063 7572 7265 6e74  ue_id] = current
-000148a0: 5f74 696d 652c 2063 7572 7265 6e74 5f7a  _time, current_z
-000148b0: 2c20 6375 7272 656e 745f 792c 2063 7572  , current_y, cur
-000148c0: 7265 6e74 5f78 2c20 6375 7272 656e 745f  rent_x, current_
-000148d0: 7261 6469 7573 2c20 6375 7272 656e 745f  radius, current_
-000148e0: 766f 6c75 6d65 2c20 6375 7272 656e 745f  volume, current_
-000148f0: 6563 6365 6e74 7269 6369 7479 5f63 6f6d  eccentricity_com
-00014900: 705f 6669 7273 742c 2063 7572 7265 6e74  p_first, current
-00014910: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
-00014920: 6d70 5f73 6563 6f6e 642c 2063 7572 7265  mp_second, curre
-00014930: 6e74 5f73 7572 6661 6365 5f61 7265 610d  nt_surface_area.
-00014940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014950: 2020 2020 756e 6971 7565 5f64 796e 616d      unique_dynam
-00014960: 6963 5f70 726f 7065 7274 6965 735f 7472  ic_properties_tr
-00014970: 6163 6b6c 6574 5b63 7572 7265 6e74 5f75  acklet[current_u
-00014980: 6e69 7175 655f 6964 5d20 3d20 6375 7272  nique_id] = curr
-00014990: 656e 745f 7469 6d65 2c20 6375 7272 656e  ent_time, curren
-000149a0: 745f 7370 6565 642c 2063 7572 7265 6e74  t_speed, current
-000149b0: 5f6d 6f74 696f 6e5f 616e 676c 652c 2063  _motion_angle, c
-000149c0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-000149d0: 696f 6e2c 2063 7572 7265 6e74 5f64 6973  ion, current_dis
-000149e0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2c  tance_cell_mask,
-000149f0: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
-00014a00: 616e 676c 652c 2063 7572 7265 6e74 5f63  angle, current_c
-00014a10: 656c 6c5f 6178 6973 5f6d 6173 6b0d 0a20  ell_axis_mask.. 
-00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a30: 2020 7365 6c66 2e75 6e69 7175 655f 6666    self.unique_ff
-00014a40: 745f 7072 6f70 6572 7469 6573 5b74 7261  t_properties[tra
-00014a50: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
-00014a60: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00014a70: 3a75 6e69 7175 655f 6666 745f 7072 6f70  :unique_fft_prop
-00014a80: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
-00014a90: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00014aa0: 645d 7d29 0d0a 2020 2020 2020 2020 2020  d]})..          
-00014ab0: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00014ac0: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
-00014ad0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
-00014ae0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
-00014af0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
-00014b00: 7565 5f63 6c75 7374 6572 5f70 726f 7065  ue_cluster_prope
-00014b10: 7274 6965 735f 7472 6163 6b6c 6574 5b63  rties_tracklet[c
-00014b20: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
-00014b30: 5d7d 290d 0a0d 0a20 2020 2020 2020 2020  ]})....         
-00014b40: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00014b50: 6e69 7175 655f 7368 6170 655f 7072 6f70  nique_shape_prop
-00014b60: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00014b70: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
-00014b80: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
-00014b90: 655f 7368 6170 655f 7072 6f70 6572 7469  e_shape_properti
-00014ba0: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
-00014bb0: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
-00014bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014bd0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00014be0: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
-00014bf0: 6965 735b 7472 6163 6b5f 6964 5d2e 7570  ies[track_id].up
-00014c00: 6461 7465 287b 6375 7272 656e 745f 756e  date({current_un
-00014c10: 6971 7565 5f69 643a 756e 6971 7565 5f64  ique_id:unique_d
-00014c20: 796e 616d 6963 5f70 726f 7065 7274 6965  ynamic_propertie
-00014c30: 735f 7472 6163 6b6c 6574 5b63 7572 7265  s_tracklet[curre
-00014c40: 6e74 5f75 6e69 7175 655f 6964 5d7d 290d  nt_unique_id]}).
-00014c50: 0a0d 0a20 2020 2064 6566 205f 7365 636f  ...    def _seco
-00014c60: 6e64 5f63 6861 6e6e 656c 5f73 706f 7473  nd_channel_spots
-00014c70: 2873 656c 662c 2066 7261 6d65 2c20 7a2c  (self, frame, z,
-00014c80: 2079 2c20 782c 2063 656c 6c5f 6964 2c20   y, x, cell_id, 
-00014c90: 7472 6163 6b5f 6964 293a 0d0a 2020 2020  track_id):..    
-00014ca0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00014cb0: 2020 2020 2074 7265 652c 2063 656e 7472       tree, centr
-00014cc0: 6f69 6473 2c20 6c61 6265 6c73 2c20 766f  oids, labels, vo
-00014cd0: 6c75 6d65 2c20 696e 7465 6e73 6974 795f  lume, intensity_
-00014ce0: 6d65 616e 2c20 696e 7465 6e73 6974 795f  mean, intensity_
-00014cf0: 746f 7461 6c2c 2062 6f75 6e64 696e 675f  total, bounding_
-00014d00: 626f 7865 7320 3d20 7365 6c66 2e5f 7469  boxes = self._ti
-00014d10: 6d65 645f 6368 616e 6e65 6c5f 7365 675f  med_channel_seg_
-00014d20: 696d 6167 655b 7374 7228 696e 7428 666c  image[str(int(fl
-00014d30: 6f61 7428 6672 616d 6529 2929 5d0d 0a20  oat(frame)))].. 
-00014d40: 2020 2020 2020 2020 2020 2070 6978 656c             pixel
-00014d50: 7465 7374 6c6f 6361 7469 6f6e 203d 2028  testlocation = (
-00014d60: 7a2c 792c 7829 0d0a 2020 2020 2020 2020  z,y,x)..        
-00014d70: 2020 2020 6469 7374 2c20 696e 6465 7820      dist, index 
-00014d80: 3d20 7472 6565 2e71 7565 7279 2870 6978  = tree.query(pix
-00014d90: 656c 7465 7374 6c6f 6361 7469 6f6e 290d  eltestlocation).
-00014da0: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00014db0: 2062 626f 7820 3d20 626f 756e 6469 6e67   bbox = bounding
-00014dc0: 5f62 6f78 6573 5b69 6e64 6578 5d0d 0a20  _boxes[index].. 
-00014dd0: 2020 2020 2020 2020 2020 2073 697a 657a             sizez
-00014de0: 203d 2061 6273 2862 626f 785b 305d 202d   = abs(bbox[0] -
-00014df0: 2062 626f 785b 335d 290d 0a20 2020 2020   bbox[3])..     
-00014e00: 2020 2020 2020 2073 697a 6579 203d 2061         sizey = a
-00014e10: 6273 2862 626f 785b 315d 202d 2062 626f  bs(bbox[1] - bbo
-00014e20: 785b 345d 290d 0a20 2020 2020 2020 2020  x[4])..         
-00014e30: 2020 2073 697a 6578 203d 2061 6273 2862     sizex = abs(b
-00014e40: 626f 785b 325d 202d 2062 626f 785b 355d  box[2] - bbox[5]
-00014e50: 2920 0d0a 2020 2020 2020 2020 2020 2020  ) ..            
-00014e60: 7665 746f 5f76 6f6c 756d 6520 3d20 7369  veto_volume = si
-00014e70: 7a65 7820 2a20 7369 7a65 7920 2a20 7369  zex * sizey * si
-00014e80: 7a65 7a0d 0a20 2020 2020 2020 2020 2020  zez..           
-00014e90: 2076 6574 6f5f 7261 6469 7573 203d 206d   veto_radius = m
-00014ea0: 6174 682e 706f 7728 3320 2a20 7665 746f  ath.pow(3 * veto
-00014eb0: 5f76 6f6c 756d 6520 2f20 2834 202a 206d  _volume / (4 * m
-00014ec0: 6174 682e 7069 292c 2031 2e30 202f 2033  ath.pi), 1.0 / 3
-00014ed0: 2e30 290d 0a0d 0a20 2020 2020 2020 2020  .0)....         
-00014ee0: 2020 206c 6f63 6174 696f 6e20 3d20 2863     location = (c
-00014ef0: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014f00: 305d 202a 2073 656c 662e 7a63 616c 6962  0] * self.zcalib
-00014f10: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
-00014f20: 735b 696e 6465 785d 5b31 5d2a 7365 6c66  s[index][1]*self
-00014f30: 2e79 6361 6c69 6272 6174 696f 6e2c 2063  .ycalibration, c
-00014f40: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
-00014f50: 325d 2a73 656c 662e 7863 616c 6962 7261  2]*self.xcalibra
-00014f60: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00014f70: 2020 2051 5541 4c49 5459 203d 206d 6174     QUALITY = mat
-00014f80: 682e 706f 7728 766f 6c75 6d65 5b69 6e64  h.pow(volume[ind
-00014f90: 6578 5d2c 2031 2e30 2f33 2e30 290d 0a20  ex], 1.0/3.0).. 
-00014fa0: 2020 2020 2020 2020 2020 2052 4144 4955             RADIU
-00014fb0: 5320 3d20 6d61 7468 2e70 6f77 2876 6f6c  S = math.pow(vol
-00014fc0: 756d 655b 696e 6465 785d 202a 2073 656c  ume[index] * sel
-00014fd0: 662e 7863 616c 6962 7261 7469 6f6e 202a  f.xcalibration *
-00014fe0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
-00014ff0: 6f6e 202a 2073 656c 662e 7a63 616c 6962  on * self.zcalib
-00015000: 7261 7469 6f6e 2c20 312e 302f 332e 3029  ration, 1.0/3.0)
-00015010: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-00015020: 2064 6973 7461 6e63 655f 6365 6c6c 5f6d   distance_cell_m
-00015030: 6173 6b2c 206d 6173 6b63 656e 7472 6f69  ask, maskcentroi
-00015040: 6420 3d20 7365 6c66 2e5f 6765 745f 626f  d = self._get_bo
-00015050: 756e 6461 7279 5f64 6973 7428 6672 616d  undary_dist(fram
-00015060: 652c 206c 6f63 6174 696f 6e29 0d0a 2020  e, location)..  
-00015070: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
-00015080: 7420 3c3d 2032 202a 2076 6574 6f5f 7261  t <= 2 * veto_ra
-00015090: 6469 7573 3a0d 0a20 2020 2020 2020 2020  dius:..         
-000150a0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-000150b0: 6e65 6c5f 756e 6971 7565 5f73 706f 745f  nel_unique_spot_
-000150c0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
-000150d0: 6964 5d20 3d20 7b0d 0a20 2020 2020 2020  id] = {..       
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2073 656c 662e 6365 6c6c 6964 5f6b 6579   self.cellid_key
-00015100: 3a20 696e 7428 6365 6c6c 5f69 6429 2c20  : int(cell_id), 
-00015110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015120: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00015130: 7261 6d65 6964 5f6b 6579 203a 2069 6e74  rameid_key : int
-00015140: 2866 7261 6d65 292c 0d0a 2020 2020 2020  (frame),..      
-00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015160: 2020 7365 6c66 2e7a 706f 7369 645f 6b65    self.zposid_ke
-00015170: 7920 3a20 666c 6f61 7428 6365 6e74 726f  y : float(centro
-00015180: 6964 735b 696e 6465 785d 5b30 5d2a 2073  ids[index][0]* s
-00015190: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-000151a0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000151b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000151c0: 2e79 706f 7369 645f 6b65 7920 3a20 666c  .yposid_key : fl
-000151d0: 6f61 7428 6365 6e74 726f 6964 735b 696e  oat(centroids[in
-000151e0: 6465 785d 5b31 5d2a 2073 656c 662e 7963  dex][1]* self.yc
-000151f0: 616c 6962 7261 7469 6f6e 292c 0d0a 2020  alibration),..  
-00015200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015210: 2020 2020 2020 7365 6c66 2e78 706f 7369        self.xposi
-00015220: 645f 6b65 7920 3a20 666c 6f61 7428 6365  d_key : float(ce
-00015230: 6e74 726f 6964 735b 696e 6465 785d 5b32  ntroids[index][2
-00015240: 5d2a 2073 656c 662e 7863 616c 6962 7261  ]* self.xcalibra
-00015250: 7469 6f6e 292c 0d0a 2020 2020 2020 2020  tion),..        
-00015260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015270: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
-00015280: 3a20 696e 7428 7472 6163 6b5f 6964 292c  : int(track_id),
-00015290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000152a0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000152b0: 6f74 616c 5f69 6e74 656e 7369 7479 5f6b  otal_intensity_k
-000152c0: 6579 203a 2028 666c 6f61 7428 696e 7465  ey : (float(inte
-000152d0: 6e73 6974 795f 746f 7461 6c5b 696e 6465  nsity_total[inde
-000152e0: 785d 2929 2c0d 0a20 2020 2020 2020 2020  x])),..         
-000152f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015300: 656c 662e 6d65 616e 5f69 6e74 656e 7369  elf.mean_intensi
-00015310: 7479 5f6b 6579 203a 2028 666c 6f61 7428  ty_key : (float(
-00015320: 696e 7465 6e73 6974 795f 6d65 616e 5b69  intensity_mean[i
-00015330: 6e64 6578 5d29 292c 0d0a 2020 2020 2020  ndex])),..      
+00014720: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
+00014730: 7361 6d70 6c65 203d 2078 665f 7361 6d70  sample = xf_samp
+00014740: 6c65 5b30 203a 206c 656e 2878 665f 7361  le[0 : len(xf_sa
+00014750: 6d70 6c65 2920 2f2f 2032 5d0d 0a20 2020  mple) // 2]..   
+00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014770: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00014780: 746f 7461 6c5f 7361 6d70 6c65 203d 2066  total_sample = f
+00014790: 6674 746f 7461 6c5f 7361 6d70 6c65 5b30  fttotal_sample[0
+000147a0: 203a 206c 656e 2866 6674 746f 7461 6c5f   : len(ffttotal_
+000147b0: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a0d  sample) // 2]...
+000147c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000147d0: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
+000147e0: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+000147f0: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00014800: 655f 6964 5d20 3d20 6578 7061 6e64 6564  e_id] = expanded
+00014810: 5f74 696d 652c 2065 7870 616e 6465 645f  _time, expanded_
+00014820: 696e 7465 6e73 6974 792c 2078 665f 7361  intensity, xf_sa
+00014830: 6d70 6c65 2c20 6666 7474 6f74 616c 5f73  mple, ffttotal_s
+00014840: 616d 706c 650d 0a20 2020 2020 2020 2020  ample..         
+00014850: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00014860: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+00014870: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00014880: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+00014890: 3d20 2063 7572 7265 6e74 5f74 696d 650d  =  current_time.
+000148a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000148b0: 2020 2020 756e 6971 7565 5f73 6861 7065      unique_shape
+000148c0: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+000148d0: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+000148e0: 7175 655f 6964 5d20 3d20 6375 7272 656e  que_id] = curren
+000148f0: 745f 7469 6d65 2c20 6375 7272 656e 745f  t_time, current_
+00014900: 7a2c 2063 7572 7265 6e74 5f79 2c20 6375  z, current_y, cu
+00014910: 7272 656e 745f 782c 2063 7572 7265 6e74  rrent_x, current
+00014920: 5f72 6164 6975 732c 2063 7572 7265 6e74  _radius, current
+00014930: 5f76 6f6c 756d 652c 2063 7572 7265 6e74  _volume, current
+00014940: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00014950: 6d70 5f66 6972 7374 2c20 6375 7272 656e  mp_first, curren
+00014960: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
+00014970: 6f6d 705f 7365 636f 6e64 2c20 6375 7272  omp_second, curr
+00014980: 656e 745f 7375 7266 6163 655f 6172 6561  ent_surface_area
+00014990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000149a0: 2020 2020 2075 6e69 7175 655f 6479 6e61       unique_dyna
+000149b0: 6d69 635f 7072 6f70 6572 7469 6573 5f74  mic_properties_t
+000149c0: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
+000149d0: 756e 6971 7565 5f69 645d 203d 2063 7572  unique_id] = cur
+000149e0: 7265 6e74 5f74 696d 652c 2063 7572 7265  rent_time, curre
+000149f0: 6e74 5f73 7065 6564 2c20 6375 7272 656e  nt_speed, curren
+00014a00: 745f 6d6f 7469 6f6e 5f61 6e67 6c65 2c20  t_motion_angle, 
+00014a10: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
+00014a20: 7469 6f6e 2c20 6375 7272 656e 745f 6469  tion, current_di
+00014a30: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00014a40: 2c20 6375 7272 656e 745f 7261 6469 616c  , current_radial
+00014a50: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
+00014a60: 6365 6c6c 5f61 7869 735f 6d61 736b 0d0a  cell_axis_mask..
+00014a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a80: 2020 2073 656c 662e 756e 6971 7565 5f66     self.unique_f
+00014a90: 6674 5f70 726f 7065 7274 6965 735b 7472  ft_properties[tr
+00014aa0: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
+00014ab0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00014ac0: 643a 756e 6971 7565 5f66 6674 5f70 726f  d:unique_fft_pro
+00014ad0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+00014ae0: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
+00014af0: 6964 5d7d 290d 0a20 2020 2020 2020 2020  id]})..         
+00014b00: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+00014b10: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
+00014b20: 6f70 6572 7469 6573 5b74 7261 636b 5f69  operties[track_i
+00014b30: 645d 2e75 7064 6174 6528 7b63 7572 7265  d].update({curre
+00014b40: 6e74 5f75 6e69 7175 655f 6964 3a75 6e69  nt_unique_id:uni
+00014b50: 7175 655f 636c 7573 7465 725f 7072 6f70  que_cluster_prop
+00014b60: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00014b70: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00014b80: 645d 7d29 0d0a 0d0a 2020 2020 2020 2020  d]})....        
+00014b90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014ba0: 756e 6971 7565 5f73 6861 7065 5f70 726f  unique_shape_pro
+00014bb0: 7065 7274 6965 735b 7472 6163 6b5f 6964  perties[track_id
+00014bc0: 5d2e 7570 6461 7465 287b 6375 7272 656e  ].update({curren
+00014bd0: 745f 756e 6971 7565 5f69 643a 756e 6971  t_unique_id:uniq
+00014be0: 7565 5f73 6861 7065 5f70 726f 7065 7274  ue_shape_propert
+00014bf0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00014c00: 7265 6e74 5f75 6e69 7175 655f 6964 5d7d  rent_unique_id]}
+00014c10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014c20: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00014c30: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
+00014c40: 7469 6573 5b74 7261 636b 5f69 645d 2e75  ties[track_id].u
+00014c50: 7064 6174 6528 7b63 7572 7265 6e74 5f75  pdate({current_u
+00014c60: 6e69 7175 655f 6964 3a75 6e69 7175 655f  nique_id:unique_
+00014c70: 6479 6e61 6d69 635f 7072 6f70 6572 7469  dynamic_properti
+00014c80: 6573 5f74 7261 636b 6c65 745b 6375 7272  es_tracklet[curr
+00014c90: 656e 745f 756e 6971 7565 5f69 645d 7d29  ent_unique_id]})
+00014ca0: 0d0a 0d0a 2020 2020 6465 6620 5f73 6563  ....    def _sec
+00014cb0: 6f6e 645f 6368 616e 6e65 6c5f 7370 6f74  ond_channel_spot
+00014cc0: 7328 7365 6c66 2c20 6672 616d 652c 207a  s(self, frame, z
+00014cd0: 2c20 792c 2078 2c20 6365 6c6c 5f69 642c  , y, x, cell_id,
+00014ce0: 2074 7261 636b 5f69 6429 3a0d 0a20 2020   track_id):..   
+00014cf0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00014d00: 2020 2020 2020 7472 6565 2c20 6365 6e74        tree, cent
+00014d10: 726f 6964 732c 206c 6162 656c 732c 2076  roids, labels, v
+00014d20: 6f6c 756d 652c 2069 6e74 656e 7369 7479  olume, intensity
+00014d30: 5f6d 6561 6e2c 2069 6e74 656e 7369 7479  _mean, intensity
+00014d40: 5f74 6f74 616c 2c20 626f 756e 6469 6e67  _total, bounding
+00014d50: 5f62 6f78 6573 203d 2073 656c 662e 5f74  _boxes = self._t
+00014d60: 696d 6564 5f63 6861 6e6e 656c 5f73 6567  imed_channel_seg
+00014d70: 5f69 6d61 6765 5b73 7472 2869 6e74 2866  _image[str(int(f
+00014d80: 6c6f 6174 2866 7261 6d65 2929 295d 0d0a  loat(frame)))]..
+00014d90: 2020 2020 2020 2020 2020 2020 7069 7865              pixe
+00014da0: 6c74 6573 746c 6f63 6174 696f 6e20 3d20  ltestlocation = 
+00014db0: 287a 2c79 2c78 290d 0a20 2020 2020 2020  (z,y,x)..       
+00014dc0: 2020 2020 2064 6973 742c 2069 6e64 6578       dist, index
+00014dd0: 203d 2074 7265 652e 7175 6572 7928 7069   = tree.query(pi
+00014de0: 7865 6c74 6573 746c 6f63 6174 696f 6e29  xeltestlocation)
+00014df0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00014e00: 2020 6262 6f78 203d 2062 6f75 6e64 696e    bbox = boundin
+00014e10: 675f 626f 7865 735b 696e 6465 785d 0d0a  g_boxes[index]..
+00014e20: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00014e30: 7a20 3d20 6162 7328 6262 6f78 5b30 5d20  z = abs(bbox[0] 
+00014e40: 2d20 6262 6f78 5b33 5d29 0d0a 2020 2020  - bbox[3])..    
+00014e50: 2020 2020 2020 2020 7369 7a65 7920 3d20          sizey = 
+00014e60: 6162 7328 6262 6f78 5b31 5d20 2d20 6262  abs(bbox[1] - bb
+00014e70: 6f78 5b34 5d29 0d0a 2020 2020 2020 2020  ox[4])..        
+00014e80: 2020 2020 7369 7a65 7820 3d20 6162 7328      sizex = abs(
+00014e90: 6262 6f78 5b32 5d20 2d20 6262 6f78 5b35  bbox[2] - bbox[5
+00014ea0: 5d29 200d 0a20 2020 2020 2020 2020 2020  ]) ..           
+00014eb0: 2076 6574 6f5f 766f 6c75 6d65 203d 2073   veto_volume = s
+00014ec0: 697a 6578 202a 2073 697a 6579 202a 2073  izex * sizey * s
+00014ed0: 697a 657a 0d0a 2020 2020 2020 2020 2020  izez..          
+00014ee0: 2020 7665 746f 5f72 6164 6975 7320 3d20    veto_radius = 
+00014ef0: 6d61 7468 2e70 6f77 2833 202a 2076 6574  math.pow(3 * vet
+00014f00: 6f5f 766f 6c75 6d65 202f 2028 3420 2a20  o_volume / (4 * 
+00014f10: 6d61 7468 2e70 6929 2c20 312e 3020 2f20  math.pi), 1.0 / 
+00014f20: 332e 3029 0d0a 0d0a 2020 2020 2020 2020  3.0)....        
+00014f30: 2020 2020 6c6f 6361 7469 6f6e 203d 2028      location = (
+00014f40: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00014f50: 5b30 5d20 2a20 7365 6c66 2e7a 6361 6c69  [0] * self.zcali
+00014f60: 6272 6174 696f 6e2c 2063 656e 7472 6f69  bration, centroi
+00014f70: 6473 5b69 6e64 6578 5d5b 315d 2a73 656c  ds[index][1]*sel
+00014f80: 662e 7963 616c 6962 7261 7469 6f6e 2c20  f.ycalibration, 
+00014f90: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
+00014fa0: 5b32 5d2a 7365 6c66 2e78 6361 6c69 6272  [2]*self.xcalibr
+00014fb0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00014fc0: 2020 2020 5155 414c 4954 5920 3d20 6d61      QUALITY = ma
+00014fd0: 7468 2e70 6f77 2876 6f6c 756d 655b 696e  th.pow(volume[in
+00014fe0: 6465 785d 2c20 312e 302f 332e 3029 0d0a  dex], 1.0/3.0)..
+00014ff0: 2020 2020 2020 2020 2020 2020 5241 4449              RADI
+00015000: 5553 203d 206d 6174 682e 706f 7728 766f  US = math.pow(vo
+00015010: 6c75 6d65 5b69 6e64 6578 5d20 2a20 7365  lume[index] * se
+00015020: 6c66 2e78 6361 6c69 6272 6174 696f 6e20  lf.xcalibration 
+00015030: 2a20 7365 6c66 2e79 6361 6c69 6272 6174  * self.ycalibrat
+00015040: 696f 6e20 2a20 7365 6c66 2e7a 6361 6c69  ion * self.zcali
+00015050: 6272 6174 696f 6e2c 2031 2e30 2f33 2e30  bration, 1.0/3.0
+00015060: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
+00015070: 2020 6469 7374 616e 6365 5f63 656c 6c5f    distance_cell_
+00015080: 6d61 736b 2c20 6d61 736b 6365 6e74 726f  mask, maskcentro
+00015090: 6964 203d 2073 656c 662e 5f67 6574 5f62  id = self._get_b
+000150a0: 6f75 6e64 6172 795f 6469 7374 2866 7261  oundary_dist(fra
+000150b0: 6d65 2c20 6c6f 6361 7469 6f6e 290d 0a20  me, location).. 
+000150c0: 2020 2020 2020 2020 2020 2069 6620 6469             if di
+000150d0: 7374 203c 3d20 3220 2a20 7665 746f 5f72  st <= 2 * veto_r
+000150e0: 6164 6975 733a 0d0a 2020 2020 2020 2020  adius:..        
+000150f0: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
+00015100: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
+00015110: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
+00015120: 5f69 645d 203d 207b 0d0a 2020 2020 2020  _id] = {..      
+00015130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015140: 2020 7365 6c66 2e63 656c 6c69 645f 6b65    self.cellid_ke
+00015150: 793a 2069 6e74 2863 656c 6c5f 6964 292c  y: int(cell_id),
+00015160: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00015170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015180: 6672 616d 6569 645f 6b65 7920 3a20 696e  frameid_key : in
+00015190: 7428 6672 616d 6529 2c0d 0a20 2020 2020  t(frame),..     
+000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151b0: 2020 2073 656c 662e 7a70 6f73 6964 5f6b     self.zposid_k
+000151c0: 6579 203a 2066 6c6f 6174 2863 656e 7472  ey : float(centr
+000151d0: 6f69 6473 5b69 6e64 6578 5d5b 305d 2a20  oids[index][0]* 
+000151e0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
+000151f0: 6e29 2c0d 0a20 2020 2020 2020 2020 2020  n),..           
+00015200: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015210: 662e 7970 6f73 6964 5f6b 6579 203a 2066  f.yposid_key : f
+00015220: 6c6f 6174 2863 656e 7472 6f69 6473 5b69  loat(centroids[i
+00015230: 6e64 6578 5d5b 315d 2a20 7365 6c66 2e79  ndex][1]* self.y
+00015240: 6361 6c69 6272 6174 696f 6e29 2c0d 0a20  calibration),.. 
+00015250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015260: 2020 2020 2020 2073 656c 662e 7870 6f73         self.xpos
+00015270: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+00015280: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00015290: 325d 2a20 7365 6c66 2e78 6361 6c69 6272  2]* self.xcalibr
+000152a0: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+000152b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152c0: 2073 656c 662e 7472 6163 6b69 645f 6b65   self.trackid_ke
+000152d0: 793a 2069 6e74 2874 7261 636b 5f69 6429  y: int(track_id)
+000152e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000152f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015300: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
+00015310: 6b65 7920 3a20 2866 6c6f 6174 2869 6e74  key : (float(int
+00015320: 656e 7369 7479 5f74 6f74 616c 5b69 6e64  ensity_total[ind
+00015330: 6578 5d29 292c 0d0a 2020 2020 2020 2020  ex])),..        
 00015340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015350: 2020 7365 6c66 2e72 6164 6975 735f 6b65    self.radius_ke
-00015360: 7920 3a20 2866 6c6f 6174 2852 4144 4955  y : (float(RADIU
-00015370: 5329 292c 0d0a 2020 2020 2020 2020 2020  S)),..          
-00015380: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015390: 6c66 2e71 7561 6c69 7479 5f6b 6579 203a  lf.quality_key :
-000153a0: 2028 666c 6f61 7428 5155 414c 4954 5929   (float(QUALITY)
-000153b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000153c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000153d0: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
-000153e0: 6173 6b5f 6b65 793a 2066 6c6f 6174 2864  ask_key: float(d
-000153f0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00015400: 6b29 2c0d 0a20 2020 2020 2020 2020 2020  k),..           
+00015350: 7365 6c66 2e6d 6561 6e5f 696e 7465 6e73  self.mean_intens
+00015360: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
+00015370: 2869 6e74 656e 7369 7479 5f6d 6561 6e5b  (intensity_mean[
+00015380: 696e 6465 785d 2929 2c0d 0a20 2020 2020  index])),..     
+00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153a0: 2020 2073 656c 662e 7261 6469 7573 5f6b     self.radius_k
+000153b0: 6579 203a 2028 666c 6f61 7428 5241 4449  ey : (float(RADI
+000153c0: 5553 2929 2c0d 0a20 2020 2020 2020 2020  US)),..         
+000153d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000153e0: 656c 662e 7175 616c 6974 795f 6b65 7920  elf.quality_key 
+000153f0: 3a20 2866 6c6f 6174 2851 5541 4c49 5459  : (float(QUALITY
+00015400: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
 00015410: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015420: 662e 6d61 736b 6365 6e74 726f 6964 5f7a  f.maskcentroid_z
-00015430: 5f6b 6579 3a20 666c 6f61 7428 6d61 736b  _key: float(mask
-00015440: 6365 6e74 726f 6964 5b30 5d29 2c0d 0a20  centroid[0]),.. 
-00015450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015460: 2020 2020 2020 2073 656c 662e 6d61 736b         self.mask
-00015470: 6365 6e74 726f 6964 5f79 5f6b 6579 3a20  centroid_y_key: 
-00015480: 666c 6f61 7428 6d61 736b 6365 6e74 726f  float(maskcentro
-00015490: 6964 5b31 5d29 2c0d 0a20 2020 2020 2020  id[1]),..       
+00015420: 662e 6469 7374 616e 6365 5f63 656c 6c5f  f.distance_cell_
+00015430: 6d61 736b 5f6b 6579 3a20 666c 6f61 7428  mask_key: float(
+00015440: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00015450: 736b 292c 0d0a 2020 2020 2020 2020 2020  sk),..          
+00015460: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015470: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00015480: 7a5f 6b65 793a 2066 6c6f 6174 286d 6173  z_key: float(mas
+00015490: 6b63 656e 7472 6f69 645b 305d 292c 0d0a  kcentroid[0]),..
 000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154b0: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
-000154c0: 6964 5f78 5f6b 6579 3a20 666c 6f61 7428  id_x_key: float(
-000154d0: 6d61 736b 6365 6e74 726f 6964 5b32 5d29  maskcentroid[2])
-000154e0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
-000154f0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00015500: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00015510: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015520: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
-00015530: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015540: 6573 5b63 656c 6c5f 6964 5d20 3d20 7365  es[cell_id] = se
-00015550: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015560: 726f 7065 7274 6965 735b 6365 6c6c 5f69  roperties[cell_i
-00015570: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-00015580: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00015590: 6e6e 656c 5f75 6e69 7175 655f 7370 6f74  nnel_unique_spot
-000155a0: 5f70 726f 7065 7274 6965 735b 6365 6c6c  _properties[cell
-000155b0: 5f69 645d 2e75 7064 6174 6528 7b73 656c  _id].update({sel
-000155c0: 662e 746f 7461 6c5f 696e 7465 6e73 6974  f.total_intensit
-000155d0: 795f 6b65 793a 202d 317d 290d 0a20 2020  y_key: -1})..   
-000155e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155f0: 2073 656c 662e 6368 616e 6e65 6c5f 756e   self.channel_un
-00015600: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015610: 7469 6573 5b63 656c 6c5f 6964 5d2e 7570  ties[cell_id].up
-00015620: 6461 7465 287b 7365 6c66 2e6d 6561 6e5f  date({self.mean_
-00015630: 696e 7465 6e73 6974 795f 6b65 793a 202d  intensity_key: -
-00015640: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-00015650: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00015660: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-00015670: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-00015680: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
-00015690: 6c66 2e72 6164 6975 735f 6b65 793a 202d  lf.radius_key: -
-000156a0: 317d 290d 0a20 2020 2020 2020 2020 2020  1})..           
-000156b0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-000156c0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-000156d0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-000156e0: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
-000156f0: 6c66 2e71 7561 6c69 7479 5f6b 6579 3a20  lf.quality_key: 
-00015700: 2d31 7d29 0d0a 0d0a 0d0a 0d0a 2020 2020  -1})........    
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015720: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00015730: 2020 2064 6566 205f 6469 6374 5f75 7064     def _dict_upd
-00015740: 6174 6528 7365 6c66 2c20 756e 6971 7565  ate(self, unique
-00015750: 5f74 7261 636b 6c65 745f 6964 733a 204c  _tracklet_ids: L
-00015760: 6973 742c 2020 6365 6c6c 5f69 643a 2069  ist,  cell_id: i
-00015770: 6e74 2c20 7472 6163 6b5f 6964 3a20 696e  nt, track_id: in
-00015780: 742c 2073 6f75 7263 655f 6964 3a20 696e  t, source_id: in
-00015790: 742c 2074 6172 6765 745f 6964 3a20 696e  t, target_id: in
-000157a0: 7429 3a0d 0a0d 0a20 0d0a 2020 2020 2020  t):.... ..      
-000157b0: 2020 6765 6e65 7261 7469 6f6e 5f69 6420    generation_id 
-000157c0: 3d20 7365 6c66 2e67 656e 6572 6174 696f  = self.generatio
-000157d0: 6e5f 6469 6374 5b63 656c 6c5f 6964 5d0d  n_dict[cell_id].
-000157e0: 0a20 2020 2020 2020 2074 7261 636b 6c65  .        trackle
-000157f0: 745f 6964 203d 2073 656c 662e 7472 6163  t_id = self.trac
-00015800: 6b6c 6574 5f64 6963 745b 6365 6c6c 5f69  klet_dict[cell_i
-00015810: 645d 0d0a 2020 2020 2020 200d 0a0d 0a20  d]..       .... 
-00015820: 2020 2020 2020 2075 6e69 7175 655f 6964         unique_id
-00015830: 203d 2073 7472 2874 7261 636b 5f69 6429   = str(track_id)
-00015840: 202b 2020 7374 7228 6765 6e65 7261 7469   +  str(generati
-00015850: 6f6e 5f69 6429 202b 2073 7472 2874 7261  on_id) + str(tra
-00015860: 636b 6c65 745f 6964 290d 0a20 2020 2020  cklet_id)..     
-00015870: 2020 200d 0a20 2020 2020 2020 2076 6563     ..        vec
-00015880: 5f6d 6173 6b20 3d20 5b66 6c6f 6174 2873  _mask = [float(s
-00015890: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-000158a0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000158b0: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-000158c0: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-000158d0: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-000158e0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000158f0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015900: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
-00015910: 7472 6f69 645f 795f 6b65 795d 292c 2066  troid_y_key]), f
-00015920: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00015930: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015940: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00015950: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-00015960: 5f7a 5f6b 6579 5d29 205d 0d0a 0d0a 2020  _z_key]) ]....  
-00015970: 2020 2020 2020 7665 635f 6365 6c6c 203d        vec_cell =
-00015980: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00015990: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000159a0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-000159b0: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-000159c0: 795d 2920 2c20 0d0a 2020 2020 2020 2020  y]) , ..        
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-000159f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015a00: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015a10: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00015a20: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
-00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a40: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-00015a50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015a60: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015a70: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00015a80: 5f6b 6579 5d29 5d0d 0a0d 0a20 2020 2020  _key])]....     
-00015a90: 2020 2061 6e67 6c65 203d 2061 6e67 756c     angle = angul
-00015aa0: 6172 5f63 6861 6e67 6528 7665 635f 6d61  ar_change(vec_ma
-00015ab0: 736b 2c20 7665 635f 6365 6c6c 290d 0a0d  sk, vec_cell)...
-00015ac0: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00015ad0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015ae0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015af0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015b00: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-00015b10: 203a 2061 6e67 6c65 7d29 2020 2020 2020   : angle})      
-00015b20: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00015b30: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
-00015b40: 5f74 7261 636b 6c65 745f 6964 732e 6170  _tracklet_ids.ap
-00015b50: 7065 6e64 2873 7472 2875 6e69 7175 655f  pend(str(unique_
-00015b60: 6964 2929 0d0a 2020 2020 2020 2020 7365  id))..        se
-00015b70: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015b80: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015b90: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015ba0: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
-00015bb0: 7920 3a20 7374 7228 756e 6971 7565 5f69  y : str(unique_i
-00015bc0: 6429 7d29 0d0a 2020 2020 2020 2020 7365  d)})..        se
-00015bd0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015be0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015bf0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015c00: 7365 6c66 2e74 7261 636b 6c65 7469 645f  self.trackletid_
-00015c10: 6b65 7920 3a20 7374 7228 7472 6163 6b6c  key : str(trackl
-00015c20: 6574 5f69 6429 7d29 200d 0a20 2020 2020  et_id)}) ..     
-00015c30: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015c40: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015c50: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015c60: 6174 6528 7b73 656c 662e 6765 6e65 7261  ate({self.genera
-00015c70: 7469 6f6e 6964 5f6b 6579 203a 2073 7472  tionid_key : str
-00015c80: 2867 656e 6572 6174 696f 6e5f 6964 297d  (generation_id)}
-00015c90: 2920 0d0a 2020 2020 2020 2020 7365 6c66  ) ..        self
-00015ca0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015cb0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-00015cc0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00015cd0: 6c66 2e74 7261 636b 6964 5f6b 6579 203a  lf.trackid_key :
-00015ce0: 2073 7472 2874 7261 636b 5f69 6429 7d29   str(track_id)})
-00015cf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00015d00: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00015d10: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00015d20: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-00015d30: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
-00015d40: 7920 3a20 302e 307d 290d 0a20 2020 2020  y : 0.0})..     
-00015d50: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015d60: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015d70: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015d80: 6174 6528 7b73 656c 662e 7370 6565 645f  ate({self.speed_
-00015d90: 6b65 7920 3a20 302e 307d 290d 0a20 2020  key : 0.0})..   
-00015da0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015db0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015dc0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015dd0: 7064 6174 6528 7b73 656c 662e 6163 6365  pdate({self.acce
-00015de0: 6c65 7261 7469 6f6e 5f6b 6579 203a 2030  leration_key : 0
-00015df0: 2e30 7d29 0d0a 2020 2020 2020 2020 7365  .0})..        se
-00015e00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015e10: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015e20: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015e30: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00015e40: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
-00015e50: 3a20 2d31 7d29 0d0a 2020 2020 2020 2020  : -1})..        
-00015e60: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015e70: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015e80: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00015e90: 287b 7365 6c66 2e65 6363 656e 7472 6963  ({self.eccentric
-00015ea0: 6974 795f 636f 6d70 5f73 6563 6f6e 646b  ity_comp_secondk
-00015eb0: 6579 203a 202d 317d 290d 0a20 2020 2020  ey : -1})..     
-00015ec0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015ed0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015ee0: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015ef0: 6174 6528 7b73 656c 662e 7375 7266 6163  ate({self.surfac
-00015f00: 655f 6172 6561 5f6b 6579 203a 202d 317d  e_area_key : -1}
-00015f10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00015f20: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00015f30: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00015f40: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00015f50: 662e 6365 6c6c 6178 6973 5f6d 6173 6b5f  f.cellaxis_mask_
-00015f60: 6b65 7920 3a20 2d31 7d29 0d0a 0d0a 2020  key : -1})....  
-00015f70: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
-00015f80: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0d  id is not None:.
-00015f90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00015fa0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00015fb0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00015fc0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00015fd0: 656c 662e 6265 666f 7265 6964 5f6b 6579  elf.beforeid_key
-00015fe0: 203a 2069 6e74 2873 6f75 7263 655f 6964   : int(source_id
-00015ff0: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
-00016000: 2076 6563 5f31 203d 205b 666c 6f61 7428   vec_1 = [float(
-00016010: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00016020: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016030: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00016040: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
-00016050: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00016060: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016070: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-00016080: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
-00016090: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160b0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000160c0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000160d0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-000160e0: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
-000160f0: 5d29 202d 2066 6c6f 6174 2873 656c 662e  ]) - float(self.
-00016100: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00016110: 6572 7469 6573 5b69 6e74 2873 6f75 7263  erties[int(sourc
-00016120: 655f 6964 295d 5b73 656c 662e 7970 6f73  e_id)][self.ypos
-00016130: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00016160: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016170: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00016180: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
-00016190: 7369 645f 6b65 795d 2920 2d20 2066 6c6f  sid_key]) -  flo
-000161a0: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-000161b0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-000161c0: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-000161d0: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-000161e0: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
-000161f0: 7065 6564 203d 206e 702e 7371 7274 286e  peed = np.sqrt(n
-00016200: 702e 646f 7428 7665 635f 312c 2076 6563  p.dot(vec_1, vec
-00016210: 5f31 2929 2f73 656c 662e 7463 616c 6962  _1))/self.tcalib
-00016220: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00016230: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00016240: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00016250: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00016260: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
-00016270: 5f6b 6579 203a 2073 7065 6564 7d29 0d0a  _key : speed})..
-00016280: 0d0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
-00016290: 7469 6f6e 5f61 6e67 6c65 203d 2061 6e67  tion_angle = ang
-000162a0: 756c 6172 5f63 6861 6e67 6528 7665 635f  ular_change(vec_
-000162b0: 6d61 736b 2c20 7665 635f 3129 0d0a 0d0a  mask, vec_1)....
-000162c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000162d0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000162e0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
-000162f0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
-00016300: 6c66 2e6d 6f74 696f 6e5f 616e 676c 655f  lf.motion_angle_
-00016310: 6b65 7920 3a20 6d6f 7469 6f6e 5f61 6e67  key : motion_ang
-00016320: 6c65 7d29 200d 0a0d 0a20 2020 2020 2020  le}) ....       
-00016330: 2020 2020 2069 6620 736f 7572 6365 5f69       if source_i
-00016340: 6420 696e 2073 656c 662e 6564 6765 5f73  d in self.edge_s
-00016350: 6f75 7263 655f 6c6f 6f6b 7570 3a0d 0a20  ource_lookup:.. 
-00016360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016370: 2020 2070 7265 5f73 6f75 7263 655f 6964     pre_source_id
-00016380: 203d 2073 656c 662e 6564 6765 5f73 6f75   = self.edge_sou
-00016390: 7263 655f 6c6f 6f6b 7570 5b73 6f75 7263  rce_lookup[sourc
-000163a0: 655f 6964 5d0d 0a20 2020 2020 2020 2020  e_id]..         
-000163b0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-000163c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163d0: 2076 6563 5f32 203d 205b 666c 6f61 7428   vec_2 = [float(
-000163e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000163f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00016400: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e78  cell_id)][self.x
-00016410: 706f 7369 645f 6b65 795d 2920 2d20 3220  posid_key]) - 2 
-00016420: 2a20 666c 6f61 7428 7365 6c66 2e75 6e69  * float(self.uni
-00016430: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00016440: 6965 735b 696e 7428 736f 7572 6365 5f69  ies[int(source_i
-00016450: 6429 5d5b 7365 6c66 2e78 706f 7369 645f  d)][self.xposid_
-00016460: 6b65 795d 2920 2b20 666c 6f61 7428 7365  key]) + float(se
-00016470: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00016480: 726f 7065 7274 6965 735b 696e 7428 7072  roperties[int(pr
-00016490: 655f 736f 7572 6365 5f69 6429 5d5b 7365  e_source_id)][se
-000164a0: 6c66 2e78 706f 7369 645f 6b65 795d 292c  lf.xposid_key]),
-000164b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000164c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000164d0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-000164e0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-000164f0: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00016500: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
-00016510: 202d 2032 202a 2066 6c6f 6174 2873 656c   - 2 * float(sel
-00016520: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00016530: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-00016540: 7263 655f 6964 295d 5b73 656c 662e 7970  rce_id)][self.yp
-00016550: 6f73 6964 5f6b 6579 5d29 202b 2066 6c6f  osid_key]) + flo
-00016560: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016570: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016580: 6e74 2870 7265 5f73 6f75 7263 655f 6964  nt(pre_source_id
-00016590: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
-000165a0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
-000165b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165c0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-000165d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000165e0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000165f0: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
-00016600: 6b65 795d 2920 2d20 2032 202a 2066 6c6f  key]) -  2 * flo
-00016610: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00016620: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00016630: 6e74 2873 6f75 7263 655f 6964 295d 5b73  nt(source_id)][s
-00016640: 656c 662e 7a70 6f73 6964 5f6b 6579 5d29  elf.zposid_key])
-00016650: 202b 2066 6c6f 6174 2873 656c 662e 756e   + float(self.un
-00016660: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00016670: 7469 6573 5b69 6e74 2870 7265 5f73 6f75  ties[int(pre_sou
-00016680: 7263 655f 6964 295d 5b73 656c 662e 7a70  rce_id)][self.zp
-00016690: 6f73 6964 5f6b 6579 5d29 5d0d 0a20 2020  osid_key])]..   
-000166a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166b0: 2061 6363 203d 206e 702e 7371 7274 286e   acc = np.sqrt(n
-000166c0: 702e 646f 7428 7665 635f 322c 2076 6563  p.dot(vec_2, vec
-000166d0: 5f32 2929 2f73 656c 662e 7463 616c 6962  _2))/self.tcalib
-000166e0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-000166f0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-00016720: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00016730: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-00016740: 7465 287b 7365 6c66 2e61 6363 656c 6572  te({self.acceler
-00016750: 6174 696f 6e5f 6b65 7920 3a20 6163 637d  ation_key : acc}
-00016760: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00016770: 736f 7572 6365 5f69 6420 6973 204e 6f6e  source_id is Non
-00016780: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00016790: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-000167a0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-000167b0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-000167c0: 287b 7365 6c66 2e62 6566 6f72 6569 645f  ({self.beforeid_
-000167d0: 6b65 7920 3a20 4e6f 6e65 7d29 200d 0a20  key : None}) .. 
-000167e0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-000167f0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00016800: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00016810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016820: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00016830: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00016840: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00016850: 7064 6174 6528 7b73 656c 662e 6166 7465  pdate({self.afte
-00016860: 7269 645f 6b65 7920 3a20 696e 7428 7461  rid_key : int(ta
-00016870: 7267 6574 5f69 6429 7d29 200d 0a20 2020  rget_id)}) ..   
-00016880: 2020 2020 2065 6c69 6620 7461 7267 6574       elif target
-00016890: 5f69 6420 6973 204e 6f6e 653a 0d0a 2020  _id is None:..  
-000168a0: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000168b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000168c0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-000168d0: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
-000168e0: 2e61 6674 6572 6964 5f6b 6579 203a 204e  .afterid_key : N
-000168f0: 6f6e 657d 290d 0a20 2020 2020 2020 2020  one})..         
-00016900: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-00016910: 662e 5f73 6563 6f6e 645f 6368 616e 6e65  f._second_channe
-00016920: 6c5f 7570 6461 7465 2863 656c 6c5f 6964  l_update(cell_id
-00016930: 2c20 7472 6163 6b5f 6964 2920 2020 200d  , track_id)    .
-00016940: 0a0d 0a0d 0a20 2020 2064 6566 205f 7465  .....    def _te
-00016950: 6d70 6f72 616c 5f70 6c6f 7473 5f74 7261  mporal_plots_tra
-00016960: 636b 6d61 7465 2873 656c 6629 3a0d 0a20  ckmate(self):.. 
-00016970: 2020 200d 0a20 2020 200d 0a20 2020 200d     ..    ..    .
-00016980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016990: 2073 656c 662e 4174 7472 203d 207b 7d0d   self.Attr = {}.
-000169a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169b0: 2073 7461 7274 7469 6d65 203d 2069 6e74   starttime = int
-000169c0: 286d 696e 2873 656c 662e 416c 6c56 616c  (min(self.AllVal
-000169d0: 7565 735b 7365 6c66 2e66 7261 6d65 6964  ues[self.frameid
-000169e0: 5f6b 6579 5d29 290d 0a20 2020 2020 2020  _key]))..       
-000169f0: 2020 2020 2020 2020 2065 6e64 7469 6d65           endtime
-00016a00: 203d 2069 6e74 286d 6178 2873 656c 662e   = int(max(self.
-00016a10: 416c 6c56 616c 7565 735b 7365 6c66 2e66  AllValues[self.f
-00016a20: 7261 6d65 6964 5f6b 6579 5d29 290d 0a20  rameid_key])).. 
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a50: 2020 7365 6c66 2e74 696d 6520 3d20 5b5d    self.time = []
-00016a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016a70: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00016a80: 6561 6e5f 6469 7370 5f7a 203d 205b 5d0d  ean_disp_z = [].
-00016a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016aa0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00016ab0: 725f 6469 7370 5f7a 203d 205b 5d0d 0a0d  r_disp_z = []...
-00016ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ad0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00016ae0: 616e 5f64 6973 705f 7920 3d20 5b5d 0d0a  an_disp_y = []..
-00016af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b00: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00016b10: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b30: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00016b40: 6e5f 6469 7370 5f78 203d 205b 5d0d 0a20  n_disp_x = [].. 
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016b60: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00016b70: 6469 7370 5f78 203d 205b 5d0d 0a0d 0a20  disp_x = [].... 
-00016b80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016b90: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00016ba0: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
-00016bb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016bc0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f72  lf.mitotic_var_r
-00016bd0: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00016be0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016bf0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00016c00: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
-00016c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016c20: 2e6d 6974 6f74 6963 5f76 6172 5f73 7065  .mitotic_var_spe
-00016c30: 6564 203d 205b 5d0d 0a0d 0a20 2020 2020  ed = []....     
-00016c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016c50: 6d69 746f 7469 635f 6d65 616e 5f61 6363  mitotic_mean_acc
-00016c60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016c70: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00016c80: 7469 635f 7661 725f 6163 6320 3d20 5b5d  tic_var_acc = []
-00016c90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016ca0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00016cb0: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00016cc0: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016ce0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00016cf0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00016d00: 6765 203d 205b 5d0d 0a0d 0a20 2020 2020  ge = []....     
-00016d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016d20: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00016d30: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
-00016d40: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016d50: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00016d60: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-00016d70: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-00016d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016d90: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00016da0: 6963 5f6d 6561 6e5f 6469 7370 5f7a 203d  ic_mean_disp_z =
-00016db0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00016dc0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00016dd0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
-00016de0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016df0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00016e00: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00016e10: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
-00016e20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016e30: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00016e40: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e60: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016e70: 5f6d 6561 6e5f 6469 7370 5f78 203d 205b  _mean_disp_x = [
-00016e80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016e90: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016ea0: 7469 635f 7661 725f 6469 7370 5f78 203d  tic_var_disp_x =
-00016eb0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00016ec0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00016ed0: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
-00016ee0: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
-00016ef0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00016f00: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f72  on_mitotic_var_r
-00016f10: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00016f20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016f30: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
-00016f40: 6561 6e5f 7370 6565 6420 3d20 5b5d 0d0a  ean_speed = []..
-00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f60: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016f70: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-00016f80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016f90: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016fa0: 7469 635f 6d65 616e 5f61 6363 203d 205b  tic_mean_acc = [
-00016fb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016fc0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016fd0: 7469 635f 7661 725f 6163 6320 3d20 5b5d  tic_var_acc = []
-00016fe0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00016ff0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00017000: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
-00017010: 696f 6e61 6c5f 6368 616e 6765 203d 205b  ional_change = [
-00017020: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017030: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00017040: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00017050: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00017060: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017070: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00017080: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
-00017090: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
-000170a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000170b0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000170c0: 6963 5f76 6172 5f64 6973 7461 6e63 655f  ic_var_distance_
-000170d0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-000170e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000170f0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00017100: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
-00017110: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017120: 662e 616c 6c5f 7661 725f 6469 7370 5f7a  f.all_var_disp_z
-00017130: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00017140: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00017150: 6c5f 6d65 616e 5f64 6973 705f 7920 3d20  l_mean_disp_y = 
-00017160: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017170: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00017180: 5f64 6973 705f 7920 3d20 5b5d 0d0a 0d0a  _disp_y = []....
-00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171a0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-000171b0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
-000171c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000171d0: 616c 6c5f 7661 725f 6469 7370 5f78 203d  all_var_disp_x =
-000171e0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000171f0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00017200: 6d65 616e 5f72 6164 6975 7320 3d20 5b5d  mean_radius = []
-00017210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017220: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f72    self.all_var_r
-00017230: 6164 6975 7320 3d20 5b5d 0d0a 0d0a 2020  adius = []....  
-00017240: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017250: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
-00017260: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-00017270: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00017280: 5f76 6172 5f73 7065 6564 203d 205b 5d0d  _var_speed = [].
-00017290: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000172a0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-000172b0: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-000172c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000172d0: 616c 6c5f 7661 725f 6163 6320 3d20 5b5d  all_var_acc = []
+000154b0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+000154c0: 6b63 656e 7472 6f69 645f 795f 6b65 793a  kcentroid_y_key:
+000154d0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
+000154e0: 6f69 645b 315d 292c 0d0a 2020 2020 2020  oid[1]),..      
+000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015500: 2020 7365 6c66 2e6d 6173 6b63 656e 7472    self.maskcentr
+00015510: 6f69 645f 785f 6b65 793a 2066 6c6f 6174  oid_x_key: float
+00015520: 286d 6173 6b63 656e 7472 6f69 645b 325d  (maskcentroid[2]
+00015530: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
+00015540: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00015550: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
+00015580: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015590: 6965 735b 6365 6c6c 5f69 645d 203d 2073  ies[cell_id] = s
+000155a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000155b0: 7072 6f70 6572 7469 6573 5b63 656c 6c5f  properties[cell_
+000155c0: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
+000155d0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
+000155e0: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
+000155f0: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
+00015600: 6c5f 6964 5d2e 7570 6461 7465 287b 7365  l_id].update({se
+00015610: 6c66 2e74 6f74 616c 5f69 6e74 656e 7369  lf.total_intensi
+00015620: 7479 5f6b 6579 3a20 2d31 7d29 0d0a 2020  ty_key: -1})..  
+00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015640: 2020 7365 6c66 2e63 6861 6e6e 656c 5f75    self.channel_u
+00015650: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015660: 7274 6965 735b 6365 6c6c 5f69 645d 2e75  rties[cell_id].u
+00015670: 7064 6174 6528 7b73 656c 662e 6d65 616e  pdate({self.mean
+00015680: 5f69 6e74 656e 7369 7479 5f6b 6579 3a20  _intensity_key: 
+00015690: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
+000156a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000156b0: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+000156c0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+000156d0: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
+000156e0: 656c 662e 7261 6469 7573 5f6b 6579 3a20  elf.radius_key: 
+000156f0: 2d31 7d29 0d0a 2020 2020 2020 2020 2020  -1})..          
+00015700: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00015710: 6861 6e6e 656c 5f75 6e69 7175 655f 7370  hannel_unique_sp
+00015720: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00015730: 6c6c 5f69 645d 2e75 7064 6174 6528 7b73  ll_id].update({s
+00015740: 656c 662e 7175 616c 6974 795f 6b65 793a  elf.quality_key:
+00015750: 202d 317d 290d 0a0d 0a0d 0a0d 0a20 2020   -1})........   
+00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015770: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00015780: 2020 2020 6465 6620 5f64 6963 745f 7570      def _dict_up
+00015790: 6461 7465 2873 656c 662c 2075 6e69 7175  date(self, uniqu
+000157a0: 655f 7472 6163 6b6c 6574 5f69 6473 3a20  e_tracklet_ids: 
+000157b0: 4c69 7374 2c20 2063 656c 6c5f 6964 3a20  List,  cell_id: 
+000157c0: 696e 742c 2074 7261 636b 5f69 643a 2069  int, track_id: i
+000157d0: 6e74 2c20 736f 7572 6365 5f69 643a 2069  nt, source_id: i
+000157e0: 6e74 2c20 7461 7267 6574 5f69 643a 2069  nt, target_id: i
+000157f0: 6e74 293a 0d0a 0d0a 200d 0a20 2020 2020  nt):.... ..     
+00015800: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
+00015810: 203d 2073 656c 662e 6765 6e65 7261 7469   = self.generati
+00015820: 6f6e 5f64 6963 745b 6365 6c6c 5f69 645d  on_dict[cell_id]
+00015830: 0d0a 2020 2020 2020 2020 7472 6163 6b6c  ..        trackl
+00015840: 6574 5f69 6420 3d20 7365 6c66 2e74 7261  et_id = self.tra
+00015850: 636b 6c65 745f 6469 6374 5b63 656c 6c5f  cklet_dict[cell_
+00015860: 6964 5d0d 0a20 2020 2020 2020 0d0a 0d0a  id]..       ....
+00015870: 2020 2020 2020 2020 756e 6971 7565 5f69          unique_i
+00015880: 6420 3d20 7374 7228 7472 6163 6b5f 6964  d = str(track_id
+00015890: 2920 2b20 2073 7472 2867 656e 6572 6174  ) +  str(generat
+000158a0: 696f 6e5f 6964 2920 2b20 7374 7228 7472  ion_id) + str(tr
+000158b0: 6163 6b6c 6574 5f69 6429 0d0a 2020 2020  acklet_id)..    
+000158c0: 2020 2020 0d0a 2020 2020 2020 2020 7665      ..        ve
+000158d0: 635f 6d61 736b 203d 205b 666c 6f61 7428  c_mask = [float(
+000158e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000158f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015900: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00015910: 6173 6b63 656e 7472 6f69 645f 785f 6b65  askcentroid_x_ke
+00015920: 795d 292c 2066 6c6f 6174 2873 656c 662e  y]), float(self.
+00015930: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015940: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015950: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
+00015960: 6e74 726f 6964 5f79 5f6b 6579 5d29 2c20  ntroid_y_key]), 
+00015970: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015980: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015990: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+000159a0: 7365 6c66 2e6d 6173 6b63 656e 7472 6f69  self.maskcentroi
+000159b0: 645f 7a5f 6b65 795d 2920 5d0d 0a0d 0a20  d_z_key]) ].... 
+000159c0: 2020 2020 2020 2076 6563 5f63 656c 6c20         vec_cell 
+000159d0: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
+000159e0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000159f0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015a00: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
+00015a10: 6579 5d29 202c 200d 0a20 2020 2020 2020  ey]) , ..       
+00015a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a30: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00015a40: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015a50: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015a60: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+00015a70: 5f6b 6579 5d29 2c20 0d0a 2020 2020 2020  _key]), ..      
+00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a90: 2020 2020 2020 666c 6f61 7428 7365 6c66        float(self
+00015aa0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015ab0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015ac0: 5f69 6429 5d5b 7365 6c66 2e7a 706f 7369  _id)][self.zposi
+00015ad0: 645f 6b65 795d 295d 0d0a 0d0a 2020 2020  d_key])]....    
+00015ae0: 2020 2020 616e 676c 6520 3d20 616e 6775      angle = angu
+00015af0: 6c61 725f 6368 616e 6765 2876 6563 5f6d  lar_change(vec_m
+00015b00: 6173 6b2c 2076 6563 5f63 656c 6c29 0d0a  ask, vec_cell)..
+00015b10: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00015b20: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015b30: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015b40: 6429 5d2e 7570 6461 7465 287b 7365 6c66  d)].update({self
+00015b50: 2e72 6164 6961 6c5f 616e 676c 655f 6b65  .radial_angle_ke
+00015b60: 7920 3a20 616e 676c 657d 2920 2020 2020  y : angle})     
+00015b70: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00015b80: 0a0d 0a20 2020 2020 2020 2075 6e69 7175  ...        uniqu
+00015b90: 655f 7472 6163 6b6c 6574 5f69 6473 2e61  e_tracklet_ids.a
+00015ba0: 7070 656e 6428 7374 7228 756e 6971 7565  ppend(str(unique
+00015bb0: 5f69 6429 290d 0a20 2020 2020 2020 2073  _id))..        s
+00015bc0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015bd0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015be0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015bf0: 7b73 656c 662e 756e 6971 7565 6964 5f6b  {self.uniqueid_k
+00015c00: 6579 203a 2073 7472 2875 6e69 7175 655f  ey : str(unique_
+00015c10: 6964 297d 290d 0a20 2020 2020 2020 2073  id)})..        s
+00015c20: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015c30: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015c40: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015c50: 7b73 656c 662e 7472 6163 6b6c 6574 6964  {self.trackletid
+00015c60: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
+00015c70: 6c65 745f 6964 297d 2920 0d0a 2020 2020  let_id)}) ..    
+00015c80: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015c90: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015ca0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015cb0: 6461 7465 287b 7365 6c66 2e67 656e 6572  date({self.gener
+00015cc0: 6174 696f 6e69 645f 6b65 7920 3a20 7374  ationid_key : st
+00015cd0: 7228 6765 6e65 7261 7469 6f6e 5f69 6429  r(generation_id)
+00015ce0: 7d29 200d 0a20 2020 2020 2020 2073 656c  }) ..        sel
+00015cf0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00015d00: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00015d10: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00015d20: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
+00015d30: 3a20 7374 7228 7472 6163 6b5f 6964 297d  : str(track_id)}
+00015d40: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015d50: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015d60: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015d70: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00015d80: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
+00015d90: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
+00015da0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015db0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015dc0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015dd0: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
+00015de0: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
+00015df0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015e00: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015e10: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015e20: 7570 6461 7465 287b 7365 6c66 2e61 6363  update({self.acc
+00015e30: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
+00015e40: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
+00015e50: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015e60: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+00015e70: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00015e80: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
+00015e90: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
+00015ea0: 203a 202d 317d 290d 0a20 2020 2020 2020   : -1})..       
+00015eb0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00015ec0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015ed0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00015ee0: 6528 7b73 656c 662e 6563 6365 6e74 7269  e({self.eccentri
+00015ef0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
+00015f00: 6b65 7920 3a20 2d31 7d29 0d0a 2020 2020  key : -1})..    
+00015f10: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+00015f20: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00015f30: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
+00015f40: 6461 7465 287b 7365 6c66 2e73 7572 6661  date({self.surfa
+00015f50: 6365 5f61 7265 615f 6b65 7920 3a20 2d31  ce_area_key : -1
+00015f60: 7d29 0d0a 2020 2020 2020 2020 7365 6c66  })..        self
+00015f70: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015f80: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015f90: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015fa0: 6c66 2e63 656c 6c61 7869 735f 6d61 736b  lf.cellaxis_mask
+00015fb0: 5f6b 6579 203a 202d 317d 290d 0a0d 0a20  _key : -1}).... 
+00015fc0: 2020 2020 2020 2069 6620 736f 7572 6365         if source
+00015fd0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00015fe0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00015ff0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016000: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00016010: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00016020: 7365 6c66 2e62 6566 6f72 6569 645f 6b65  self.beforeid_ke
+00016030: 7920 3a20 696e 7428 736f 7572 6365 5f69  y : int(source_i
+00016040: 6429 7d29 0d0a 2020 2020 2020 2020 2020  d)})..          
+00016050: 2020 7665 635f 3120 3d20 5b66 6c6f 6174    vec_1 = [float
+00016060: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00016070: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00016080: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00016090: 7870 6f73 6964 5f6b 6579 5d29 202d 2066  xposid_key]) - f
+000160a0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000160b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000160c0: 5b69 6e74 2873 6f75 7263 655f 6964 295d  [int(source_id)]
+000160d0: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+000160e0: 5d29 2c20 0d0a 2020 2020 2020 2020 2020  ]), ..          
+000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016100: 2020 666c 6f61 7428 7365 6c66 2e75 6e69    float(self.uni
+00016110: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00016120: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00016130: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
+00016140: 795d 2920 2d20 666c 6f61 7428 7365 6c66  y]) - float(self
+00016150: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00016160: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
+00016170: 6365 5f69 6429 5d5b 7365 6c66 2e79 706f  ce_id)][self.ypo
+00016180: 7369 645f 6b65 795d 292c 200d 0a20 2020  sid_key]), ..   
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 2020 2020 2020 2020 2066 6c6f 6174 2873           float(s
+000161b0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000161c0: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
+000161d0: 656c 6c5f 6964 295d 5b73 656c 662e 7a70  ell_id)][self.zp
+000161e0: 6f73 6964 5f6b 6579 5d29 202d 2020 666c  osid_key]) -  fl
+000161f0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00016200: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016210: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+00016220: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00016230: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
+00016240: 7370 6565 6420 3d20 6e70 2e73 7172 7428  speed = np.sqrt(
+00016250: 6e70 2e64 6f74 2876 6563 5f31 2c20 7665  np.dot(vec_1, ve
+00016260: 635f 3129 292f 7365 6c66 2e74 6361 6c69  c_1))/self.tcali
+00016270: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00016280: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00016290: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000162a0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000162b0: 7064 6174 6528 7b73 656c 662e 7370 6565  pdate({self.spee
+000162c0: 645f 6b65 7920 3a20 7370 6565 647d 290d  d_key : speed}).
+000162d0: 0a0d 0a20 2020 2020 2020 2020 2020 206d  ...            m
+000162e0: 6f74 696f 6e5f 616e 676c 6520 3d20 616e  otion_angle = an
+000162f0: 6775 6c61 725f 6368 616e 6765 2876 6563  gular_change(vec
+00016300: 5f6d 6173 6b2c 2076 6563 5f31 290d 0a0d  _mask, vec_1)...
+00016310: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016320: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00016330: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00016340: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00016350: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
+00016360: 5f6b 6579 203a 206d 6f74 696f 6e5f 616e  _key : motion_an
+00016370: 676c 657d 2920 0d0a 0d0a 2020 2020 2020  gle}) ....      
+00016380: 2020 2020 2020 6966 2073 6f75 7263 655f        if source_
+00016390: 6964 2069 6e20 7365 6c66 2e65 6467 655f  id in self.edge_
+000163a0: 736f 7572 6365 5f6c 6f6f 6b75 703a 0d0a  source_lookup:..
+000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163c0: 2020 2020 7072 655f 736f 7572 6365 5f69      pre_source_i
+000163d0: 6420 3d20 7365 6c66 2e65 6467 655f 736f  d = self.edge_so
+000163e0: 7572 6365 5f6c 6f6f 6b75 705b 736f 7572  urce_lookup[sour
+000163f0: 6365 5f69 645d 0d0a 2020 2020 2020 2020  ce_id]..        
+00016400: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00016410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016420: 2020 7665 635f 3220 3d20 5b66 6c6f 6174    vec_2 = [float
+00016430: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00016440: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00016450: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00016460: 7870 6f73 6964 5f6b 6579 5d29 202d 2032  xposid_key]) - 2
+00016470: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
+00016480: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00016490: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+000164a0: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+000164b0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
+000164c0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000164d0: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
+000164e0: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
+000164f0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
+00016500: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00016510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016520: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00016530: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016540: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00016550: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
+00016560: 2920 2d20 3220 2a20 666c 6f61 7428 7365  ) - 2 * float(se
+00016570: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00016580: 726f 7065 7274 6965 735b 696e 7428 736f  roperties[int(so
+00016590: 7572 6365 5f69 6429 5d5b 7365 6c66 2e79  urce_id)][self.y
+000165a0: 706f 7369 645f 6b65 795d 2920 2b20 666c  posid_key]) + fl
+000165b0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000165c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000165d0: 696e 7428 7072 655f 736f 7572 6365 5f69  int(pre_source_i
+000165e0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
+000165f0: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016610: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
+00016620: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016630: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016640: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+00016650: 5f6b 6579 5d29 202d 2020 3220 2a20 666c  _key]) -  2 * fl
+00016660: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+00016670: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+00016680: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+00016690: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+000166a0: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
+000166b0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+000166c0: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
+000166d0: 7572 6365 5f69 6429 5d5b 7365 6c66 2e7a  urce_id)][self.z
+000166e0: 706f 7369 645f 6b65 795d 295d 0d0a 2020  posid_key])]..  
+000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016700: 2020 6163 6320 3d20 6e70 2e73 7172 7428    acc = np.sqrt(
+00016710: 6e70 2e64 6f74 2876 6563 5f32 2c20 7665  np.dot(vec_2, ve
+00016720: 635f 3229 292f 7365 6c66 2e74 6361 6c69  c_2))/self.tcali
+00016730: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+00016740: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016760: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00016770: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00016780: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
+00016790: 6174 6528 7b73 656c 662e 6163 6365 6c65  ate({self.accele
+000167a0: 7261 7469 6f6e 5f6b 6579 203a 2061 6363  ration_key : acc
+000167b0: 7d29 0d0a 2020 2020 2020 2020 656c 6966  })..        elif
+000167c0: 2073 6f75 7263 655f 6964 2069 7320 4e6f   source_id is No
+000167d0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+000167e0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+000167f0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00016800: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00016810: 6528 7b73 656c 662e 6265 666f 7265 6964  e({self.beforeid
+00016820: 5f6b 6579 203a 204e 6f6e 657d 2920 0d0a  _key : None}) ..
+00016830: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
+00016840: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00016850: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00016860: 3a20 2020 2020 2020 0d0a 2020 2020 2020  :       ..      
+00016870: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00016880: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00016890: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+000168a0: 7570 6461 7465 287b 7365 6c66 2e61 6674  update({self.aft
+000168b0: 6572 6964 5f6b 6579 203a 2069 6e74 2874  erid_key : int(t
+000168c0: 6172 6765 745f 6964 297d 2920 0d0a 2020  arget_id)}) ..  
+000168d0: 2020 2020 2020 656c 6966 2074 6172 6765        elif targe
+000168e0: 745f 6964 2069 7320 4e6f 6e65 3a0d 0a20  t_id is None:.. 
+000168f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016900: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00016910: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00016920: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00016930: 662e 6166 7465 7269 645f 6b65 7920 3a20  f.afterid_key : 
+00016940: 4e6f 6e65 7d29 0d0a 2020 2020 2020 2020  None})..        
+00016950: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+00016960: 6c66 2e5f 7365 636f 6e64 5f63 6861 6e6e  lf._second_chann
+00016970: 656c 5f75 7064 6174 6528 6365 6c6c 5f69  el_update(cell_i
+00016980: 642c 2074 7261 636b 5f69 6429 2020 2020  d, track_id)    
+00016990: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f74  ......    def _t
+000169a0: 656d 706f 7261 6c5f 706c 6f74 735f 7472  emporal_plots_tr
+000169b0: 6163 6b6d 6174 6528 7365 6c66 293a 0d0a  ackmate(self):..
+000169c0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
+000169d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000169e0: 2020 7365 6c66 2e41 7474 7220 3d20 7b7d    self.Attr = {}
+000169f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016a00: 2020 7374 6172 7474 696d 6520 3d20 696e    starttime = in
+00016a10: 7428 6d69 6e28 7365 6c66 2e41 6c6c 5661  t(min(self.AllVa
+00016a20: 6c75 6573 5b73 656c 662e 6672 616d 6569  lues[self.framei
+00016a30: 645f 6b65 795d 2929 0d0a 2020 2020 2020  d_key]))..      
+00016a40: 2020 2020 2020 2020 2020 656e 6474 696d            endtim
+00016a50: 6520 3d20 696e 7428 6d61 7828 7365 6c66  e = int(max(self
+00016a60: 2e41 6c6c 5661 6c75 6573 5b73 656c 662e  .AllValues[self.
+00016a70: 6672 616d 6569 645f 6b65 795d 2929 0d0a  frameid_key]))..
+00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00016aa0: 2020 2073 656c 662e 7469 6d65 203d 205b     self.time = [
+00016ab0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016ac0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00016ad0: 6d65 616e 5f64 6973 705f 7a20 3d20 5b5d  mean_disp_z = []
+00016ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016af0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00016b00: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
+00016b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00016b20: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00016b30: 6561 6e5f 6469 7370 5f79 203d 205b 5d0d  ean_disp_y = [].
+00016b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b50: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00016b60: 725f 6469 7370 5f79 203d 205b 5d0d 0a0d  r_disp_y = []...
+00016b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016b80: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
+00016b90: 616e 5f64 6973 705f 7820 3d20 5b5d 0d0a  an_disp_x = []..
+00016ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bb0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00016bc0: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
+00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016be0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00016bf0: 6e5f 7261 6469 7573 203d 205b 5d0d 0a20  n_radius = [].. 
+00016c00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016c10: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
+00016c20: 7261 6469 7573 203d 205b 5d0d 0a0d 0a20  radius = [].... 
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016c40: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00016c50: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
+00016c60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016c70: 662e 6d69 746f 7469 635f 7661 725f 7370  f.mitotic_var_sp
+00016c80: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
+00016c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016ca0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6163  .mitotic_mean_ac
+00016cb0: 6320 3d20 5b5d 0d0a 2020 2020 2020 2020  c = []..        
+00016cc0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00016cd0: 6f74 6963 5f76 6172 5f61 6363 203d 205b  otic_var_acc = [
+00016ce0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016cf0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00016d00: 635f 6d65 616e 5f64 6972 6563 7469 6f6e  c_mean_direction
+00016d10: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
+00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d30: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00016d40: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00016d50: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
+00016d60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016d70: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00016d80: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00016d90: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016da0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00016db0: 7469 635f 7661 725f 6469 7374 616e 6365  tic_var_distance
+00016dc0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00016dd0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016de0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00016df0: 7469 635f 6d65 616e 5f64 6973 705f 7a20  tic_mean_disp_z 
+00016e00: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016e10: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00016e20: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00016e30: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
+00016e40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00016e50: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+00016e60: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+00016e70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016e80: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00016e90: 725f 6469 7370 5f79 203d 205b 5d0d 0a0d  r_disp_y = []...
+00016ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016eb0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016ec0: 635f 6d65 616e 5f64 6973 705f 7820 3d20  c_mean_disp_x = 
+00016ed0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016ee0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016ef0: 6f74 6963 5f76 6172 5f64 6973 705f 7820  otic_var_disp_x 
+00016f00: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00016f10: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00016f20: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7261  _mitotic_mean_ra
+00016f30: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
+00016f40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016f50: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00016f60: 7261 6469 7573 203d 205b 5d0d 0a0d 0a20  radius = [].... 
+00016f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016f80: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016f90: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
+00016fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016fb0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016fc0: 635f 7661 725f 7370 6565 6420 3d20 5b5d  c_var_speed = []
+00016fd0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00016fe0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00016ff0: 6f74 6963 5f6d 6561 6e5f 6163 6320 3d20  otic_mean_acc = 
+00017000: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017010: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00017020: 6f74 6963 5f76 6172 5f61 6363 203d 205b  otic_var_acc = [
+00017030: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00017040: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00017050: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
+00017060: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
+00017070: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017080: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00017090: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+000170a0: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000170b0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000170c0: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+000170d0: 6f74 6963 5f6d 6561 6e5f 6469 7374 616e  otic_mean_distan
+000170e0: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
+000170f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017100: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00017110: 7469 635f 7661 725f 6469 7374 616e 6365  tic_var_distance
+00017120: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00017130: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00017140: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00017150: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
+00017160: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017170: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
+00017180: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
+00017190: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000171a0: 6c6c 5f6d 6561 6e5f 6469 7370 5f79 203d  ll_mean_disp_y =
+000171b0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000171c0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+000171d0: 725f 6469 7370 5f79 203d 205b 5d0d 0a0d  r_disp_y = []...
+000171e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000171f0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+00017200: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
+00017210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017220: 2e61 6c6c 5f76 6172 5f64 6973 705f 7820  .all_var_disp_x 
+00017230: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00017240: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00017250: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
+00017260: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00017270: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00017280: 7261 6469 7573 203d 205b 5d0d 0a0d 0a20  radius = [].... 
+00017290: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000172a0: 656c 662e 616c 6c5f 6d65 616e 5f73 7065  elf.all_mean_spe
+000172b0: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
+000172c0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000172d0: 6c5f 7661 725f 7370 6565 6420 3d20 5b5d  l_var_speed = []
 000172e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
 000172f0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00017300: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00017310: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
-00017320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017330: 616c 6c5f 7661 725f 6469 7265 6374 696f  all_var_directio
-00017340: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
-00017350: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00017360: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00017370: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00017380: 6173 6b20 3d20 5b5d 0d0a 2020 2020 2020  ask = []..      
-00017390: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000173a0: 6c6c 5f76 6172 5f64 6973 7461 6e63 655f  ll_var_distance_
-000173b0: 6365 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a  cell_mask = []..
-000173c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000173d0: 2020 2020 616c 6c5f 7370 6f74 735f 7472      all_spots_tr
-000173e0: 6163 6b73 203d 207b 7d0d 0a20 2020 2020  acks = {}..     
-000173f0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00017400: 6b2c 7629 2069 6e20 7365 6c66 2e75 6e69  k,v) in self.uni
-00017410: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00017420: 6965 732e 6974 656d 7328 293a 0d0a 2020  ies.items():..  
-00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017440: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00017450: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017460: 7370 6f74 7320 3d20 7365 6c66 2e75 6e69  spots = self.uni
-00017470: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00017480: 6965 735b 6b5d 0d0a 2020 2020 2020 2020  ies[k]..        
-00017490: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000174a0: 2073 656c 662e 7472 6163 6b69 645f 6b65   self.trackid_ke
-000174b0: 7920 696e 2061 6c6c 5f73 706f 7473 3a0d  y in all_spots:.
-000174c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000174d0: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
-000174e0: 706f 7473 5f74 7261 636b 735b 6b5d 203d  pots_tracks[k] =
-000174f0: 2061 6c6c 5f73 706f 7473 0d0a 2020 2020   all_spots..    
-00017500: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017530: 2020 6675 7475 7265 7320 3d20 5b5d 0d0a    futures = []..
-00017540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017550: 7769 7468 2063 6f6e 6375 7272 656e 742e  with concurrent.
-00017560: 6675 7475 7265 732e 5468 7265 6164 506f  futures.ThreadPo
-00017570: 6f6c 4578 6563 7574 6f72 286d 6178 5f77  olExecutor(max_w
-00017580: 6f72 6b65 7273 203d 206f 732e 6370 755f  orkers = os.cpu_
-00017590: 636f 756e 7428 2929 2061 7320 6578 6563  count()) as exec
-000175a0: 7574 6f72 3a0d 0a20 2020 2020 2020 2020  utor:..         
-000175b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000175c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175d0: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
-000175e0: 2872 616e 6765 2873 7461 7274 7469 6d65  (range(starttime
-000175f0: 2c20 656e 6474 696d 6529 2c20 746f 7461  , endtime), tota
-00017600: 6c3d 656e 6474 696d 6520 2d20 7374 6172  l=endtime - star
-00017610: 7474 696d 6529 3a0d 0a20 2020 2020 2020  ttime):..       
-00017620: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00017630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017640: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-00017650: 2e61 7070 656e 6428 6578 6563 7574 6f72  .append(executor
-00017660: 2e73 7562 6d69 7428 7365 6c66 2e5f 636f  .submit(self._co
-00017670: 6d70 7574 655f 7465 6d70 6f72 616c 2c20  mpute_temporal, 
-00017680: 692c 2061 6c6c 5f73 706f 7473 5f74 7261  i, all_spots_tra
-00017690: 636b 7329 290d 0a20 0d0a 2020 2020 2020  cks)).. ..      
-000176a0: 2020 2020 2020 2020 2020 2020 2020 5b72                [r
-000176b0: 2e72 6573 756c 7428 2920 666f 7220 7220  .result() for r 
-000176c0: 696e 2063 6f6e 6375 7272 656e 742e 6675  in concurrent.fu
-000176d0: 7475 7265 732e 6173 5f63 6f6d 706c 6574  tures.as_complet
-000176e0: 6564 2866 7574 7572 6573 295d 0d0a 0d0a  ed(futures)]....
-000176f0: 0d0a 2020 2020 6465 6620 5f63 6f6d 7075  ..    def _compu
-00017700: 7465 5f74 656d 706f 7261 6c28 7365 6c66  te_temporal(self
-00017710: 2c20 692c 2061 6c6c 5f73 706f 7473 5f74  , i, all_spots_t
-00017720: 7261 636b 7329 3a20 2020 2020 2020 2020  racks):         
-00017730: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00017740: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017750: 6f74 6963 5f64 6973 705f 7a20 3d20 5b5d  otic_disp_z = []
-00017760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00017770: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00017780: 7370 5f79 203d 205b 5d0d 0a20 2020 2020  sp_y = []..     
-00017790: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000177a0: 6974 6f74 6963 5f64 6973 705f 7820 3d20  itotic_disp_x = 
-000177b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000177c0: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-000177d0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00017300: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
+00017310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017320: 2e61 6c6c 5f76 6172 5f61 6363 203d 205b  .all_var_acc = [
+00017330: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00017340: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+00017350: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00017360: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+00017370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017380: 2e61 6c6c 5f76 6172 5f64 6972 6563 7469  .all_var_directi
+00017390: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
+000173a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000173b0: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+000173c0: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
+000173d0: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
+000173e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000173f0: 616c 6c5f 7661 725f 6469 7374 616e 6365  all_var_distance
+00017400: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
+00017410: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
+00017420: 2020 2020 2061 6c6c 5f73 706f 7473 5f74       all_spots_t
+00017430: 7261 636b 7320 3d20 7b7d 0d0a 2020 2020  racks = {}..    
+00017440: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00017450: 286b 2c76 2920 696e 2073 656c 662e 756e  (k,v) in self.un
+00017460: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00017470: 7469 6573 2e69 7465 6d73 2829 3a0d 0a20  ties.items():.. 
+00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017490: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+000174a0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000174b0: 5f73 706f 7473 203d 2073 656c 662e 756e  _spots = self.un
+000174c0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000174d0: 7469 6573 5b6b 5d0d 0a20 2020 2020 2020  ties[k]..       
+000174e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000174f0: 6620 7365 6c66 2e74 7261 636b 6964 5f6b  f self.trackid_k
+00017500: 6579 2069 6e20 616c 6c5f 7370 6f74 733a  ey in all_spots:
+00017510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017520: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+00017530: 7370 6f74 735f 7472 6163 6b73 5b6b 5d20  spots_tracks[k] 
+00017540: 3d20 616c 6c5f 7370 6f74 730d 0a20 2020  = all_spots..   
+00017550: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+00017560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017570: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017580: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+00017590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000175a0: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+000175b0: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+000175c0: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+000175d0: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+000175e0: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+000175f0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+00017600: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017620: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
+00017630: 6d28 7261 6e67 6528 7374 6172 7474 696d  m(range(starttim
+00017640: 652c 2065 6e64 7469 6d65 292c 2074 6f74  e, endtime), tot
+00017650: 616c 3d65 6e64 7469 6d65 202d 2073 7461  al=endtime - sta
+00017660: 7274 7469 6d65 293a 0d0a 2020 2020 2020  rttime):..      
+00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017690: 2020 2020 2020 2020 2020 6675 7475 7265            future
+000176a0: 732e 6170 7065 6e64 2865 7865 6375 746f  s.append(executo
+000176b0: 722e 7375 626d 6974 2873 656c 662e 5f63  r.submit(self._c
+000176c0: 6f6d 7075 7465 5f74 656d 706f 7261 6c2c  ompute_temporal,
+000176d0: 2069 2c20 616c 6c5f 7370 6f74 735f 7472   i, all_spots_tr
+000176e0: 6163 6b73 2929 0d0a 200d 0a20 2020 2020  acks)).. ..     
+000176f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00017700: 722e 7265 7375 6c74 2829 2066 6f72 2072  r.result() for r
+00017710: 2069 6e20 636f 6e63 7572 7265 6e74 2e66   in concurrent.f
+00017720: 7574 7572 6573 2e61 735f 636f 6d70 6c65  utures.as_comple
+00017730: 7465 6428 6675 7475 7265 7329 5d0d 0a0d  ted(futures)]...
+00017740: 0a0d 0a20 2020 2064 6566 205f 636f 6d70  ...    def _comp
+00017750: 7574 655f 7465 6d70 6f72 616c 2873 656c  ute_temporal(sel
+00017760: 662c 2069 2c20 616c 6c5f 7370 6f74 735f  f, i, all_spots_
+00017770: 7472 6163 6b73 293a 2020 2020 2020 2020  tracks):        
+00017780: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00017790: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+000177a0: 746f 7469 635f 6469 7370 5f7a 203d 205b  totic_disp_z = [
+000177b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000177c0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+000177d0: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
 000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177f0: 206d 6974 6f74 6963 5f73 7065 6564 203d   mitotic_speed =
+000177f0: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
 00017800: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
 00017810: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017820: 5f61 6363 203d 205b 5d0d 0a20 2020 2020  _acc = []..     
-00017830: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00017840: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00017850: 616c 5f63 6861 6e67 6520 3d20 5b5d 0d0a  al_change = []..
-00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017870: 2020 2020 6d69 746f 7469 635f 6469 7374      mitotic_dist
-00017880: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00017890: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000178a0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000178b0: 6974 6f74 6963 5f64 6973 705f 7a20 3d20  itotic_disp_z = 
-000178c0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000178d0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000178e0: 7469 635f 6469 7370 5f79 203d 205b 5d0d  tic_disp_y = [].
-000178f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017900: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017910: 5f64 6973 705f 7820 3d20 5b5d 0d0a 2020  _disp_x = []..  
-00017920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017930: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
-00017940: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-00017950: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017960: 6f6e 5f6d 6974 6f74 6963 5f73 7065 6564  on_mitotic_speed
-00017970: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00017980: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00017990: 6974 6f74 6963 5f61 6363 203d 205b 5d0d  itotic_acc = [].
-000179a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179b0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000179c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000179d0: 6e67 6520 3d20 5b5d 0d0a 2020 2020 2020  nge = []..      
-000179e0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-000179f0: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00017a00: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00017a10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017a20: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00017a30: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017a40: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a60: 2020 616c 6c5f 6469 7370 5f79 203d 205b    all_disp_y = [
-00017a70: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017a80: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00017a90: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00017aa0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00017ab0: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2061 6c6c 5f73 7065 6564 203d 205b 5d0d   all_speed = [].
-00017ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017af0: 2020 2020 2061 6c6c 5f61 6363 203d 205b       all_acc = [
-00017b00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017b10: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00017b20: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00017b30: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00017b40: 2020 2020 2020 2020 616c 6c5f 6469 7374          all_dist
-00017b50: 616e 6365 5f63 656c 6c5f 6d61 736b 203d  ance_cell_mask =
-00017b60: 205b 5d0d 0a0d 0a0d 0a0d 0a0d 0a20 2020   []..........   
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b80: 2066 6f72 2028 6b2c 7629 2069 6e20 616c   for (k,v) in al
-00017b90: 6c5f 7370 6f74 735f 7472 6163 6b73 2e69  l_spots_tracks.i
-00017ba0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00017bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bc0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017be0: 2020 2063 7572 7265 6e74 5f74 696d 6520     current_time 
-00017bf0: 3d20 616c 6c5f 7370 6f74 735f 7472 6163  = all_spots_trac
-00017c00: 6b73 5b6b 5d5b 7365 6c66 2e66 7261 6d65  ks[k][self.frame
-00017c10: 6964 5f6b 6579 5d0d 0a20 2020 2020 2020  id_key]..       
+00017820: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017840: 2020 6d69 746f 7469 635f 7370 6565 6420    mitotic_speed 
+00017850: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00017860: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017870: 635f 6163 6320 3d20 5b5d 0d0a 2020 2020  c_acc = []..    
+00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017890: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+000178a0: 6e61 6c5f 6368 616e 6765 203d 205b 5d0d  nal_change = [].
+000178b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000178c0: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+000178d0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+000178e0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+000178f0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00017900: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
+00017910: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017920: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017930: 6f74 6963 5f64 6973 705f 7920 3d20 5b5d  otic_disp_y = []
+00017940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017950: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017960: 635f 6469 7370 5f78 203d 205b 5d0d 0a20  c_disp_x = [].. 
+00017970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017980: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f72     non_mitotic_r
+00017990: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179b0: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
+000179c0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+000179d0: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+000179e0: 6d69 746f 7469 635f 6163 6320 3d20 5b5d  mitotic_acc = []
+000179f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017a00: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017a10: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+00017a20: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+00017a30: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00017a40: 6f6e 5f6d 6974 6f74 6963 5f64 6973 7461  on_mitotic_dista
+00017a50: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00017a60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017a70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00017a80: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00017a90: 6c5f 6469 7370 5f7a 203d 205b 5d0d 0a20  l_disp_z = [].. 
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ab0: 2020 2061 6c6c 5f64 6973 705f 7920 3d20     all_disp_y = 
+00017ac0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017ad0: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
+00017ae0: 5f78 203d 205b 5d0d 0a20 2020 2020 2020  _x = []..       
+00017af0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00017b00: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b20: 2020 616c 6c5f 7370 6565 6420 3d20 5b5d    all_speed = []
+00017b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017b40: 2020 2020 2020 616c 6c5f 6163 6320 3d20        all_acc = 
+00017b50: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00017b60: 2020 2020 2020 2020 616c 6c5f 6469 7265          all_dire
+00017b70: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00017b80: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+00017b90: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
+00017ba0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00017bb0: 3d20 5b5d 0d0a 0d0a 0d0a 0d0a 0d0a 2020  = []..........  
+00017bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017bd0: 2020 666f 7220 286b 2c76 2920 696e 2061    for (k,v) in a
+00017be0: 6c6c 5f73 706f 7473 5f74 7261 636b 732e  ll_spots_tracks.
+00017bf0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00017c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 2020 2020 206d 6974 6f74 6963 203d 2061       mitotic = a
-00017c40: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017c50: 6b5d 5b73 656c 662e 6469 7669 6469 6e67  k][self.dividing
-00017c60: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
+00017c30: 2020 2020 6375 7272 656e 745f 7469 6d65      current_time
+00017c40: 203d 2061 6c6c 5f73 706f 7473 5f74 7261   = all_spots_tra
+00017c50: 636b 735b 6b5d 5b73 656c 662e 6672 616d  cks[k][self.fram
+00017c60: 6569 645f 6b65 795d 0d0a 2020 2020 2020  eid_key]..      
 00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c80: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ca0: 6966 2069 203d 3d20 696e 7428 6375 7272  if i == int(curr
-00017cb0: 656e 745f 7469 6d65 293a 0d0a 2020 2020  ent_time):..    
+00017c80: 2020 2020 2020 6d69 746f 7469 6320 3d20        mitotic = 
+00017c90: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
+00017ca0: 5b6b 5d5b 7365 6c66 2e64 6976 6964 696e  [k][self.dividin
+00017cb0: 675f 6b65 795d 0d0a 2020 2020 2020 2020  g_key]..        
 00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00017ce0: 206d 6974 6f74 6963 3a0d 0a20 2020 2020   mitotic:..     
-00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d10: 2020 206d 6974 6f74 6963 5f64 6973 705f     mitotic_disp_
-00017d20: 7a2e 6170 7065 6e64 2861 6c6c 5f73 706f  z.append(all_spo
-00017d30: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017d40: 662e 7a70 6f73 6964 5f6b 6579 5d29 0d0a  f.zposid_key])..
+00017cd0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cf0: 2069 6620 6920 3d3d 2069 6e74 2863 7572   if i == int(cur
+00017d00: 7265 6e74 5f74 696d 6529 3a0d 0a20 2020  rent_time):..   
+00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017d30: 6620 6d69 746f 7469 633a 0d0a 2020 2020  f mitotic:..    
+00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
-00017d80: 6469 7370 5f79 2e61 7070 656e 6428 616c  disp_y.append(al
-00017d90: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017da0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-00017db0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-00017dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017dd0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017de0: 6f74 6963 5f64 6973 705f 782e 6170 7065  otic_disp_x.appe
-00017df0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017e00: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
-00017e10: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
-00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e40: 2020 6966 2061 6c6c 5f73 706f 7473 5f74    if all_spots_t
-00017e50: 7261 636b 735b 6b5d 5b73 656c 662e 7261  racks[k][self.ra
-00017e60: 6469 7573 5f6b 6579 5d20 3e20 303a 0d0a  dius_key] > 0:..
+00017d60: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00017d70: 5f7a 2e61 7070 656e 6428 616c 6c5f 7370  _z.append(all_sp
+00017d80: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+00017d90: 6c66 2e7a 706f 7369 645f 6b65 795d 290d  lf.zposid_key]).
+00017da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017dc0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+00017dd0: 5f64 6973 705f 792e 6170 7065 6e64 2861  _disp_y.append(a
+00017de0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017df0: 6b5d 5b73 656c 662e 7970 6f73 6964 5f6b  k][self.yposid_k
+00017e00: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e20: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017e30: 746f 7469 635f 6469 7370 5f78 2e61 7070  totic_disp_x.app
+00017e40: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017e50: 6163 6b73 5b6b 5d5b 7365 6c66 2e78 706f  acks[k][self.xpo
+00017e60: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
 00017e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017ea0: 6963 5f72 6164 6975 732e 6170 7065 6e64  ic_radius.append
-00017eb0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017ec0: 735b 6b5d 5b73 656c 662e 7261 6469 7573  s[k][self.radius
-00017ed0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00017f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 2020 6d69 746f 7469 635f 7261 6469 7573    mitotic_radius
-00017f40: 2e61 7070 656e 6428 4e6f 6e65 2920 2020  .append(None)   
-00017f50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00017e90: 2020 2069 6620 616c 6c5f 7370 6f74 735f     if all_spots_
+00017ea0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e72  tracks[k][self.r
+00017eb0: 6164 6975 735f 6b65 795d 203e 2030 3a0d  adius_key] > 0:.
+00017ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ee0: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017ef0: 7469 635f 7261 6469 7573 2e61 7070 656e  tic_radius.appen
+00017f00: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017f10: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
+00017f20: 735f 6b65 795d 290d 0a20 2020 2020 2020  s_key])..       
+00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
 00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f70: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017f80: 746f 7469 635f 7370 6565 642e 6170 7065  totic_speed.appe
-00017f90: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017fa0: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00017fb0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
-00017fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017fe0: 206d 6974 6f74 6963 5f61 6363 2e61 7070   mitotic_acc.app
-00017ff0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00018000: 6163 6b73 5b6b 5d5b 7365 6c66 2e61 6363  acks[k][self.acc
-00018010: 656c 6572 6174 696f 6e5f 6b65 795d 290d  eleration_key]).
-00018020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018040: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00018050: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00018060: 6e67 652e 6170 7065 6e64 2861 6c6c 5f73  nge.append(all_s
-00018070: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00018080: 656c 662e 6d6f 7469 6f6e 5f61 6e67 6c65  elf.motion_angle
-00018090: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
-000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000180d0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-000180e0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
-000180f0: 6b73 5b6b 5d5b 7365 6c66 2e64 6973 7461  ks[k][self.dista
-00018100: 6e63 655f 6365 6c6c 5f6d 6173 6b5f 6b65  nce_cell_mask_ke
-00018110: 795d 290d 0a0d 0a0d 0a20 2020 2020 2020  y])......       
-00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018130: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00018140: 7420 6d69 746f 7469 633a 0d0a 2020 2020  t mitotic:..    
-00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018170: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00018180: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-00018190: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-000181a0: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-000181b0: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
-000181c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000181d0: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-000181e0: 5f6d 6974 6f74 6963 5f64 6973 705f 792e  _mitotic_disp_y.
-000181f0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018200: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018210: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
-00018220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018240: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00018250: 635f 6469 7370 5f78 2e61 7070 656e 6428  c_disp_x.append(
-00018260: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00018270: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
-00018280: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000182b0: 6620 616c 6c5f 7370 6f74 735f 7472 6163  f all_spots_trac
-000182c0: 6b73 5b6b 5d5b 7365 6c66 2e72 6164 6975  ks[k][self.radiu
-000182d0: 735f 6b65 795d 203e 2030 3a0d 0a20 2020  s_key] > 0:..   
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 2020 206d 6974 6f74 6963 5f72 6164 6975     mitotic_radiu
+00017f90: 732e 6170 7065 6e64 284e 6f6e 6529 2020  s.append(None)  
+00017fa0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fc0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00017fd0: 6974 6f74 6963 5f73 7065 6564 2e61 7070  itotic_speed.app
+00017fe0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017ff0: 6163 6b73 5b6b 5d5b 7365 6c66 2e73 7065  acks[k][self.spe
+00018000: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
+00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018030: 2020 6d69 746f 7469 635f 6163 632e 6170    mitotic_acc.ap
+00018040: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
+00018050: 7261 636b 735b 6b5d 5b73 656c 662e 6163  racks[k][self.ac
+00018060: 6365 6c65 7261 7469 6f6e 5f6b 6579 5d29  celeration_key])
+00018070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018090: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+000180a0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
+000180b0: 616e 6765 2e61 7070 656e 6428 616c 6c5f  ange.append(all_
+000180c0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000180d0: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+000180e0: 655f 6b65 795d 290d 0a20 2020 2020 2020  e_key])..       
+000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018110: 206d 6974 6f74 6963 5f64 6973 7461 6e63   mitotic_distanc
+00018120: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00018130: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00018140: 636b 735b 6b5d 5b73 656c 662e 6469 7374  cks[k][self.dist
+00018150: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
+00018160: 6579 5d29 0d0a 0d0a 0d0a 2020 2020 2020  ey])......      
+00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018180: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00018190: 6f74 206d 6974 6f74 6963 3a0d 0a20 2020  ot mitotic:..   
+000181a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000181c0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+000181d0: 5f64 6973 705f 7a2e 6170 7065 6e64 2861  _disp_z.append(a
+000181e0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+000181f0: 6b5d 5b73 656c 662e 7a70 6f73 6964 5f6b  k][self.zposid_k
+00018200: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018230: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00018240: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00018250: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018260: 2e79 706f 7369 645f 6b65 795d 290d 0a20  .yposid_key]).. 
+00018270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018290: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+000182a0: 6963 5f64 6973 705f 782e 6170 7065 6e64  ic_disp_x.append
+000182b0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+000182c0: 735b 6b5d 5b73 656c 662e 7870 6f73 6964  s[k][self.xposid
+000182d0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018300: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
-00018310: 6f74 6963 5f72 6164 6975 732e 6170 7065  otic_radius.appe
-00018320: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00018330: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
-00018340: 7573 5f6b 6579 5d29 0d0a 2020 2020 2020  us_key])..      
-00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018370: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00018380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183a0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-000183b0: 5f72 6164 6975 732e 6170 7065 6e64 284e  _radius.append(N
-000183c0: 6f6e 6529 2020 2020 2020 2020 2020 0d0a  one)          ..
+00018300: 6966 2061 6c6c 5f73 706f 7473 5f74 7261  if all_spots_tra
+00018310: 636b 735b 6b5d 5b73 656c 662e 7261 6469  cks[k][self.radi
+00018320: 7573 5f6b 6579 5d20 3e20 303a 0d0a 2020  us_key] > 0:..  
+00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018350: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00018360: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
+00018370: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00018380: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
+00018390: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
 000183d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-00018400: 7469 635f 7370 6565 642e 6170 7065 6e64  tic_speed.append
-00018410: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00018420: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
-00018430: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00018460: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2e61  on_mitotic_acc.a
-00018470: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00018480: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e61  tracks[k][self.a
-00018490: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
-000184a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184c0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000184d0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-000184e0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000184f0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00018500: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-00018510: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-00018520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018540: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00018550: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00018560: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
-00018570: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00018580: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-00018590: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a0d  ll_mask_key])...
-000185a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185c0: 2020 2061 6c6c 5f64 6973 705f 7a2e 6170     all_disp_z.ap
-000185d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-000185e0: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
-000185f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000183f0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00018400: 635f 7261 6469 7573 2e61 7070 656e 6428  c_radius.append(
+00018410: 4e6f 6e65 2920 2020 2020 2020 2020 200d  None)          .
+00018420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018440: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00018450: 6f74 6963 5f73 7065 6564 2e61 7070 656e  otic_speed.appen
+00018460: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00018470: 6b73 5b6b 5d5b 7365 6c66 2e73 7065 6564  ks[k][self.speed
+00018480: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+00018490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184b0: 6e6f 6e5f 6d69 746f 7469 635f 6163 632e  non_mitotic_acc.
+000184c0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+000184d0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+000184e0: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
+000184f0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018510: 2020 2020 2020 2020 2020 2020 6e6f 6e5f              non_
+00018520: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+00018530: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018540: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00018550: 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74 696f  ks[k][self.motio
+00018560: 6e5f 616e 676c 655f 6b65 795d 290d 0a20  n_angle_key]).. 
+00018570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018590: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+000185a0: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000185b0: 5f6d 6173 6b2e 6170 7065 6e64 2861 6c6c  _mask.append(all
+000185c0: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+000185d0: 5b73 656c 662e 6469 7374 616e 6365 5f63  [self.distance_c
+000185e0: 656c 6c5f 6d61 736b 5f6b 6579 5d29 0d0a  ell_mask_key])..
+000185f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00018600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018610: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018620: 6c5f 6469 7370 5f79 2e61 7070 656e 6428  l_disp_y.append(
-00018630: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00018640: 5b6b 5d5b 7365 6c66 2e79 706f 7369 645f  [k][self.yposid_
-00018650: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018670: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00018680: 705f 782e 6170 7065 6e64 2861 6c6c 5f73  p_x.append(all_s
-00018690: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-000186a0: 656c 662e 7870 6f73 6964 5f6b 6579 5d29  elf.xposid_key])
-000186b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000186c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186d0: 2020 2020 6966 2061 6c6c 5f73 706f 7473      if all_spots
-000186e0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000186f0: 7261 6469 7573 5f6b 6579 5d20 3e20 303a  radius_key] > 0:
-00018700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018610: 2020 2020 616c 6c5f 6469 7370 5f7a 2e61      all_disp_z.a
+00018620: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00018630: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e7a  tracks[k][self.z
+00018640: 706f 7369 645f 6b65 795d 290d 0a20 2020  posid_key])..   
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00018670: 6c6c 5f64 6973 705f 792e 6170 7065 6e64  ll_disp_y.append
+00018680: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00018690: 735b 6b5d 5b73 656c 662e 7970 6f73 6964  s[k][self.yposid
+000186a0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000186b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186c0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+000186d0: 7370 5f78 2e61 7070 656e 6428 616c 6c5f  sp_x.append(all_
+000186e0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000186f0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+00018700: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00018710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018720: 2020 2020 2020 2020 616c 6c5f 7261 6469          all_radi
-00018730: 7573 2e61 7070 656e 6428 616c 6c5f 7370  us.append(all_sp
-00018740: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00018750: 6c66 2e72 6164 6975 735f 6b65 795d 290d  lf.radius_key]).
-00018760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00018790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187b0: 616c 6c5f 7261 6469 7573 2e61 7070 656e  all_radius.appen
-000187c0: 6428 4e6f 6e65 2920 2020 2020 2020 0d0a  d(None)       ..
-000187d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018720: 2020 2020 2069 6620 616c 6c5f 7370 6f74       if all_spot
+00018730: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018740: 2e72 6164 6975 735f 6b65 795d 203e 2030  .radius_key] > 0
+00018750: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018770: 2020 2020 2020 2020 2061 6c6c 5f72 6164           all_rad
+00018780: 6975 732e 6170 7065 6e64 2861 6c6c 5f73  ius.append(all_s
+00018790: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000187a0: 656c 662e 7261 6469 7573 5f6b 6579 5d29  elf.radius_key])
+000187b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187d0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
 000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 2020 616c 6c5f 7370 6565 642e 6170 7065    all_speed.appe
-00018800: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00018810: 636b 735b 6b5d 5b73 656c 662e 7370 6565  cks[k][self.spee
-00018820: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
+000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018800: 2061 6c6c 5f72 6164 6975 732e 6170 7065   all_radius.appe
+00018810: 6e64 284e 6f6e 6529 2020 2020 2020 200d  nd(None)       .
+00018820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018840: 2020 2020 2020 2020 2020 2061 6c6c 5f61             all_a
-00018850: 6363 2e61 7070 656e 6428 616c 6c5f 7370  cc.append(all_sp
-00018860: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00018870: 6c66 2e61 6363 656c 6572 6174 696f 6e5f  lf.acceleration_
-00018880: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
-00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 2020 2020 2020 2020 2061 6c6c 5f64 6972           all_dir
-000188b0: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-000188c0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000188d0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000188e0: 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b 6579  motion_angle_key
-000188f0: 5d29 2020 200d 0a20 2020 2020 2020 2020  ])   ..         
-00018900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018910: 2020 2020 2020 2020 2061 6c6c 5f64 6973           all_dis
-00018920: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00018930: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-00018940: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-00018950: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018960: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
-00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018990: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189b0: 6d69 746f 7469 635f 6469 7370 5f7a 203d  mitotic_disp_z =
-000189c0: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
-000189d0: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-000189e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000189f0: 2020 2020 2020 6d69 746f 7469 635f 6469        mitotic_di
-00018a00: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00018a10: 2e64 6966 6628 6d69 746f 7469 635f 6469  .diff(mitotic_di
-00018a20: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00018a30: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
-00018a40: 7469 635f 6469 7370 5f78 203d 206e 702e  tic_disp_x = np.
-00018a50: 6162 7328 6e70 2e64 6966 6628 6d69 746f  abs(np.diff(mito
-00018a60: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
-00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a80: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00018a90: 6469 7370 5f7a 203d 206e 702e 6162 7328  disp_z = np.abs(
-00018aa0: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
-00018ab0: 7469 635f 6469 7370 5f7a 2929 0d0a 2020  tic_disp_z))..  
-00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 2020 6e6f 6e5f 6d69 746f 7469 635f 6469    non_mitotic_di
-00018ae0: 7370 5f79 203d 206e 702e 6162 7328 6e70  sp_y = np.abs(np
-00018af0: 2e64 6966 6628 6e6f 6e5f 6d69 746f 7469  .diff(non_mitoti
-00018b00: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
+00018840: 2020 2061 6c6c 5f73 7065 6564 2e61 7070     all_speed.app
+00018850: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00018860: 6163 6b73 5b6b 5d5b 7365 6c66 2e73 7065  acks[k][self.spe
+00018870: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
+00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018890: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
+000188a0: 6163 632e 6170 7065 6e64 2861 6c6c 5f73  acc.append(all_s
+000188b0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000188c0: 656c 662e 6163 6365 6c65 7261 7469 6f6e  elf.acceleration
+000188d0: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
+000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188f0: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00018900: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018910: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00018920: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00018930: 2e6d 6f74 696f 6e5f 616e 676c 655f 6b65  .motion_angle_ke
+00018940: 795d 2920 2020 0d0a 2020 2020 2020 2020  y])   ..        
+00018950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018960: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00018970: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00018980: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00018990: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000189a0: 2e64 6973 7461 6e63 655f 6365 6c6c 5f6d  .distance_cell_m
+000189b0: 6173 6b5f 6b65 795d 290d 0a20 2020 2020  ask_key])..     
+000189c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189e0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 206d 6974 6f74 6963 5f64 6973 705f 7a20   mitotic_disp_z 
+00018a10: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
+00018a20: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
+00018a30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018a40: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00018a50: 6973 705f 7920 3d20 6e70 2e61 6273 286e  isp_y = np.abs(n
+00018a60: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
+00018a70: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+00018a80: 2020 2020 2020 2020 2020 2020 206d 6974               mit
+00018a90: 6f74 6963 5f64 6973 705f 7820 3d20 6e70  otic_disp_x = np
+00018aa0: 2e61 6273 286e 702e 6469 6666 286d 6974  .abs(np.diff(mit
+00018ab0: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
+00018ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018ad0: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
+00018ae0: 5f64 6973 705f 7a20 3d20 6e70 2e61 6273  _disp_z = np.abs
+00018af0: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
+00018b00: 6f74 6963 5f64 6973 705f 7a29 290d 0a20  otic_disp_z)).. 
 00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b20: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018b30: 5f78 203d 206e 702e 6162 7328 6e70 2e64  _x = np.abs(np.d
-00018b40: 6966 6628 6e6f 6e5f 6d69 746f 7469 635f  iff(non_mitotic_
-00018b50: 6469 7370 5f78 2929 0d0a 0d0a 2020 2020  disp_x))....    
+00018b20: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
+00018b30: 6973 705f 7920 3d20 6e70 2e61 6273 286e  isp_y = np.abs(n
+00018b40: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
+00018b50: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
 00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b70: 616c 6c5f 6469 7370 5f7a 203d 206e 702e  all_disp_z = np.
-00018b80: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
-00018b90: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00018ba0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018bb0: 6c5f 6469 7370 5f79 203d 206e 702e 6162  l_disp_y = np.ab
-00018bc0: 7328 6e70 2e64 6966 6628 616c 6c5f 6469  s(np.diff(all_di
-00018bd0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00018be0: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00018bf0: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
-00018c00: 6e70 2e64 6966 6628 616c 6c5f 6469 7370  np.diff(all_disp
-00018c10: 5f78 2929 0d0a 0d0a 0d0a 2020 2020 2020  _x))......      
-00018c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00018c50: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00018c60: 652e 6170 7065 6e64 2869 202a 2073 656c  e.append(i * sel
-00018c70: 662e 7463 616c 6962 7261 7469 6f6e 290d  f.tcalibration).
-00018c80: 0a0d 0a0d 0a20 2020 2020 2020 2020 2020  .....           
-00018c90: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018ca0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00018cb0: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-00018cc0: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
-00018cd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018ce0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018cf0: 7469 635f 7661 725f 6469 7370 5f7a 2e61  tic_var_disp_z.a
-00018d00: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00018d10: 6f74 6963 5f64 6973 705f 7a29 290d 0a0d  otic_disp_z))...
-00018d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d30: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018d40: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-00018d50: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018d60: 6f74 6963 5f64 6973 705f 7929 290d 0a20  otic_disp_y)).. 
-00018d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d80: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018d90: 7661 725f 6469 7370 5f79 2e61 7070 656e  var_disp_y.appen
-00018da0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018db0: 5f64 6973 705f 7929 290d 0a0d 0a20 2020  _disp_y))....   
+00018b70: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00018b80: 705f 7820 3d20 6e70 2e61 6273 286e 702e  p_x = np.abs(np.
+00018b90: 6469 6666 286e 6f6e 5f6d 6974 6f74 6963  diff(non_mitotic
+00018ba0: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
+00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bc0: 2061 6c6c 5f64 6973 705f 7a20 3d20 6e70   all_disp_z = np
+00018bd0: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
+00018be0: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00018c00: 6c6c 5f64 6973 705f 7920 3d20 6e70 2e61  ll_disp_y = np.a
+00018c10: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
+00018c20: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+00018c30: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+00018c40: 5f64 6973 705f 7820 3d20 6e70 2e61 6273  _disp_x = np.abs
+00018c50: 286e 702e 6469 6666 2861 6c6c 5f64 6973  (np.diff(all_dis
+00018c60: 705f 7829 290d 0a0d 0a0d 0a20 2020 2020  p_x))......     
+00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00018ca0: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
+00018cb0: 6d65 2e61 7070 656e 6428 6920 2a20 7365  me.append(i * se
+00018cc0: 6c66 2e74 6361 6c69 6272 6174 696f 6e29  lf.tcalibration)
+00018cd0: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00018ce0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018cf0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018d00: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+00018d10: 6e28 6d69 746f 7469 635f 6469 7370 5f7a  n(mitotic_disp_z
+00018d20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018d30: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018d40: 6f74 6963 5f76 6172 5f64 6973 705f 7a2e  otic_var_disp_z.
+00018d50: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+00018d60: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
+00018d70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018d80: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018d90: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
+00018da0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00018db0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
 00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2073 656c 662e 6d69 746f 7469 635f 6d65   self.mitotic_me
-00018de0: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00018df0: 286e 702e 6d65 616e 286d 6974 6f74 6963  (np.mean(mitotic
-00018e00: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
-00018e10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018e20: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00018e30: 6469 7370 5f78 2e61 7070 656e 6428 6e70  disp_x.append(np
-00018e40: 2e73 7464 286d 6974 6f74 6963 5f64 6973  .std(mitotic_dis
-00018e50: 705f 7829 290d 0a0d 0a20 2020 2020 2020  p_x))....       
-00018e60: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00018e70: 7465 7265 645f 7661 6c75 6573 203d 205b  tered_values = [
-00018e80: 7661 6c20 666f 7220 7661 6c20 696e 206d  val for val in m
-00018e90: 6974 6f74 6963 5f72 6164 6975 7320 6966  itotic_radius if
-00018ea0: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
-00018eb0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00018ec0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018ed0: 7469 635f 6d65 616e 5f72 6164 6975 732e  tic_mean_radius.
-00018ee0: 6170 7065 6e64 286e 702e 6d65 616e 2866  append(np.mean(f
-00018ef0: 696c 7465 7265 645f 7661 6c75 6573 2929  iltered_values))
-00018f00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018f10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00018f20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018f30: 2e6d 6974 6f74 6963 5f76 6172 5f72 6164  .mitotic_var_rad
-00018f40: 6975 732e 6170 7065 6e64 286e 702e 7374  ius.append(np.st
-00018f50: 6428 6669 6c74 6572 6564 5f76 616c 7565  d(filtered_value
-00018f60: 7329 290d 0a20 2020 2020 2020 2020 2020  s))..           
-00018f70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00018f80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018f90: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
-00018fa0: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
-00018fb0: 2e6d 6561 6e28 6d69 746f 7469 635f 7370  .mean(mitotic_sp
-00018fc0: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
-00018fd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018fe0: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00018ff0: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00019000: 6d69 746f 7469 635f 7370 6565 6429 290d  mitotic_speed)).
-00019010: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00019020: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00019030: 7469 635f 6d65 616e 5f61 6363 2e61 7070  tic_mean_acc.app
-00019040: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00019050: 7469 635f 6163 6329 290d 0a20 2020 2020  tic_acc))..     
-00019060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019070: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00019080: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-00019090: 6428 6d69 746f 7469 635f 6163 6329 290d  d(mitotic_acc)).
-000190a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000190b0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-000190c0: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
-000190d0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-000190e0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
-000190f0: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
-00019100: 6861 6e67 6529 290d 0a20 2020 2020 2020  hange))..       
-00019110: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019120: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
-00019130: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00019140: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
-00019150: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-00019160: 616c 5f63 6861 6e67 6529 290d 0a0d 0a20  al_change)).... 
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00019190: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
-000191a0: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-000191b0: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
-000191c0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-000191d0: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-000191e0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-000191f0: 746f 7469 635f 7661 725f 6469 7374 616e  totic_var_distan
-00019200: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00019210: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00019220: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
-00019230: 5f6d 6173 6b29 290d 0a0d 0a20 2020 2020  _mask))....     
-00019240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019250: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00019260: 6d65 616e 5f64 6973 705f 7a2e 6170 7065  mean_disp_z.appe
-00019270: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
-00019280: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
-00019290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000192a0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000192b0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
-000192c0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-000192d0: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
-000192e0: 7a29 290d 0a0d 0a20 2020 2020 2020 2020  z))....         
-000192f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019300: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00019310: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00019320: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
-00019330: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00019360: 635f 7661 725f 6469 7370 5f79 2e61 7070  c_var_disp_y.app
-00019370: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
-00019380: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
-00019390: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000193a0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-000193b0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-000193c0: 705f 782e 6170 7065 6e64 286e 702e 6d65  p_x.append(np.me
-000193d0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-000193e0: 6973 705f 7829 290d 0a20 2020 2020 2020  isp_x))..       
-000193f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019400: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-00019410: 725f 6469 7370 5f78 2e61 7070 656e 6428  r_disp_x.append(
-00019420: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00019430: 6963 5f64 6973 705f 7829 290d 0a0d 0a20  ic_disp_x)).... 
-00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019450: 2020 2066 696c 7465 7265 645f 7661 6c75     filtered_valu
-00019460: 6573 203d 205b 7661 6c20 666f 7220 7661  es = [val for va
-00019470: 6c20 696e 206e 6f6e 5f6d 6974 6f74 6963  l in non_mitotic
-00019480: 5f72 6164 6975 7320 6966 2076 616c 2069  _radius if val i
-00019490: 7320 6e6f 7420 4e6f 6e65 5d0d 0a20 2020  s not None]..   
-000194a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194b0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000194c0: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
-000194d0: 7065 6e64 286e 702e 6d65 616e 2866 696c  pend(np.mean(fil
-000194e0: 7465 7265 645f 7661 6c75 6573 2929 0d0a  tered_values))..
+00018dd0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018de0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
+00018df0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018e00: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
+00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e20: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
+00018e30: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00018e40: 6428 6e70 2e6d 6561 6e28 6d69 746f 7469  d(np.mean(mitoti
+00018e50: 635f 6469 7370 5f78 2929 0d0a 2020 2020  c_disp_x))..    
+00018e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e70: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00018e80: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
+00018e90: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00018ea0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00018ec0: 6c74 6572 6564 5f76 616c 7565 7320 3d20  ltered_values = 
+00018ed0: 5b76 616c 2066 6f72 2076 616c 2069 6e20  [val for val in 
+00018ee0: 6d69 746f 7469 635f 7261 6469 7573 2069  mitotic_radius i
+00018ef0: 6620 7661 6c20 6973 206e 6f74 204e 6f6e  f val is not Non
+00018f00: 655d 0d0a 2020 2020 2020 2020 2020 2020  e]..            
+00018f10: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018f20: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
+00018f30: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018f40: 6669 6c74 6572 6564 5f76 616c 7565 7329  filtered_values)
+00018f50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018f60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00018f70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018f80: 662e 6d69 746f 7469 635f 7661 725f 7261  f.mitotic_var_ra
+00018f90: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+00018fa0: 7464 2866 696c 7465 7265 645f 7661 6c75  td(filtered_valu
+00018fb0: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
+00018fc0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fe0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00018ff0: 6e5f 7370 6565 642e 6170 7065 6e64 286e  n_speed.append(n
+00019000: 702e 6d65 616e 286d 6974 6f74 6963 5f73  p.mean(mitotic_s
+00019010: 7065 6564 2929 0d0a 2020 2020 2020 2020  peed))..        
+00019020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019030: 2e6d 6974 6f74 6963 5f76 6172 5f73 7065  .mitotic_var_spe
+00019040: 6564 2e61 7070 656e 6428 6e70 2e73 7464  ed.append(np.std
+00019050: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
+00019060: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019070: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00019080: 6f74 6963 5f6d 6561 6e5f 6163 632e 6170  otic_mean_acc.ap
+00019090: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
+000190a0: 6f74 6963 5f61 6363 2929 0d0a 2020 2020  otic_acc))..    
+000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190c0: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+000190d0: 5f61 6363 2e61 7070 656e 6428 6e70 2e73  _acc.append(np.s
+000190e0: 7464 286d 6974 6f74 6963 5f61 6363 2929  td(mitotic_acc))
+000190f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019100: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00019110: 6f74 6963 5f6d 6561 6e5f 6469 7265 6374  otic_mean_direct
+00019120: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+00019130: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
+00019140: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
+00019150: 6368 616e 6765 2929 0d0a 2020 2020 2020  change))..      
+00019160: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019170: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
+00019180: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00019190: 652e 6170 7065 6e64 286e 702e 7374 6428  e.append(np.std(
+000191a0: 6d69 746f 7469 635f 6469 7265 6374 696f  mitotic_directio
+000191b0: 6e61 6c5f 6368 616e 6765 2929 0d0a 0d0a  nal_change))....
+000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191d0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+000191e0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+000191f0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00019200: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
+00019210: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00019220: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+00019230: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00019240: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
+00019250: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
+00019260: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00019270: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+00019280: 6c5f 6d61 736b 2929 0d0a 0d0a 2020 2020  l_mask))....    
+00019290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192a0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+000192b0: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
+000192c0: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+000192d0: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
+000192e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000192f0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00019300: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
+00019310: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
+00019320: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+00019330: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
+00019340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019350: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00019360: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
+00019370: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00019380: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+000193b0: 6963 5f76 6172 5f64 6973 705f 792e 6170  ic_var_disp_y.ap
+000193c0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
+000193d0: 6d69 746f 7469 635f 6469 7370 5f79 2929  mitotic_disp_y))
+000193e0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000193f0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00019400: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
+00019410: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
+00019420: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
+00019430: 6469 7370 5f78 2929 0d0a 2020 2020 2020  disp_x))..      
+00019440: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019450: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00019460: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
+00019470: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+00019480: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
+00019490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194a0: 2020 2020 6669 6c74 6572 6564 5f76 616c      filtered_val
+000194b0: 7565 7320 3d20 5b76 616c 2066 6f72 2076  ues = [val for v
+000194c0: 616c 2069 6e20 6e6f 6e5f 6d69 746f 7469  al in non_mitoti
+000194d0: 635f 7261 6469 7573 2069 6620 7661 6c20  c_radius if val 
+000194e0: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
 000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00019510: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00019520: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f72  on_mitotic_var_r
-00019530: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00019540: 7374 6428 6669 6c74 6572 6564 5f76 616c  std(filtered_val
-00019550: 7565 7329 290d 0a0d 0a20 2020 2020 2020  ues))....       
-00019560: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019570: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019580: 616e 5f73 7065 6564 2e61 7070 656e 6428  an_speed.append(
-00019590: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-000195a0: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-000195d0: 635f 7661 725f 7370 6565 642e 6170 7065  c_var_speed.appe
-000195e0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-000195f0: 746f 7469 635f 7370 6565 6429 290d 0a0d  totic_speed))...
-00019600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019610: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00019620: 746f 7469 635f 6d65 616e 5f61 6363 2e61  totic_mean_acc.a
-00019630: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00019640: 6e5f 6d69 746f 7469 635f 6163 6329 290d  n_mitotic_acc)).
-00019650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019660: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00019670: 746f 7469 635f 7661 725f 6163 632e 6170  totic_var_acc.ap
-00019680: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00019690: 6d69 746f 7469 635f 6163 6329 290d 0a0d  mitotic_acc))...
-000196a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000196b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000196c0: 746f 7469 635f 6d65 616e 5f64 6972 6563  totic_mean_direc
-000196d0: 7469 6f6e 616c 5f63 6861 6e67 652e 6170  tional_change.ap
-000196e0: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-000196f0: 5f6d 6974 6f74 6963 5f64 6972 6563 7469  _mitotic_directi
-00019700: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019720: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00019730: 7469 635f 7661 725f 6469 7265 6374 696f  tic_var_directio
-00019740: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
-00019750: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-00019760: 6f74 6963 5f64 6972 6563 7469 6f6e 616c  otic_directional
-00019770: 5f63 6861 6e67 6529 2920 0d0a 0d0a 2020  _change)) ....  
-00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019790: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000197a0: 6963 5f6d 6561 6e5f 6469 7374 616e 6365  ic_mean_distance
-000197b0: 5f63 656c 6c5f 6d61 736b 2e61 7070 656e  _cell_mask.appen
-000197c0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
-000197d0: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
-000197e0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
-000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019800: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00019810: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-00019820: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-00019830: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00019840: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00019850: 6d61 736b 2929 0d0a 0d0a 0d0a 2020 2020  mask))......    
-00019860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019870: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00019880: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
-00019890: 6561 6e28 616c 6c5f 6469 7370 5f7a 2929  ean(all_disp_z))
-000198a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000198b0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-000198c0: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
-000198d0: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-000198e0: 5f7a 2929 0d0a 0d0a 2020 2020 2020 2020  _z))....        
-000198f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019900: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f79  .all_mean_disp_y
-00019910: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019920: 616c 6c5f 6469 7370 5f79 2929 0d0a 2020  all_disp_y))..  
-00019930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019940: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00019950: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-00019960: 7374 6428 616c 6c5f 6469 7370 5f79 2929  std(all_disp_y))
-00019970: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019980: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00019990: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
-000199a0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-000199b0: 6469 7370 5f78 2929 0d0a 2020 2020 2020  disp_x))..      
-000199c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000199d0: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-000199e0: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
-000199f0: 616c 6c5f 6469 7370 5f78 2929 0d0a 0d0a  all_disp_x))....
-00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a10: 2020 2020 6669 6c74 6572 6564 5f76 616c      filtered_val
-00019a20: 7565 7320 3d20 5b76 616c 2066 6f72 2076  ues = [val for v
-00019a30: 616c 2069 6e20 616c 6c5f 7261 6469 7573  al in all_radius
-00019a40: 2069 6620 7661 6c20 6973 206e 6f74 204e   if val is not N
-00019a50: 6f6e 655d 0d0a 2020 2020 2020 2020 2020  one]..          
-00019a60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00019a70: 6c6c 5f6d 6561 6e5f 7261 6469 7573 2e61  ll_mean_radius.a
-00019a80: 7070 656e 6428 6e70 2e6d 6561 6e28 6669  ppend(np.mean(fi
-00019a90: 6c74 6572 6564 5f76 616c 7565 7329 290d  ltered_values)).
-00019aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ab0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00019ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019ad0: 616c 6c5f 7661 725f 7261 6469 7573 2e61  all_var_radius.a
-00019ae0: 7070 656e 6428 6e70 2e73 7464 2866 696c  ppend(np.std(fil
-00019af0: 7465 7265 645f 7661 6c75 6573 2929 0d0a  tered_values))..
-00019b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019b10: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00019b20: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
-00019b30: 286e 702e 6d65 616e 2861 6c6c 5f73 7065  (np.mean(all_spe
-00019b40: 6564 2929 0d0a 2020 2020 2020 2020 2020  ed))..          
-00019b50: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-00019b60: 6c6c 5f76 6172 5f73 7065 6564 2e61 7070  ll_var_speed.app
-00019b70: 656e 6428 6e70 2e73 7464 2861 6c6c 5f73  end(np.std(all_s
-00019b80: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
-00019b90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019ba0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6163 632e  lf.all_mean_acc.
-00019bb0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-00019bc0: 6c6c 5f61 6363 2929 0d0a 2020 2020 2020  ll_acc))..      
-00019bd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019be0: 6c66 2e61 6c6c 5f76 6172 5f61 6363 2e61  lf.all_var_acc.a
-00019bf0: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00019c00: 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a 2020  _acc))........  
-00019c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c20: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-00019c30: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00019c40: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
-00019c50: 6e28 616c 6c5f 6469 7265 6374 696f 6e61  n(all_directiona
-00019c60: 6c5f 6368 616e 6765 2929 0d0a 2020 2020  l_change))..    
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c80: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6972  self.all_var_dir
-00019c90: 6563 7469 6f6e 616c 5f63 6861 6e67 652e  ectional_change.
-00019ca0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00019cb0: 6c5f 6469 7265 6374 696f 6e61 6c5f 6368  l_directional_ch
-00019cc0: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
-00019cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019ce0: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7374  lf.all_mean_dist
-00019cf0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
-00019d00: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00019d10: 6c5f 6469 7374 616e 6365 5f63 656c 6c5f  l_distance_cell_
-00019d20: 6d61 736b 2929 0d0a 2020 2020 2020 2020  mask))..        
-00019d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019d40: 2e61 6c6c 5f76 6172 5f64 6973 7461 6e63  .all_var_distanc
-00019d50: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
-00019d60: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-00019d70: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00019d80: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019da0: 0d0a 2020 2020 2020 2020 0d0a 6465 6620  ..        ..def 
-00019db0: 626f 756e 6461 7279 5f70 6f69 6e74 7328  boundary_points(
-00019dc0: 6d61 736b 2c20 7863 616c 6962 7261 7469  mask, xcalibrati
-00019dd0: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
-00019de0: 2c20 7a63 616c 6962 7261 7469 6f6e 293a  , zcalibration):
-00019df0: 0d0a 0d0a 2020 2020 6e64 696d 203d 206c  ....    ndim = l
-00019e00: 656e 286d 6173 6b2e 7368 6170 6529 0d0a  en(mask.shape)..
-00019e10: 2020 2020 7469 6d65 645f 6d61 736b 203d      timed_mask =
-00019e20: 207b 7d0d 0a20 2020 206d 6173 6b20 3d20   {}..    mask = 
-00019e30: 6d61 736b 203e 2030 0d0a 2020 2020 6d61  mask > 0..    ma
-00019e40: 736b 203d 206d 6173 6b2e 6173 7479 7065  sk = mask.astype
-00019e50: 2827 7569 6e74 3827 290d 0a20 2020 2023  ('uint8')..    #
-00019e60: 2059 5820 7368 6170 6564 206f 626a 6563   YX shaped objec
-00019e70: 740d 0a20 2020 2069 6620 6e64 696d 203d  t..    if ndim =
-00019e80: 3d20 323a 0d0a 2020 2020 2020 2020 0d0a  = 2:..        ..
-00019e90: 2020 2020 2020 2020 626f 756e 6461 7279          boundary
-00019ea0: 203d 2066 696e 645f 626f 756e 6461 7269   = find_boundari
-00019eb0: 6573 286d 6173 6b29 0d0a 2020 2020 2020  es(mask)..      
-00019ec0: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
-00019ed0: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
-00019ee0: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-00019ef0: 6172 7929 200d 0a20 2020 2020 2020 2069  ary) ..        i
-00019f00: 6e64 6963 6573 203d 206e 702e 7768 6572  ndices = np.wher
-00019f10: 6528 626f 756e 6461 7279 203e 2030 290d  e(boundary > 0).
-00019f20: 0a20 2020 2020 2020 2072 6561 6c5f 696e  .        real_in
-00019f30: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-00019f40: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-00019f50: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
-00019f60: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
-00019f70: 2829 0d0a 0d0a 2020 2020 2020 2020 666f  ()....        fo
-00019f80: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-00019f90: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
-00019fa0: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
-00019fb0: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00019fc0: 6a5d 5b30 5d20 3d20 7265 616c 5f69 6e64  j][0] = real_ind
-00019fd0: 6963 6573 5b6a 5d5b 305d 202a 2079 6361  ices[j][0] * yca
-00019fe0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019ff0: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-0001a000: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
-0001a010: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
-0001a020: 2078 6361 6c69 6272 6174 696f 6e0d 0a0d   xcalibration...
-0001a030: 0a20 2020 2020 2020 2074 7265 6520 3d20  .        tree = 
-0001a040: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-0001a050: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
-0001a060: 2020 2020 2020 2023 2054 6869 7320 6f62         # This ob
-0001a070: 6a65 6374 2063 6f6e 7461 696e 7320 6c69  ject contains li
-0001a080: 7374 206f 6620 616c 6c20 7468 6520 706f  st of all the po
-0001a090: 696e 7473 2066 6f72 2061 6c6c 2074 6865  ints for all the
-0001a0a0: 206c 6162 656c 7320 696e 2074 6865 204d   labels in the M
-0001a0b0: 6173 6b20 696d 6167 6520 7769 7468 2074  ask image with t
-0001a0c0: 6865 206c 6162 656c 2069 6420 616e 6420  he label id and 
-0001a0d0: 766f 6c75 6d65 206f 6620 6561 6368 206c  volume of each l
-0001a0e0: 6162 656c 0d0a 2020 2020 2020 2020 7469  abel..        ti
-0001a0f0: 6d65 645f 6d61 736b 5b73 7472 2830 295d  med_mask[str(0)]
-0001a100: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-0001a110: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-0001a120: 645d 0d0a 0d0a 2020 2020 2320 5459 5820  d]....    # TYX 
-0001a130: 7368 6170 6564 206f 626a 6563 740d 0a20  shaped object.. 
-0001a140: 2020 2069 6620 6e64 696d 203d 3d20 333a     if ndim == 3:
-0001a150: 0d0a 0d0a 0d0a 2020 2020 2020 2020 666f  ......        fo
-0001a160: 7220 6920 696e 2074 7164 6d28 7261 6e67  r i in tqdm(rang
-0001a170: 6528 302c 206d 6173 6b2e 7368 6170 655b  e(0, mask.shape[
-0001a180: 305d 2929 3a0d 0a20 2020 2020 2020 2020  0])):..         
-0001a190: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001a1a0: 2020 2020 2020 2020 2062 6f75 6e64 6172           boundar
-0001a1b0: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
-0001a1c0: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
-0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1e0: 7265 6769 6f6e 6365 6e74 726f 6964 203d  regioncentroid =
-0001a1f0: 2028 302c 2920 2b20 636f 6d70 7574 655f   (0,) + compute_
-0001a200: 6365 6e74 726f 6964 2862 6f75 6e64 6172  centroid(boundar
-0001a210: 7929 200d 0a20 2020 2020 2020 2020 2020  y) ..           
-0001a220: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001a230: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-0001a240: 203e 2030 290d 0a20 2020 2020 2020 2020   > 0)..         
-0001a250: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-0001a260: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
-0001a270: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
-0001a280: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
-0001a290: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
-0001a2a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a2b0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-0001a2c0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
-0001a2d0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
-0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2f0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-0001a300: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
-0001a310: 6573 5b6a 5d5b 305d 202a 2079 6361 6c69  es[j][0] * ycali
-0001a320: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-0001a330: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-0001a340: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-0001a350: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-0001a360: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
-0001a370: 696f 6e0d 0a0d 0a20 2020 2020 2020 2020  ion....         
-0001a380: 2020 2020 2020 2074 7265 6520 3d20 7370         tree = sp
-0001a390: 6174 6961 6c2e 634b 4454 7265 6528 7265  atial.cKDTree(re
-0001a3a0: 616c 5f69 6e64 6963 6573 290d 0a0d 0a20  al_indices).... 
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001a3c0: 696d 6564 5f6d 6173 6b5b 7374 7228 6929  imed_mask[str(i)
-0001a3d0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-0001a3e0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-0001a3f0: 6964 5d0d 0a20 2020 2020 2020 2020 2020  id]..           
-0001a400: 200d 0a20 2020 2023 2054 5a59 5820 7368   ..    # TZYX sh
-0001a410: 6170 6564 206f 626a 6563 740d 0a20 2020  aped object..   
-0001a420: 2069 6620 6e64 696d 203d 3d20 343a 0d0a   if ndim == 4:..
-0001a430: 2020 2020 2020 2020 7072 696e 7428 274d          print('M
-0001a440: 616b 696e 6720 6d61 736b 2069 6e20 3444  aking mask in 4D
-0001a450: 2729 0d0a 2020 2020 2020 2020 626f 756e  ')..        boun
-0001a460: 6461 7279 203d 206e 702e 7a65 726f 7328  dary = np.zeros(
-0001a470: 0d0a 2020 2020 2020 2020 2020 2020 5b6d  ..            [m
-0001a480: 6173 6b2e 7368 6170 655b 305d 2c20 6d61  ask.shape[0], ma
-0001a490: 736b 2e73 6861 7065 5b31 5d2c 206d 6173  sk.shape[1], mas
-0001a4a0: 6b2e 7368 6170 655b 325d 2c20 6d61 736b  k.shape[2], mask
-0001a4b0: 2e73 6861 7065 5b33 5d5d 2c20 6474 7970  .shape[3]], dtyp
-0001a4c0: 653d 6e70 2e75 696e 7438 0d0a 2020 2020  e=np.uint8..    
-0001a4d0: 2020 2020 290d 0a20 2020 2020 2020 2066      )..        f
-0001a4e0: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
-0001a4f0: 206d 6173 6b2e 7368 6170 655b 305d 293a   mask.shape[0]):
-0001a500: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0001a510: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-0001a520: 6461 7279 5b69 2c3a 5d20 3d20 6669 6e64  dary[i,:] = find
-0001a530: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
-0001a540: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
-0001a550: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
-0001a560: 6964 203d 2063 6f6d 7075 7465 5f63 656e  id = compute_cen
-0001a570: 7472 6f69 6428 626f 756e 6461 7279 5b69  troid(boundary[i
-0001a580: 2c3a 5d29 200d 0a20 2020 2020 2020 2020  ,:]) ..         
-0001a590: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
-0001a5a0: 7768 6572 6528 626f 756e 6461 7279 5b69  where(boundary[i
-0001a5b0: 2c3a 5d20 3e20 3029 0d0a 2020 2020 2020  ,:] > 0)..      
-0001a5c0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-0001a5d0: 6573 203d 206e 702e 7472 616e 7370 6f73  es = np.transpos
-0001a5e0: 6528 6e70 2e61 7361 7272 6179 2869 6e64  e(np.asarray(ind
-0001a5f0: 6963 6573 2c20 6474 7970 653d 6e70 2e66  ices, dtype=np.f
-0001a600: 6c6f 6174 3332 2929 2e63 6f70 7928 290d  loat32)).copy().
-0001a610: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-0001a620: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-0001a630: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-0001a640: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-0001a650: 2020 2020 2020 2020 2020 2020 7265 616c              real
-0001a660: 5f69 6e64 6963 6573 5b6a 5d5b 305d 203d  _indices[j][0] =
-0001a670: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
-0001a680: 5b30 5d20 2a20 7a63 616c 6962 7261 7469  [0] * zcalibrati
-0001a690: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-0001a6a0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-0001a6b0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-0001a6c0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-0001a6d0: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
-0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6f0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-0001a700: 5b6a 5d5b 325d 203d 2072 6561 6c5f 696e  [j][2] = real_in
-0001a710: 6469 6365 735b 6a5d 5b32 5d20 2a20 7863  dices[j][2] * xc
-0001a720: 616c 6962 7261 7469 6f6e 0d0a 0d0a 2020  alibration....  
-0001a730: 2020 2020 2020 2020 2020 7472 6565 203d            tree =
-0001a740: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-0001a750: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-0001a760: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0001a770: 645f 6d61 736b 5b73 7472 2869 295d 203d  d_mask[str(i)] =
-0001a780: 205b 7472 6565 2c20 696e 6469 6365 732c   [tree, indices,
-0001a790: 2072 6567 696f 6e63 656e 7472 6f69 645d   regioncentroid]
-0001a7a0: 0d0a 2020 2020 7072 696e 7428 2743 6f6d  ..    print('Com
-0001a7b0: 7075 7465 6420 7468 6520 626f 756e 6461  puted the bounda
-0001a7c0: 7279 2070 6f69 6e74 7327 290d 0a0d 0a20  ry points').... 
-0001a7d0: 2020 2072 6574 7572 6e20 7469 6d65 645f     return timed_
-0001a7e0: 6d61 736b 2c20 626f 756e 6461 7279 2020  mask, boundary  
-0001a7f0: 2020 2020 2020 0d0a 0d0a 6465 6620 636f        ....def co
-0001a800: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
-0001a810: 696e 6172 795f 696d 6167 6529 3a0d 0a20  inary_image):.. 
-0001a820: 2020 2023 2045 6e73 7572 6520 6269 6e61     # Ensure bina
-0001a830: 7279 2069 6d61 6765 2069 7320 6120 4e75  ry image is a Nu
-0001a840: 6d50 7920 6172 7261 790d 0a20 2020 2062  mPy array..    b
-0001a850: 696e 6172 795f 696d 6167 6520 3d20 6e70  inary_image = np
-0001a860: 2e61 7272 6179 2862 696e 6172 795f 696d  .array(binary_im
-0001a870: 6167 6529 0d0a 0d0a 2020 2020 7768 6974  age)....    whit
-0001a880: 655f 7069 7865 6c73 203d 206e 702e 7768  e_pixels = np.wh
-0001a890: 6572 6528 6269 6e61 7279 5f69 6d61 6765  ere(binary_image
-0001a8a0: 203d 3d20 3129 0d0a 2020 2020 6e75 6d5f   == 1)..    num_
-0001a8b0: 7069 7865 6c73 203d 206c 656e 2877 6869  pixels = len(whi
-0001a8c0: 7465 5f70 6978 656c 735b 305d 290d 0a0d  te_pixels[0])...
-0001a8d0: 0a20 2020 2023 2043 6f6d 7075 7465 2074  .    # Compute t
-0001a8e0: 6865 2063 656e 7472 6f69 6420 6f66 2074  he centroid of t
-0001a8f0: 6865 2077 6869 7465 2070 6978 656c 7320  he white pixels 
-0001a900: 696e 2074 6865 2062 6f75 6e64 6172 7920  in the boundary 
-0001a910: 696d 6167 650d 0a20 2020 2063 656e 7472  image..    centr
-0001a920: 6f69 6420 3d20 6e70 2e7a 6572 6f73 2862  oid = np.zeros(b
-0001a930: 696e 6172 795f 696d 6167 652e 6e64 696d  inary_image.ndim
-0001a940: 290d 0a20 2020 2066 6f72 2064 696d 2069  )..    for dim i
-0001a950: 6e20 7261 6e67 6528 6269 6e61 7279 5f69  n range(binary_i
-0001a960: 6d61 6765 2e6e 6469 6d29 3a0d 0a20 2020  mage.ndim):..   
-0001a970: 2020 2020 2063 656e 7472 6f69 645b 6469       centroid[di
-0001a980: 6d5d 203d 2077 6869 7465 5f70 6978 656c  m] = white_pixel
-0001a990: 735b 6469 6d5d 2e73 756d 2829 202f 206e  s[dim].sum() / n
-0001a9a0: 756d 5f70 6978 656c 730d 0a0d 0a20 2020  um_pixels....   
-0001a9b0: 2072 6574 7572 6e20 6365 6e74 726f 6964   return centroid
-0001a9c0: 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64 6566  ........ ....def
-0001a9d0: 2067 6574 5f63 7376 5f64 6174 6128 6373   get_csv_data(cs
-0001a9e0: 7629 3a0d 0a0d 0a20 2020 2020 2020 2064  v):....        d
-0001a9f0: 6174 6173 6574 203d 2070 642e 7265 6164  ataset = pd.read
-0001aa00: 5f63 7376 280d 0a20 2020 2020 2020 2020  _csv(..         
-0001aa10: 2020 2063 7376 2c20 6465 6c69 6d69 7465     csv, delimite
-0001aa20: 723d 222c 222c 2065 6e63 6f64 696e 673d  r=",", encoding=
-0001aa30: 2275 6e69 636f 6465 5f65 7363 6170 6522  "unicode_escape"
-0001aa40: 2c20 6c6f 775f 6d65 6d6f 7279 3d46 616c  , low_memory=Fal
-0001aa50: 7365 0d0a 2020 2020 2020 2020 295b 333a  se..        )[3:
-0001aa60: 5d0d 0a20 2020 2020 2020 2064 6174 6173  ]..        datas
-0001aa70: 6574 5f69 6e64 6578 203d 2064 6174 6173  et_index = datas
-0001aa80: 6574 2e69 6e64 6578 0d0a 2020 2020 2020  et.index..      
-0001aa90: 2020 7265 7475 726e 2064 6174 6173 6574    return dataset
-0001aaa0: 2c20 6461 7461 7365 745f 696e 6465 780d  , dataset_index.
-0001aab0: 0a20 2020 200d 0a64 6566 2067 6574 5f73  .    ..def get_s
-0001aac0: 706f 745f 6461 7461 7365 7428 7370 6f74  pot_dataset(spot
-0001aad0: 5f64 6174 6173 6574 2c20 7472 6163 6b5f  _dataset, track_
-0001aae0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001aaf0: 7973 2c20 7863 616c 6962 7261 7469 6f6e  ys, xcalibration
-0001ab00: 2c20 7963 616c 6962 7261 7469 6f6e 2c20  , ycalibration, 
-0001ab10: 7a63 616c 6962 7261 7469 6f6e 2c20 4174  zcalibration, At
-0001ab20: 7472 6962 7574 6542 6f78 6e61 6d65 2c20  tributeBoxname, 
-0001ab30: 6465 7465 6374 696f 6e63 6861 6e6e 656c  detectionchannel
-0001ab40: 293a 0d0a 2020 2020 2020 2020 416c 6c56  ):..        AllV
-0001ab50: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
-0001ab60: 2020 2020 706f 7369 7820 3d20 7472 6163      posix = trac
-0001ab70: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001ab80: 6b65 7973 5b22 706f 7369 7822 5d0d 0a20  keys["posix"].. 
-0001ab90: 2020 2020 2020 2070 6f73 6979 203d 2074         posiy = t
-0001aba0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001abb0: 6f74 5f6b 6579 735b 2270 6f73 6979 225d  ot_keys["posiy"]
-0001abc0: 0d0a 2020 2020 2020 2020 706f 7369 7a20  ..        posiz 
-0001abd0: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001abe0: 5f73 706f 745f 6b65 7973 5b22 706f 7369  _spot_keys["posi
-0001abf0: 7a22 5d0d 0a20 2020 2020 2020 2066 7261  z"]..        fra
-0001ac00: 6d65 203d 2074 7261 636b 5f61 6e61 6c79  me = track_analy
-0001ac10: 7369 735f 7370 6f74 5f6b 6579 735b 2266  sis_spot_keys["f
-0001ac20: 7261 6d65 225d 0d0a 2020 2020 2020 2020  rame"]..        
-0001ac30: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-0001ac40: 6f6e 5820 3d20 280d 0a20 2020 2020 2020  onX = (..       
-0001ac50: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-0001ac60: 745b 706f 7369 785d 2e61 7374 7970 6528  t[posix].astype(
-0001ac70: 2266 6c6f 6174 2229 202f 2078 6361 6c69  "float") / xcali
-0001ac80: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-0001ac90: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-0001aca0: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-0001acb0: 6f6e 5920 3d20 280d 0a20 2020 2020 2020  onY = (..       
-0001acc0: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-0001acd0: 745b 706f 7369 795d 2e61 7374 7970 6528  t[posiy].astype(
-0001ace0: 2266 6c6f 6174 2229 202f 2079 6361 6c69  "float") / ycali
-0001acf0: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-0001ad00: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-0001ad10: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-0001ad20: 6f6e 5a20 3d20 280d 0a20 2020 2020 2020  onZ = (..       
-0001ad30: 2020 2020 2073 706f 745f 6461 7461 7365       spot_datase
-0001ad40: 745b 706f 7369 7a5d 2e61 7374 7970 6528  t[posiz].astype(
-0001ad50: 2266 6c6f 6174 2229 202f 207a 6361 6c69  "float") / zcali
-0001ad60: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
-0001ad70: 2029 2e61 7374 7970 6528 2269 6e74 2229   ).astype("int")
-0001ad80: 0d0a 2020 2020 2020 2020 4c6f 6361 7469  ..        Locati
-0001ad90: 6f6e 5420 3d20 2873 706f 745f 6461 7461  onT = (spot_data
-0001ada0: 7365 745b 6672 616d 655d 2e61 7374 7970  set[frame].astyp
-0001adb0: 6528 2266 6c6f 6174 2229 292e 6173 7479  e("float")).asty
-0001adc0: 7065 2822 696e 7422 290d 0a20 2020 2020  pe("int")..     
-0001add0: 2020 200d 0a0d 0a20 2020 2020 2020 2069     ....        i
-0001ade0: 676e 6f72 655f 7661 6c75 6573 203d 205b  gnore_values = [
-0001adf0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001ae00: 706f 745f 6b65 7973 5b22 6d65 616e 5f69  pot_keys["mean_i
-0001ae10: 6e74 656e 7369 7479 225d 2c74 7261 636b  ntensity"],track
-0001ae20: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001ae30: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
-0001ae40: 7369 7479 225d 5d0d 0a20 2020 2020 2020  sity"]]..       
-0001ae50: 2066 6f72 2028 6b2c 7629 2069 6e20 7472   for (k,v) in tr
-0001ae60: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001ae70: 745f 6b65 7973 2e69 7465 6d73 2829 3a0d  t_keys.items():.
-0001ae80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001ae90: 2020 2069 6620 6465 7465 6374 696f 6e63     if detectionc
-0001aea0: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aec0: 2020 2069 6620 6b20 3d3d 2022 6d65 616e     if k == "mean
-0001aed0: 5f69 6e74 656e 7369 7479 5f63 6832 223a  _intensity_ch2":
-0001aee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aef0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0001af00: 7565 203d 2074 7261 636b 5f61 6e61 6c79  ue = track_analy
-0001af10: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
-0001af20: 6561 6e5f 696e 7465 6e73 6974 7922 5d0d  ean_intensity"].
-0001af30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001af40: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
-0001af50: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
-0001af60: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
-0001af70: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af90: 2020 2020 2069 6620 6b20 3d3d 2022 746f       if k == "to
-0001afa0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0001afb0: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
-0001afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afd0: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
-0001afe0: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001aff0: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001b000: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
+00019500: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00019510: 6963 5f6d 6561 6e5f 7261 6469 7573 2e61  ic_mean_radius.a
+00019520: 7070 656e 6428 6e70 2e6d 6561 6e28 6669  ppend(np.mean(fi
+00019530: 6c74 6572 6564 5f76 616c 7565 7329 290d  ltered_values)).
+00019540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019550: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00019560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019570: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019580: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00019590: 2e73 7464 2866 696c 7465 7265 645f 7661  .std(filtered_va
+000195a0: 6c75 6573 2929 0d0a 0d0a 2020 2020 2020  lues))....      
+000195b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000195c0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+000195d0: 6561 6e5f 7370 6565 642e 6170 7065 6e64  ean_speed.append
+000195e0: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
+000195f0: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
+00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019610: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00019620: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
+00019630: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00019640: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
+00019650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019660: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00019670: 6974 6f74 6963 5f6d 6561 6e5f 6163 632e  itotic_mean_acc.
+00019680: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00019690: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2929  on_mitotic_acc))
+000196a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000196b0: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+000196c0: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
+000196d0: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
+000196e0: 5f6d 6974 6f74 6963 5f61 6363 2929 0d0a  _mitotic_acc))..
+000196f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019700: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00019710: 6974 6f74 6963 5f6d 6561 6e5f 6469 7265  itotic_mean_dire
+00019720: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00019730: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00019740: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+00019750: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019770: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00019780: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
+00019790: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+000197a0: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+000197b0: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+000197c0: 6c5f 6368 616e 6765 2929 200d 0a0d 0a20  l_change)) .... 
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000197f0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
+00019800: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
+00019810: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00019820: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00019830: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019850: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00019860: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00019870: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00019880: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00019890: 6963 5f64 6973 7461 6e63 655f 6365 6c6c  ic_distance_cell
+000198a0: 5f6d 6173 6b29 290d 0a0d 0a0d 0a20 2020  _mask))......   
+000198b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198c0: 2073 656c 662e 616c 6c5f 6d65 616e 5f64   self.all_mean_d
+000198d0: 6973 705f 7a2e 6170 7065 6e64 286e 702e  isp_z.append(np.
+000198e0: 6d65 616e 2861 6c6c 5f64 6973 705f 7a29  mean(all_disp_z)
+000198f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019900: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00019910: 7661 725f 6469 7370 5f7a 2e61 7070 656e  var_disp_z.appen
+00019920: 6428 6e70 2e73 7464 2861 6c6c 5f64 6973  d(np.std(all_dis
+00019930: 705f 7a29 290d 0a0d 0a20 2020 2020 2020  p_z))....       
+00019940: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019950: 662e 616c 6c5f 6d65 616e 5f64 6973 705f  f.all_mean_disp_
+00019960: 792e 6170 7065 6e64 286e 702e 6d65 616e  y.append(np.mean
+00019970: 2861 6c6c 5f64 6973 705f 7929 290d 0a20  (all_disp_y)).. 
+00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019990: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+000199a0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
+000199b0: 2e73 7464 2861 6c6c 5f64 6973 705f 7929  .std(all_disp_y)
+000199c0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+000199d0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000199e0: 6c5f 6d65 616e 5f64 6973 705f 782e 6170  l_mean_disp_x.ap
+000199f0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
+00019a00: 5f64 6973 705f 7829 290d 0a20 2020 2020  _disp_x))..     
+00019a10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019a20: 656c 662e 616c 6c5f 7661 725f 6469 7370  elf.all_var_disp
+00019a30: 5f78 2e61 7070 656e 6428 6e70 2e73 7464  _x.append(np.std
+00019a40: 2861 6c6c 5f64 6973 705f 7829 290d 0a0d  (all_disp_x))...
+00019a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019a60: 2020 2020 2066 696c 7465 7265 645f 7661       filtered_va
+00019a70: 6c75 6573 203d 205b 7661 6c20 666f 7220  lues = [val for 
+00019a80: 7661 6c20 696e 2061 6c6c 5f72 6164 6975  val in all_radiu
+00019a90: 7320 6966 2076 616c 2069 7320 6e6f 7420  s if val is not 
+00019aa0: 4e6f 6e65 5d0d 0a20 2020 2020 2020 2020  None]..         
+00019ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019ac0: 616c 6c5f 6d65 616e 5f72 6164 6975 732e  all_mean_radius.
+00019ad0: 6170 7065 6e64 286e 702e 6d65 616e 2866  append(np.mean(f
+00019ae0: 696c 7465 7265 645f 7661 6c75 6573 2929  iltered_values))
+00019af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019b00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019b20: 2e61 6c6c 5f76 6172 5f72 6164 6975 732e  .all_var_radius.
+00019b30: 6170 7065 6e64 286e 702e 7374 6428 6669  append(np.std(fi
+00019b40: 6c74 6572 6564 5f76 616c 7565 7329 290d  ltered_values)).
+00019b50: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019b60: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00019b70: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
+00019b80: 6428 6e70 2e6d 6561 6e28 616c 6c5f 7370  d(np.mean(all_sp
+00019b90: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
+00019ba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019bb0: 616c 6c5f 7661 725f 7370 6565 642e 6170  all_var_speed.ap
+00019bc0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+00019bd0: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00019be0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019bf0: 656c 662e 616c 6c5f 6d65 616e 5f61 6363  elf.all_mean_acc
+00019c00: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00019c10: 616c 6c5f 6163 6329 290d 0a20 2020 2020  all_acc))..     
+00019c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019c30: 656c 662e 616c 6c5f 7661 725f 6163 632e  elf.all_var_acc.
+00019c40: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00019c50: 6c5f 6163 6329 290d 0a0d 0a0d 0a0d 0a20  l_acc))........ 
+00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c70: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00019c80: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019c90: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+00019ca0: 616e 2861 6c6c 5f64 6972 6563 7469 6f6e  an(all_direction
+00019cb0: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00019cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cd0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00019ce0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00019cf0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+00019d00: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
+00019d10: 6861 6e67 6529 290d 0a0d 0a20 2020 2020  hange))....     
+00019d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019d30: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00019d40: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00019d50: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
+00019d60: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+00019d70: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+00019d80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019d90: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
+00019da0: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00019db0: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
+00019dc0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00019dd0: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
+00019de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019df0: 200d 0a20 2020 2020 2020 200d 0a64 6566   ..        ..def
+00019e00: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
+00019e10: 286d 6173 6b2c 2078 6361 6c69 6272 6174  (mask, xcalibrat
+00019e20: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
+00019e30: 6e2c 207a 6361 6c69 6272 6174 696f 6e29  n, zcalibration)
+00019e40: 3a0d 0a0d 0a20 2020 206e 6469 6d20 3d20  :....    ndim = 
+00019e50: 6c65 6e28 6d61 736b 2e73 6861 7065 290d  len(mask.shape).
+00019e60: 0a20 2020 2074 696d 6564 5f6d 6173 6b20  .    timed_mask 
+00019e70: 3d20 7b7d 0d0a 2020 2020 6d61 736b 203d  = {}..    mask =
+00019e80: 206d 6173 6b20 3e20 300d 0a20 2020 206d   mask > 0..    m
+00019e90: 6173 6b20 3d20 6d61 736b 2e61 7374 7970  ask = mask.astyp
+00019ea0: 6528 2775 696e 7438 2729 0d0a 2020 2020  e('uint8')..    
+00019eb0: 2320 5958 2073 6861 7065 6420 6f62 6a65  # YX shaped obje
+00019ec0: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00019ed0: 3d3d 2032 3a0d 0a20 2020 2020 2020 200d  == 2:..        .
+00019ee0: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
+00019ef0: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
+00019f00: 6965 7328 6d61 736b 290d 0a20 2020 2020  ies(mask)..     
+00019f10: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
+00019f20: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
+00019f30: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
+00019f40: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
+00019f50: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
+00019f60: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
+00019f70: 0d0a 2020 2020 2020 2020 7265 616c 5f69  ..        real_i
+00019f80: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
+00019f90: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
+00019fa0: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
+00019fb0: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
+00019fc0: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
+00019fd0: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+00019fe0: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
+00019ff0: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
+0001a000: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+0001a010: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+0001a020: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
+0001a030: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+0001a040: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+0001a050: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
+0001a060: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+0001a070: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
+0001a080: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
+0001a090: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
+0001a0a0: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
+0001a0b0: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
+0001a0c0: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
+0001a0d0: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
+0001a0e0: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
+0001a0f0: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
+0001a100: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
+0001a110: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
+0001a120: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
+0001a130: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
+0001a140: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
+0001a150: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
+0001a160: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
+0001a170: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
+0001a180: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
+0001a190: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
+0001a1a0: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
+0001a1b0: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
+0001a1c0: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
+0001a1d0: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
+0001a1e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a1f0: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
+0001a200: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
+0001a210: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
+0001a220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a230: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
+0001a240: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
+0001a250: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
+0001a260: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
+0001a270: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+0001a280: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
+0001a290: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
+0001a2a0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+0001a2b0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
+0001a2c0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
+0001a2d0: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
+0001a2e0: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
+0001a2f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+0001a300: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0001a310: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
+0001a320: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
+0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a340: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+0001a350: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
+0001a360: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
+0001a370: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001a380: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001a390: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+0001a3a0: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+0001a3b0: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
+0001a3c0: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+0001a3d0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
+0001a3e0: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
+0001a3f0: 6561 6c5f 696e 6469 6365 7329 0d0a 0d0a  eal_indices)....
+0001a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a410: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
+0001a420: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
+0001a430: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
+0001a440: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
+0001a450: 2020 0d0a 2020 2020 2320 545a 5958 2073    ..    # TZYX s
+0001a460: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
+0001a470: 2020 6966 206e 6469 6d20 3d3d 2034 3a0d    if ndim == 4:.
+0001a480: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0001a490: 4d61 6b69 6e67 206d 6173 6b20 696e 2034  Making mask in 4
+0001a4a0: 4427 290d 0a20 2020 2020 2020 2062 6f75  D')..        bou
+0001a4b0: 6e64 6172 7920 3d20 6e70 2e7a 6572 6f73  ndary = np.zeros
+0001a4c0: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
+0001a4d0: 6d61 736b 2e73 6861 7065 5b30 5d2c 206d  mask.shape[0], m
+0001a4e0: 6173 6b2e 7368 6170 655b 315d 2c20 6d61  ask.shape[1], ma
+0001a4f0: 736b 2e73 6861 7065 5b32 5d2c 206d 6173  sk.shape[2], mas
+0001a500: 6b2e 7368 6170 655b 335d 5d2c 2064 7479  k.shape[3]], dty
+0001a510: 7065 3d6e 702e 7569 6e74 380d 0a20 2020  pe=np.uint8..   
+0001a520: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001a530: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+0001a540: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
+0001a550: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
+0001a560: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
+0001a570: 6e64 6172 795b 692c 3a5d 203d 2066 696e  ndary[i,:] = fin
+0001a580: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
+0001a590: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
+0001a5a0: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+0001a5b0: 6f69 6420 3d20 636f 6d70 7574 655f 6365  oid = compute_ce
+0001a5c0: 6e74 726f 6964 2862 6f75 6e64 6172 795b  ntroid(boundary[
+0001a5d0: 692c 3a5d 2920 0d0a 2020 2020 2020 2020  i,:]) ..        
+0001a5e0: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+0001a5f0: 2e77 6865 7265 2862 6f75 6e64 6172 795b  .where(boundary[
+0001a600: 692c 3a5d 203e 2030 290d 0a20 2020 2020  i,:] > 0)..     
+0001a610: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
+0001a620: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
+0001a630: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
+0001a640: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
+0001a650: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
+0001a660: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001a670: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
+0001a680: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
+0001a690: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
+0001a6a0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0001a6b0: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+0001a6c0: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+0001a6d0: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
+0001a6e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+0001a6f0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+0001a700: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
+0001a710: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
+0001a720: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+0001a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a740: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+0001a750: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
+0001a760: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
+0001a770: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+0001a780: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
+0001a790: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+0001a7a0: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+0001a7b0: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+0001a7c0: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
+0001a7d0: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
+0001a7e0: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
+0001a7f0: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
+0001a800: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
+0001a810: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
+0001a820: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
+0001a830: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
+0001a840: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
+0001a850: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+0001a860: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
+0001a870: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
+0001a880: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
+0001a890: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
+0001a8a0: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
+0001a8b0: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
+0001a8c0: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
+0001a8d0: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
+0001a8e0: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
+0001a8f0: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
+0001a900: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
+0001a910: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
+0001a920: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
+0001a930: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
+0001a940: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
+0001a950: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
+0001a960: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
+0001a970: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
+0001a980: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
+0001a990: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
+0001a9a0: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
+0001a9b0: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
+0001a9c0: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
+0001a9d0: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
+0001a9e0: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
+0001a9f0: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
+0001aa00: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
+0001aa10: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
+0001aa20: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
+0001aa30: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
+0001aa40: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
+0001aa50: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
+0001aa60: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
+0001aa70: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
+0001aa80: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
+0001aa90: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
+0001aaa0: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
+0001aab0: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
+0001aac0: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
+0001aad0: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
+0001aae0: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
+0001aaf0: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
+0001ab00: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
+0001ab10: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
+0001ab20: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
+0001ab30: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001ab40: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
+0001ab50: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
+0001ab60: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
+0001ab70: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
+0001ab80: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
+0001ab90: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
+0001aba0: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
+0001abb0: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
+0001abc0: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001abd0: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
+0001abe0: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
+0001abf0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001ac00: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
+0001ac10: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
+0001ac20: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
+0001ac30: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
+0001ac40: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
+0001ac50: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
+0001ac60: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001ac70: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
+0001ac80: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
+0001ac90: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
+0001aca0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001acb0: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
+0001acc0: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
+0001acd0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001ace0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001acf0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001ad00: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
+0001ad10: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001ad20: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
+0001ad30: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
+0001ad40: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001ad50: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001ad60: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001ad70: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
+0001ad80: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
+0001ad90: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
+0001ada0: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
+0001adb0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
+0001adc0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
+0001add0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
+0001ade0: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
+0001adf0: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
+0001ae00: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
+0001ae10: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
+0001ae20: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0001ae30: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
+0001ae40: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
+0001ae50: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
+0001ae60: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
+0001ae70: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+0001ae80: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
+0001ae90: 6e73 6974 7922 5d5d 0d0a 2020 2020 2020  nsity"]]..      
+0001aea0: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
+0001aeb0: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001aec0: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
+0001aed0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+0001aee0: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
+0001aef0: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
+0001af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af10: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
+0001af20: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
+0001af30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001af40: 2020 2020 2020 2020 2020 2020 2020 7661                va
+0001af50: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
+0001af60: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001af70: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
+0001af80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001af90: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
+0001afa0: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
+0001afb0: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
+0001afc0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001afd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001afe0: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
+0001aff0: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
+0001b000: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
 0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b020: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
-0001b030: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
-0001b040: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-0001b050: 2229 2020 2020 2020 200d 0a0d 0a20 2020  ")       ....   
-0001b060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001b070: 7620 6e6f 7420 696e 2069 676e 6f72 655f  v not in ignore_
-0001b080: 7661 6c75 6573 3a0d 0a20 2020 2020 2020  values:..       
-0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b0b0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
-0001b0c0: 6573 5b76 5d20 3d20 7370 6f74 5f64 6174  es[v] = spot_dat
-0001b0d0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001b0e0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001b0f0: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-0001b100: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001b110: 735b 706f 7369 785d 203d 2072 6f75 6e64  s[posix] = round
-0001b120: 284c 6f63 6174 696f 6e58 2c33 290d 0a20  (LocationX,3).. 
-0001b130: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001b140: 5b70 6f73 6979 5d20 3d20 726f 756e 6428  [posiy] = round(
-0001b150: 4c6f 6361 7469 6f6e 592c 3329 0d0a 2020  LocationY,3)..  
-0001b160: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001b170: 706f 7369 7a5d 203d 2072 6f75 6e64 284c  posiz] = round(L
-0001b180: 6f63 6174 696f 6e5a 2c33 290d 0a20 2020  ocationZ,3)..   
-0001b190: 2020 2020 2041 6c6c 5661 6c75 6573 5b66       AllValues[f
-0001b1a0: 7261 6d65 5d20 3d20 726f 756e 6428 4c6f  rame] = round(Lo
-0001b1b0: 6361 7469 6f6e 542c 3329 0d0a 2020 2020  cationT,3)..    
-0001b1c0: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
-0001b1d0: 203d 205b 5d0d 0a20 2020 2020 2020 2041   = []..        A
-0001b1e0: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
-0001b1f0: 6e64 2841 7474 7269 6275 7465 426f 786e  nd(AttributeBoxn
-0001b200: 616d 6529 0d0a 2020 2020 2020 2020 666f  ame)..        fo
-0001b210: 7220 6174 7472 6962 7574 656e 616d 6520  r attributename 
-0001b220: 696e 2041 6c6c 5661 6c75 6573 2e6b 6579  in AllValues.key
-0001b230: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-0001b240: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
-0001b250: 2e61 7070 656e 6428 6174 7472 6962 7574  .append(attribut
-0001b260: 656e 616d 6529 2020 2020 0d0a 2020 2020  ename)    ..    
-0001b270: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001b280: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
-0001b290: 726e 2041 7474 7269 6275 7465 6964 732c  rn Attributeids,
-0001b2a0: 2041 6c6c 5661 6c75 6573 2020 2020 200d   AllValues     .
-0001b2b0: 0a20 2020 200d 0a64 6566 2067 6574 5f74  .    ..def get_t
-0001b2c0: 7261 636b 5f64 6174 6173 6574 2874 7261  rack_dataset(tra
-0001b2d0: 636b 5f64 6174 6173 6574 2c20 7472 6163  ck_dataset, trac
-0001b2e0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001b2f0: 6b65 7973 2c20 7472 6163 6b5f 616e 616c  keys, track_anal
-0001b300: 7973 6973 5f74 7261 636b 5f6b 6579 732c  ysis_track_keys,
-0001b310: 2054 7261 636b 4174 7472 6962 7574 6542   TrackAttributeB
-0001b320: 6f78 6e61 6d65 293a 0d0a 0d0a 2020 2020  oxname):....    
-0001b330: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
-0001b340: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001b350: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
-0001b360: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001b370: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
-0001b380: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
-0001b390: 7472 6163 6b5f 6461 7461 7365 745b 7472  track_dataset[tr
-0001b3a0: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
-0001b3b0: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001b3c0: 0d0a 2020 2020 2020 2020 416c 6c54 7261  ..        AllTra
-0001b3d0: 636b 5661 6c75 6573 5b74 7261 636b 5f69  ckValues[track_i
-0001b3e0: 645d 203d 2054 6964 0d0a 2020 2020 2020  d] = Tid..      
-0001b3f0: 0d0a 2020 2020 2020 2020 666f 7220 286b  ..        for (k
-0001b400: 2c20 7629 2069 6e20 7472 6163 6b5f 616e  , v) in track_an
-0001b410: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
-0001b420: 732e 6974 656d 7328 293a 0d0a 0d0a 2020  s.items():....  
-0001b430: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-0001b440: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
-0001b450: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-0001b460: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0001b470: 2020 2020 6d69 6e76 616c 203d 206d 696e      minval = min
-0001b480: 2878 290d 0a20 2020 2020 2020 2020 2020  (x)..           
-0001b490: 2020 2020 206d 6178 7661 6c20 3d20 6d61       maxval = ma
-0001b4a0: 7828 7829 0d0a 0d0a 2020 2020 2020 2020  x(x)....        
-0001b4b0: 2020 2020 2020 2020 6966 206d 696e 7661          if minva
-0001b4c0: 6c20 3e20 3020 616e 6420 6d61 7876 616c  l > 0 and maxval
-0001b4d0: 203c 3d20 313a 0d0a 0d0a 2020 2020 2020   <= 1:....      
-0001b4e0: 2020 2020 2020 2020 2020 2020 2020 7820                x 
-0001b4f0: 3d20 7820 2b20 310d 0a0d 0a20 2020 2020  = x + 1....     
-0001b500: 2020 2020 2020 2020 2020 2041 6c6c 5472             AllTr
-0001b510: 6163 6b56 616c 7565 735b 6b5d 203d 2072  ackValues[k] = r
-0001b520: 6f75 6e64 2878 2c20 3329 0d0a 0d0a 2020  ound(x, 3)....  
-0001b530: 2020 2020 2020 5472 6163 6b41 7474 7269        TrackAttri
-0001b540: 6275 7465 6964 7320 3d20 5b5d 0d0a 2020  buteids = []..  
-0001b550: 2020 2020 2020 5472 6163 6b41 7474 7269        TrackAttri
-0001b560: 6275 7465 6964 732e 6170 7065 6e64 2854  buteids.append(T
-0001b570: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
-0001b580: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
-0001b590: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
-0001b5a0: 2069 6e20 7472 6163 6b5f 616e 616c 7973   in track_analys
-0001b5b0: 6973 5f74 7261 636b 5f6b 6579 732e 6b65  is_track_keys.ke
-0001b5c0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0001b5d0: 2020 2054 7261 636b 4174 7472 6962 7574     TrackAttribut
-0001b5e0: 6569 6473 2e61 7070 656e 6428 6174 7472  eids.append(attr
-0001b5f0: 6962 7574 656e 616d 6529 2020 2020 0d0a  ibutename)    ..
-0001b600: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-0001b610: 7475 726e 2054 7261 636b 4174 7472 6962  turn TrackAttrib
-0001b620: 7574 6569 6473 2c20 416c 6c54 7261 636b  uteids, AllTrack
-0001b630: 5661 6c75 6573 0d0a 2020 2020 0d0a 6465  Values..    ..de
-0001b640: 6620 6765 745f 6564 6765 735f 6461 7461  f get_edges_data
-0001b650: 7365 7428 6564 6765 735f 6461 7461 7365  set(edges_datase
-0001b660: 742c 2065 6467 6573 5f64 6174 6173 6574  t, edges_dataset
-0001b670: 5f69 6e64 6578 2c20 7472 6163 6b5f 616e  _index, track_an
-0001b680: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001b690: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
-0001b6a0: 5f65 6467 6573 5f6b 6579 7329 3a0d 0a0d  _edges_keys):...
-0001b6b0: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
-0001b6c0: 7356 616c 7565 7320 3d20 7b7d 0d0a 2020  sValues = {}..  
-0001b6d0: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
-0001b6e0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001b6f0: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
-0001b700: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
-0001b710: 6964 203d 2065 6467 6573 5f64 6174 6173  id = edges_datas
-0001b720: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
-0001b730: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
-0001b740: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-0001b750: 6e70 2e77 6865 7265 2854 6964 203d 3d20  np.where(Tid == 
-0001b760: 3029 0d0a 2020 2020 2020 2020 6d61 7874  0)..        maxt
-0001b770: 7261 636b 5f69 6420 3d20 6d61 7828 5469  rack_id = max(Ti
-0001b780: 6429 0d0a 2020 2020 2020 2020 636f 6e64  d)..        cond
-0001b790: 6974 696f 6e5f 696e 6469 6365 7320 3d20  ition_indices = 
-0001b7a0: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
-0001b7b0: 6465 785b 696e 6469 6365 735d 0d0a 2020  dex[indices]..  
-0001b7c0: 2020 2020 2020 5469 645b 636f 6e64 6974        Tid[condit
-0001b7d0: 696f 6e5f 696e 6469 6365 735d 203d 206d  ion_indices] = m
-0001b7e0: 6178 7472 6163 6b5f 6964 202b 2031 0d0a  axtrack_id + 1..
-0001b7f0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
-0001b800: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
-0001b810: 203d 2054 6964 0d0a 0d0a 2020 2020 2020   = Tid....      
-0001b820: 2020 666f 7220 6b20 696e 2074 7261 636b    for k in track
-0001b830: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
-0001b840: 6b65 7973 2e76 616c 7565 7328 293a 0d0a  keys.values():..
-0001b850: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001b860: 206b 2021 3d20 7472 6163 6b5f 6964 3a0d   k != track_id:.
-0001b870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b880: 2078 203d 2065 6467 6573 5f64 6174 6173   x = edges_datas
-0001b890: 6574 5b6b 5d2e 6173 7479 7065 2822 666c  et[k].astype("fl
-0001b8a0: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
-0001b8b0: 2020 2020 2020 2020 2041 6c6c 4564 6765           AllEdge
-0001b8c0: 7356 616c 7565 735b 6b5d 203d 2078 2020  sValues[k] = x  
-0001b8d0: 200d 0a20 2020 2020 2020 2020 0d0a 2020   ..         ..  
-0001b8e0: 2020 2020 2020 7265 7475 726e 2041 6c6c        return All
-0001b8f0: 4564 6765 7356 616c 7565 7320 2020 0d0a  EdgesValues   ..
-0001b900: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
-0001b910: 2020 200d 0a64 6566 2073 6361 6c65 5f76     ..def scale_v
-0001b920: 616c 7565 2878 2c20 7363 616c 6520 3d20  alue(x, scale = 
-0001b930: 3235 3520 2a20 3235 3529 3a0d 0a0d 0a0d  255 * 255):.....
-0001b940: 0a20 2020 2020 7265 7475 726e 2078 202a  .     return x *
-0001b950: 2073 6361 6c65 2020 200d 0a20 2020 200d   scale   ..    .
-0001b960: 0a0d 0a0d 0a64 6566 2070 726f 625f 7369  .....def prob_si
-0001b970: 676d 6f69 6428 7829 3a0d 0a20 2020 2072  gmoid(x):..    r
-0001b980: 6574 7572 6e20 3120 2d20 6d61 7468 2e65  eturn 1 - math.e
-0001b990: 7870 282d 7829 0d0a 0d0a 0d0a 6465 6620  xp(-x)......def 
-0001b9a0: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
-0001b9b0: 6563 5f30 2c20 7665 635f 3129 3a0d 0a20  ec_0, vec_1):.. 
-0001b9c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001b9d0: 2076 6563 5f30 203d 2076 6563 5f30 202f   vec_0 = vec_0 /
-0001b9e0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0001b9f0: 7665 635f 3029 0d0a 2020 2020 2020 2020  vec_0)..        
-0001ba00: 7665 635f 3120 3d20 7665 635f 3120 2f20  vec_1 = vec_1 / 
-0001ba10: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
-0001ba20: 6563 5f31 290d 0a20 2020 2020 2020 2061  ec_1)..        a
-0001ba30: 6e67 6c65 203d 206e 702e 6172 6363 6f73  ngle = np.arccos
-0001ba40: 286e 702e 636c 6970 286e 702e 646f 7428  (np.clip(np.dot(
-0001ba50: 7665 635f 302c 2076 6563 5f31 292c 202d  vec_0, vec_1), -
-0001ba60: 312e 302c 2031 2e30 2929 0d0a 2020 2020  1.0, 1.0))..    
-0001ba70: 2020 2020 616e 676c 6520 3d20 616e 676c      angle = angl
-0001ba80: 6520 2a20 3138 3020 2f20 6e70 2e70 690d  e * 180 / np.pi.
-0001ba90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001baa0: 616e 676c 650d 0a20 2020 2020 0d0a 0d0a  angle..     ....
-0001bab0: 6465 6620 6576 616c 5f62 6f6f 6c28 7661  def eval_bool(va
-0001bac0: 6c75 6529 3a0d 0a20 2020 2020 2020 2020  lue):..         
-0001bad0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001bae0: 2020 2069 6620 7661 6c75 6520 203d 3d20     if value  == 
-0001baf0: 2754 7275 6527 3a20 0d0a 2020 2020 2020  'True': ..      
-0001bb00: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
-0001bb10: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
-0001bb20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001bb30: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
-0001bb40: 203d 2046 616c 7365 200d 0a0d 0a20 2020   = False ....   
-0001bb50: 2020 2020 2072 6574 7572 6e20 6469 765f       return div_
-0001bb60: 6b65 7920 2020 2020 2020 2020 2020 2020  key             
-0001bb70: 2020 200d 0a0d 0a64 6566 2063 6865 636b     ....def check
-0001bb80: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
-0001bb90: 286d 6173 6b2c 696d 6167 6529 3a0d 0a20  (mask,image):.. 
-0001bba0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001bbb0: 6966 206c 656e 286d 6173 6b2e 7368 6170  if len(mask.shap
-0001bbc0: 6529 203c 206c 656e 2869 6d61 6765 2e73  e) < len(image.s
-0001bbd0: 6861 7065 293a 0d0a 2020 2020 2020 2020  hape):..        
-0001bbe0: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
-0001bbf0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
-0001bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc10: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
-0001bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc30: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001bc40: 652e 7368 6170 655b 305d 2c0d 0a20 2020  e.shape[0],..   
-0001bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc60: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001bc70: 6765 2e73 6861 7065 5b31 5d2c 0d0a 2020  ge.shape[1],..  
-0001bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc90: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001bca0: 6167 652e 7368 6170 655b 325d 2c0d 0a20  age.shape[2],.. 
-0001bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bcd0: 6d61 6765 2e73 6861 7065 5b33 5d2c 0d0a  mage.shape[3],..
-0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcf0: 2020 2020 2020 2020 2020 2020 5d2c 2064              ], d
-0001bd00: 7479 7065 3d22 7569 6e74 3822 0d0a 2020  type="uint8"..  
-0001bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd20: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001bd30: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-0001bd40: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
-0001bd50: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
-0001bd60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001bd70: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-0001bd80: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
-0001bd90: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
-0001bda0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0001bdb0: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
-0001bdc0: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
-0001bdd0: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
-0001bde0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-0001bdf0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
-0001be00: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
-0001be10: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
-0001be20: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
-0001be30: 0a20 2020 2020 2020 0d0a                 .       ..
+0001b020: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
+0001b030: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
+0001b040: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
+0001b050: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
+0001b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b070: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
+0001b080: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001b090: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001b0a0: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
+0001b0b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b0c0: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
+0001b0d0: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
+0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001b100: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
+0001b110: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
+0001b120: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
+0001b130: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
+0001b140: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+0001b150: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
+0001b160: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
+0001b170: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
+0001b180: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001b190: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
+0001b1a0: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
+0001b1b0: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
+0001b1c0: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
+0001b1d0: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
+0001b1e0: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001b1f0: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
+0001b200: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
+0001b210: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001b220: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0001b230: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001b240: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
+0001b250: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
+0001b260: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
+0001b270: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
+0001b280: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
+0001b290: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
+0001b2a0: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
+0001b2b0: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
+0001b2c0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001b2d0: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+0001b2e0: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
+0001b2f0: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
+0001b300: 0d0a 2020 2020 0d0a 0d0a 6465 6620 6765  ..    ....def ge
+0001b310: 745f 7472 6163 6b5f 6461 7461 7365 7428  t_track_dataset(
+0001b320: 7472 6163 6b5f 6461 7461 7365 742c 2074  track_dataset, t
+0001b330: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001b340: 6f74 5f6b 6579 732c 2074 7261 636b 5f61  ot_keys, track_a
+0001b350: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001b360: 7973 2c20 5472 6163 6b41 7474 7269 6275  ys, TrackAttribu
+0001b370: 7465 426f 786e 616d 6529 3a0d 0a20 2020  teBoxname):..   
+0001b380: 2041 6c6c 5472 6163 6b56 616c 7565 7320   AllTrackValues 
+0001b390: 3d20 7b7d 0d0a 2020 2020 7472 6163 6b5f  = {}..    track_
+0001b3a0: 6964 203d 2074 7261 636b 5f61 6e61 6c79  id = track_analy
+0001b3b0: 7369 735f 7370 6f74 5f6b 6579 735b 2274  sis_spot_keys["t
+0001b3c0: 7261 636b 5f69 6422 5d0d 0a20 2020 2054  rack_id"]..    T
+0001b3d0: 6964 203d 2074 7261 636b 5f64 6174 6173  id = track_datas
+0001b3e0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
+0001b3f0: 7970 6528 2266 6c6f 6174 2229 0d0a 0d0a  ype("float")....
+0001b400: 2020 2020 416c 6c54 7261 636b 5661 6c75      AllTrackValu
+0001b410: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
+0001b420: 7d0d 0a20 2020 2041 6c6c 5472 6163 6b56  }..    AllTrackV
+0001b430: 616c 7565 735b 7472 6163 6b5f 6964 5d5b  alues[track_id][
+0001b440: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
+0001b450: 786e 616d 655d 203d 2054 6964 0d0a 0d0a  xname] = Tid....
+0001b460: 2020 2020 666f 7220 286b 2c20 7629 2069      for (k, v) i
+0001b470: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001b480: 5f74 7261 636b 5f6b 6579 732e 6974 656d  _track_keys.item
+0001b490: 7328 293a 0d0a 2020 2020 2020 2020 7820  s():..        x 
+0001b4a0: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
+0001b4b0: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
+0001b4c0: 2229 0d0a 2020 2020 2020 2020 6d69 6e76  ")..        minv
+0001b4d0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
+0001b4e0: 2020 2020 206d 6178 7661 6c20 3d20 6d61       maxval = ma
+0001b4f0: 7828 7829 0d0a 0d0a 2020 2020 2020 2020  x(x)....        
+0001b500: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
+0001b510: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
+0001b520: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+0001b530: 7820 2b20 310d 0a0d 0a20 2020 2020 2020  x + 1....       
+0001b540: 2041 6c6c 5472 6163 6b56 616c 7565 735b   AllTrackValues[
+0001b550: 7472 6163 6b5f 6964 5d5b 6b5d 203d 2072  track_id][k] = r
+0001b560: 6f75 6e64 2878 2c20 3329 0d0a 0d0a 2020  ound(x, 3)....  
+0001b570: 2020 5472 6163 6b41 7474 7269 6275 7465    TrackAttribute
+0001b580: 6964 7320 3d20 5b54 7261 636b 4174 7472  ids = [TrackAttr
+0001b590: 6962 7574 6542 6f78 6e61 6d65 5d20 2b20  ibuteBoxname] + 
+0001b5a0: 6c69 7374 2874 7261 636b 5f61 6e61 6c79  list(track_analy
+0001b5b0: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
+0001b5c0: 6579 7328 2929 0d0a 0d0a 2020 2020 7265  eys())....    re
+0001b5d0: 7475 726e 2054 7261 636b 4174 7472 6962  turn TrackAttrib
+0001b5e0: 7574 6569 6473 2c20 416c 6c54 7261 636b  uteids, AllTrack
+0001b5f0: 5661 6c75 6573 0d0a 2020 2020 0d0a 6465  Values..    ..de
+0001b600: 6620 6765 745f 6564 6765 735f 6461 7461  f get_edges_data
+0001b610: 7365 7428 6564 6765 735f 6461 7461 7365  set(edges_datase
+0001b620: 742c 2065 6467 6573 5f64 6174 6173 6574  t, edges_dataset
+0001b630: 5f69 6e64 6578 2c20 7472 6163 6b5f 616e  _index, track_an
+0001b640: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001b650: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001b660: 5f65 6467 6573 5f6b 6579 7329 3a0d 0a0d  _edges_keys):...
+0001b670: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
+0001b680: 7356 616c 7565 7320 3d20 7b7d 0d0a 2020  sValues = {}..  
+0001b690: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+0001b6a0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001b6b0: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+0001b6c0: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
+0001b6d0: 6964 203d 2065 6467 6573 5f64 6174 6173  id = edges_datas
+0001b6e0: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
+0001b6f0: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001b700: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
+0001b710: 6e70 2e77 6865 7265 2854 6964 203d 3d20  np.where(Tid == 
+0001b720: 3029 0d0a 2020 2020 2020 2020 6d61 7874  0)..        maxt
+0001b730: 7261 636b 5f69 6420 3d20 6d61 7828 5469  rack_id = max(Ti
+0001b740: 6429 0d0a 2020 2020 2020 2020 636f 6e64  d)..        cond
+0001b750: 6974 696f 6e5f 696e 6469 6365 7320 3d20  ition_indices = 
+0001b760: 6564 6765 735f 6461 7461 7365 745f 696e  edges_dataset_in
+0001b770: 6465 785b 696e 6469 6365 735d 0d0a 2020  dex[indices]..  
+0001b780: 2020 2020 2020 5469 645b 636f 6e64 6974        Tid[condit
+0001b790: 696f 6e5f 696e 6469 6365 735d 203d 206d  ion_indices] = m
+0001b7a0: 6178 7472 6163 6b5f 6964 202b 2031 0d0a  axtrack_id + 1..
+0001b7b0: 2020 2020 2020 2020 416c 6c45 6467 6573          AllEdges
+0001b7c0: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
+0001b7d0: 203d 2054 6964 0d0a 0d0a 2020 2020 2020   = Tid....      
+0001b7e0: 2020 666f 7220 6b20 696e 2074 7261 636b    for k in track
+0001b7f0: 5f61 6e61 6c79 7369 735f 6564 6765 735f  _analysis_edges_
+0001b800: 6b65 7973 2e76 616c 7565 7328 293a 0d0a  keys.values():..
+0001b810: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001b820: 206b 2021 3d20 7472 6163 6b5f 6964 3a0d   k != track_id:.
+0001b830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b840: 2078 203d 2065 6467 6573 5f64 6174 6173   x = edges_datas
+0001b850: 6574 5b6b 5d2e 6173 7479 7065 2822 666c  et[k].astype("fl
+0001b860: 6f61 7422 290d 0a0d 0a20 2020 2020 2020  oat")....       
+0001b870: 2020 2020 2020 2020 2041 6c6c 4564 6765           AllEdge
+0001b880: 7356 616c 7565 735b 6b5d 203d 2078 2020  sValues[k] = x  
+0001b890: 200d 0a20 2020 2020 2020 2020 0d0a 2020   ..         ..  
+0001b8a0: 2020 2020 2020 7265 7475 726e 2041 6c6c        return All
+0001b8b0: 4564 6765 7356 616c 7565 7320 2020 0d0a  EdgesValues   ..
+0001b8c0: 2020 2020 0d0a 2020 2020 2020 200d 0a20      ..       .. 
+0001b8d0: 2020 200d 0a64 6566 2073 6361 6c65 5f76     ..def scale_v
+0001b8e0: 616c 7565 2878 2c20 7363 616c 6520 3d20  alue(x, scale = 
+0001b8f0: 3235 3520 2a20 3235 3529 3a0d 0a0d 0a0d  255 * 255):.....
+0001b900: 0a20 2020 2020 7265 7475 726e 2078 202a  .     return x *
+0001b910: 2073 6361 6c65 2020 200d 0a20 2020 200d   scale   ..    .
+0001b920: 0a0d 0a0d 0a64 6566 2070 726f 625f 7369  .....def prob_si
+0001b930: 676d 6f69 6428 7829 3a0d 0a20 2020 2072  gmoid(x):..    r
+0001b940: 6574 7572 6e20 3120 2d20 6d61 7468 2e65  eturn 1 - math.e
+0001b950: 7870 282d 7829 0d0a 0d0a 0d0a 6465 6620  xp(-x)......def 
+0001b960: 616e 6775 6c61 725f 6368 616e 6765 2876  angular_change(v
+0001b970: 6563 5f30 2c20 7665 635f 3129 3a0d 0a20  ec_0, vec_1):.. 
+0001b980: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001b990: 2076 6563 5f30 203d 2076 6563 5f30 202f   vec_0 = vec_0 /
+0001b9a0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0001b9b0: 7665 635f 3029 0d0a 2020 2020 2020 2020  vec_0)..        
+0001b9c0: 7665 635f 3120 3d20 7665 635f 3120 2f20  vec_1 = vec_1 / 
+0001b9d0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2876  np.linalg.norm(v
+0001b9e0: 6563 5f31 290d 0a20 2020 2020 2020 2061  ec_1)..        a
+0001b9f0: 6e67 6c65 203d 206e 702e 6172 6363 6f73  ngle = np.arccos
+0001ba00: 286e 702e 636c 6970 286e 702e 646f 7428  (np.clip(np.dot(
+0001ba10: 7665 635f 302c 2076 6563 5f31 292c 202d  vec_0, vec_1), -
+0001ba20: 312e 302c 2031 2e30 2929 0d0a 2020 2020  1.0, 1.0))..    
+0001ba30: 2020 2020 616e 676c 6520 3d20 616e 676c      angle = angl
+0001ba40: 6520 2a20 3138 3020 2f20 6e70 2e70 690d  e * 180 / np.pi.
+0001ba50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001ba60: 616e 676c 650d 0a20 2020 2020 0d0a 0d0a  angle..     ....
+0001ba70: 6465 6620 6576 616c 5f62 6f6f 6c28 7661  def eval_bool(va
+0001ba80: 6c75 6529 3a0d 0a20 2020 2020 2020 2020  lue):..         
+0001ba90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001baa0: 2020 2069 6620 7661 6c75 6520 203d 3d20     if value  == 
+0001bab0: 2754 7275 6527 3a20 0d0a 2020 2020 2020  'True': ..      
+0001bac0: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
+0001bad0: 7920 3d20 5472 7565 0d0a 2020 2020 2020  y = True..      
+0001bae0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0001baf0: 2020 2020 2020 2020 2064 6976 5f6b 6579           div_key
+0001bb00: 203d 2046 616c 7365 200d 0a0d 0a20 2020   = False ....   
+0001bb10: 2020 2020 2072 6574 7572 6e20 6469 765f       return div_
+0001bb20: 6b65 7920 2020 2020 2020 2020 2020 2020  key             
+0001bb30: 2020 200d 0a0d 0a64 6566 2063 6865 636b     ....def check
+0001bb40: 5f61 6e64 5f75 7064 6174 655f 6d61 736b  _and_update_mask
+0001bb50: 286d 6173 6b2c 696d 6167 6529 3a0d 0a20  (mask,image):.. 
+0001bb60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001bb70: 6966 206c 656e 286d 6173 6b2e 7368 6170  if len(mask.shap
+0001bb80: 6529 203c 206c 656e 2869 6d61 6765 2e73  e) < len(image.s
+0001bb90: 6861 7065 293a 0d0a 2020 2020 2020 2020  hape):..        
+0001bba0: 2020 2020 7570 6461 7465 5f6d 6173 6b20      update_mask 
+0001bbb0: 3d20 6e70 2e7a 6572 6f73 280d 0a20 2020  = np.zeros(..   
+0001bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbd0: 2020 2020 2020 2020 205b 0d0a 2020 2020           [..    
+0001bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbf0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001bc00: 652e 7368 6170 655b 305d 2c0d 0a20 2020  e.shape[0],..   
+0001bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc20: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001bc30: 6765 2e73 6861 7065 5b31 5d2c 0d0a 2020  ge.shape[1],..  
+0001bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc50: 2020 2020 2020 2020 2020 2020 2020 696d                im
+0001bc60: 6167 652e 7368 6170 655b 325d 2c0d 0a20  age.shape[2],.. 
+0001bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001bc90: 6d61 6765 2e73 6861 7065 5b33 5d2c 0d0a  mage.shape[3],..
+0001bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcb0: 2020 2020 2020 2020 2020 2020 5d2c 2064              ], d
+0001bcc0: 7479 7065 3d22 7569 6e74 3822 0d0a 2020  type="uint8"..  
+0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bce0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001bcf0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0001bd00: 6e67 6528 302c 2075 7064 6174 655f 6d61  nge(0, update_ma
+0001bd10: 736b 2e73 6861 7065 5b30 5d29 3a0d 0a20  sk.shape[0]):.. 
+0001bd20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001bd30: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
+0001bd40: 2075 7064 6174 655f 6d61 736b 2e73 6861   update_mask.sha
+0001bd50: 7065 5b31 5d29 3a0d 0a0d 0a20 2020 2020  pe[1]):....     
+0001bd60: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0001bd70: 7064 6174 655f 6d61 736b 5b69 2c20 6a2c  pdate_mask[i, j,
+0001bd80: 203a 2c20 3a5d 203d 206d 6173 6b5b 692c   :, :] = mask[i,
+0001bd90: 203a 2c20 3a5d 0d0a 2020 2020 2020 2020   :, :]..        
+0001bda0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001bdb0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
+0001bdc0: 736b 203d 206d 6173 6b0d 0a0d 0a20 2020  sk = mask....   
+0001bdd0: 2020 2020 2072 6574 7572 6e20 7570 6461       return upda
+0001bde0: 7465 5f6d 6173 6b20 2020 2020 2020 200d  te_mask        .
+0001bdf0: 0a20 2020 2020 2020 0d0a                 .       ..
```

### Comparing `napatrackmater-3.9.2/napatrackmater/Trackvector.py` & `napatrackmater-3.9.3/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/__init__.py` & `napatrackmater-3.9.3/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/clustering.py` & `napatrackmater-3.9.3/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.9.3/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/fate_mapping.py` & `napatrackmater-3.9.3/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater/pretrained.py` & `napatrackmater-3.9.3/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.9.3/napatrackmater.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.9.2
+Version: 3.9.3
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.9.2/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.9.3/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.9.2/setup.py` & `napatrackmater-3.9.3/setup.py`

 * *Files identical despite different names*

