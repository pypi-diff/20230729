# Comparing `tmp/rfb_mc-0.0.8.tar.gz` & `tmp/rfb_mc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfb_mc-0.0.8.tar", last modified: Tue Apr 27 14:22:04 2021, max compression
+gzip compressed data, was "rfb_mc-0.0.9.tar", last modified: Wed Apr 28 12:12:47 2021, max compression
```

## Comparing `rfb_mc-0.0.8.tar` & `rfb_mc-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.654104 rfb_mc-0.0.8/
--rw-rw-rw-   0        0        0     1086 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       40 2021-04-27 14:20:46.000000 rfb_mc-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      590 2021-04-27 14:22:04.651624 rfb_mc-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      145 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.609463 rfb_mc-0.0.8/rfb_mc/
--rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.635751 rfb_mc-0.0.8/rfb_mc/component/
--rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.638231 rfb_mc-0.0.8/rfb_mc/component/aws/
--rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/aws/__init__.py
--rw-rw-rw-   0        0        0     6758 2021-04-26 13:51:22.000000 rfb_mc-0.0.8/rfb_mc/component/aws/dynamodb_store.py
--rw-rw-rw-   0        0        0     3573 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/direct_integrator.py
--rw-rw-rw-   0        0        0      414 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/direct_integrator_z3.py
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.647161 rfb_mc-0.0.8/rfb_mc/component/eamp/
--rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/__init__.py
--rw-rw-rw-   0        0        0     9096 2021-04-26 14:08:44.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_edge_scheduler.py
--rw-rw-rw-   0        0        0     4590 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_rfm.py
--rw-rw-rw-   0        0        0     3300 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_rfmi_z3.py
--rw-rw-rw-   0        0        0      821 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/primes.py
--rw-rw-rw-   0        0        0     9937 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/primes.txt
--rw-rw-rw-   0        0        0     1425 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/eamp/utility.py
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.650136 rfb_mc-0.0.8/rfb_mc/component/helper/
--rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/helper/__init__.py
--rw-rw-rw-   0        0        0     2724 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/helper/z3_helper.py
--rw-rw-rw-   0        0        0      347 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/in_memory_store.py
--rw-rw-rw-   0        0        0     9424 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/multi_processing_integrator.py
--rw-rw-rw-   0        0        0      969 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/multi_processing_integrator_z3.py
--rw-rw-rw-   0        0        0     4898 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/component/runner_z3.py
--rw-rw-rw-   0        0        0     1302 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/integrator.py
--rw-rw-rw-   0        0        0     3466 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/restrictive_formula_module.py
--rw-rw-rw-   0        0        0     1347 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/restrictive_formula_module_implementation.py
--rw-rw-rw-   0        0        0     3377 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/runner.py
--rw-rw-rw-   0        0        0      178 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/runner_random.py
--rw-rw-rw-   0        0        0     1926 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/scheduler.py
--rw-rw-rw-   0        0        0     4312 2021-04-27 13:50:56.000000 rfb_mc-0.0.8/rfb_mc/serialization.py
--rw-rw-rw-   0        0        0     1848 2021-04-26 13:53:06.000000 rfb_mc-0.0.8/rfb_mc/store.py
--rw-rw-rw-   0        0        0      953 2021-04-26 08:10:47.000000 rfb_mc-0.0.8/rfb_mc/types.py
-drwxrwxrwx   0        0        0        0 2021-04-27 14:22:04.627815 rfb_mc-0.0.8/rfb_mc.egg-info/
--rw-rw-rw-   0        0        0      590 2021-04-27 14:22:04.000000 rfb_mc-0.0.8/rfb_mc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2021-04-27 14:22:04.000000 rfb_mc-0.0.8/rfb_mc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-27 14:22:04.000000 rfb_mc-0.0.8/rfb_mc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-04-27 14:22:04.000000 rfb_mc-0.0.8/rfb_mc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-04-27 14:22:04.654600 rfb_mc-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      662 2021-04-27 14:21:47.000000 rfb_mc-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.077077 rfb_mc-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       40 2021-04-28 10:45:07.000000 rfb_mc-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      590 2021-04-28 12:12:47.076581 rfb_mc-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      145 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.050788 rfb_mc-0.0.9/rfb_mc/
+-rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/__init__.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.064181 rfb_mc-0.0.9/rfb_mc/component/
+-rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/__init__.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.065669 rfb_mc-0.0.9/rfb_mc/component/aws/
+-rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/aws/__init__.py
+-rw-rw-rw-   0        0        0     6758 2021-04-26 13:51:22.000000 rfb_mc-0.0.9/rfb_mc/component/aws/dynamodb_store.py
+-rw-rw-rw-   0        0        0     3629 2021-04-27 14:46:48.000000 rfb_mc-0.0.9/rfb_mc/component/direct_integrator.py
+-rw-rw-rw-   0        0        0      414 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/direct_integrator_z3.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.074101 rfb_mc-0.0.9/rfb_mc/component/eamp/
+-rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/__init__.py
+-rw-rw-rw-   0        0        0    10295 2021-04-28 12:09:33.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_edge_scheduler.py
+-rw-rw-rw-   0        0        0     4590 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_rfm.py
+-rw-rw-rw-   0        0        0     3300 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_rfmi_z3.py
+-rw-rw-rw-   0        0        0      821 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/primes.py
+-rw-rw-rw-   0        0        0     9937 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/primes.txt
+-rw-rw-rw-   0        0        0     1425 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/eamp/utility.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.075589 rfb_mc-0.0.9/rfb_mc/component/helper/
+-rw-rw-rw-   0        0        0        0 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/helper/__init__.py
+-rw-rw-rw-   0        0        0     2724 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/helper/z3_helper.py
+-rw-rw-rw-   0        0        0      347 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/in_memory_store.py
+-rw-rw-rw-   0        0        0     9424 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/multi_processing_integrator.py
+-rw-rw-rw-   0        0        0      969 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/component/multi_processing_integrator_z3.py
+-rw-rw-rw-   0        0        0     5214 2021-04-27 14:45:19.000000 rfb_mc-0.0.9/rfb_mc/component/runner_z3.py
+-rw-rw-rw-   0        0        0     1302 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/integrator.py
+-rw-rw-rw-   0        0        0     3466 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/restrictive_formula_module.py
+-rw-rw-rw-   0        0        0     1347 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/restrictive_formula_module_implementation.py
+-rw-rw-rw-   0        0        0     3377 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/runner.py
+-rw-rw-rw-   0        0        0      178 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/runner_random.py
+-rw-rw-rw-   0        0        0     1926 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/scheduler.py
+-rw-rw-rw-   0        0        0     4312 2021-04-27 13:50:56.000000 rfb_mc-0.0.9/rfb_mc/serialization.py
+-rw-rw-rw-   0        0        0     1848 2021-04-26 13:53:06.000000 rfb_mc-0.0.9/rfb_mc/store.py
+-rw-rw-rw-   0        0        0      953 2021-04-26 08:10:47.000000 rfb_mc-0.0.9/rfb_mc/types.py
+drwxrwxrwx   0        0        0        0 2021-04-28 12:12:47.057734 rfb_mc-0.0.9/rfb_mc.egg-info/
+-rw-rw-rw-   0        0        0      590 2021-04-28 12:12:46.000000 rfb_mc-0.0.9/rfb_mc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2021-04-28 12:12:47.000000 rfb_mc-0.0.9/rfb_mc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-28 12:12:46.000000 rfb_mc-0.0.9/rfb_mc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2021-04-28 12:12:47.000000 rfb_mc-0.0.9/rfb_mc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-04-28 12:12:47.077573 rfb_mc-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      702 2021-04-28 12:12:13.000000 rfb_mc-0.0.9/setup.py
```

### Comparing `rfb_mc-0.0.8/LICENSE` & `rfb_mc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/PKG-INFO` & `rfb_mc-0.0.9/rfb_mc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rfb_mc
-Version: 0.0.8
+Name: rfb-mc
+Version: 0.0.9
 Summary: Performs model counting using restrictive formulas
 Home-page: https://github.com/Meterius/rfb-mc
 Author: Jonah Leander Hoff
 Author-email: jonah-hoff@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Meterius/rfb-mc/issues
 Description: # Restrictive Formula based Model Counting
