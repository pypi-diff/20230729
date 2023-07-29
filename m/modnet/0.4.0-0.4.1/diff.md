# Comparing `tmp/modnet-0.4.0.tar.gz` & `tmp/modnet-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.4.0.tar", last modified: Wed Jul 19 13:06:53 2023, max compression
+gzip compressed data, was "dist/modnet-0.4.1.tar", last modified: Sat Jul 29 11:01:49 2023, max compression
```

## Comparing `modnet-0.4.0.tar` & `modnet-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.0/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.0/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-19 13:06:53.000000 modnet-0.4.0/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.0/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-07-13 18:46:04.000000 modnet-0.4.0/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.0/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.0/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    12289 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9990 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9213 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    15893 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/featurizers/presets/matminer_all_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      492 2021-09-08 13:24:57.000000 modnet-0.4.0/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.0/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    27253 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.0/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.0/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.4.0/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    14851 2023-07-11 14:46:35.000000 modnet-0.4.0/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17885 2023-07-13 18:28:15.000000 modnet-0.4.0/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    59819 2023-07-14 09:39:48.000000 modnet-0.4.0/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    41703 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.4.0/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.0/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.0/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-07-11 13:21:01.000000 modnet-0.4.0/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-07-11 13:24:52.000000 modnet-0.4.0/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.0/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.0/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-19 13:06:53.000000 modnet-0.4.0/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      223 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-07-19 13:06:52.000000 modnet-0.4.0/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-07-19 13:06:53.000000 modnet-0.4.0/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2085 2023-07-11 13:21:01.000000 modnet-0.4.0/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.1/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.1/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-29 11:01:49.000000 modnet-0.4.1/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.1/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-07-28 12:19:26.000000 modnet-0.4.1/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.1/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.1/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12534 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.1/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27250 2023-07-28 12:18:53.000000 modnet-0.4.1/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.1/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.1/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.4.1/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    14851 2023-07-11 14:46:35.000000 modnet-0.4.1/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17885 2023-07-13 18:28:15.000000 modnet-0.4.1/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    59819 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    41902 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.4.1/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.1/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.1/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-07-11 13:24:52.000000 modnet-0.4.1/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.1/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      223 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-07-29 11:01:49.000000 modnet-0.4.1/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2085 2023-07-11 13:21:01.000000 modnet-0.4.1/setup.py
```

### Comparing `modnet-0.4.0/LICENSE.md` & `modnet-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/PKG-INFO` & `modnet-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.0
+Version: 0.4.1
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
```

### Comparing `modnet-0.4.0/README.md` & `modnet-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/data/Features_cross` & `modnet-0.4.1/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/ext_data.py` & `modnet-0.4.1/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/featurizers/featurizers.py` & `modnet-0.4.1/modnet/featurizers/featurizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,36 +44,41 @@
     composition_featurizers: Optional[Iterable[BaseFeaturizer]] = None
     oxid_composition_featurizers: Optional[Iterable[BaseFeaturizer]] = None
     structure_featurizers: Optional[Iterable[BaseFeaturizer]] = None
     site_featurizers: Optional[Iterable[BaseFeaturizer]] = None
     site_stats: Tuple[str] = ("mean", "std_dev")
     featurizer_mode: str = "multi"
 
-    def __init__(self, n_jobs=None):
+    def __init__(self, n_jobs=None, drop_allnan: bool = True):
         """Initialise the MODFeaturizer object with a requested
         number of threads to use during featurization.
 
         Arguments:
             n_jobs: The number of threads to use. If `None`, matminer
             will use `multiprocessing.cpu_count()` by default.
+            drop_allnan: if True, features that are fully NaNs will be removed.
 
         """
         self.set_n_jobs(n_jobs)
+        self.set_drop_allnan(drop_allnan)
 
     def set_n_jobs(self, n_jobs: Optional[int]):
         """Set the no. of threads to pass to matminer for featurizer
         initialisation.
 
         Arguments:
             n_jobs: The number of threads to use. If `None`, matminer
             will use `multiprocessing.cpu_count()` by default.
 
         """
         self._n_jobs = n_jobs
 
