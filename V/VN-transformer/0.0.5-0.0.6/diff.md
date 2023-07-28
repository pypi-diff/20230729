# Comparing `tmp/VN-transformer-0.0.5.tar.gz` & `tmp/VN-transformer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.5.tar", last modified: Fri Jul 28 18:19:29 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.6.tar", last modified: Fri Jul 28 22:50:02 2023, max compression
```

## Comparing `VN-transformer-0.0.5.tar` & `VN-transformer-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 18:19:29.000000 VN-transformer-0.0.5/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:19:29.709806 VN-transformer-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 18:19:16.000000 VN-transformer-0.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.883736 VN-transformer-0.0.6/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/tests/test.py
```

### Comparing `VN-transformer-0.0.5/LICENSE` & `VN-transformer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.5/PKG-INFO` & `VN-transformer-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.5/README.md` & `VN-transformer-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.5/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.6/VN_transformer/VN_transformer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from einops.layers.torch import Rearrange, Reduce
 
 # helper
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def inner_dot_product(x, y, *, dim = -1, keepdim = True):
     return (x * y).sum(dim = dim, keepdim = keepdim)
 
 # layernorm
 
 class LayerNorm(nn.Module):
     def __init__(self, dim):
@@ -142,14 +145,36 @@
 
     def forward(self, x):
         norms = x.norm(dim = -1)
         x = x / rearrange(norms.clamp(min = self.eps), '... -> ... 1')
         ln_out = self.ln(norms)
         return x * rearrange(ln_out, '... -> ... 1')
 
+class VNWeightedPool(nn.Module):
+    def __init__(
+        self,
+        dim,
+        dim_out = None,
+        num_pooled_tokens = 1,
+        squeeze_out_pooled_dim = True
+    ):
+        super().__init__()
+        dim_out = default(dim_out, dim)
+        self.weight = nn.Parameter(torch.randn(num_pooled_tokens, dim, dim_out))
+        self.squeeze_out_pooled_dim = num_pooled_tokens == 1 and squeeze_out_pooled_dim
+
+    def forward(self, x):
+        out = einsum('b n d c, m d e -> b m e c', x, self.weight)
+
+        if not self.squeeze_out_pooled_dim:
+            return out
+
+        out = rearrange(out, 'b 1 d c -> b d c')
+        return out
+
 # equivariant VN transformer encoder
 
 class VNTransformerEncoder(nn.Module):
     def __init__(
         self,
         dim,
         *,
```

### Comparing `VN-transformer-0.0.5/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.6/VN_transformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.5/setup.py` & `VN-transformer-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.5/tests/test.py` & `VN-transformer-0.0.6/tests/test.py`

 * *Files identical despite different names*

