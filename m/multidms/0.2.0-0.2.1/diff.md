# Comparing `tmp/multidms-0.2.0-py3-none-any.whl.zip` & `tmp/multidms-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 36831 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1995 b- defN 23-Jul-21 21:41 multidms/__init__.py
--rw-r--r--  2.0 unx    13851 b- defN 23-Jul-21 21:41 multidms/biophysical.py
--rw-r--r--  2.0 unx    24850 b- defN 23-Jul-21 21:41 multidms/data.py
--rw-r--r--  2.0 unx    42354 b- defN 23-Jul-21 21:41 multidms/model.py
--rw-r--r--  2.0 unx    31292 b- defN 23-Jul-21 21:41 multidms/plot.py
--rw-r--r--  2.0 unx     9969 b- defN 23-Jul-21 21:41 multidms/utils.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4072 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 23-Jul-21 21:44 multidms-0.2.0.dist-info/RECORD
-11 files, 130424 bytes uncompressed, 35427 bytes compressed:  72.8%
+Zip file size: 36949 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1995 b- defN 23-Jul-29 03:06 multidms/__init__.py
+-rw-r--r--  2.0 unx    13851 b- defN 23-Jul-29 03:06 multidms/biophysical.py
+-rw-r--r--  2.0 unx    24852 b- defN 23-Jul-29 03:06 multidms/data.py
+-rw-r--r--  2.0 unx    42848 b- defN 23-Jul-29 03:06 multidms/model.py
+-rw-r--r--  2.0 unx    31294 b- defN 23-Jul-29 03:06 multidms/plot.py
+-rw-r--r--  2.0 unx    10004 b- defN 23-Jul-29 03:06 multidms/utils.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Jul-29 03:08 multidms-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4072 b- defN 23-Jul-29 03:08 multidms-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 03:08 multidms-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-29 03:08 multidms-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      846 b- defN 23-Jul-29 03:08 multidms-0.2.1.dist-info/RECORD
+11 files, 130958 bytes uncompressed, 35545 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: multidms/plot.py
 Comment: 
 
 Filename: multidms/utils.py
 Comment: 
 
-Filename: multidms-0.2.0.dist-info/LICENSE
+Filename: multidms-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: multidms-0.2.0.dist-info/METADATA
+Filename: multidms-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: multidms-0.2.0.dist-info/WHEEL
+Filename: multidms-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: multidms-0.2.0.dist-info/top_level.txt
+Filename: multidms-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: multidms-0.2.0.dist-info/RECORD
+Filename: multidms-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## multidms/__init__.py

```diff
@@ -49,15 +49,15 @@
 
  - :const:`~multidms.alphabets.AAS_WITHSTOP_WITHGAP`
 
 """
 
 __author__ = "Jared Galloway"
 __email__ = "jgallowa@fredhutch.org"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __url__ = "https://github.com/matsengrp/multidms"
 
 from polyclonal.alphabets import AAS  # noqa: F401
 from polyclonal.alphabets import AAS_WITHGAP  # noqa: F401
 from polyclonal.alphabets import AAS_WITHSTOP  # noqa: F401
 from polyclonal.alphabets import AAS_WITHSTOP_WITHGAP  # noqa: F401
```

## multidms/data.py

```diff
@@ -26,15 +26,15 @@
 import jax.numpy as jnp
 import seaborn as sns
 from jax.experimental import sparse
 from matplotlib import pyplot as plt
 from pandarallel import pandarallel
 
 jax.config.update("jax_enable_x64", True)
-tqdm.pandas()
+# tqdm.pandas()
 
 
 class Data:
     r"""
     Prep and store one-hot encoding of
     variant substitutions data.
     Individual objects of this type can be shared
```

## multidms/model.py

