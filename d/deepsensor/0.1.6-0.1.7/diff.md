# Comparing `tmp/deepsensor-0.1.6.tar.gz` & `tmp/deepsensor-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.6.tar", last modified: Fri Jul 28 21:05:21 2023, max compression
+gzip compressed data, was "deepsensor-0.1.7.tar", last modified: Fri Jul 28 22:17:52 2023, max compression
```

## Comparing `deepsensor-0.1.6.tar` & `deepsensor-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.427621 deepsensor-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 21:05:21.427621 deepsensor-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-28 21:05:12.000000 deepsensor-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/active_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/acquisition_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/active_learning/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23532 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/convnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/model/nps.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor/train/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-28 21:05:12.000000 deepsensor-0.1.6/deepsensor/train/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/deepsensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 21:05:21.000000 deepsensor-0.1.6/deepsensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 21:05:12.000000 deepsensor-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 21:05:21.427621 deepsensor-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 21:05:12.000000 deepsensor-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:21.423621 deepsensor-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 21:05:12.000000 deepsensor-0.1.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.302002 deepsensor-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 22:17:52.302002 deepsensor-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-28 22:17:39.000000 deepsensor-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.294002 deepsensor-0.1.7/deepsensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/active_learning/acquisition_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/active_learning/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/data/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23532 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/model/convnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/model/nps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.298002 deepsensor-0.1.7/deepsensor/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-28 22:17:39.000000 deepsensor-0.1.7/deepsensor/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.294002 deepsensor-0.1.7/deepsensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 22:17:52.000000 deepsensor-0.1.7/deepsensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-28 22:17:39.000000 deepsensor-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 22:17:52.302002 deepsensor-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 22:17:39.000000 deepsensor-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:52.302002 deepsensor-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 22:17:39.000000 deepsensor-0.1.7/tests/utils.py
```

### Comparing `deepsensor-0.1.6/PKG-INFO` & `deepsensor-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.6/README.md` & `deepsensor-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/__init__.py` & `deepsensor-0.1.7/deepsensor/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/active_learning/acquisition_fns.py` & `deepsensor-0.1.7/deepsensor/active_learning/acquisition_fns.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,16 @@
     def __call__(self, task, X_s):
         return self.rng.random(X_s.shape[1])
 
 
 class ContextDist(AcquisitionFunctionParallel):
     """Distance to closest context point."""
 
-    def __init__(self, model: ProbabilisticModel):
-        super().__init__(model)
+    def __init__(self, context_set_idx: int = 0):
+        self.context_set_idx = context_set_idx
         self.min_or_max = "max"
 
     def __call__(self, task, X_s):
         X_c = task["X_c"][self.context_set_idx]
 
         if X_c.size == 0:
             # No sensors placed yet, so arbitrarily choose first query point by setting its
@@ -203,15 +203,15 @@
 
 
 class Stddev(AcquisitionFunctionParallel):
     """Random acquisition function."""
 
     def __init__(self, model: ProbabilisticModel):
         super().__init__(model)
-        self.min_or_max = "min"
+        self.min_or_max = "max"
 
     def __call__(self, task, X_s, target_set_idx=0):
         # Set the target points to the search points
         task = copy.deepcopy(task)
         task["X_t"] = X_s
 
         return self.model.stddev(task)[target_set_idx]
```

### Comparing `deepsensor-0.1.6/deepsensor/active_learning/algorithms.py` & `deepsensor-0.1.7/deepsensor/active_learning/algorithms.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/data/loader.py` & `deepsensor-0.1.7/deepsensor/data/loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/data/processor.py` & `deepsensor-0.1.7/deepsensor/data/processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/data/task.py` & `deepsensor-0.1.7/deepsensor/data/task.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/data/utils.py` & `deepsensor-0.1.7/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/errors.py` & `deepsensor-0.1.7/deepsensor/errors.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/model/convnp.py` & `deepsensor-0.1.7/deepsensor/model/convnp.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/model/defaults.py` & `deepsensor-0.1.7/deepsensor/model/defaults.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/model/model.py` & `deepsensor-0.1.7/deepsensor/model/model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/model/nps.py` & `deepsensor-0.1.7/deepsensor/model/nps.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/plot.py` & `deepsensor-0.1.7/deepsensor/plot.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.7/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/torch/__init__.py` & `deepsensor-0.1.7/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor/train/train.py` & `deepsensor-0.1.7/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.7/deepsensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.6/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.7/deepsensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/setup.cfg` & `deepsensor-0.1.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.6
+version = 0.1.7
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
```

### Comparing `deepsensor-0.1.6/tests/test_active_learning.py` & `deepsensor-0.1.7/tests/test_active_learning.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/test_data_processor.py` & `deepsensor-0.1.7/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/test_model.py` & `deepsensor-0.1.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/test_plotting.py` & `deepsensor-0.1.7/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/test_task_loader.py` & `deepsensor-0.1.7/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/test_training.py` & `deepsensor-0.1.7/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.6/tests/utils.py` & `deepsensor-0.1.7/tests/utils.py`

 * *Files identical despite different names*

