# Comparing `tmp/scorecardpy-0.1.9.6.tar.gz` & `tmp/scorecardpy-0.1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecardpy-0.1.9.6.tar", last modified: Mon May 22 15:18:07 2023, max compression
+gzip compressed data, was "scorecardpy-0.1.9.7.tar", last modified: Sat Jul 29 15:22:00 2023, max compression
```

## Comparing `scorecardpy-0.1.9.6.tar` & `scorecardpy-0.1.9.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 15:18:07.373690 scorecardpy-0.1.9.6/
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     1067 2018-04-24 03:25:44.000000 scorecardpy-0.1.9.6/LICENSE
--rwxr-xr-x   0 shichenxie   (501) staff       (20)      128 2018-04-24 03:52:54.000000 scorecardpy-0.1.9.6/MANIFEST.in
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     4638 2023-05-22 14:51:54.000000 scorecardpy-0.1.9.6/NEWS.md
--rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-05-22 15:18:07.373517 scorecardpy-0.1.9.6/PKG-INFO
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     3285 2020-02-24 13:15:32.000000 scorecardpy-0.1.9.6/README.md
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 15:18:07.370446 scorecardpy-0.1.9.6/scorecardpy/
--rwxr-xr-x   0 shichenxie   (501) staff       (20)      738 2023-05-22 15:17:47.000000 scorecardpy-0.1.9.6/scorecardpy/__init__.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     8108 2023-05-22 15:09:13.000000 scorecardpy-0.1.9.6/scorecardpy/condition_fun.py
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 15:18:07.372108 scorecardpy-0.1.9.6/scorecardpy/data/
--rw-r--r--   0 shichenxie   (501) staff       (20)   268042 2020-11-30 13:17:38.000000 scorecardpy-0.1.9.6/scorecardpy/data/germancredit.csv
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     3697 2020-11-30 13:32:32.000000 scorecardpy-0.1.9.6/scorecardpy/germancredit.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     6092 2018-05-22 08:16:36.000000 scorecardpy-0.1.9.6/scorecardpy/info_ent_indx_gini.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     4582 2019-09-10 14:47:10.000000 scorecardpy-0.1.9.6/scorecardpy/info_value.py
--rw-r--r--   0 shichenxie   (501) staff       (20)     4215 2018-12-18 08:12:56.000000 scorecardpy-0.1.9.6/scorecardpy/one_hot.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)    22105 2018-10-11 03:57:32.000000 scorecardpy-0.1.9.6/scorecardpy/perf.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)    12640 2023-05-22 15:15:40.000000 scorecardpy-0.1.9.6/scorecardpy/scorecard.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     2360 2020-10-11 10:21:02.000000 scorecardpy-0.1.9.6/scorecardpy/split_df.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     5709 2019-09-10 15:02:37.000000 scorecardpy-0.1.9.6/scorecardpy/var_filter.py
--rw-r--r--   0 shichenxie   (501) staff       (20)     2274 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.6/scorecardpy/vif.py
--rwxr-xr-x   0 shichenxie   (501) staff       (20)    59997 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.6/scorecardpy/woebin.py
-drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-05-22 15:18:07.371926 scorecardpy-0.1.9.6/scorecardpy.egg-info/
--rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-05-22 15:18:07.000000 scorecardpy-0.1.9.6/scorecardpy.egg-info/PKG-INFO
--rw-r--r--   0 shichenxie   (501) staff       (20)      554 2023-05-22 15:18:07.000000 scorecardpy-0.1.9.6/scorecardpy.egg-info/SOURCES.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)        1 2023-05-22 15:18:07.000000 scorecardpy-0.1.9.6/scorecardpy.egg-info/dependency_links.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       70 2023-05-22 15:18:07.000000 scorecardpy-0.1.9.6/scorecardpy.egg-info/requires.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       12 2023-05-22 15:18:07.000000 scorecardpy-0.1.9.6/scorecardpy.egg-info/top_level.txt
--rw-r--r--   0 shichenxie   (501) staff       (20)       38 2023-05-22 15:18:07.373738 scorecardpy-0.1.9.6/setup.cfg
--rwxr-xr-x   0 shichenxie   (501) staff       (20)     2775 2023-05-22 14:46:51.000000 scorecardpy-0.1.9.6/setup.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-07-29 15:22:00.639066 scorecardpy-0.1.9.7/
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     1067 2018-04-24 03:25:44.000000 scorecardpy-0.1.9.7/LICENSE
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)      128 2018-04-24 03:52:54.000000 scorecardpy-0.1.9.7/MANIFEST.in
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     4696 2023-05-24 15:25:58.000000 scorecardpy-0.1.9.7/NEWS.md
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-07-29 15:22:00.638904 scorecardpy-0.1.9.7/PKG-INFO
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     3285 2020-02-24 13:15:32.000000 scorecardpy-0.1.9.7/README.md
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-07-29 15:22:00.636025 scorecardpy-0.1.9.7/scorecardpy/
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)      738 2023-05-24 15:25:51.000000 scorecardpy-0.1.9.7/scorecardpy/__init__.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     8150 2023-07-29 15:00:56.000000 scorecardpy-0.1.9.7/scorecardpy/condition_fun.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-07-29 15:22:00.637586 scorecardpy-0.1.9.7/scorecardpy/data/
+-rw-r--r--   0 shichenxie   (501) staff       (20)   268042 2020-11-30 13:17:38.000000 scorecardpy-0.1.9.7/scorecardpy/data/germancredit.csv
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     3697 2020-11-30 13:32:32.000000 scorecardpy-0.1.9.7/scorecardpy/germancredit.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     6092 2018-05-22 08:16:36.000000 scorecardpy-0.1.9.7/scorecardpy/info_ent_indx_gini.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     4582 2019-09-10 14:47:10.000000 scorecardpy-0.1.9.7/scorecardpy/info_value.py
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4215 2018-12-18 08:12:56.000000 scorecardpy-0.1.9.7/scorecardpy/one_hot.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    22121 2023-05-24 15:18:00.000000 scorecardpy-0.1.9.7/scorecardpy/perf.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    12640 2023-05-22 15:15:40.000000 scorecardpy-0.1.9.7/scorecardpy/scorecard.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     2360 2020-10-11 10:21:02.000000 scorecardpy-0.1.9.7/scorecardpy/split_df.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     5709 2019-09-10 15:02:37.000000 scorecardpy-0.1.9.7/scorecardpy/var_filter.py
+-rw-r--r--   0 shichenxie   (501) staff       (20)     2274 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.7/scorecardpy/vif.py
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)    59997 2023-05-22 12:21:28.000000 scorecardpy-0.1.9.7/scorecardpy/woebin.py
+drwxr-xr-x   0 shichenxie   (501) staff       (20)        0 2023-07-29 15:22:00.637430 scorecardpy-0.1.9.7/scorecardpy.egg-info/
+-rw-r--r--   0 shichenxie   (501) staff       (20)     4276 2023-07-29 15:22:00.000000 scorecardpy-0.1.9.7/scorecardpy.egg-info/PKG-INFO
+-rw-r--r--   0 shichenxie   (501) staff       (20)      554 2023-07-29 15:22:00.000000 scorecardpy-0.1.9.7/scorecardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)        1 2023-07-29 15:22:00.000000 scorecardpy-0.1.9.7/scorecardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       70 2023-07-29 15:22:00.000000 scorecardpy-0.1.9.7/scorecardpy.egg-info/requires.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       12 2023-07-29 15:22:00.000000 scorecardpy-0.1.9.7/scorecardpy.egg-info/top_level.txt
+-rw-r--r--   0 shichenxie   (501) staff       (20)       38 2023-07-29 15:22:00.639121 scorecardpy-0.1.9.7/setup.cfg
+-rwxr-xr-x   0 shichenxie   (501) staff       (20)     2775 2023-05-22 14:46:51.000000 scorecardpy-0.1.9.7/setup.py
```

### Comparing `scorecardpy-0.1.9.6/LICENSE` & `scorecardpy-0.1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/NEWS.md` & `scorecardpy-0.1.9.7/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# scorecardpy 0.1.9.5
-* fixed a bug on woebin function caused by pandas update (by @CBravoR)
+# scorecardpy 0.1.9.7
+* fixed a bug in function perf_eva
+
+# scorecardpy 0.1.9.6
+* fixed a bug in woebin function caused by pandas update (by @CBravoR)
 * suppressed warnings in woebin function caused by groupby operations (by @CBravoR)
 * added new functions vif, scorecard2
 
 # scorecardpy 0.1.9.2
 * fixed a bug in woebin function caused by the new function explode in pandas >= 0.25
 * fixed a bug when intialzing binning
 * modified the method to create initial fine binning breaks.