```diff
@@ -131,25 +131,27 @@
 
     However, if accessed directly through the :class:`Model` object, you will
     get the same information, along with model/parameter specific
     features included. These are automatically updated each time you
     request the property.
 
     >>> model.mutations_df  # doctest: +NORMALIZE_WHITESPACE
-      mutation wts  sites muts  times_seen_a  times_seen_b      beta  \
-    0      M1E   M      1    E             1           3.0  0.080868   
-    1      M1W   M      1    W             1           0.0 -0.386247   
-    2      G3P   G      3    P             1           1.0 -0.375656   
-    3      G3R   G      3    R             1           2.0  1.668974   
+             wts  sites muts  times_seen_a  times_seen_b      beta  \
+    mutation                                                         
+    M1E        M      1    E             1           3.0  0.080868   
+    M1W        M      1    W             1           0.0 -0.386247   
+    G3P        G      3    P             1           1.0 -0.375656   
+    G3R        G      3    R             1           2.0  1.668974   
     <BLANKLINE>
-       predicted_func_score  shift_b  
-    0             -2.398970      0.0  
-    1             -2.976895      0.0  
-    2             -2.964124      0.0  
-    3             -0.792805      0.0  
+              a_predicted_func_score  shift_b  b_predicted_func_score  
+    mutation                                                           
+    M1E                    -2.398970      0.0               -2.398970  
+    M1W                    -2.976895      0.0               -2.976895  
+    G3P                    -2.964124      0.0               -2.964124  
+    G3R                    -0.792805      0.0               -0.792805 
 
     Notice the respective single mutation effects (``"beta"``), conditional shifts
     (``shift_d``),
     and predicted functional score (``F_d``) of each mutation in the model are now
     easily accessible. Similarly, we can take a look at the variants_df for the model,
 
     >>> model.variants_df  # doctest: +NORMALIZE_WHITESPACE
@@ -441,19 +443,22 @@
             wildtype prediction. Otherwise, report the unmodified
             model prediction.
 
         Returns
         -------
         pandas.DataFrame
             A copy of the mutations data, `self.data.mutations_df`,
-            with the phenotypes added. Phenotypes are predicted
+            with the mutations column set as the index, and columns
+            with the mutational attributes (e.g. betas, shifts) and
+            conditional phenotypes (e.g. func_scores) added.
+            Phenotypes are predicted
             based on the current state of the model.
         """
         # we're updating this
-        mutations_df = self.data.mutations_df.copy()
+        mutations_df = self.data.mutations_df.set_index("mutation")
 
         # for effect calculation
         if phenotype_as_effect:
             wildtype_df = self.wildtype_df
 
         # add betas i.e. 'latent effect'
         mutations_df.loc[:, "beta"] = self._params["beta"]
@@ -462,15 +467,15 @@
             # shift of latent effect
             if condition != self._data.reference:
                 mutations_df[f"shift_{condition}"] = self._params[f"shift_{condition}"]
 
             Y_pred = self.phenotype_frombinary(X, condition)
             if phenotype_as_effect:
                 Y_pred -= wildtype_df.loc[condition, "predicted_func_score"]
-            mutations_df["predicted_func_score"] = Y_pred
+            mutations_df[f"{condition}_predicted_func_score"] = Y_pred
 
         return mutations_df
 
     def add_phenotypes_to_df(
         self,
         df,
         substitutions_col="aa_substitutions",
```

## multidms/plot.py

```diff
@@ -46,15 +46,15 @@
     """
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
         name="_", colors=[start, end], N=n
     )
     return [matplotlib.colors.rgb2hex(tup) for tup in cmap(list(range(0, n)))]
 
 
-def lineplot_and_heatmap(
+def _lineplot_and_heatmap(
     *,
     data_df,
     stat_col,
     category_col,
     alphabet=None,
     sites=None,
     addtl_tooltip_stats=None,
@@ -819,14 +819,14 @@
 
     if "alphabet" not in kwargs:
         kwargs["alphabet"] = fit.data.alphabet
 
     if biochem_order_aas:
         kwargs["alphabet"] = polyclonal.alphabets.biochem_order_aas(kwargs["alphabet"])
 
-    return lineplot_and_heatmap(**kwargs)
+    return _lineplot_and_heatmap(**kwargs)
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

## multidms/utils.py

```diff
@@ -236,25 +236,26 @@
     ax.set_ylabel("Loss")
     ax.set_xlabel("Iterations")
     ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
 
     plt.show()
 
 
-def combine_replicate_muts(fit_dict, times_seen_threshold=3, how="inner"):
+def combine_replicate_muts(
+    fit_dict, times_seen_threshold=3, how="inner", phenotype_as_effect=True
+):
     """
     Take a dictionary of fit objects, with key's as the prefix for individual
     replicate values, and merge then such that all individual and average mutation
     values are present in both.
     """
     # obtain and curate each of the replicate mutational dataframes
     mutations_dfs = []
     for replicate, fit in fit_dict.items():
