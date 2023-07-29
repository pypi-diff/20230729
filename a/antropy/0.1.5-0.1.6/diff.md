# Comparing `tmp/antropy-0.1.5.tar.gz` & `tmp/antropy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antropy-0.1.5.tar", last modified: Sat Dec 17 18:31:16 2022, max compression
+gzip compressed data, was "antropy-0.1.6.tar", last modified: Sat Jul 29 05:04:11 2023, max compression
```

## Comparing `antropy-0.1.5.tar` & `antropy-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 raphael    (501) staff       (20)        0 2022-12-17 18:31:16.147092 antropy-0.1.5/
--rw-r--r--   0 raphael    (501) staff       (20)     1518 2021-03-17 01:16:13.000000 antropy-0.1.5/LICENSE
--rw-r--r--   0 raphael    (501) staff       (20)      101 2021-03-17 00:58:44.000000 antropy-0.1.5/MANIFEST.in
--rw-r--r--   0 raphael    (501) staff       (20)      751 2022-12-17 18:31:16.147221 antropy-0.1.5/PKG-INFO
--rw-r--r--   0 raphael    (501) staff       (20)     5061 2022-12-17 18:23:37.000000 antropy-0.1.5/README.rst
-drwxr-xr-x   0 raphael    (501) staff       (20)        0 2022-12-17 18:31:16.145705 antropy-0.1.5/antropy/
--rw-r--r--   0 raphael    (501) staff       (20)      115 2022-12-17 17:57:43.000000 antropy-0.1.5/antropy/__init__.py
--rw-r--r--   0 raphael    (501) staff       (20)    32646 2022-12-17 18:27:41.000000 antropy-0.1.5/antropy/entropy.py
--rw-r--r--   0 raphael    (501) staff       (20)    13444 2022-12-17 17:56:11.000000 antropy-0.1.5/antropy/fractal.py
--rw-r--r--   0 raphael    (501) staff       (20)     4070 2022-12-17 18:27:41.000000 antropy-0.1.5/antropy/utils.py
-drwxr-xr-x   0 raphael    (501) staff       (20)        0 2022-12-17 18:31:16.146840 antropy-0.1.5/antropy.egg-info/
--rw-r--r--   0 raphael    (501) staff       (20)      751 2022-12-17 18:31:16.000000 antropy-0.1.5/antropy.egg-info/PKG-INFO
--rw-r--r--   0 raphael    (501) staff       (20)      280 2022-12-17 18:31:16.000000 antropy-0.1.5/antropy.egg-info/SOURCES.txt
--rw-r--r--   0 raphael    (501) staff       (20)        1 2022-12-17 18:31:16.000000 antropy-0.1.5/antropy.egg-info/dependency_links.txt
--rw-r--r--   0 raphael    (501) staff       (20)        8 2022-12-17 18:31:16.000000 antropy-0.1.5/antropy.egg-info/top_level.txt
--rw-r--r--   0 raphael    (501) staff       (20)       31 2022-12-17 18:28:32.000000 antropy-0.1.5/pyproject.toml
--rw-r--r--   0 raphael    (501) staff       (20)       42 2022-12-17 17:55:06.000000 antropy-0.1.5/requirements.txt
--rw-r--r--   0 raphael    (501) staff       (20)      263 2022-12-17 18:31:16.147822 antropy-0.1.5/setup.cfg
--rw-r--r--   0 raphael    (501) staff       (20)     2057 2022-12-17 17:57:34.000000 antropy-0.1.5/setup.py
+drwxr-xr-x   0 raphael    (501) staff       (20)        0 2023-07-29 05:04:11.191203 antropy-0.1.6/
+-rw-r--r--   0 raphael    (501) staff       (20)     1518 2021-03-17 01:16:13.000000 antropy-0.1.6/LICENSE
+-rw-r--r--   0 raphael    (501) staff       (20)      101 2021-03-17 00:58:44.000000 antropy-0.1.6/MANIFEST.in
+-rw-r--r--   0 raphael    (501) staff       (20)      734 2023-07-29 05:04:11.191364 antropy-0.1.6/PKG-INFO
+-rw-r--r--   0 raphael    (501) staff       (20)     4929 2023-07-29 04:55:39.000000 antropy-0.1.6/README.rst
+drwxr-xr-x   0 raphael    (501) staff       (20)        0 2023-07-29 05:04:11.189190 antropy-0.1.6/antropy/
+-rw-r--r--   0 raphael    (501) staff       (20)      115 2023-07-29 04:53:35.000000 antropy-0.1.6/antropy/__init__.py
+-rw-r--r--   0 raphael    (501) staff       (20)    32990 2023-07-29 04:40:13.000000 antropy-0.1.6/antropy/entropy.py
+-rw-r--r--   0 raphael    (501) staff       (20)    13500 2023-02-12 13:41:22.000000 antropy-0.1.6/antropy/fractal.py
+-rw-r--r--   0 raphael    (501) staff       (20)     4070 2022-12-17 18:27:41.000000 antropy-0.1.6/antropy/utils.py
+drwxr-xr-x   0 raphael    (501) staff       (20)        0 2023-07-29 05:04:11.190952 antropy-0.1.6/antropy.egg-info/
+-rw-r--r--   0 raphael    (501) staff       (20)      734 2023-07-29 05:04:11.000000 antropy-0.1.6/antropy.egg-info/PKG-INFO
+-rw-r--r--   0 raphael    (501) staff       (20)      280 2023-07-29 05:04:11.000000 antropy-0.1.6/antropy.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael    (501) staff       (20)        1 2023-07-29 05:04:11.000000 antropy-0.1.6/antropy.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael    (501) staff       (20)        8 2023-07-29 05:04:11.000000 antropy-0.1.6/antropy.egg-info/top_level.txt
+-rw-r--r--   0 raphael    (501) staff       (20)       31 2022-12-17 18:28:32.000000 antropy-0.1.6/pyproject.toml
+-rw-r--r--   0 raphael    (501) staff       (20)       48 2023-07-29 04:47:30.000000 antropy-0.1.6/requirements.txt
+-rw-r--r--   0 raphael    (501) staff       (20)      263 2023-07-29 05:04:11.191965 antropy-0.1.6/setup.cfg
+-rw-r--r--   0 raphael    (501) staff       (20)     2062 2023-07-29 04:53:18.000000 antropy-0.1.6/setup.py
```

### Comparing `antropy-0.1.5/LICENSE` & `antropy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antropy-0.1.5/PKG-INFO` & `antropy-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: antropy
-Version: 0.1.5
+Version: 0.1.6
 Summary: AntroPy: entropy and complexity of time-series in Python
 Home-page: https://raphaelvallat.com/antropy/build/html/index.html
