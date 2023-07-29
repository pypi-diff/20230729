# Comparing `tmp/freq_mob-0.12.tar.gz` & `tmp/freq_mob-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freq_mob-0.12.tar", last modified: Fri Jul 28 06:45:00 2023, max compression
+gzip compressed data, was "freq_mob-0.13.tar", last modified: Sat Jul 29 06:14:41 2023, max compression
```

## Comparing `freq_mob-0.12.tar` & `freq_mob-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-28 06:45:00.117485 freq_mob-0.12/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 freq_mob-0.12/LICENSE.txt
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1939 2023-07-28 06:45:00.117485 freq_mob-0.12/PKG-INFO
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1515 2023-07-28 06:39:41.000000 freq_mob-0.12/README.md
-drwxr-xr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-28 06:45:00.086010 freq_mob-0.12/freq_mob/
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       69 2023-07-04 21:48:53.000000 freq_mob-0.12/freq_mob/__init__.py
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17366 2023-07-28 06:42:59.000000 freq_mob-0.12/freq_mob/freq_mob.py
-drwxr-xr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-28 06:45:00.112927 freq_mob-0.12/freq_mob.egg-info/
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1939 2023-07-28 06:45:00.000000 freq_mob-0.12/freq_mob.egg-info/PKG-INFO
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-28 06:45:00.000000 freq_mob-0.12/freq_mob.egg-info/SOURCES.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-28 06:45:00.000000 freq_mob-0.12/freq_mob.egg-info/dependency_links.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       55 2023-07-28 06:45:00.000000 freq_mob-0.12/freq_mob.egg-info/requires.txt
--rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-28 06:45:00.000000 freq_mob-0.12/freq_mob.egg-info/top_level.txt
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-28 06:45:00.117485 freq_mob-0.12/setup.cfg
--rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      716 2023-07-28 06:40:07.000000 freq_mob-0.12/setup.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 06:14:41.499529 freq_mob-0.13/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1073 2023-07-28 04:54:22.000000 freq_mob-0.13/LICENSE.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1939 2023-07-29 06:14:41.487462 freq_mob-0.13/PKG-INFO
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)     1515 2023-07-28 06:39:41.000000 freq_mob-0.13/README.md
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 06:14:41.462627 freq_mob-0.13/freq_mob/
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)       69 2023-07-04 21:48:53.000000 freq_mob-0.13/freq_mob/__init__.py
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)    17348 2023-07-29 06:13:35.000000 freq_mob-0.13/freq_mob/freq_mob.py
+drwxrwxr-x   0 liuwensui  (1000) liuwensui  (1000)        0 2023-07-29 06:14:41.485492 freq_mob-0.13/freq_mob.egg-info/
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)     1939 2023-07-29 06:14:41.000000 freq_mob-0.13/freq_mob.egg-info/PKG-INFO
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)      231 2023-07-29 06:14:41.000000 freq_mob-0.13/freq_mob.egg-info/SOURCES.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        1 2023-07-29 06:14:41.000000 freq_mob-0.13/freq_mob.egg-info/dependency_links.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       46 2023-07-29 06:14:41.000000 freq_mob-0.13/freq_mob.egg-info/requires.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)        9 2023-07-29 06:14:41.000000 freq_mob-0.13/freq_mob.egg-info/top_level.txt
+-rw-rw-r--   0 liuwensui  (1000) liuwensui  (1000)       38 2023-07-29 06:14:41.499529 freq_mob-0.13/setup.cfg
+-rw-r--r--   0 liuwensui  (1000) liuwensui  (1000)      704 2023-07-29 06:10:58.000000 freq_mob-0.13/setup.py
```

### Comparing `freq_mob-0.12/LICENSE.txt` & `freq_mob-0.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `freq_mob-0.12/PKG-INFO` & `freq_mob-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freq_mob
-Version: 0.12
+Version: 0.13
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `freq_mob-0.12/README.md` & `freq_mob-0.13/README.md`

 * *Files identical despite different names*

### Comparing `freq_mob-0.12/freq_mob/freq_mob.py` & `freq_mob-0.13/freq_mob/freq_mob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # freq_mob/freq_mob.py
-# version 0.12, 07/28/2023
-# import freq_mob
+# version 0.13, 07/29/2023
 
 import tabulate, numpy, cytoolz, operator
 from scipy.stats import spearmanr
 from sklearn.isotonic import IsotonicRegression as isoreg
 from sklearn.cluster import KMeans as kmeans
 from sklearn import metrics 
 from lightgbm import LGBMRegressor as gbmreg
 
+
 ########## 01. qcut() ##########
 
 def qcut(x, n):
   """
   It is an utility function to discretizes a numeric vector into n pieces based on quantiles.
   Parameters:
     x : A numeric vector.
@@ -522,8 +522,7 @@
          if numpy.abs(round(l[3], 8)) == 1 and round(l[1], 8) > 0][0]
 
   _l4 = sorted(*[l[1] for l in _l1 if l[0] == _l3], key = lambda x: x["ysum"] / x["freq"])
 
   _l5 = add_miss(_data, _l4)
 
   return({"cut": _l3, "tbl": gen_rule(gen_newx(_l5), _l3)})
-
```

### Comparing `freq_mob-0.12/freq_mob.egg-info/PKG-INFO` & `freq_mob-0.13/freq_mob.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freq-mob
-Version: 0.12
+Version: 0.13
 Summary: Monotonic Optimal Binning for Frequency Models
 Home-page: https://github.com/statcompute/freq_mob
 Author: WenSui Liu
 Author-email: liuwensui@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `freq_mob-0.12/setup.py` & `freq_mob-0.13/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
  
 with open("README.md", "r") as fh:
   long_description = fh.read()
  
 setuptools.setup(
   name = "freq_mob",
-  version = "0.12",
+  version = "0.13",
   author = "WenSui Liu",
   author_email = "liuwensui@gmail.com",
   description = "Monotonic Optimal Binning for Frequency Models",
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = "https://github.com/statcompute/freq_mob",
   packages = setuptools.find_packages(),
-  install_requires = ['numpy', 'scipy', 'sklearn', 'lightgbm', 'tabulate', 'cytoolz', 'operator'], 
+  install_requires = ['numpy', 'scipy', 'sklearn', 'lightgbm', 'tabulate', 'cytoolz'], 
   classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
 )
```

