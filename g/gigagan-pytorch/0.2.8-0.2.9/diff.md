# Comparing `tmp/gigagan-pytorch-0.2.8.tar.gz` & `tmp/gigagan-pytorch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagan-pytorch-0.2.8.tar", last modified: Wed Jul 26 14:38:37 2023, max compression
+gzip compressed data, was "gigagan-pytorch-0.2.9.tar", last modified: Sat Jul 29 16:50:37 2023, max compression
```

## Comparing `gigagan-pytorch-0.2.8.tar` & `gigagan-pytorch-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/gigagan_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    83779 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/gigagan_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/open_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/unet_upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/gigagan_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 14:38:37.000000 gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:38:37.021111 gigagan-pytorch-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-26 14:38:27.000000 gigagan-pytorch-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:50:37.326774 gigagan-pytorch-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-29 16:50:37.326774 gigagan-pytorch-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:50:37.326774 gigagan-pytorch-0.2.9/gigagan_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83823 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/gigagan_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/open_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/unet_upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/gigagan_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 16:50:37.326774 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-29 16:50:37.000000 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-29 16:50:37.000000 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 16:50:37.000000 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-29 16:50:37.000000 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 16:50:37.000000 gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 16:50:37.326774 gigagan-pytorch-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-29 16:50:28.000000 gigagan-pytorch-0.2.9/setup.py
```

### Comparing `gigagan-pytorch-0.2.8/LICENSE` & `gigagan-pytorch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/PKG-INFO` & `gigagan-pytorch-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.8/README.md` & `gigagan-pytorch-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 - All the maintainers at <a href="https://github.com/mlfoundations/open_clip">OpenClip</a>, for their SOTA open sourced contrastive learning text-image models
 
 - <a href="https://github.com/XavierXiao">Xavier</a> for the very helpful code review, and for discussions on how the scale invariance in the discriminator should be built!
 
 - <a href="https://github.com/CerebralSeed">@CerebralSeed</a> for pull requesting the initial sampling code for both the generator and upsampler!
 