+Download-URL: https://github.com/raphaelvallat/antropy/
 Author: Raphael Vallat
 Author-email: raphaelvallat9@gmail.com
 Maintainer: Raphael Vallat
 Maintainer-email: raphaelvallat9@gmail.com
 License: BSD (3-clause)
-Download-URL: https://github.com/raphaelvallat/antropy/
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
```

### Comparing `antropy-0.1.5/README.rst` & `antropy-0.1.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 .. -*- mode: rst -*-
 
 |
 
-.. image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg
-    :target: https://www.python.org/downloads/
-
 .. image:: https://img.shields.io/github/license/raphaelvallat/antropy.svg
   :target: https://github.com/raphaelvallat/antropy/blob/master/LICENSE
 
 .. image:: https://github.com/raphaelvallat/antropy/actions/workflows/python_tests.yml/badge.svg
   :target: https://github.com/raphaelvallat/antropy/actions/workflows/python_tests.yml
 
 .. image:: https://codecov.io/gh/raphaelvallat/antropy/branch/master/graph/badge.svg
```

### Comparing `antropy-0.1.5/antropy/entropy.py` & `antropy-0.1.6/antropy/entropy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Entropy functions"""
 import numpy as np
-from numba import jit
+from numba import jit, types
 from math import factorial, log
 from sklearn.neighbors import KDTree
 from scipy.signal import periodogram, welch
 
 from .utils import _embed, _xlogx
 
 all = [
@@ -369,14 +369,15 @@
         svd_e /= np.log2(order)
     return svd_e
 
 
 def _app_samp_entropy(x, order, metric="chebyshev", approximate=True):
     """Utility function for `app_entropy`` and `sample_entropy`."""
     _all_metrics = KDTree.valid_metrics
+    _all_metrics = _all_metrics() if callable(_all_metrics) else _all_metrics
     if metric not in _all_metrics:
         raise ValueError(
             "The given metric (%s) is not valid. The valid "
             "metric names are: %s" % (metric, _all_metrics)
         )
     phi = np.zeros(2)
     r = 0.2 * np.std(x, ddof=0)
@@ -404,67 +405,58 @@
         phi[1] = np.mean(np.log(count2 / emb_data2.shape[0]))
     else:
         phi[0] = np.mean((count1 - 1) / (emb_data1.shape[0] - 1))
         phi[1] = np.mean((count2 - 1) / (emb_data2.shape[0] - 1))
     return phi
 
 
-@jit("f8(f8[:], i4, f8)", nopython=True)
-def _numba_sampen(x, order, r):
+@jit((types.Array(types.float64, 1, "C", readonly=True), types.int32, types.float64), nopython=True)
+def _numba_sampen(sequence, order, r):
     """
     Fast evaluation of the sample entropy using Numba.
     """
-    n = x.size
-    n1 = n - 1
-    order += 1
-    order_dbld = 2 * order
-
-    # Define threshold
-    # r *= x.std()
-
-    # initialize the lists
-    run = [0] * n
-    run1 = run[:]
-    r1 = [0] * (n * order_dbld)
-    a = [0] * order
-    b = a[:]
-    p = a[:]
-
-    for i in range(n1):
-        nj = n1 - i
-
-        for jj in range(nj):
-            j = jj + i + 1
-            if abs(x[j] - x[i]) < r:
-                run[jj] = run1[jj] + 1
-                m1 = order if order < run[jj] else run[jj]
-                for m in range(m1):
-                    a[m] += 1
-                    if j < n1:
-                        b[m] += 1
-            else:
-                run[jj] = 0
-        for j in range(order_dbld):
-            run1[j] = run[j]
-            r1[i + n * j] = run[j]
-        if nj > order_dbld - 1:
-            for j in range(order_dbld, nj):
-                run1[j] = run[j]
-
-    m = order - 1
-
-    while m > 0:
-        b[m] = b[m - 1]
-        m -= 1
-
-    b[0] = n * n1 / 2
-    a = np.array([float(aa) for aa in a])
-    b = np.array([float(bb) for bb in b])
-    p = np.true_divide(a, b)
-    return -log(p[-1])
+
+    size = sequence.size
+    # sequence = sequence.tolist()
+
+    numerator = 0
+    denominator = 0
+
+    for offset in range(1, size - order):
+        n_numerator = int(abs(sequence[order] - sequence[order + offset]) >= r)
+        n_denominator = 0
+
+        for idx in range(order):
+            n_numerator += abs(sequence[idx] - sequence[idx + offset]) >= r
+            n_denominator += abs(sequence[idx] - sequence[idx + offset]) >= r
+
+        if n_numerator == 0:
+            numerator += 1
+        if n_denominator == 0:
+            denominator += 1
+
+        prev_in_diff = int(abs(sequence[order] - sequence[offset + order]) >= r)
+        for idx in range(1, size - offset - order):
+            out_diff = int(abs(sequence[idx - 1] - sequence[idx + offset - 1]) >= r)
+            in_diff = int(abs(sequence[idx + order] - sequence[idx + offset + order]) >= r)
+            n_numerator += in_diff - out_diff
+            n_denominator += prev_in_diff - out_diff
+            prev_in_diff = in_diff
+
+            if n_numerator == 0:
+                numerator += 1
+            if n_denominator == 0:
+                denominator += 1
+
+    if denominator == 0:
+        return 0  # use 0/0 == 0
+    elif numerator == 0:
+        return np.inf
+    else:
+        return -log(numerator / denominator)
 
 
 def app_entropy(x, order=2, metric="chebyshev"):
     """Approximate Entropy.
 
     Parameters
     ----------
@@ -684,15 +676,15 @@
     pointer = 0
 
     # Iterate until the entire string has not been parsed
     while prefix_len + len_substring <= len(binary_string):
         # Given a prefix length, find the largest substring
         if (
             binary_string[pointer + len_substring - 1]
-            == binary_string[prefix_len + len_substring - 1]
+            == binary_string[prefix_len + len_substring - 1]  # noqa: W503
         ):
             len_substring += 1  # increase the length of the substring
         else:
             max_len_substring = max(len_substring, max_len_substring)
             pointer += 1
             # Since all pointers have been scanned, pick largest as the jump
             # size
```