-        fit_mut_df = fit.mutations_df.set_index("mutation")
-
+        fit_mut_df = fit.get_mutations_df(phenotype_as_effect=phenotype_as_effect)
         new_column_name_map = {c: f"{replicate}_{c}" for c in fit_mut_df.columns}
         fit_mut_df = fit_mut_df.rename(new_column_name_map, axis=1)
 
         times_seen_cols = [c for c in fit_mut_df.columns if "times" in c]
         for c in times_seen_cols:
             fit_mut_df = fit_mut_df[fit_mut_df[c] >= times_seen_threshold]
         mutations_dfs.append(fit_mut_df)
@@ -266,15 +267,15 @@
         ),
         mutations_dfs,
     )
 
     column_order = []
     # now compute replicate averages
     for c in fit.mutations_df.columns:
-        if c == "mutation" or "times_seen" in c:
+        if "times_seen" in c:
             continue
         cols_to_combine = [f"{replicate}_{c}" for replicate in fit_dict.keys()]
 
         # just keep one replicate wt, site, mut .. as they are shared.
         if c in ["wts", "sites", "muts"]:
             mut_df[c] = mut_df[cols_to_combine[0]]
             mut_df.drop(cols_to_combine, axis=1, inplace=True)
```

## Comparing `multidms-0.2.0.dist-info/LICENSE` & `multidms-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `multidms-0.2.0.dist-info/METADATA` & `multidms-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidms
-Version: 0.2.0
+Version: 0.2.1
 Summary: Joint modeling of multiple deep mutational scanning experiments.
 Author-email: Jared Galloway <jgallowa@fredhutch.org>, Hugh Haddox <hkhaddox@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Fred Hutchinson Cancer Research Center
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `multidms-0.2.0.dist-info/RECORD` & `multidms-0.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-multidms/__init__.py,sha256=gyh40ejo0E6fYptgcA3Rrqe1_MGULhErTVfizgIGUnw,1995
+multidms/__init__.py,sha256=WzaMJhsoOg9nAQnM-asQEQ6c49ha5da0jc2_MKlduVE,1995
 multidms/biophysical.py,sha256=FPsCns-ScjROhQkwiKtCsmez_qORJjC_PelWv19a6KE,13851
-multidms/data.py,sha256=YeJOps6WCQ0iT9rFw6b-hSYyq5s6fNd-JxZEV5zHL14,24850
-multidms/model.py,sha256=wilzGfCwyPr__4ZyUQ0XQPqk_vnE9mLDsR0UsJCEYyI,42354
-multidms/plot.py,sha256=ogz6l_7p0eH0VjbRsUbCQiM2ifjxtoFJnQsEPj5QcBw,31292
-multidms/utils.py,sha256=NP3ik1q2XiS6I2lCQjMDFbL6qI-1anhxIc27WC8PVNw,9969
-multidms-0.2.0.dist-info/LICENSE,sha256=mJ4ZEGg5nui2ZBfp2ROb3o3ft3TJ4TkypMQnImQoCDo,1095
-multidms-0.2.0.dist-info/METADATA,sha256=Mhp3uDBqTo69P2IBctnGM1mT6SjoWxYKl0ExZVb0bKA,4072
-multidms-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-multidms-0.2.0.dist-info/top_level.txt,sha256=NIdwAxUTLTJjI9-QL1q_dkT2pVlN3yOZY7apfx0X2nk,9
-multidms-0.2.0.dist-info/RECORD,,
+multidms/data.py,sha256=FselhVQ9oni90iVD3seP5AVGdWNu_jS3aznSbg3Uxnk,24852
+multidms/model.py,sha256=zrDBeWxTbmlPpDKJRxs9Hvv4XT-A3bLZbo0ZoEuA1qQ,42848
+multidms/plot.py,sha256=cGDNUv-B2bQEfvMsOKa2ewO2zRugTLr2Ekgq5Yi2yRg,31294
+multidms/utils.py,sha256=HNsU75QYC32pbfAfLuh3zWtorVCtZZu3pgL7LIimOD8,10004
+multidms-0.2.1.dist-info/LICENSE,sha256=mJ4ZEGg5nui2ZBfp2ROb3o3ft3TJ4TkypMQnImQoCDo,1095
+multidms-0.2.1.dist-info/METADATA,sha256=41lEAAm8ilVblB9zVJ0Nu5QWzZCBGEnR7KYRMJ8SGzY,4072
+multidms-0.2.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+multidms-0.2.1.dist-info/top_level.txt,sha256=NIdwAxUTLTJjI9-QL1q_dkT2pVlN3yOZY7apfx0X2nk,9
+multidms-0.2.1.dist-info/RECORD,,
```