```

### Comparing `scorecardpy-0.1.9.6/PKG-INFO` & `scorecardpy-0.1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpy
-Version: 0.1.9.6
+Version: 0.1.9.7
 Summary: Credit Risk Scorecard
 Home-page: http://github.com/shichenxie/scorecardpy
 Author: Shichen Xie
 Author-email: xie@shichen.name
 Project-URL: Bug Reports, https://github.com/shichenxie/scorecardpy/issues
 Project-URL: Source, https://github.com/shichenxie/scorecardpy/
 Keywords: credit scorecard,woe binning,performace evaluation
```

### Comparing `scorecardpy-0.1.9.6/README.md` & `scorecardpy-0.1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/__init__.py` & `scorecardpy-0.1.9.7/scorecardpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from scorecardpy.woebin import (woebin, woebin_ply, woebin_plot, woebin_adj)
 from scorecardpy.perf import (perf_eva, perf_psi)
 from scorecardpy.scorecard import (scorecard, scorecard_ply, scorecard2)
 from scorecardpy.one_hot import one_hot
 from scorecardpy.vif import vif
 
 
-__version__ = '0.1.9.6'
+__version__ = '0.1.9.7'
 
 __all__ = (
     germancredit,
     split_df, 
     iv,
     var_filter,
     woebin, woebin_ply, woebin_plot, woebin_adj,
```

### Comparing `scorecardpy-0.1.9.6/scorecardpy/condition_fun.py` & `scorecardpy-0.1.9.7/scorecardpy/condition_fun.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,16 @@
             if (y1 != y2).any():
                 dat.loc[:,y] = y2#dat[y] = y2
                 warnings.warn("The positive value in \"{}\" was replaced by 1 and negative value by 0.".format(y))
         else:
             raise Exception("Incorrect inputs; the positive value in \"{}\" is not specified".format(y))
     else:
         raise Exception("Incorrect inputs; the length of unique values in y column \'{}\' != 2.".format(y))
-    
+    # to int
+    dat[y] = dat[y].astype('int')
     return dat
 
 
 # check print_step
 #' @import data.table
 #'
 def check_print_step(print_step):
```

### Comparing `scorecardpy-0.1.9.6/scorecardpy/data/germancredit.csv` & `scorecardpy-0.1.9.7/scorecardpy/data/germancredit.csv`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/germancredit.py` & `scorecardpy-0.1.9.7/scorecardpy/germancredit.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/info_ent_indx_gini.py` & `scorecardpy-0.1.9.7/scorecardpy/info_ent_indx_gini.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/info_value.py` & `scorecardpy-0.1.9.7/scorecardpy/info_value.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/one_hot.py` & `scorecardpy-0.1.9.7/scorecardpy/one_hot.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/perf.py` & `scorecardpy-0.1.9.7/scorecardpy/perf.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     TNR, True Negative Rate(Specificity) = 
         true negative/total actual negative
     NPV, Negative Predicted Value = 
         true negative/total predicted negative
         
     Examples
     ------
-    import scorecardpy
+    import scorecardpy as sc
     
     # load data
     dat = sc.germancredit()
     
     # filter variable via missing rate, iv, identical value rate
     dt_sel = sc.var_filter(dat, "creditability")
     
@@ -306,16 +306,16 @@
         ### 
         rt['AUC'] = round(auc, 4)
         rt['Gini'] = round(2*auc-1, 4)
     
     ### export plot ### 
     if show_plot:
         plist = ["eva_p"+i+'(df_'+i+',title)' for i in plot_type]
-        subplot_nrows = np.ceil(len(plist)/2)
-        subplot_ncols = np.ceil(len(plist)/subplot_nrows)
+        subplot_nrows = int(np.ceil(len(plist)/2))
+        subplot_ncols = int(np.ceil(len(plist)/subplot_nrows))
         
         fig = plt.figure()
         for i in np.arange(len(plist)):
             plt.subplot(subplot_nrows,subplot_ncols,i+1)
             eval(plist[i])
         plt.show()
         rt['pic'] = fig
```

### Comparing `scorecardpy-0.1.9.6/scorecardpy/scorecard.py` & `scorecardpy-0.1.9.7/scorecardpy/scorecard.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/split_df.py` & `scorecardpy-0.1.9.7/scorecardpy/split_df.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/var_filter.py` & `scorecardpy-0.1.9.7/scorecardpy/var_filter.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/vif.py` & `scorecardpy-0.1.9.7/scorecardpy/vif.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy/woebin.py` & `scorecardpy-0.1.9.7/scorecardpy/woebin.py`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/scorecardpy.egg-info/PKG-INFO` & `scorecardpy-0.1.9.7/scorecardpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecardpy
-Version: 0.1.9.6
+Version: 0.1.9.7
 Summary: Credit Risk Scorecard
 Home-page: http://github.com/shichenxie/scorecardpy
 Author: Shichen Xie
 Author-email: xie@shichen.name
 Project-URL: Bug Reports, https://github.com/shichenxie/scorecardpy/issues
 Project-URL: Source, https://github.com/shichenxie/scorecardpy/
 Keywords: credit scorecard,woe binning,performace evaluation
```

### Comparing `scorecardpy-0.1.9.6/scorecardpy.egg-info/SOURCES.txt` & `scorecardpy-0.1.9.7/scorecardpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scorecardpy-0.1.9.6/setup.py` & `scorecardpy-0.1.9.7/setup.py`

 * *Files identical despite different names*

