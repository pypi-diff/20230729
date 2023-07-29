# Comparing `tmp/close_numerical_matches-0.1.4-py3-none-any.whl.zip` & `tmp/close_numerical_matches-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8659 bytes, number of entries: 9
--rw-r--r--  2.0 unx      233 b- defN 23-Apr-10 17:03 close_numerical_matches/__init__.py
--rw-r--r--  2.0 unx    10980 b- defN 23-Apr-10 17:03 close_numerical_matches/find_matches.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 17:03 close_numerical_matches/py.typed
--rw-r--r--  2.0 unx       58 b- defN 23-Apr-10 17:03 close_numerical_matches/version.py
--rw-r--r--  2.0 unx     1080 b- defN 23-Apr-10 17:04 close_numerical_matches-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     7464 b- defN 23-Apr-10 17:04 close_numerical_matches-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 17:04 close_numerical_matches-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Apr-10 17:04 close_numerical_matches-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      829 b- defN 23-Apr-10 17:04 close_numerical_matches-0.1.4.dist-info/RECORD
-9 files, 20760 bytes uncompressed, 7195 bytes compressed:  65.3%
+Zip file size: 9401 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      233 b- defN 23-Jul-29 05:56 close_numerical_matches/__init__.py
+-rw-r--r--  2.0 unx    11977 b- defN 23-Jul-29 05:56 close_numerical_matches/find_matches.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 05:56 close_numerical_matches/py.typed
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-29 05:56 close_numerical_matches/version.py
+-rw-r--r--  2.0 unx     1080 b- defN 23-Jul-29 05:56 close_numerical_matches-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8580 b- defN 23-Jul-29 05:56 close_numerical_matches-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 05:56 close_numerical_matches-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-29 05:56 close_numerical_matches-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-29 05:56 close_numerical_matches-0.2.0.dist-info/RECORD
+9 files, 22873 bytes uncompressed, 7937 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: close_numerical_matches/py.typed
 Comment: 
 
 Filename: close_numerical_matches/version.py
 Comment: 
 
-Filename: close_numerical_matches-0.1.4.dist-info/LICENSE
+Filename: close_numerical_matches-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: close_numerical_matches-0.1.4.dist-info/METADATA
+Filename: close_numerical_matches-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: close_numerical_matches-0.1.4.dist-info/WHEEL
+Filename: close_numerical_matches-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: close_numerical_matches-0.1.4.dist-info/top_level.txt
+Filename: close_numerical_matches-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: close_numerical_matches-0.1.4.dist-info/RECORD
+Filename: close_numerical_matches-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## close_numerical_matches/find_matches.py

