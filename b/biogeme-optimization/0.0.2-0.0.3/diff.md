# Comparing `tmp/biogeme_optimization-0.0.2.tar.gz` & `tmp/biogeme_optimization-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeme_optimization-0.0.2.tar", last modified: Thu Jul 27 16:49:52 2023, max compression
+gzip compressed data, was "biogeme_optimization-0.0.3.tar", last modified: Sat Jul 29 06:51:46 2023, max compression
```

## Comparing `biogeme_optimization-0.0.2.tar` & `biogeme_optimization-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.644309 biogeme_optimization-0.0.2/
--rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-27 16:49:52.644360 biogeme_optimization-0.0.2/PKG-INFO
--rw-r--r--   0 bierlair   (503) staff       (20)     2337 2023-07-03 14:06:53.000000 biogeme_optimization-0.0.2/README.md
--rw-r--r--   0 bierlair   (503) staff       (20)     1084 2023-07-27 16:49:52.644576 biogeme_optimization-0.0.2/setup.cfg
--rw-r--r--   0 bierlair   (503) staff       (20)       69 2023-06-21 07:47:31.000000 biogeme_optimization-0.0.2/setup.py
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.639953 biogeme_optimization-0.0.2/src/
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.642122 biogeme_optimization-0.0.2/src/biogeme_optimization/
--rw-r--r--   0 bierlair   (503) staff       (20)      105 2023-06-21 08:14:43.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/__init__.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6589 2023-06-23 08:47:20.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/algebra.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2790 2023-07-04 09:14:44.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/bfgs.py
--rw-r--r--   0 bierlair   (503) staff       (20)    32223 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)      605 2023-07-03 14:01:16.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/diagnostics.py
--rw-r--r--   0 bierlair   (503) staff       (20)      203 2023-06-22 14:15:04.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/exceptions.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2707 2023-07-04 14:20:02.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/format.py
--rw-r--r--   0 bierlair   (503) staff       (20)    12844 2023-07-08 15:15:57.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6404 2023-07-08 15:16:05.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/hybrid_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)    11130 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/linesearch.py
--rw-r--r--   0 bierlair   (503) staff       (20)     1851 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/logging.py
--rw-r--r--   0 bierlair   (503) staff       (20)     8540 2023-07-20 20:56:33.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/neighborhood.py
--rw-r--r--   0 bierlair   (503) staff       (20)    14134 2023-07-21 22:06:30.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/pareto.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9681 2023-07-22 20:56:54.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/simple_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)    20403 2023-07-08 15:17:14.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/trust_region.py
--rw-r--r--   0 bierlair   (503) staff       (20)     7986 2023-07-14 16:12:58.000000 biogeme_optimization-0.0.2/src/biogeme_optimization/vns.py
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.642805 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/
--rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/PKG-INFO
--rw-r--r--   0 bierlair   (503) staff       (20)     1130 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 bierlair   (503) staff       (20)        1 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 bierlair   (503) staff       (20)       83 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/requires.txt
--rw-r--r--   0 bierlair   (503) staff       (20)       21 2023-07-27 16:49:52.000000 biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/top_level.txt
-drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-27 16:49:52.644208 biogeme_optimization-0.0.2/tests/
--rw-r--r--   0 bierlair   (503) staff       (20)     6383 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_algebra.py
--rw-r--r--   0 bierlair   (503) staff       (20)     3644 2023-06-24 16:11:17.000000 biogeme_optimization-0.0.2/tests/test_bfgs.py
--rw-r--r--   0 bierlair   (503) staff       (20)    28630 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)     2923 2023-07-03 12:35:53.000000 biogeme_optimization-0.0.2/tests/test_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     4592 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_hybrid_function.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9329 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_linesearch.py
--rw-r--r--   0 bierlair   (503) staff       (20)     4822 2023-07-27 16:37:09.000000 biogeme_optimization-0.0.2/tests/test_neighborhood.py
--rw-r--r--   0 bierlair   (503) staff       (20)     6436 2023-07-14 11:47:18.000000 biogeme_optimization-0.0.2/tests/test_pareto.py
--rw-r--r--   0 bierlair   (503) staff       (20)     9166 2023-07-03 13:09:42.000000 biogeme_optimization-0.0.2/tests/test_simple_bounds.py
--rw-r--r--   0 bierlair   (503) staff       (20)    21752 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_trust_region.py
--rw-r--r--   0 bierlair   (503) staff       (20)     3674 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.2/tests/test_vns.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-29 06:51:46.808006 biogeme_optimization-0.0.3/
+-rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-29 06:51:46.808066 biogeme_optimization-0.0.3/PKG-INFO
+-rw-r--r--   0 bierlair   (503) staff       (20)     2337 2023-07-03 14:06:53.000000 biogeme_optimization-0.0.3/README.md
+-rw-r--r--   0 bierlair   (503) staff       (20)     1084 2023-07-29 06:51:46.808291 biogeme_optimization-0.0.3/setup.cfg
+-rw-r--r--   0 bierlair   (503) staff       (20)       69 2023-06-21 07:47:31.000000 biogeme_optimization-0.0.3/setup.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-29 06:51:46.799581 biogeme_optimization-0.0.3/src/
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-29 06:51:46.804293 biogeme_optimization-0.0.3/src/biogeme_optimization/
+-rw-r--r--   0 bierlair   (503) staff       (20)      105 2023-06-21 08:14:43.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/__init__.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6589 2023-06-23 08:47:20.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/algebra.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2790 2023-07-04 09:14:44.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/bfgs.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    32316 2023-07-28 15:26:30.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)      605 2023-07-03 14:01:16.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/diagnostics.py
+-rw-r--r--   0 bierlair   (503) staff       (20)      203 2023-06-22 14:15:04.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/exceptions.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2707 2023-07-04 14:20:02.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/format.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    12844 2023-07-08 15:15:57.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6404 2023-07-08 15:16:05.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/hybrid_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    11130 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/linesearch.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     1851 2023-07-07 13:49:21.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/logging.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     8540 2023-07-20 20:56:33.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/neighborhood.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    14134 2023-07-21 22:06:30.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/pareto.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9681 2023-07-22 20:56:54.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/simple_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    20403 2023-07-08 15:17:14.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/trust_region.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     7986 2023-07-14 16:12:58.000000 biogeme_optimization-0.0.3/src/biogeme_optimization/vns.py
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-29 06:51:46.805155 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/
+-rw-r--r--   0 bierlair   (503) staff       (20)     3171 2023-07-29 06:51:46.000000 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 bierlair   (503) staff       (20)     1130 2023-07-29 06:51:46.000000 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)        1 2023-07-29 06:51:46.000000 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)       83 2023-07-29 06:51:46.000000 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/requires.txt
+-rw-r--r--   0 bierlair   (503) staff       (20)       21 2023-07-29 06:51:46.000000 biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/top_level.txt
+drwxr-xr-x   0 bierlair   (503) staff       (20)        0 2023-07-29 06:51:46.807703 biogeme_optimization-0.0.3/tests/
+-rw-r--r--   0 bierlair   (503) staff       (20)     6383 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_algebra.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     3644 2023-06-24 16:11:17.000000 biogeme_optimization-0.0.3/tests/test_bfgs.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    28630 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     2923 2023-07-03 12:35:53.000000 biogeme_optimization-0.0.3/tests/test_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     4592 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_hybrid_function.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9329 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_linesearch.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     4822 2023-07-27 16:37:09.000000 biogeme_optimization-0.0.3/tests/test_neighborhood.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     6436 2023-07-14 11:47:18.000000 biogeme_optimization-0.0.3/tests/test_pareto.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     9166 2023-07-03 13:09:42.000000 biogeme_optimization-0.0.3/tests/test_simple_bounds.py
+-rw-r--r--   0 bierlair   (503) staff       (20)    21752 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_trust_region.py
+-rw-r--r--   0 bierlair   (503) staff       (20)     3674 2023-07-08 15:17:23.000000 biogeme_optimization-0.0.3/tests/test_vns.py
```

### Comparing `biogeme_optimization-0.0.2/PKG-INFO` & `biogeme_optimization-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme_optimization
-Version: 0.0.2
+Version: 0.0.3
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme_optimization-0.0.2/README.md` & `biogeme_optimization-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/setup.cfg` & `biogeme_optimization-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = biogeme_optimization
-version = 0.0.2
+version = 0.0.3
 description = Various optimization algorithms for teaching and research
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Michel Bierlaire
 author_email = michel.bierlaire@epfl.ch
 url = http://biogeme.epfl.ch
 download_urls = https://pypi.org/project/bierlaire_optimization