+- <a href="https://github.com/randintgenr ">Keerth</a> for the code review and pointing out some discrepancies with the paper!
+
 ## Install
 
 ```bash
 $ pip install gigagan-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -8,41 +8,42 @@
 ## Appreciation - StabilityAI and ð¤_Huggingface for the generous
 sponsorship, as well as my other sponsors, for affording me the independence to
 open source artificial intelligence. - ð¤_Huggingface for their accelerate
 library - All the maintainers at OpenClip, for their SOTA open sourced
 contrastive learning text-image models - Xavier for the very helpful code
 review, and for discussions on how the scale invariance in the discriminator
 should be built! - @CerebralSeed for pull requesting the initial sampling code
-for both the generator and upsampler! ## Install ```bash $ pip install gigagan-
-pytorch ``` ## Usage Simple unconditional GAN, for starters ```python import
-torch from gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN
-( generator = dict( dim_capacity = 8, style_network = dict( dim = 64, depth = 4
-), image_size = 256, dim_max = 512, num_skip_layers_excite = 4, unconditional =
-True ), discriminator = dict( dim_capacity = 16, dim_max = 512, image_size =
-256, num_skip_layers_excite = 4, unconditional = True ), amp = True ).cuda() #
-dataset dataset = ImageDataset( folder = '/path/to/your/data', image_size = 256
-) dataloader = dataset.get_dataloader(batch_size = 1) # you must then set the
-dataloader for the GAN before training gan.set_dataloader(dataloader) #
-training the discriminator and generator alternating # for 100 steps in this
-example, batch size 1, gradient accumulated 8 times gan( steps = 100,
-grad_accum_every = 8 ) # after much training images = gan.generate(batch_size =
-4) # (4, 3, 256, 256) ``` For unconditional Unet Upsampler ```python import
-torch from gigagan_pytorch import ( GigaGAN, ImageDataset ) gan = GigaGAN
-( train_upsampler = True, # set this to True generator = dict( style_network =
-dict( dim = 64, depth = 4 ), dim = 32, image_size = 256, input_image_size = 64,
+for both the generator and upsampler! - Keerth for the code review and pointing
+out some discrepancies with the paper! ## Install ```bash $ pip install
+gigagan-pytorch ``` ## Usage Simple unconditional GAN, for starters ```python
+import torch from gigagan_pytorch import ( GigaGAN, ImageDataset ) gan =
+GigaGAN( generator = dict( dim_capacity = 8, style_network = dict( dim = 64,
+depth = 4 ), image_size = 256, dim_max = 512, num_skip_layers_excite = 4,
 unconditional = True ), discriminator = dict( dim_capacity = 16, dim_max = 512,
-image_size = 256, num_skip_layers_excite = 4, multiscale_input_resolutions =
-(128,), unconditional = True ), amp = True ).cuda() dataset = ImageDataset
-( folder = '/path/to/your/data', image_size = 256 ) dataloader =
-dataset.get_dataloader(batch_size = 1) gan.set_dataloader(dataloader) #
-training the discriminator and generator alternating # for 100 steps in this
-example, batch size 1, gradient accumulated 8 times gan( steps = 100,
-grad_accum_every = 8 ) # after much training lowres = torch.randn(1, 3, 64,
-64).cuda() images = gan.generate(lowres) # (1, 3, 256, 256) ``` ## Losses * `G`
-- Generator * `MSG` - Multiscale Generator * `D` - Discriminator * `MSD` -
+image_size = 256, num_skip_layers_excite = 4, unconditional = True ), amp =
+True ).cuda() # dataset dataset = ImageDataset( folder = '/path/to/your/data',
+image_size = 256 ) dataloader = dataset.get_dataloader(batch_size = 1) # you
+must then set the dataloader for the GAN before training gan.set_dataloader
+(dataloader) # training the discriminator and generator alternating # for 100
+steps in this example, batch size 1, gradient accumulated 8 times gan( steps =
+100, grad_accum_every = 8 ) # after much training images = gan.generate
+(batch_size = 4) # (4, 3, 256, 256) ``` For unconditional Unet Upsampler
+```python import torch from gigagan_pytorch import ( GigaGAN, ImageDataset )
+gan = GigaGAN( train_upsampler = True, # set this to True generator = dict
+( style_network = dict( dim = 64, depth = 4 ), dim = 32, image_size = 256,
+input_image_size = 64, unconditional = True ), discriminator = dict
+( dim_capacity = 16, dim_max = 512, image_size = 256, num_skip_layers_excite =
+4, multiscale_input_resolutions = (128,), unconditional = True ), amp = True
+).cuda() dataset = ImageDataset( folder = '/path/to/your/data', image_size =
+256 ) dataloader = dataset.get_dataloader(batch_size = 1) gan.set_dataloader
+(dataloader) # training the discriminator and generator alternating # for 100
+steps in this example, batch size 1, gradient accumulated 8 times gan( steps =
+100, grad_accum_every = 8 ) # after much training lowres = torch.randn(1, 3,
+64, 64).cuda() images = gan.generate(lowres) # (1, 3, 256, 256) ``` ## Losses *
+`G` - Generator * `MSG` - Multiscale Generator * `D` - Discriminator * `MSD` -
 Multiscale Discriminator * `GP` - Gradient Penalty * `SSL` - Auxiliary
 Reconstruction in Discriminator (from Lightweight GAN) * `VD` - Vision-aided
 Discriminator * `VG` - Vision-aided Generator * `CL` - Generator Constrastive
 Loss * `MAL` - Matching Aware Loss A healthy run would have `G`, `MSG`, `D`,
 `MSD` with values hovering between `0` to `10`, and usually staying pretty
 constant. If at any time after 1k training steps these values persist at triple
 digits, that would mean something is wrong. It is ok for generator and
```

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/__init__.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/attend.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/data.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/gigagan_pytorch.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/gigagan_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     requires_grad: bool
 ):
     for p in m.parameters():
         p.requires_grad = requires_grad
 
 # activation functions
 
-def leaky_relu(neg_slope = 0.1):
+def leaky_relu(neg_slope = 0.2):
     return nn.LeakyReLU(neg_slope)
 
 def conv2d_3x3(dim_in, dim_out):
     return nn.Conv2d(dim_in, dim_out, 3, padding = 1)
 
 # tensor helpers
 
@@ -954,15 +954,15 @@
                 Noise(dim_out),
                 leaky_relu(),
                 adaptive_conv(dim_out, dim_out),
                 Noise(dim_out),
                 leaky_relu()
             ])
 
-            to_rgb = adaptive_conv(dim_out, channels)
+            to_rgb = AdaptiveConv2DMod(dim_out, channels, 1, num_conv_kernels = 1, demod = False)
 
             self_attn = cross_attn = rgb_upsample = upsample = None
 
             upsample_klass = Upsample if not pixel_shuffle_upsample else PixelShuffleUpsample
 
             upsample = upsample_klass(dim_in) if should_upsample else None
             rgb_upsample = upsample_klass(channels) if should_upsample_rgb else None
```

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/open_clip.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/optimizer.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch/unet_upsampler.py` & `gigagan-pytorch-0.2.9/gigagan_pytorch/unet_upsampler.py`

 * *Files identical despite different names*

### Comparing `gigagan-pytorch-0.2.8/gigagan_pytorch.egg-info/PKG-INFO` & `gigagan-pytorch-0.2.9/gigagan_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gigagan-pytorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: GigaGAN - Pytorch
 Home-page: https://github.com/lucidrains/ETSformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,generative adversarial networks
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gigagan-pytorch-0.2.8/setup.py` & `gigagan-pytorch-0.2.9/setup.py`

 * *Files identical despite different names*

