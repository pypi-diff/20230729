# Comparing `tmp/VN-transformer-0.0.7.tar.gz` & `tmp/VN-transformer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VN-transformer-0.0.7.tar", last modified: Fri Jul 28 23:15:46 2023, max compression
+gzip compressed data, was "VN-transformer-0.0.8.tar", last modified: Sat Jul 29 17:31:54 2023, max compression
```

## Comparing `VN-transformer-0.0.7.tar` & `VN-transformer-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/VN_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/VN_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/VN_transformer/rotations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/VN_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 23:15:46.000000 VN-transformer-0.0.7/VN_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:15:46.276082 VN-transformer-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-28 23:15:35.000000 VN-transformer-0.0.7/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/VN_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/VN_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/VN_transformer/rotations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/VN_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 17:31:54.000000 VN-transformer-0.0.8/VN_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:31:54.232356 VN-transformer-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-29 17:31:42.000000 VN-transformer-0.0.8/tests/test.py
```

### Comparing `VN-transformer-0.0.7/LICENSE` & `VN-transformer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `VN-transformer-0.0.7/PKG-INFO` & `VN-transformer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.7/README.md` & `VN-transformer-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <img src="./vn-transformer.png" width="300px"></img>
 
-## VN (Vector Neuron) Transformer (wip)
+## VN (Vector Neuron) Transformer
 
 A <a href="https://arxiv.org/abs/2206.04176">Transformer made of Rotation-equivariant Attention</a> using <a href="https://arxiv.org/abs/2104.12229">Vector Neurons</a>
 
 <a href="https://openreview.net/forum?id=EiX2L4sDPG">Open Review</a>
 
 ## Install
 
@@ -19,14 +19,15 @@
 from VN_transformer import VNTransformer
 
 model = VNTransformer(
     dim = 64,
     depth = 2,
     dim_head = 64,
     heads = 8,
+    dim_feat = 64,       # will default to early fusion, since this was the best performing
     beta_epsilon = 1e-6  # in this paper, they propose breaking equivariance with a tiny bit of bias noise in the VN linear. they claim this leads to improved stability. setting this to 0 would turn off the epsilon approximate equivariance
 )
 
 feats = torch.randn(1, 32, 64)
 coors = torch.randn(1, 32, 3)    # (batch, sequence, spatial coordinates)
 
 feats, coors = model(feats, coors)
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-[./vn-transformer.png] ## VN (Vector Neuron) Transformer (wip) A Transformer
-made_of_Rotation-equivariant_Attention using Vector_Neurons Open_Review ##
-Install ```bash $ pip install VN-transformer ``` ## Usage ```python import
-torch from VN_transformer import VNTransformer model = VNTransformer( dim = 64,
-depth = 2, dim_head = 64, heads = 8, beta_epsilon = 1e-6 # in this paper, they
-propose breaking equivariance with a tiny bit of bias noise in the VN linear.
-they claim this leads to improved stability. setting this to 0 would turn off
-the epsilon approximate equivariance ) feats = torch.randn(1, 32, 64) coors =
+[./vn-transformer.png] ## VN (Vector Neuron) Transformer A Transformer_made_of
+Rotation-equivariant_Attention using Vector_Neurons Open_Review ## Install
+```bash $ pip install VN-transformer ``` ## Usage ```python import torch from
+VN_transformer import VNTransformer model = VNTransformer( dim = 64, depth = 2,
+dim_head = 64, heads = 8, dim_feat = 64, # will default to early fusion, since
+this was the best performing beta_epsilon = 1e-6 # in this paper, they propose
+breaking equivariance with a tiny bit of bias noise in the VN linear. they
+claim this leads to improved stability. setting this to 0 would turn off the
+epsilon approximate equivariance ) feats = torch.randn(1, 32, 64) coors =
 torch.randn(1, 32, 3) # (batch, sequence, spatial coordinates) feats, coors =
 model(feats, coors) ``` ## Tests Confidence in equivariance ```bash $ python
 setup.py test ``` ## Todo - [ ] complete the perceiver like feature aggregation
 - [ ] offer both early and late fusion within `VNTransformer` - [ ] see if it
 is straightforward to make translation in/equivariant - [ ] test on protein
 backbone denoising if above could be done ## Citations ```bibtex @inproceedings
 {Assaad2022VNTransformerRA, title = {VN-Transformer: Rotation-Equivariant
```

### Comparing `VN-transformer-0.0.7/VN_transformer/VN_transformer.py` & `VN-transformer-0.0.8/VN_transformer/VN_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -248,46 +248,60 @@
 
 class VNTransformer(nn.Module):
     def __init__(
         self,
         *,
         dim,
         depth,
+        dim_feat = None,
         dim_head = 64,
         heads = 8,
+        dim_coor = 3,
         reduce_dim_out = True,
         bias_epsilon = 0.
     ):
         super().__init__()
+        dim_feat = default(dim_feat, 0)
+        self.dim_feat = dim_feat
+        self.dim_coor_total = dim_coor + dim_feat
 
         self.vn_proj_in = nn.Sequential(
             Rearrange('... c -> ... 1 c'),
             VNLinear(1, dim, bias_epsilon = bias_epsilon)
         )
 
         self.encoder = VNTransformerEncoder(
             dim = dim,
             depth = depth,
             dim_head = dim_head,
             heads = heads,
-            bias_epsilon = bias_epsilon
+            bias_epsilon = bias_epsilon,
+            dim_coor = self.dim_coor_total
         )
 
         if reduce_dim_out:
             self.vn_proj_out = nn.Sequential(
                 VNLayerNorm(dim),
                 VNLinear(dim, 1, bias_epsilon = bias_epsilon),
                 Rearrange('... 1 c -> ... c')
             )
         else:
             self.vn_proj_out = nn.Identity()
 
     def forward(
         self,
-        feats,
         coors,
+        *,
+        feats = None,
         mask = None
     ):
+        if exists(feats):
+            assert feats.ndim == 3
+            assert feats.shape[-1] == self.dim_feat, f'dim_feat should be set to {feats.shape[-1]}'
+            coors = torch.cat((coors, feats), dim = -1)
+
+        assert coors.shape[-1] == self.dim_coor_total
+
         coors = self.vn_proj_in(coors)
         coors = self.encoder(coors, mask = mask)
         coors = self.vn_proj_out(coors)
         return feats, coors
```

### Comparing `VN-transformer-0.0.7/VN_transformer.egg-info/PKG-INFO` & `VN-transformer-0.0.8/VN_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VN-transformer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Vector Neuron Transformer (VN-Transformer)
 Home-page: https://github.com/lucidrains/VN-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,equivariance,vector neurons,transformers,attention mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `VN-transformer-0.0.7/setup.py` & `VN-transformer-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'VN-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Vector Neuron Transformer (VN-Transformer)',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/VN-transformer',
   keywords = [
```

### Comparing `VN-transformer-0.0.7/tests/test.py` & `VN-transformer-0.0.8/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,40 @@
     model = VNTransformer(
         dim = 64,
         depth = 2,
         dim_head = 64,
         heads = 8
     )
 
+    coors = torch.randn(1, 32, 3)
+    mask  = torch.ones(1, 32).bool()
+
+    R   = rot(*torch.randn(3))
+    _, out1 = model(coors @ R, mask = mask)
+    out2 = model(coors, mask = mask)[1] @ R
+
+    assert torch.allclose(out1, out2, atol = 1e-6), 'is not equivariant'
+
+# # test equivariance
+
+def test_equivariance_with_early_fusion():
+
+    model = VNTransformer(
+        dim = 64,
+        depth = 2,
+        dim_head = 64,
+        heads = 8,
+        dim_feat = 64
+    )
+
     feats = torch.randn(1, 32, 64)
     coors = torch.randn(1, 32, 3)
     mask  = torch.ones(1, 32).bool()
 
     R   = rot(*torch.randn(3))
-    _, out1 = model(feats, coors @ R, mask)
-    out2 = model(feats, coors, mask)[1] @ R
+    _, out1 = model(coors @ R, feats = feats, mask = mask)
+    out1 = out1[..., :3]
+
+    out2 = model(coors, feats = feats, mask = mask)[1]
+    out2 = out2[..., :3] @ R
 
     assert torch.allclose(out1, out2, atol = 1e-6), 'is not equivariant'
```