```diff
@@ -3,43 +3,67 @@
 import itertools
 from typing import Callable
 from typing import Generator
 from typing import Union
 
 import numpy as np
 
-DistFunc = Callable[[np.ndarray], np.ndarray]
+DistFunc = Callable[[np.ndarray, np.ndarray], np.ndarray]
 DistFuncArg = Union[str, DistFunc]
+NORM, MAX, COS = 'norm', 'max', 'cos'
 
 OVERHEAD_MULT = 5
-NORM, MAX = 'norm', 'max'
-
 DELTAS_1D = [-1, 0, 1]
 
 
+def _normalize_vectors(arr: np.ndarray) -> np.ndarray:
+    """
+    Takes an array and returns a copy of it where each row has been
+    normalized to unit norm
+    """
+    return arr / np.linalg.norm(arr, axis=1).reshape(-1, 1)
+
+
+def _norm(arr: np.ndarray, row: np.ndarray) -> np.ndarray:
+    return np.linalg.norm(arr - row, axis=1)
+
+
+def _max_abs(arr: np.ndarray, row: np.ndarray) -> np.ndarray:
+    return np.max(np.abs(arr - row), axis=1)
+
+
+def _cosine_dist(arr: np.ndarray, row: np.ndarray) -> np.ndarray:
+    num = arr @ row
+    denom = np.linalg.norm(arr, axis=1) * np.linalg.norm(row)
+    cosine_sim = num / denom
+    # Value is now similarity in [-1, 1] so we want to
+    # convert to distance in [0, 2]
+    return 1.0 - cosine_sim
+
+
+DIST_FUNCS: dict[str, DistFunc] = {
+    NORM: _norm,
+    MAX: _max_abs,
+    COS: _cosine_dist,
+}
+
+
 def _get_dist_func(dist_metric: DistFuncArg) -> DistFunc:
     """Returns the appropriate distance function for a given dist_metric"""
     if isinstance(dist_metric, str):
-        if dist_metric == NORM:
-            def norm(arr: np.ndarray) -> np.ndarray:
-                return np.linalg.norm(arr, axis=1)
-            return norm
-
-        if dist_metric == MAX:
-            def max_abs(arr: np.ndarray) -> np.ndarray:
-                return np.max(np.abs(arr), axis=1)
-            return max_abs
+        if dist_metric in DIST_FUNCS:
+            return DIST_FUNCS[dist_metric]
 
         raise ValueError(
-            f'If dist_metric is a string, it has to be {NORM}'
-            + f' or {MAX} but got {dist_metric}',
+            'If dist_metric is a string, it has to be one of '
+            + f'{list(DIST_FUNCS.keys())} but got "{dist_metric}"',
         )
 
     if callable(dist_metric):
-        test_res = dist_metric(np.array([[1, 1]]))
+        test_res = dist_metric(np.array([[1]]), np.array([1]))
         is_valid = (
             isinstance(test_res, np.ndarray)
             and len(test_res.shape) == 1
             and len(test_res) == 1
         )
         if is_valid:
             return dist_metric
@@ -83,15 +107,15 @@
             = arr1, arr1_indices, arr0, arr0_indices
 
     matches: list[list[int]] = []
     arr1_filtered = arr1[arr1_indices]
     for arr0_idx in arr0_indices:
         arr0_idx = int(arr0_idx)
         row = arr0[arr0_idx]
-        inner_diff = dist_func(arr1_filtered - row)
+        inner_diff = dist_func(arr1_filtered, row)
         inner_matches_idx = np.where(inner_diff <= tol)[0]
         new_matches: list[list[int]] = [[arr0_idx, int(arr1_indices[i])] for i in inner_matches_idx]
         matches.extend(new_matches)
 
     if matches and reverse:
         matches = list(np.array(matches)[::, ::-1])
 
@@ -121,15 +145,15 @@
     assign_arr_to_buckets(arr1, 1)
     return buckets
 
 
 def _make_deltas_iter(dim: int) -> Generator[tuple[int, ...], None, None]:
     """
     Constructs the delta values to use together with the base element for a
-    given dimension to visit all neighbours and the base element itself
+    given dimension to visit all neighbors and the base element itself
 
     Examples
     --------
     >>> list(_make_deltas_iter(1))
     [(-1,), (0,), (1,)]
     >>> list(_make_deltas_iter(2))
     [(-1, -1), (-1, 0), (-1, 1),
@@ -173,19 +197,19 @@
     ----------
     arr0 : np.ndarray
         First array to find matches against. Should be of size (n, d).
 
     arr1 : np.ndarray
         Second array to find matches against. Should be of size (m, d).
 
-    dist : {'norm', 'max'} or Callable[[np.ndarray], np.ndarray]
-        Distance metric to calculate distance. `'norm'` and `'max'` are
+    dist : {'norm', 'max', 'cos'} or Callable[[np.ndarray, np.ndarray], np.ndarray]
+        Distance metric to calculate distance. `'norm'`, `'max'` and `'cos'` are
         currently supported. If you want some other distance function, you can
-        supply your own function. It should take an (n, d) array as argument
-        and return an (n,) array.
+        supply your own function. It should take an (n, d) array and (d,) array
+        as argument and return an (n,) array.
 
     tol : float, default=0.1
         The tolerance where values are considered the similar enough to count
         as a match. Should be > 0.
 
     Returns
     -------
@@ -212,14 +236,17 @@
 
     assert arr0.shape[1] == arr1.shape[1], \
         ('Arrays should be of equivalent size in the second axis, but got'
          + f' {arr0.shape[1]} and {arr1.shape[1]}')
 
     assert tol > 0, f'Tolerance has to be strictly positive but got {tol}'
 
+    if dist == COS:
+        arr0, arr1 = _normalize_vectors(arr0), _normalize_vectors(arr1)
+
     matches = _naive_find_matches(
         arr0=arr0,
         arr0_indices=np.arange(len(arr0)),
         arr1=arr1,
         arr1_indices=np.arange(len(arr1)),
         dist_func=_get_dist_func(dist),
         tol=tol,
@@ -228,42 +255,43 @@
 
 
 def find_matches(
     arr0: np.ndarray,
     arr1: np.ndarray,
     dist: DistFuncArg = NORM,
     tol: float = 0.1,
-    bucket_tol_mult: int = 2,
+    bucket_tol_mult: float = 2.0,
 ) -> np.ndarray:
     """
     Finds all numerical matches in two 2D ndarrays of shape (n, d) and (m, d)
     that are within tolerance level and returns the indices. Works best for
     small d and large n and m where there are relatively few matches.
 
     Parameters
     ----------
     arr0 : np.ndarray
         First array to find matches against. Should be of size (n, d).
 
     arr1 : np.ndarray
         Second array to find matches against. Should be of size (m, d).
 
-    dist : {'norm', 'max'} or Callable[[np.ndarray], np.ndarray]
-        Distance metric to calculate distance. `'norm'` and `'max'` are
+    dist : {'norm', 'max', 'cos'} or Callable[[np.ndarray, np.ndarray], np.ndarray]
+        Distance metric to calculate distance. `'norm'`, `'max'` and `'cos'` are
         currently supported. If you want some other distance function, you can
-        supply your own function. It should take an (n, d) array as argument
-        and return an (n,) array.
+        supply your own function. It should take an (n, d) array and (d,) array
+        as argument and return an (n,) array.
 
     tol : float, default=0.1
         The tolerance where values are considered the similar enough to count
         as a match. Should be > 0.
 
-    bucket_tol_mult : int, default=2
+    bucket_tol_mult : float, default=2.0
         The tolerance multiplier to use for assigning buckets. Can in some
-        instances make algorithm faster to tweak this. Should never be less
+        instances make algorithm faster to tweak this. For cosine distance,
+        you likely want to set this much higher. Should never be less
         than 1.
 
     Returns
     -------
     matches : np.ndarray
         Array of corresponding indices of the numerical matches in the arrays.
 
@@ -289,14 +317,17 @@
         ('Arrays should be of equivalent size in the second axis, but got'
          + f' {arr0.shape[1]} and {arr1.shape[1]}')
 
     assert tol > 0, f'Tolerance has to be strictly positive but got {tol}'
     assert bucket_tol_mult >= 1.0, \
         f'bucket_tol_mult should be >= 1 but got {bucket_tol_mult}'
 
+    if dist == COS:
+        arr0, arr1 = _normalize_vectors(arr0), _normalize_vectors(arr1)
+
     buckets = _assign_to_buckets(arr0, arr1, bucket_tol_mult * tol)
 
     # Check if O(nmd) < O(bd^3) * const in which case it makes better sense
     # to run naive algorithm
     n, m, b, d = len(arr0), len(arr1), len(buckets), arr0.shape[1]
     if n * m * d < b * d**3 * OVERHEAD_MULT:
         return naive_find_matches(arr0, arr1, dist, tol)
```