```

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/algebra.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/bfgs.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/bounds.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
     return result
 
 
 class Bounds:
     """This class is designed for the management of simple bound constraints."""
 
+    INFINITY = np.sqrt(np.finfo(float).max)
     def __init__(self, bounds):
         """Constructor.
 
         :param bounds: list of tuples (ell,u) containing the lower and
                   upper bounds for each free parameter.
 
         :type bounds: list(tuple)
@@ -121,15 +122,15 @@
 
             :return: The modified value. If x is None, returns
                 -infinity; otherwise, returns x.
             :rtype: float
 
             """
             if value is None:
-                return -np.inf
+                return -self.INFINITY
 
             return value
 
         def none_to_plus_infinity(value):
             """Returns +infinity if the input is None, otherwise
                 returns the input value.
 
@@ -138,15 +139,15 @@
 
             :return: The modified value. If x is None, returns
                 +infinity; otherwise, returns x.
             :rtype: float
 
             """
             if value is None:
-                return np.inf
+                return self.INFINITY
 
             return value
 
         self.bounds = bounds
         """list of tuples (ell, u) containing the lower and upper bounds for
             each free parameter.
         """
@@ -719,16 +720,16 @@
             bd[list(activated)] = direction[list(activated)]
             b = h_current @ bd
 
             d_dot_g = np.sum([direction[i] * g[i] for i in activated])
             fprime += delta_t * fsecond - np.inner(b, x) - d_dot_g
             fsecond += np.inner(b, bd - 2 * direction)
             direction[list(activated)] = 0.0
-
-            if fprime >= 0:
+            
+            if sum(activated) == 0 or fprime >= 0:
                 return x
 
         return x
 
     def truncated_conjugate_gradient(self, gradient, hessian, tol=1.0e-6):
         """Find an approximation of the trust region subproblem using
             the truncated conjugate gradient method, where the step d
```

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/diagnostics.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/diagnostics.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/format.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/format.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/function.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/hybrid_function.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/linesearch.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/logging.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/logging.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/neighborhood.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/pareto.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/simple_bounds.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/trust_region.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization/vns.py` & `biogeme_optimization-0.0.3/src/biogeme_optimization/vns.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/PKG-INFO` & `biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.2
+Version: 0.0.3
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme_optimization-0.0.2/src/biogeme_optimization.egg-info/SOURCES.txt` & `biogeme_optimization-0.0.3/src/biogeme_optimization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_algebra.py` & `biogeme_optimization-0.0.3/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_bfgs.py` & `biogeme_optimization-0.0.3/tests/test_bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_bounds.py` & `biogeme_optimization-0.0.3/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_function.py` & `biogeme_optimization-0.0.3/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_hybrid_function.py` & `biogeme_optimization-0.0.3/tests/test_hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_linesearch.py` & `biogeme_optimization-0.0.3/tests/test_linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_neighborhood.py` & `biogeme_optimization-0.0.3/tests/test_neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_pareto.py` & `biogeme_optimization-0.0.3/tests/test_pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_simple_bounds.py` & `biogeme_optimization-0.0.3/tests/test_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_trust_region.py` & `biogeme_optimization-0.0.3/tests/test_trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme_optimization-0.0.2/tests/test_vns.py` & `biogeme_optimization-0.0.3/tests/test_vns.py`

 * *Files identical despite different names*