```

### Comparing `rfb_mc-0.0.8/rfb_mc/component/aws/dynamodb_store.py` & `rfb_mc-0.0.9/rfb_mc/component/aws/dynamodb_store.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/direct_integrator.py` & `rfb_mc-0.0.9/rfb_mc/component/direct_integrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         )
 
         algorithm_generator = scheduler.run()
         prev_intermediate_result = None
 
         s1 = perf_counter()
 
+        self._print_debug("Starting integrator run")
+
         try:
             # execute tasks until the algorithm stops the iteration thus indicating the final result
             while True:
                 # execute an algorithm step
                 algorithm_yield = next(algorithm_generator)
 
                 # if the intermediate result has changed, it should be published via a yield
```

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_edge_scheduler.py` & `rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_edge_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,14 +229,40 @@
         model_count / (1 + epsilon) <= geometric_mean <= model_count * (1 + epsilon).
         """
 
         g, lg = EampEdgeScheduler.get_g_and_lg(a)
         return int(ceil(0.5 * log(2 * lg / g, 1 + epsilon)))
 
     @staticmethod
+    def get_a_for_fixed_q_that_ensures_upper_bound_for_multiplicative_gap_of_result(
+        q: int,
+        epsilon: float,
+    ) -> int:
+        """
+        Returns the minimal parameter a that ensures that for the given q we have,
+        get_upper_bound_for_multiplicative_gap_of_result(a, q) <= (1 + epsilon) ** 2.
+        That condition is equivalent to the statement that the geometric mean of the final edge interval
+        is a multiplicative approximation with error epsilon i.e.
+        model_count / (1 + epsilon) <= geometric_mean <= model_count * (1 + epsilon).
+        """
+
+        if 2 ** (1 / q) >= (1 + epsilon) ** 2:
+            raise ValueError(f"For epsilon={epsilon} and q={q} "
+                             f"i.e. (1 + epsilon) ** 2 = {(1 + epsilon) ** 2}, higher a "
+                             f"values will only be able to converge to {2 ** (1 / q)} thus epsilon "
+                             f"{sqrt(2 ** (1 / q)) - 1}")
+
+        # TODO: replace by proper formula
+        a = 1
+        while EampEdgeScheduler.get_upper_bound_for_multiplicative_gap_of_result(a, q) > (1 + epsilon) ** 2:
+            a += 1
+
+        return a
+
+    @staticmethod
     def get_upper_bound_for_multiplicative_gap_of_result(a: int, q: int) -> float:
         """
         Returns an upper bound on the multiplicative gap of the final edge interval returned
         by the eamp edge scheduler.
         """
 
         g, lg = EampEdgeScheduler.get_g_and_lg(a)
```

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_rfm.py` & `rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_rfm.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/eamp_rfmi_z3.py` & `rfb_mc-0.0.9/rfb_mc/component/eamp/eamp_rfmi_z3.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/primes.py` & `rfb_mc-0.0.9/rfb_mc/component/eamp/primes.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/primes.txt` & `rfb_mc-0.0.9/rfb_mc/component/eamp/primes.txt`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/eamp/utility.py` & `rfb_mc-0.0.9/rfb_mc/component/eamp/utility.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/helper/z3_helper.py` & `rfb_mc-0.0.9/rfb_mc/component/helper/z3_helper.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/multi_processing_integrator.py` & `rfb_mc-0.0.9/rfb_mc/component/multi_processing_integrator.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/multi_processing_integrator_z3.py` & `rfb_mc-0.0.9/rfb_mc/component/multi_processing_integrator_z3.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/component/runner_z3.py` & `rfb_mc-0.0.9/rfb_mc/component/runner_z3.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 
 class RunnerZ3(RunnerBase[FormulaParamsZ3, RfmiGenerationArgsZ3, z3.BoolRef]):
     def __init__(
         self,
         params: Params,
         formula_params: FormulaParamsZ3,
     ):
-        super().__init__(params, formula_params)
+        super().__init__(params, FormulaParamsZ3(
+            # translates the contexts, thus the formula and variables need not be created with the context
+            # the z3 runner will use
+            formula=formula_params.formula.translate(z3.main_ctx()),
+            variables=[x.translate(z3.main_ctx()) for x in formula_params.variables],
+        ))
 
         # maps q to a solver that has a q-times conjunction asserted
         self._solver_map: Dict[int, Tuple[z3.Solver, List[z3.BitVecRef]]] = {}
 
     def _get_solver(self, q: int) -> (z3.Solver, List[z3.BitVecRef]):
         """
         Returns the solver and cloned variables, of which the solver
```