## close_numerical_matches/version.py

```diff
@@ -1,3 +1,3 @@
 from __future__ import annotations
 
-__version__ = '0.1.4'
+__version__ = '0.2.0'
```

## Comparing `close_numerical_matches-0.1.4.dist-info/LICENSE` & `close_numerical_matches-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `close_numerical_matches-0.1.4.dist-info/METADATA` & `close_numerical_matches-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: close-numerical-matches
-Version: 0.1.4
+Version: 0.2.0
 Summary: Finds close numerical matches across two arrays.
 Home-page: https://github.com/shmulvad/close_numerical_matches
 Author: Soeren Mulvad
-Author-email: Soeren Mulvad <post@kaasogmulvad.dk>
+Author-email: Soeren Mulvad <shmulvad@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2021 Søren Mulvad
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -30,24 +30,24 @@
 Project-URL: Documentation, https://github.com/shmulvad/close_numerical_matches/
 Project-URL: Changelog, https://github.com/shmulvad/close_numerical_matches/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://github.com/shmulvad/close_numerical_matches/
 Project-URL: Github, https://github.com/shmulvad/close_numerical_matches
 Project-URL: Source, https://github.com/shmulvad/close_numerical_matches
 Project-URL: Issues, https://github.com/shmulvad/close_numerical_matches/issues
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 # Close Numerical Matches
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/close_numerical_matches)][pypi]
 [![PyPI - Version](https://img.shields.io/pypi/v/close_numerical_matches)][pypi]
 ![GitHub Workflow Status (branch)](https://github.com/shmulvad/close_numerical_matches/workflows/CI/badge.svg)
 [![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/shmulvad/close_numerical_matches/main)][codefactor]
@@ -62,31 +62,33 @@
 
 You can install `close-numerical-matches` from [PyPI][pypi]:
 
 ```bash
 $ pip install close-numerical-matches
 ```
 
-The package is supported on Python 3.7 and above and requires Numpy.
+The package is supported on Python 3.8 and above and requires Numpy.
 
 
 ## How to use
 
 Import `find_matches` from `close_numerical_matches` and supply two arrays of shape (n, d) and (m, d) and a given tolerance level. Optionally provide your desired distance metric and a bucket tolerance multiplier. The arguments in more detail:
 
 * `arr0` : `np.ndarray`
     First array to find matches against. Should be of size (n, d).
 * `arr1` : `np.ndarray`
     Second array to find matches against. Should be of size (m, d).
-* `dist` : `{'norm', 'max'}` or `Callable[[np.ndarray], np.ndarray]`, default='norm'
-    Distance metric to calculate distance. `'norm'` and `'max'` are currently supported. If you want some other distance function, you can supply your own function. It should take an (n, d) array as argument and return an (n,) array.
+* `dist` : `{'norm', 'max', 'cos'}` or `Callable[[np.ndarray, np.ndarray], np.ndarray]`, default='norm'
+    Distance metric to calculate distance. `'norm'`, `'max'` and `'cos'` are currently supported. If you want some other distance function, you can supply your own function. It should take two arrays: One array of size (n, d) of entries and another array of size (d,) of a particular entry. Should return an (n,) array of distances.
 * `tol` : `float`, default=0.1
     The tolerance where values are considered the similar enough to count as a match. Should be > 0.
 * `bucket_tol_mult` : `int`, default=2
-    The tolerance multiplier to use for assigning buckets. Can in some instances make algorithm faster to tweak this. Should never be less than 1.
+    The tolerance multiplier to use for assigning buckets. By setting this lower, there are fewer potential close points that need to be checked (faster runtime), but you risk missing some match pairs. By setting it higher, you need to compare more potential matches, but the risk of missing any close pair is lower. For cosine distance, you might need to set this high.
+    If you supply your own distance function, do take this parameter into consideration.
+    Should never be less than 1.
 
 ### Example
 
 ```python
 >>> import numpy as np
 >>> from close_numerical_matches import find_matches
 >>> arr0 = np.array([[25, 24], [50, 50], [25, 26]])
@@ -95,15 +97,17 @@
 array([[0, 0], [0, 1], [1, 2], [2, 1]])
 >>> find_matches(arr0, arr1, tol=0.9999)
 array([[1, 2]])
 >>> find_matches(arr0, arr1, tol=0.60001)
 array([], dtype=int64)
 >>> find_matches(arr0, arr1, tol=0.60001, dist='max')
 array([[1, 2]])
->>> manhatten_dist = lambda arr: np.sum(np.abs(arr), axis=1)
+>>> find_matches([[0, 0.05]], [[0, 5], [0, -0.01]], tol=0.1, dist='cos')
+array([[0, 0]])
+>>> manhatten_dist = lambda arr, row: np.sum(np.abs(arr - row), axis=1)
 >>> matches = find_matches(arr0, arr1, tol=1.0001, dist=manhatten_dist)
 >>> matches
 array([[0, 0], [0, 1], [2, 1]])
 >>> indices0, indices1 = matches.T
 >>> arr0[indices0]
 array([[25, 24], [25, 24], [25, 26]])
 ```
@@ -136,14 +140,21 @@
 
 ## How it works
 
 Instead of comparing every element in the first array against every element in the second array, resulting in an O(nmd) runtime, all elements are at first assigned to buckets so only elements that are relatively close are compared. In the case of relatively few matches and a low dimensionality d, this cuts the runtime down to almost linear O((n + m)d).
 
 In general, the algorithm runtime of the bucket approach is O((n + m)d + Bd³ + ∑\_{b ∈ B} n\_b m\_b) where B is the number of buckets and n\_b and m\_b are the number of items assigned to bucket b. As can be seen, it scales bad with dimensionality and also does not improve from the naive approach if all elements are assigned to the same bucket. In case the bucket approach is likely to be slower than the naive approach, this library will fall back to the naive approach.
 
+
+## When NOT to use this library
+
+* If you are working with arrays with very high dimensionalities, the algorithm employed here does not scale well. As mentioned above, the naive algorithm will be used in such cases. See if another library exists for your particular problem.
+* If you are expecting that a lot of pairs will match, this is not suitable. This algorithm is targeted for the case where there are extremely many data points and only a fraction of those are expected to match.
+* If you need to use a distance function that does not map well to being assigned to buckets.
+
 [testCasesFile]: https://github.com/shmulvad/close_numerical_matches/blob/main/tests/test_find_matches.py
 [pypi]: https://pypi.org/project/close-numerical-matches/
 [license]: https://github.com/shmulvad/close_numerical_matches/blob/master/LICENSE
 [issues]: https://github.com/shmulvad/close_numerical_matches/issues
 [release]: https://github.com/shmulvad/close_numerical_matches/releases/latest
 [codefactor]: https://www.codefactor.io/repository/github/shmulvad/close_numerical_matches
 [makeAPullRequest]: https://makeapullrequest.com
```

## Comparing `close_numerical_matches-0.1.4.dist-info/RECORD` & `close_numerical_matches-0.2.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 close_numerical_matches/__init__.py,sha256=RaZR1BMexPS45_F-2uPEWFBc1VTsYXJdxrd1QR-M_4w,233
-close_numerical_matches/find_matches.py,sha256=rsG8nFC5Yq45mbJHci-Y2wR0HfB7zsoBg4-HqKBcbLU,10980
+close_numerical_matches/find_matches.py,sha256=JC1TCyno13onirBaNWYinbXAxUVgEANGH609HqWqQCY,11977
 close_numerical_matches/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-close_numerical_matches/version.py,sha256=TNKSgiXUWtUH-GUwDyQgbEVoj1hX7KWVJqg6EDX41ho,58
-close_numerical_matches-0.1.4.dist-info/LICENSE,sha256=wnDx8_ZSMu8xcmmAQ-vnTKLf4E0a93JRBpy9NNadNJE,1080
-close_numerical_matches-0.1.4.dist-info/METADATA,sha256=pekwuM4CUhRMiJvFIDXmop_M7tgW8KPejhxFiUgRFZo,7464
-close_numerical_matches-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-close_numerical_matches-0.1.4.dist-info/top_level.txt,sha256=czM2dobUrxyWUCqo3-iGecd1JX1bHspVUljbpBXrjDk,24
-close_numerical_matches-0.1.4.dist-info/RECORD,,
+close_numerical_matches/version.py,sha256=MXjrFZc-D-DqRo1kL05QtZYawV2UzKckf7Bcw63pXdE,58
+close_numerical_matches-0.2.0.dist-info/LICENSE,sha256=wnDx8_ZSMu8xcmmAQ-vnTKLf4E0a93JRBpy9NNadNJE,1080
+close_numerical_matches-0.2.0.dist-info/METADATA,sha256=SkEd1r1CREDCFayIV-w5YoDM5I1KaCnrdVRYVfnJFgY,8580
+close_numerical_matches-0.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+close_numerical_matches-0.2.0.dist-info/top_level.txt,sha256=czM2dobUrxyWUCqo3-iGecd1JX1bHspVUljbpBXrjDk,24
+close_numerical_matches-0.2.0.dist-info/RECORD,,
```