+    def set_drop_allnan(self, drop_allnan: bool = True):
+        self.drop_allnan = drop_allnan
+
     def featurize(self, df: pd.DataFrame) -> pd.DataFrame:
         """Run all of the preset featurizers on the input dataframe.
 
         Arguments:
             df: the input dataframe with a `"structure"` column
                 containing pymatgen `Structure` objects.
```

### Comparing `modnet-0.4.0/modnet/featurizers/presets/__init__.py` & `modnet-0.4.1/modnet/featurizers/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.4.1/modnet/featurizers/presets/debreuck_2020.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         df["AtomicOrbitals|HOMO_element"] = df["AtomicOrbitals|HOMO_element"].apply(
             lambda x: -1 if not isinstance(x, str) else Element(x).Z
         )
         df["AtomicOrbitals|LUMO_element"] = df["AtomicOrbitals|LUMO_element"].apply(
             lambda x: -1 if not isinstance(x, str) else Element(x).Z
         )
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_structure(self, df):
         """Applies the preset structural featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -222,15 +222,15 @@
         df["GlobalSymmetryFeatures|crystal_system"] = df[
             "GlobalSymmetryFeatures|crystal_system"
         ].map(_crystal_system)
         df["GlobalSymmetryFeatures|is_centrosymmetric"] = df[
             "GlobalSymmetryFeatures|is_centrosymmetric"
         ].map(_int_map)
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_site(self, df):
         """Applies the preset site featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -239,15 +239,15 @@
             "GeneralizedRadialDistributionFunction": "GeneralizedRDF",
             "AGNIFingerprints": "AGNIFingerPrint",
             "BondOrientationalParameter": "BondOrientationParameter",
         }
         df = super().featurize_site(df, aliases=aliases)
         df = df.loc[:, (df != 0).any(axis=0)]
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
 
 class CompositionOnlyFeaturizer(DeBreuck2020Featurizer):
     """This subclass simply disables structure and site-level features
     from the main `DeBreuck2020Featurizer` class.
 
         **Materials property prediction for limited datasets enabled
```

### Comparing `modnet-0.4.0/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.4.1/modnet/featurizers/presets/matminer_2023.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             df["AtomicOrbitals|LUMO_element"] = df["AtomicOrbitals|LUMO_element"].apply(
                 lambda x: -1 if not isinstance(x, str) else Element(x).Z
             )
 
         else:
             df.drop(columns=["IonProperty|max ionic char"], inplace=True)
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_structure(self, df):
         """Applies the preset structural featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -211,15 +211,15 @@
         df["GlobalSymmetryFeatures|crystal_system"] = df[
             "GlobalSymmetryFeatures|crystal_system"
         ].map(_crystal_system)
         df["GlobalSymmetryFeatures|is_centrosymmetric"] = df[
             "GlobalSymmetryFeatures|is_centrosymmetric"
         ].map(_int_map)
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_site(self, df):
         """Applies the preset site featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -228,15 +228,15 @@
             "GeneralizedRadialDistributionFunction": "GeneralizedRDF",
             "AGNIFingerprints": "AGNIFingerPrint",
             "BondOrientationalParameter": "BondOrientationParameter",
         }
         df = super().featurize_site(df, aliases=aliases)
         df = df.loc[:, (df != 0).any(axis=0)]
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
 
 class CompositionOnlyMatminer2023Featurizer(Matminer2023Featurizer):
     """This subclass simply disables structure and site-level features
     from the main `Matminer2023Featurizer` class.
 
     This should yield identical results to the original 2020 version.
```

### Comparing `modnet-0.4.0/modnet/featurizers/presets/matminer_all_2023.py` & `modnet-0.4.1/modnet/featurizers/presets/matminer_all_2023.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     Follows the same philosophy as the `DeBreuck2020Featurizer`
     but with many features changing their underlying matminer implementation,
     definition and behaviour since the creation of the former featurizer.
     The featurizer list has also been updated to include all the available featurizers.
 
     """
 
-    def __init__(self, fast_oxid: bool = False, continuous_only: bool = False):
+    def __init__(
+        self,
+        fast_oxid: bool = False,
+        continuous_only: bool = False,
+    ):
         """Creates the featurizer and imports all featurizer functions.
 
         Parameters:
             fast_oxid: Whether to use the accelerated oxidation state parameters within
                 pymatgen when constructing features that constrain oxidation states such
                 that all sites with the same species in a structure will have the same
                 oxidation state (recommended if featurizing any structure
@@ -319,15 +323,15 @@
                 ],
                 inplace=True,
             )
 
             if self.oxid_composition_featurizers:
                 df.drop(columns=["IonProperty|max ionic char"], inplace=True)
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_structure(self, df):
         """Applies the preset structural featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -355,15 +359,15 @@
         df["GlobalSymmetryFeatures|crystal_system"] = df[
             "GlobalSymmetryFeatures|crystal_system"
         ].map(_crystal_system)
         df["GlobalSymmetryFeatures|is_centrosymmetric"] = df[
             "GlobalSymmetryFeatures|is_centrosymmetric"
         ].map(_int_map)
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
     def featurize_site(self, df):
         """Applies the preset site featurizers to the input dataframe,
         renames some fields and cleans the output dataframe.
 
         """
 
@@ -372,15 +376,15 @@
             "GeneralizedRadialDistributionFunction": "GeneralizedRDF",
             "AGNIFingerprints": "AGNIFingerPrint",
             "BondOrientationalParameter": "BondOrientationParameter",
         }
         df = super().featurize_site(df, aliases=aliases)
         df = df.loc[:, (df != 0).any(axis=0)]
 