### Comparing `rfb_mc-0.0.8/rfb_mc/integrator.py` & `rfb_mc-0.0.9/rfb_mc/integrator.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/restrictive_formula_module.py` & `rfb_mc-0.0.9/rfb_mc/restrictive_formula_module.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/restrictive_formula_module_implementation.py` & `rfb_mc-0.0.9/rfb_mc/restrictive_formula_module_implementation.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/runner.py` & `rfb_mc-0.0.9/rfb_mc/runner.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/scheduler.py` & `rfb_mc-0.0.9/rfb_mc/scheduler.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/serialization.py` & `rfb_mc-0.0.9/rfb_mc/serialization.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/store.py` & `rfb_mc-0.0.9/rfb_mc/store.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc/types.py` & `rfb_mc-0.0.9/rfb_mc/types.py`

 * *Files identical despite different names*

### Comparing `rfb_mc-0.0.8/rfb_mc.egg-info/PKG-INFO` & `rfb_mc-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rfb-mc
-Version: 0.0.8
+Name: rfb_mc
+Version: 0.0.9
 Summary: Performs model counting using restrictive formulas
 Home-page: https://github.com/Meterius/rfb-mc
 Author: Jonah Leander Hoff
 Author-email: jonah-hoff@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Meterius/rfb-mc/issues
 Description: # Restrictive Formula based Model Counting
```

### Comparing `rfb_mc-0.0.8/rfb_mc.egg-info/SOURCES.txt` & `rfb_mc-0.0.9/rfb_mc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

