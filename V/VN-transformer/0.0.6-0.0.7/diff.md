# Comparing `tmp/VN-transformer-0.0.6.tar.gz` & `tmp/VN-transformer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.6.tar", last modified: Fri Jul 28 22:50:02 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.7.tar", last modified: Fri Jul 28 23:15:46 2023, max compression
```

## Comparing `VN-transformer-0.0.6.tar` & `VN-transformer-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.883736 VN-transformer-0.0.6/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 22:50:02.000000 VN-transformer-0.0.6/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 22:50:02.887736 VN-transformer-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 22:49:52.000000 VN-transformer-0.0.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/tests/test.py
```

### Comparing `VN-transformer-0.0.6/LICENSE` & `VN-transformer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.6/PKG-INFO` & `VN-transformer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.6/README.md` & `VN-transformer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.6/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.7/VN_transformer/VN_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,22 +83,28 @@
 class VNAttention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         dim_coor = 3,
-        bias_epsilon = 0.
+        bias_epsilon = 0.,
+        num_latents = None   # setting this would enable perceiver-like cross attention from latents to sequence, with the latents derived from VNWeightedPool
     ):
         super().__init__()
         self.scale = (dim_coor * dim_head) ** -0.5
         dim_inner = dim_head * heads
         self.heads = heads
 
-        self.to_qkv = VNLinear(dim, dim_inner * 3, bias_epsilon = bias_epsilon)
+        self.to_q_input = None
+        if exists(num_latents):
+            self.to_q_input = VNWeightedPool(dim, num_pooled_tokens = num_latents, squeeze_out_pooled_dim = False)
+
+        self.to_q = VNLinear(dim, dim_inner, bias_epsilon = bias_epsilon)
+        self.to_kv = VNLinear(dim, dim_inner * 2, bias_epsilon = bias_epsilon)
         self.to_out = VNLinear(dim_inner, dim, bias_epsilon = bias_epsilon)
 
     def forward(self, x, mask = None):
         """
         einstein notation
         b - batch
         n - sequence
@@ -107,15 +113,17 @@
         c - coordinate dimension (3 for 3d space)
         i - source sequence dimension
         j - target sequence dimension
         """
 
         c = x.shape[-1]
 
-        q, k, v = self.to_qkv(x).chunk(3, dim = -2)
+        q_input = self.to_q_input(x) if exists(self.to_q_input) else x
+
+        q, k, v = (self.to_q(q_input), *self.to_kv(x).chunk(2, dim = -2))
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) c -> b h n d c', h = self.heads), (q, k, v))
 
         q = q * self.scale
 
         sim = einsum('b h i d c, b h j d c -> b h i j', q, k)
 
         if exists(mask):
```

### Comparing `VN-transformer-0.0.6/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.7/VN_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.6/setup.py` & `VN-transformer-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.6/tests/test.py` & `VN-transformer-0.0.7/tests/test.py`

 * *Files identical despite different names*

