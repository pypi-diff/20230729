# Comparing `tmp/curvit-1.6.8.tar.gz` & `tmp/curvit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.6.8.tar", last modified: Mon May 29 13:11:43 2023, max compression
+gzip compressed data, was "curvit-1.7.0.tar", last modified: Sat Jul 29 18:55:11 2023, max compression
```

## Comparing `curvit-1.6.8.tar` & `curvit-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.678469 curvit-1.6.8/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.8/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-29 13:11:43.678469 curvit-1.6.8/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.8/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.676469 curvit-1.6.8/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.6.8/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.8/curvit/check_curvit_variability_V.0.4.py
--rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    76303 2023-05-29 13:07:17.000000 curvit-1.6.8/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.6.8/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.6.8/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.677469 curvit-1.6.8/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-05-29 13:11:43.678469 curvit-1.6.8/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      847 2023-05-29 13:10:04.000000 curvit-1.6.8/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-07-29 18:55:11.756717 curvit-1.7.0/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.7.0/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-07-29 18:55:11.756717 curvit-1.7.0/PKG-INFO
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.7.0/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-07-29 18:55:11.754717 curvit-1.7.0/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.7.0/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.7.0/curvit/check_curvit_variability_V.0.4.py
+-rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    77830 2023-07-29 18:37:49.000000 curvit-1.7.0/curvit/curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.7.0/curvit/profile_curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.7.0/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-07-29 18:55:11.755717 curvit-1.7.0/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-07-29 18:55:11.000000 curvit-1.7.0/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-07-29 18:55:11.000000 curvit-1.7.0/curvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-07-29 18:55:11.000000 curvit-1.7.0/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2023-07-29 18:55:11.000000 curvit-1.7.0/curvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-07-29 18:55:11.000000 curvit-1.7.0/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-07-29 18:55:11.756717 curvit-1.7.0/setup.cfg
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      847 2023-07-29 18:41:48.000000 curvit-1.7.0/setup.py
```

### Comparing `curvit-1.6.8/LICENSE` & `curvit-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.6.8/PKG-INFO` & `curvit-1.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.8
+Version: 1.7.0
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.8 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.7.0 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.8/README.md` & `curvit-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `curvit-1.6.8/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.7.0/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.8/curvit/curvit.py` & `curvit-1.7.0/curvit/curvit.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 """The following parameters determines whether corrections are
 applied to the CPF. They are aperture-correction and
 saturation-correction."""
 aperture_correction = None  # valid inputs are None / 'fuv' / 'nuv'.
 saturation_correction = False  # True or False.
-
+ZEF_correction_factor = 1  # 1 when no frames are present with zero events.
 
 # Following parameters need not be changed (unless you want to).
 whole_figure_resolution = 256  # resolution of full figure.
 sub_fig_size = 40  # size of sub figure.
 fontsize = 9  # fontsize for plots.
 
 # Encircled energy data (https://doi.org/10.3847/1538-3881/ab72a3).
@@ -270,15 +270,17 @@
         events_list = events_list[:-5]
     if events_list[-8:] == ".fits.gz":
         events_list = events_list[:-8]
     return events_list
 
 
 # To automatically choose background region.
-def auto_bg(fx, fy, time, photons, radius, framecount_per_sec, sky_radius):
+def auto_bg(
+    fx, fy, time, photons, radius, framecount_per_sec, sky_radius, ZEF_correction_factor
+):
     weights = photons / framecount_per_sec
     bins = np.arange(0, 4801, 16)
     lowres_counts, lowres_xedges, lowres_yedges = np.histogram2d(
         fx, fy, bins=(bins, bins), weights=weights
     )
     lowres_xcentres = (lowres_xedges[:-1] + lowres_xedges[1:]) / 2.0
     lowres_ycentres = (lowres_yedges[:-1] + lowres_yedges[1:]) / 2.0
@@ -299,15 +301,24 @@
 
     bg_CPS_sample = []
     bg_CPS_e_sample = []
     sample_size = 100
     for d in range(sample_size):
         r_count, x_bg, y_bg = random.choice(polished_array[bg_mask])
         bg_CPS, bg_CPS_e = bg_estimate(
-            fx, fy, time, photons, framecount_per_sec, radius, x_bg, y_bg, sky_radius
+            fx,
+            fy,
+            time,
+            photons,
+            framecount_per_sec,
+            radius,
+            x_bg,
+            y_bg,
+            sky_radius,
+            ZEF_correction_factor,
         )
         bg_CPS_sample.append(bg_CPS)
         bg_CPS_e_sample.append(bg_CPS_e)
 
     bg_CPS_sample = np.array(bg_CPS_sample)
     bg_CPS_e_sample = np.array(bg_CPS_e_sample)
     bg_CPS_mask = sigma_clip(bg_CPS_sample, sigma=3, maxiters=5)
@@ -315,30 +326,39 @@
     bg_CPS = np.mean(bg_CPS_sample[bg_CPS_mask])
     bg_CPS_e = np.mean(bg_CPS_e_sample[bg_CPS_mask])
     return lowres_counts, bg_CPS, bg_CPS_e
 
 
 # To estimate background CPS.
 def bg_estimate(
-    fx, fy, time, photons, framecount_per_sec, radius, x_bg, y_bg, sky_radius
+    fx,
+    fy,
+    time,
+    photons,
+    framecount_per_sec,
+    radius,
+    x_bg,
+    y_bg,
+    sky_radius,
+    ZEF_correction_factor,
 ):
     weights = photons / framecount_per_sec
     mask = ((fx - x_bg) ** 2 + (fy - y_bg) ** 2) <= sky_radius**2
     T = time[mask]
     W = weights[mask]
 
     if len(T) != 0:
         scaled_events = (np.sum(W) * radius**2) / float(sky_radius**2)
         scaled_events_e = (np.sqrt(len(T)) * radius**2) / float(sky_radius**2)
     else:
         scaled_events = 0
         scaled_events_e = 0
 
     unique_time = np.unique(time)
-    Number_of_frames = float(len(unique_time))
+    Number_of_frames = ZEF_correction_factor * len(unique_time)
     bg_CPS = (scaled_events * framecount_per_sec) / Number_of_frames
     bg_CPS_e = (scaled_events_e * framecount_per_sec) / Number_of_frames
     return bg_CPS, bg_CPS_e
 
 
 # To create subset images.
 def create_sub_image(
@@ -484,17 +504,19 @@
     mcounts,
     frames_in_bin,
     bg_CPS,
     bg_CPS_e,
     weighted_mcounts,
     saturation_correction,
     aperture_correction,
+    ZEF_correction_factor,
     radius,
     framecount_per_sec,
 ):
+    frames_in_bin = ZEF_correction_factor * frames_in_bin
     if saturation_correction is True:
         if aperture_correction is None:
             raise ValueError(
                 "If saturation_correction parameter is True, "
                 "then aperture_correction parameter should not be None!"
             )
 
@@ -539,14 +561,15 @@
     framecount_per_sec=framecount_per_sec,
     background=background,
     sky_radius=sky_radius,
     x_bg=x_bg,
     y_bg=y_bg,
     aperture_correction=aperture_correction,
     saturation_correction=saturation_correction,
+    ZEF_correction_factor=ZEF_correction_factor,
     whole_figure_resolution=whole_figure_resolution,
     sub_fig_size=sub_fig_size,
     fontsize=fontsize,
 ):
     """Automatically detect sources amd create light curves.
 
     Parameters
@@ -630,14 +653,18 @@
 
     saturation_correction : bool, optional
         If `True`, saturation correction is applied.
         The default value is `False`.
         Note that aperture correction should be applied if you apply
         saturation correction.
 
+    ZEF_correction_factor : float, optional
+        To apply the correction for zero event frames.
+        The default value is 1 (no correction).
+
     Note
     ----
     It is essential to set the correct value of the framerate.
     Most UVIT observations are carried out in 512 x 512 window mode.
 
     Example
     --------
@@ -699,15 +726,22 @@
     np.savetxt(coo_file, uA, fmt="%4.2f\t%4.2f")
     print("\nDetected source coordinates saved in file:\n* {}".format(coo_file))
 
     # To automatically choose background region.
     plt.figure(figsize=(10.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
-            fx, fy, time, photons, radius, framecount_per_sec, sky_radius
+            fx,
+            fy,
+            time,
+            photons,
+            radius,
+            framecount_per_sec,
+            sky_radius,
+            ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
 
     plt.tick_params(axis="both", labelsize=fontsize)
@@ -747,14 +781,15 @@
                 time,
                 photons,
                 framecount_per_sec,
                 radius,
                 x_bg,
                 y_bg,
                 sky_radius,
+                ZEF_correction_factor,
             )
             bg_png = create_sub_image(
                 x_bg,
                 y_bg,
                 sub_fig_size,
                 sky_radius,
                 "background_",
@@ -838,14 +873,15 @@
             mcounts,
             frames_in_bin,
             bg_CPS,
             bg_CPS_e,
             weighted_mcounts,
             saturation_correction,
             aperture_correction,
+            ZEF_correction_factor,
             radius,
             framecount_per_sec,
         )
 
         CPS = CPF * framecount_per_sec
         CPS_err = CPF_err * framecount_per_sec
 
@@ -885,14 +921,15 @@
     framecount_per_sec=framecount_per_sec,
     background=background,
     sky_radius=sky_radius,
     x_bg=x_bg,
     y_bg=y_bg,
     aperture_correction=aperture_correction,
     saturation_correction=saturation_correction,
+    ZEF_correction_factor=ZEF_correction_factor,
     whole_figure_resolution=whole_figure_resolution,
     sub_fig_size=sub_fig_size,
     fontsize=fontsize,
 ):
     """Create light curve for a source.
 
     Parameters
@@ -967,14 +1004,18 @@
 
     saturation_correction : bool, optional
         If `True`, saturation correction is applied.
         The default value is `False`.
         Note that aperture correction should be applied if you apply
         saturation correction.
 
+    ZEF_correction_factor : float, optional
+        To apply the correction for zero event frames.
+        The default value is 1 (no correction).
+
     Note
     ----
     It is essential to set the correct value of the framerate.
     Most UVIT observations are carried out in 512 x 512 window mode.
 
     Example
     --------
@@ -1025,15 +1066,22 @@
     path_to_events_list, events_list = ntpath.split(events_list)
     events_list = modify_string(events_list)
 
     # To automatically choose background region.
     plt.figure(figsize=(10.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
-            fx, fy, time, photons, radius, framecount_per_sec, sky_radius
+            fx,
+            fy,
+            time,
+            photons,
+            radius,
+            framecount_per_sec,
+            sky_radius,
+            ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
 
     plt.tick_params(axis="both", labelsize=fontsize)
@@ -1082,14 +1130,15 @@
                 time,
                 photons,
                 framecount_per_sec,
                 radius,
                 x_bg,
                 y_bg,
                 sky_radius,
+                ZEF_correction_factor,
             )
             bg_png = create_sub_image(
                 x_bg,
                 y_bg,
                 sub_fig_size,
                 sky_radius,
                 "background_",
@@ -1163,14 +1212,15 @@
         mcounts,
         frames_in_bin,
         bg_CPS,
         bg_CPS_e,
         weighted_mcounts,
         saturation_correction,
         aperture_correction,
+        ZEF_correction_factor,
         radius,
         framecount_per_sec,
     )
 
     CPS = CPF * framecount_per_sec
     CPS_err = CPF_err * framecount_per_sec
 
@@ -1213,14 +1263,15 @@
     framecount_per_sec=framecount_per_sec,
     background=background,
     sky_radius=sky_radius,
     x_bg=x_bg,
     y_bg=y_bg,
     aperture_correction=aperture_correction,
     saturation_correction=saturation_correction,
+    ZEF_correction_factor=ZEF_correction_factor,
     whole_figure_resolution=whole_figure_resolution,
     sub_fig_size=sub_fig_size,
     fontsize=fontsize,
 ):
     """
     Create a light curve for a source, generating one data point per orbit.
     This function works best with the combined events list produced using
@@ -1298,14 +1349,18 @@
 
     saturation_correction : bool, optional
         If `True`, saturation correction is applied.
         The default value is `False`.
         Note that aperture correction should be applied if you apply
         saturation correction.
 
+    ZEF_correction_factor : float, optional
+        To apply the correction for zero event frames.
+        The default value is 1 (no correction).
+
     Note
     ----
     It is essential to set the correct value of the framerate.
     Most UVIT observations are carried out in 512 x 512 window mode.
 
     Example
     --------
@@ -1354,15 +1409,22 @@
     path_to_events_list, events_list = ntpath.split(events_list)
     events_list = modify_string(events_list)
 
     # To automatically choose background region.
     plt.figure(figsize=(10.5, 10))
     if background == "auto":
         lowres_counts, bg_CPS, bg_CPS_e = auto_bg(
-            fx, fy, time, photons, radius, framecount_per_sec, sky_radius
+            fx,
+            fy,
+            time,
+            photons,
+            radius,
+            framecount_per_sec,
+            sky_radius,
+            ZEF_correction_factor,
         )
 
     # To create a quick look figure marking sources and background.
     bins = np.arange(0, 4801, 4096 / whole_figure_resolution)
     plt.hist2d(fx, fy, bins=(bins, bins), weights=weights, norm=LogNorm())
 
     plt.tick_params(axis="both", labelsize=fontsize)
@@ -1411,14 +1473,15 @@
                 time,
                 photons,
                 framecount_per_sec,
                 radius,
                 x_bg,
                 y_bg,
                 sky_radius,
+                ZEF_correction_factor,
             )
             bg_png = create_sub_image(
                 x_bg,
                 y_bg,
                 sub_fig_size,
                 sky_radius,
                 "background_",
@@ -1505,14 +1568,15 @@
         mcounts,
         frames_in_bin,
         bg_CPS,
         bg_CPS_e,
         weighted_mcounts,
         saturation_correction,
         aperture_correction,
+        ZEF_correction_factor,
         radius,
         framecount_per_sec,
     )
 
     CPS = CPF * framecount_per_sec
     CPS_err = CPF_err * framecount_per_sec
```

### Comparing `curvit-1.6.8/curvit/test_curvit.py` & `curvit-1.7.0/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.8/curvit.egg-info/PKG-INFO` & `curvit-1.7.0/curvit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.8
+Version: 1.7.0
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.8 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.7.0 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.8/setup.py` & `curvit-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit",
-    version="1.6.8",
+    version="1.7.0",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```