-        return modnet.featurizers.clean_df(df)
+        return modnet.featurizers.clean_df(df, drop_allnan=self.drop_allnan)
 
 
 class CompositionOnlyMatminerAll2023Featurizer(MatminerAll2023Featurizer):
     """This subclass simply disables structure and site-level features
     from the main `Matminer2023Featurizer` class.
 
     This should yield identical results to the original 2020 version.
@@ -389,13 +393,16 @@
 
     def __init__(
         self,
         continuous_only: bool = False,
         oxidation_featurizers: bool = False,
         fast_oxid: bool = False,
     ):
-        super().__init__(fast_oxid=fast_oxid, continuous_only=continuous_only)
+        super().__init__(
+            fast_oxid=fast_oxid,
+            continuous_only=continuous_only,
+        )
         self.fast_oxid = fast_oxid
         self.structure_featurizers = ()
         self.site_featurizers = ()
         if not oxidation_featurizers:
             self.oxid_composition_featurizers = ()
```

### Comparing `modnet-0.4.0/modnet/hyper_opt/fit_genetic.py` & `modnet-0.4.1/modnet/hyper_opt/fit_genetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,15 +654,15 @@
             """
             self.best_model = self.best_individual.refit_model(
                 self.data, n_models=refit, n_jobs=n_jobs or 1, fast=fast
             )
 
         else:
             ensemble = []
-            for m in models[ranking[:refit]]:
+            for m in models[ranking[:10]]:
                 ensemble += m.models
             self.best_model = EnsembleMODNetModel(models=ensemble)
 
         self.results = self.best_individual.genes
 
         return self.best_model
```

### Comparing `modnet-0.4.0/modnet/matbench/benchmark.py` & `modnet-0.4.1/modnet/matbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/model_presets/presets.py` & `modnet-0.4.1/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/models/bayesian.py` & `modnet-0.4.1/modnet/models/bayesian.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/models/ensemble.py` & `modnet-0.4.1/modnet/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/models/vanilla.py` & `modnet-0.4.1/modnet/models/vanilla.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/preprocessing.py` & `modnet-0.4.1/modnet/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,28 +702,31 @@
             if num_classes is not None:
                 self.num_classes.update(num_classes)
 
         # set up dataframe for structures with columns (id, structure)
         self.df_structure = pd.DataFrame({"id": structure_ids, "structure": materials})
         self.df_structure.set_index("id", inplace=True)
 
-    def featurize(self, fast: bool = False, db_file=None, n_jobs=None):
+    def featurize(
+        self, fast: bool = False, db_file=None, n_jobs=None, drop_allnan: bool = True
+    ):
         """For the input structures, construct many matminer features
         and save a featurized dataframe. If `db_file` is specified, this
         method will try to load previous feature calculations for each
         structure ID instead of recomputing.
 
         Sets the `self.df_featurized` attribute.
 
         Args:
             fast (bool): whether or not to load from the Materials Project Database.
             Please be sure to have provided the mp-ids in the MODData structure_ids keyword.
             Note : The database will be downloaded in this case, and takes around 2GB of space on your drive !
 
             db_file: Deprecated. Do Not use this anymore.
+            drop_allnan: if True, features that are fully NaNs will be removed.
 
 
         """
 
         if db_file is not None:
             LOG.warning(
                 "Please remove the db_file argument, no longer supported. A default MP DB is downloaded instead."
@@ -733,14 +736,16 @@
 
         df_done = None
         df_todo = None
 
         if n_jobs is not None:
             self.featurizer.set_n_jobs(n_jobs)
 
+        self.featurizer.set_drop_allnan(drop_allnan)
+
         if self.df_featurized is not None:
             raise RuntimeError("Not overwriting existing featurized dataframe.")
 
         if fast:
             LOG.info("Fast featurization on, retrieving from database...")
 
             global DATABASE
@@ -774,15 +779,15 @@
                 df_final = df_done
 
         # otherwise, no structures were loaded, so we need to compute all
         else:
             df_final = self.featurizer.featurize(self.df_structure)
 
         # replace infinite values by nan that are handled during the fit
-        df_final = clean_df(df_final)
+        df_final = clean_df(df_final, drop_allnan=drop_allnan)
 
         self.df_featurized = df_final
         LOG.info("Data has successfully been featurized!")
 
     def feature_selection(
         self,
         n: int = 1500,
```

### Comparing `modnet-0.4.0/modnet/sklearn.py` & `modnet-0.4.1/modnet/sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/conftest.py` & `modnet-0.4.1/modnet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_benchmark.py` & `modnet-0.4.1/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_ext_data.py` & `modnet-0.4.1/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_hyper_opt.py` & `modnet-0.4.1/modnet/tests/test_hyper_opt.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_model.py` & `modnet-0.4.1/modnet/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_preprocessing.py` & `modnet-0.4.1/modnet/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/tests/test_sklearn.py` & `modnet-0.4.1/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet/utils.py` & `modnet-0.4.1/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/modnet.egg-info/PKG-INFO` & `modnet-0.4.1/modnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.0
+Version: 0.4.1
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
```

### Comparing `modnet-0.4.0/modnet.egg-info/SOURCES.txt` & `modnet-0.4.1/modnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modnet-0.4.0/setup.py` & `modnet-0.4.1/setup.py`

 * *Files identical despite different names*

