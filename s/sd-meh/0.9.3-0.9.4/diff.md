# Comparing `tmp/sd_meh-0.9.3.tar.gz` & `tmp/sd_meh-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.9.3.tar", max compression
+gzip compressed data, was "sd_meh-0.9.4.tar", max compression
```

## Comparing `sd_meh-0.9.3.tar` & `sd_meh-0.9.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1062 2023-07-24 13:44:17.967581 sd_meh-0.9.3/LICENSE.txt
--rw-r--r--   0        0        0     1987 2023-07-24 13:44:17.967581 sd_meh-0.9.3/README.md
--rw-r--r--   0        0        0      390 2023-07-24 13:44:17.967581 sd_meh-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/__init__.py
--rw-r--r--   0        0        0    13790 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/merge.py
--rw-r--r--   0        0        0     6626 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1606 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/model.py
--rw-r--r--   0        0        0    10306 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/presets.py
--rw-r--r--   0        0        0    83496 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/rebasin.py
--rw-r--r--   0        0        0     3481 2023-07-24 13:44:17.967581 sd_meh-0.9.3/sd_meh/utils.py
--rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 sd_meh-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-29 19:14:41.606939 sd_meh-0.9.4/LICENSE.txt
+-rw-r--r--   0        0        0     1987 2023-07-29 19:14:41.606939 sd_meh-0.9.4/README.md
+-rw-r--r--   0        0        0      390 2023-07-29 19:14:41.606939 sd_meh-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/__init__.py
+-rw-r--r--   0        0        0    13751 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/merge.py
+-rw-r--r--   0        0        0     6626 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1606 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/model.py
+-rw-r--r--   0        0        0    10306 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/presets.py
+-rw-r--r--   0        0        0    83654 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     3481 2023-07-29 19:14:41.606939 sd_meh-0.9.4/sd_meh/utils.py
+-rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 sd_meh-0.9.4/PKG-INFO
```

### Comparing `sd_meh-0.9.3/LICENSE.txt` & `sd_meh-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/README.md` & `sd_meh-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/sd_meh/merge.py` & `sd_meh-0.9.4/sd_meh/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,14 @@
         except AttributeError as e:
             raise ValueError(f"{merge_mode} not implemented, aborting merge!") from e
 
         merge_args = get_merge_method_args(current_bases, thetas, key, work_device)
 
         # dealing wiht pix2pix and inpainting models
         if (a_size := merge_args["a"].size()) != (b_size := merge_args["b"].size()):
-            print(key, a_size, b_size)
             if a_size[1] > b_size[1]:
                 merged_key = merge_args["a"]
             else:
                 merged_key = merge_args["b"]
         else:
             merged_key = merge_method(**merge_args).to(device)
```

### Comparing `sd_meh-0.9.3/sd_meh/merge_methods.py` & `sd_meh-0.9.4/sd_meh/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/sd_meh/model.py` & `sd_meh-0.9.4/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/sd_meh/presets.py` & `sd_meh-0.9.4/sd_meh/presets.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/sd_meh/rebasin.py` & `sd_meh-0.9.4/sd_meh/rebasin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2195,17 +2195,21 @@
 def apply_permutation(ps: PermutationSpec, perm, params):
     """Apply a `perm` to `params`."""
     return {k: get_permuted_param(ps, perm, k, params) for k in params.keys()}
 
 
 def update_model_a(ps: PermutationSpec, perm, model_a, new_alpha):
     for k in model_a:
-        model_a[k] = model_a[k] * (1 - new_alpha) + new_alpha * get_permuted_param(
-            ps, perm, k, model_a
-        )
+        try:
+            perm_params = get_permuted_param(
+                ps, perm, k, model_a
+            )
+            model_a[k] = model_a[k] * (1 - new_alpha) + new_alpha * perm_params
+        except RuntimeError: # dealing with pix2pix and inpainting models
+            continue
     return model_a
 
 
 def inner_matching(
     n,
     ps,
     p,
```

### Comparing `sd_meh-0.9.3/sd_meh/utils.py` & `sd_meh-0.9.4/sd_meh/utils.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.9.3/PKG-INFO` & `sd_meh-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.9.3
+Version: 0.9.4
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