### Comparing `antropy-0.1.5/antropy/fractal.py` & `antropy-0.1.6/antropy/fractal.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     d = np.max(np.abs(aux_d), axis=axis)
     kfd = np.squeeze(ln / (ln + np.log10(d / ll)))
     if not kfd.ndim:
         kfd = kfd.item()
     return kfd
 
 
-@jit((types.Array(types.float64, 1, "C", readonly=True), types.int32))
+@jit((types.Array(types.float64, 1, "C", readonly=True), types.int32), nopython=True)
 def _higuchi_fd(x, kmax):
     """Utility function for `higuchi_fd`."""
     n_times = x.size
     lk = np.empty(kmax)
     x_reg = np.empty(kmax)
     y_reg = np.empty(kmax)
     for k in range(1, kmax + 1):
@@ -295,15 +295,15 @@
     1.0040
     """
     x = np.asarray(x, dtype=np.float64)
     kmax = int(kmax)
     return _higuchi_fd(x, kmax)
 
 
-@jit("f8(f8[:])", nopython=True)
+@jit((types.Array(types.float64, 1, "C", readonly=True),), nopython=True)
 def _dfa(x):
     """
     Utility function for detrended fluctuation analysis
     """
     N = len(x)
     nvals = _log_n(4, 0.1 * N, 1.2)
     walk = np.cumsum(x - x.mean())
```

### Comparing `antropy-0.1.5/antropy/utils.py` & `antropy-0.1.6/antropy/utils.py`

 * *Files identical despite different names*

### Comparing `antropy-0.1.5/antropy.egg-info/PKG-INFO` & `antropy-0.1.6/antropy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: antropy
-Version: 0.1.5
+Version: 0.1.6
 Summary: AntroPy: entropy and complexity of time-series in Python
 Home-page: https://raphaelvallat.com/antropy/build/html/index.html
+Download-URL: https://github.com/raphaelvallat/antropy/
 Author: Raphael Vallat
 Author-email: raphaelvallat9@gmail.com
 Maintainer: Raphael Vallat
 Maintainer-email: raphaelvallat9@gmail.com
 License: BSD (3-clause)
-Download-URL: https://github.com/raphaelvallat/antropy/
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
```

### Comparing `antropy-0.1.5/setup.py` & `antropy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 DESCRIPTION = "AntroPy: entropy and complexity of time-series in Python"
 DISTNAME = "antropy"
 MAINTAINER = "Raphael Vallat"
 MAINTAINER_EMAIL = "raphaelvallat9@gmail.com"
 URL = "https://raphaelvallat.com/antropy/build/html/index.html"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/raphaelvallat/antropy/"
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 PACKAGE_DATA = {"antropy.data.icons": ["*.ico"]}
 
 try:
     from setuptools import setup
 
     _has_setuptools = True
 except ImportError:
@@ -36,26 +36,25 @@
         import sklearn
     except ImportError:
         install_requires.append("scikit-learn")
 
     try:
         import numba
     except ImportError:
-        install_requires.append("numba")
+        install_requires.append("numba>=0.57")
 
     try:
         import stochastic
     except ImportError:
         install_requires.append("stochastic")
 
     return install_requires
 
 
 if __name__ == "__main__":
-
     install_requires = check_dependencies()
 
     setup(
         name=DISTNAME,
         author=MAINTAINER,
         author_email=MAINTAINER_EMAIL,
         maintainer=MAINTAINER,
```

