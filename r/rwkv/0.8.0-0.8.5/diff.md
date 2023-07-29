# Comparing `tmp/rwkv-0.8.0.tar.gz` & `tmp/rwkv-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.8.0.tar", last modified: Mon Jun 26 03:15:20 2023, max compression
+gzip compressed data, was "rwkv-0.8.5.tar", last modified: Sat Jul 29 01:20:39 2023, max compression
```

## Comparing `rwkv-0.8.0.tar` & `rwkv-0.8.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.0/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.0/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4840 2023-06-26 03:15:20.000000 rwkv-0.8.0/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4370 2023-06-26 03:06:27.000000 rwkv-0.8.0/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-06-26 02:50:44.000000 rwkv-0.8.0/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-06-26 03:15:20.000000 rwkv-0.8.0/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.0/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.0/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4702 2023-04-27 19:18:02.000000 rwkv-0.8.0/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    33248 2023-05-20 13:47:14.000000 rwkv-0.8.0/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.0/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.0/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4840 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      374 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.5/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.5/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 01:20:39.000000 rwkv-0.8.5/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.5/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-27 23:10:42.000000 rwkv-0.8.5/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 01:20:39.000000 rwkv-0.8.5/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.5/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     2934 2023-07-24 21:43:08.000000 rwkv-0.8.5/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.5/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4897 2023-07-24 21:43:08.000000 rwkv-0.8.5/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    39350 2023-07-29 01:08:41.000000 rwkv-0.8.5/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.5/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.5/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.5/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.8.0/LICENSE` & `rwkv-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.0/PKG-INFO` & `rwkv-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.0
+Version: 0.8.5
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -76,15 +76,15 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
-                     alpha_decay=0.996, # gradually decay the penalty
+                     alpha_decay = 0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
```

### Comparing `rwkv-0.8.0/README.md` & `rwkv-0.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
-                     alpha_decay=0.996, # gradually decay the penalty
+                     alpha_decay = 0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
```

### Comparing `rwkv-0.8.0/src/rwkv/cuda/operators.cu` & `rwkv-0.8.5/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.0/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.5/src/rwkv/cuda/wrapper.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -112,18 +112,24 @@
             y.data_ptr<float>());
         break;
     default:
         assert(false && "Only FP16 and FP32 are currently supported");
     }
 }
 
+using torch::Tensor;
+
+void gemm_fp16_cublas(Tensor a, Tensor b, Tensor c);
+
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
     m.def("wkv_forward", &wkv_forward, "wkv forward");
     m.def("mm8_seq", &mm8_seq, "mm8 seq");
     m.def("mm8_one", &mm8_one, "mm8 one");
+    m.def("gemm_fp16_cublas", &gemm_fp16_cublas, "gemv fp16 cublas");
 }
 
 TORCH_LIBRARY(rwkv, m) {
     m.def("wkv_forward", wkv_forward);
     m.def("mm8_seq", mm8_seq);
     m.def("mm8_one", mm8_one);
+    m.def("gemm_fp16_cublas", gemm_fp16_cublas);
 }
```

### Comparing `rwkv-0.8.0/src/rwkv/model.py` & `rwkv-0.8.5/src/rwkv/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ########################################################################################################
 # The RWKV Language Model - https://github.com/BlinkDL/RWKV-LM
 ########################################################################################################
 
+from typing import Optional
 import types, gc, os, time, re
 import torch
 from torch.nn import functional as F
 torch.backends.cudnn.benchmark = True
 torch.backends.cudnn.allow_tf32 = True
 torch.backends.cuda.matmul.allow_tf32 = True
 current_path = os.path.dirname(os.path.abspath(__file__))
@@ -24,15 +25,15 @@
     MyFunction = __nop
     MyStatic = __nop
 
 if os.environ.get('RWKV_CUDA_ON') == '1':
     from torch.utils.cpp_extension import load
     load(
         name=f"wkv_cuda",
-        sources=[f"{current_path}/cuda/wrapper.cpp", f"{current_path}/cuda/operators.cu"],
+        sources=[f"{current_path}/cuda/wrapper.cpp", f"{current_path}/cuda/operators.cu", f"{current_path}/cuda/gemm_fp16_cublas.cpp"],
         verbose=True,
         extra_cuda_cflags=["-t 4", "-std=c++17", "--use_fast_math", "-O3", "--extra-device-vectorization"],
         is_python_module=False)
 
     @MyStatic
     def cuda_wkv(T: int, C: int, w, u, k, v, aa, bb, pp):
         assert 1 * C % min(C, 32) == 0
@@ -46,35 +47,54 @@
         torch.ops.rwkv.wkv_forward(1, T, C, w, u, k, v, y, aa, bb, pp)
         return y, aa, bb, pp
     @MyStatic
     def cuda_mm8_seq(B: int, N: int, M: int, x, w, mx, rx, my, ry):
         assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype
         assert x.dtype == torch.float32 or x.dtype == torch.float16
         assert w.dtype == torch.uint8
-        assert x.shape == [B, N]
-        assert w.shape == [N, M]
-        assert rx.shape == mx.shape == [M]
-        assert ry.shape == my.shape == [N, 1]
+        assert x.shape == (B, N)
+        assert w.shape == (N, M)
+        assert rx.shape == mx.shape == (M,)
+        assert ry.shape == my.shape == (N, 1)
         y = torch.empty((B, M), device=w.device, dtype=x.dtype)
         torch.ops.rwkv.mm8_seq(B, N, M, x, w, mx, rx, my, ry, y)
         return y
     @MyStatic
     def cuda_mm8_one(N: int, M: int, x, w, mx, rx, my, ry):
         assert x.dtype == mx.dtype == rx.dtype == my.dtype == ry.dtype
         assert x.dtype == torch.float32 or x.dtype == torch.float16
         assert w.dtype == torch.uint8
-        assert x.shape == [N]
-        assert w.shape == [N, M]
-        assert rx.shape == mx.shape == [M]
-        assert ry.shape == my.shape == [N, 1]
+        assert x.shape == (N,)
+        assert w.shape == (N, M)
+        assert rx.shape == mx.shape == (M,)
+        assert ry.shape == my.shape == (N, 1)
         y = torch.zeros((M,), device=w.device, dtype=torch.float32)
         torch.ops.rwkv.mm8_one(N, M, x, w, mx, rx, my, ry, y)
         return y.to(dtype=x.dtype)
+    @MyStatic
+    def gemm(a, b, output_dtype: Optional[torch.dtype]=None):
+        if output_dtype is None:
+            output_dtype = a.dtype
+        if a.dtype == b.dtype == torch.float16 and a.device.type == 'cuda':
+            assert len(b.shape) == 2
+            if len(a.shape) == 1:
+                c = torch.empty((b.shape[-1],), dtype=output_dtype, device=a.device)
+                a = a.unsqueeze(0)
+            else:
+                c = torch.empty((a.shape[0], b.shape[-1]), dtype=output_dtype, device=a.device)
+            torch.ops.rwkv.gemm_fp16_cublas(a, b, c)
+            return c
+        else:
+            return (a @ b).to(output_dtype)
 else:
     os.environ["RWKV_CUDA_ON"] = '0'
+    def gemm(a, b, output_dtype: Optional[torch.dtype]=None):
+        if output_dtype is None:
+            output_dtype = a.dtype
+        return (a @ b).to(output_dtype)
 
 ########################################################################################################
 
 class RWKV(MyModule):
     def __init__(self, model, strategy, verbose = True, convert_and_save_and_exit = None):
         super().__init__()
         if verbose:
@@ -116,17 +136,22 @@
                 del w['_strategy']
                 del w['_version']
                 del w['_rescale_layer']
             
             args.n_embd = w['emb.weight'].shape[1]
             args.n_layer = 0
             keys = list(w.keys())
+            self.version = 4
             for x in keys:
                 layer_id = int(x.split('.')[1]) if ('blocks.' in x) else 0
                 args.n_layer = max(args.n_layer, layer_id+1)
+                if 'ln_x' in x:
+                    self.version = 5
+                if self.version == 5 and 'att.time_decay' in x:
+                    args.n_head = w[x].shape[0]
 
             ####################### Compute strategy
 
             s = [x.strip().split(' ') for x in strategy.split('->')]
             plan = [0] * len(s)
             stream_i = -1
             stream_count = 0
@@ -223,17 +248,23 @@
 
                     if '.time_' in x:
                         w[x] = w[x].squeeze()
                     if 'key.weight' in x or 'value.weight' in x or 'receptance.weight' in x or 'output.weight' in x or 'head.weight' in x:
                         w[x] = w[x].t()
 
                     if '.time_decay' in x: # need fp32 for this
-                        w[x] = -torch.exp(w[x].float())
+                        if self.version == 4:
+                            w[x] = -torch.exp(w[x].float())
+                        elif self.version == 5:
+                            w[x] = torch.exp(-torch.exp(w[x].float())).reshape(-1,1,1)
                     elif '.time_first' in x: # need fp32 for this
-                        w[x] = w[x].float()
+                        if self.version == 4:
+                            w[x] = w[x].float()
+                        elif self.version == 5:
+                            w[x] = torch.exp(w[x].float()).reshape(-1,1,1)
                     else:
                         if (len(w[x].shape) == 2) and ('emb' not in x):
                             if WTYPE != torch.uint8:
                                 w[x] = w[x].to(dtype=WTYPE)
                             else:
                                 w[x] = w[x].float()
 
@@ -355,17 +386,17 @@
 
     @MyFunction
     def ffn_one(self, x, sx, ln_w, ln_b, k_mix, r_mix, kw, vw, rw, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         kx = xx * k_mix + sx * (1 - k_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
 
-        r = torch.sigmoid(rx @ rw)
-        vx = torch.square(torch.relu(kx @ kw))
-        out = r * (vx @ vw)
+        r = torch.sigmoid(gemm(rx, rw))
+        vx = torch.square(torch.relu(gemm(kx, kw)))
+        out = r * gemm(vx, vw)
         return x + out, xx
 
     @MyFunction
     def ffn_one_i8(self, x, sx, ln_w, ln_b, k_mix, r_mix, kw, vw, rw, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         kx = xx * k_mix + sx * (1 - k_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
@@ -380,17 +411,17 @@
     @MyFunction
     def ffn_seq(self, x, sx, ln_w, ln_b, k_mix, r_mix, kw, vw, rw, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
         kx = xx * k_mix + sx * (1 - k_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
 
-        r = torch.sigmoid(rx @ rw)
-        vx = torch.square(torch.relu(kx @ kw))
-        out = r * (vx @ vw)
+        r = torch.sigmoid(gemm(rx, rw))
+        vx = torch.square(torch.relu(gemm(kx, kw)))
+        out = r * gemm(vx, vw)
         return x + out, xx[-1,:]
 
     @MyFunction
     def ffn_seq_i8(self, x, sx, ln_w, ln_b, k_mix, r_mix, kw, vw, rw, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
         kx = xx * k_mix + sx * (1 - k_mix)
@@ -406,29 +437,29 @@
     @MyFunction
     def att_one(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         kx = xx * k_mix + sx * (1 - k_mix)
         vx = xx * v_mix + sx * (1 - v_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
 
-        r = torch.sigmoid(rx @ rw)
-        k = (kx @ kw).float()
-        v = (vx @ vw).float()
+        r = torch.sigmoid(gemm(rx, rw))
+        k = gemm(kx, kw, output_dtype=torch.float32)
+        v = gemm(vx, vw, output_dtype=torch.float32)
 
         ww = t_first + k
         p = torch.maximum(pp, ww)
         e1 = torch.exp(pp - p)
         e2 = torch.exp(ww - p)
         wkv = ((e1 * aa + e2 * v) / (e1 * bb + e2)).to(dtype=x.dtype)
         ww = t_decay + pp
         p = torch.maximum(ww, k)
         e1 = torch.exp(ww - p)
         e2 = torch.exp(k - p)
 
-        out = (r * wkv) @ ow
+        out = gemm(r * wkv, ow)
         return x + out, xx, e1 * aa + e2 * v, e1 * bb + e2, p
 
     @MyFunction
     def att_one_i8(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         kx = xx * k_mix + sx * (1 - k_mix)
         vx = xx * v_mix + sx * (1 - v_mix)
@@ -457,17 +488,17 @@
     def att_seq(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
         kx = xx * k_mix + sx * (1 - k_mix)
         vx = xx * v_mix + sx * (1 - v_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
 
-        r = torch.sigmoid(rx @ rw)
-        k = (kx @ kw).float()
-        v = (vx @ vw).float()
+        r = torch.sigmoid(gemm(rx, rw))
+        k = gemm(kx, kw, output_dtype=torch.float32)
+        v = gemm(vx, vw, output_dtype=torch.float32)
 
         T = x.shape[0]
         for t in range(T):
             kk = k[t]
             vv = v[t]
             ww = t_first + kk
             p = torch.maximum(pp, ww)
@@ -477,15 +508,15 @@
             ww = t_decay + pp
             p = torch.maximum(ww, kk)
             e1 = torch.exp(ww - p)
             e2 = torch.exp(kk - p)
             aa = e1 * aa + e2 * vv
             bb = e1 * bb + e2
             pp = p
-        out = (r * sx) @ ow
+        out = gemm(r * sx, ow)
         return x + out, xx[-1,:], aa, bb, pp
 
     @MyFunction
     def att_seq_i8(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
         sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
         kx = xx * k_mix + sx * (1 - k_mix)
@@ -513,30 +544,94 @@
             bb = e1 * bb + e2
             pp = p
         out = self.mm8_seq(r * sx, ow, omx, orx, omy, ory)
         return x + out, xx[-1,:], aa, bb, pp
 
     ########################################################################################################
 
+    @MyFunction
+    def att_one_v5(self, x, sx, s, ln_w, ln_b, lx_w, lx_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
+        xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
+        kx = xx * k_mix + sx * (1 - k_mix)
+        vx = xx * v_mix + sx * (1 - v_mix)
+        rx = xx * r_mix + sx * (1 - r_mix)
+
+        H = t_decay.shape[0]
+        S = x.shape[-1] // H
+
+        r = gemm(rx, rw).view(H, 1, S)
+        k = gemm(kx, kw).view(H, S, 1)
+        v = gemm(vx, vw).view(H, 1, S)
+        
+        a = (k @ v).float()
+        out = r @ (t_first * a + s).to(dtype=r.dtype)
+        s = a + t_decay * s
+
+        out = out.flatten()
+        out = F.group_norm(out.unsqueeze(0), num_groups=H, weight=lx_w, bias=lx_b).squeeze(0)
+        out = gemm(out, ow)
+
+        return x + out, xx, s
+
+    @MyFunction
+    def att_seq_v5(self, x, sx, s, ln_w, ln_b, lx_w, lx_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
+        xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
+        sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
+        kx = xx * k_mix + sx * (1 - k_mix)
+        vx = xx * v_mix + sx * (1 - v_mix)
+        rx = xx * r_mix + sx * (1 - r_mix)
+
+        H = t_decay.shape[0]
+        S = x.shape[-1] // H
+        T = x.shape[0]
+
+        w = t_decay.reshape(-1, 1)
+        u = t_first.reshape(-1, 1)
+        ws = w.pow(T).reshape(H, 1, 1)
+        ind = torch.arange(T-1, -1, -1, device=w.device).unsqueeze(0).repeat(H, 1)
+        w = w.repeat(1, T).pow(ind)
+        wk = w.reshape(H, 1, T)
+        wb = wk.transpose(-2, -1).flip(1)
+        w = torch.cat([w[:, 1:], u], dim=1)
+        w = F.pad(w, (0, T))
+        w = torch.tile(w, [T])
+        w = w[:, :-T].reshape(-1, T, 2 * T - 1)
+        w = w[:, :, T-1:].reshape(H, T, T)
+
+        r = gemm(rx, rw).view(T, H, S).transpose(0, 1)
+        k = gemm(kx, kw).view(T, H, S).transpose(0, 1).transpose(-2, -1)
+        v = gemm(vx, vw).view(T, H, S).transpose(0, 1)
+
+        out = ((r @ k) * w) @ v + (r @ s) * wb
+        s = ws * s + (k * wk) @ v
+        
+        out = out.transpose(0, 1).contiguous().reshape(T, H*S)
+        out = F.group_norm(out, num_groups=H, weight=lx_w, bias=lx_b)
+        out = gemm(out, ow)
+
+        return x + out, xx[-1,:], s
+
+    ########################################################################################################
+
     if os.environ["RWKV_CUDA_ON"] == '1':
         @MyFunction
         def cuda_att_seq(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
             T, C = x.size()
             xx = F.layer_norm(x, (C,), weight=ln_w, bias=ln_b)
             sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
             kx = xx * k_mix + sx * (1 - k_mix)
             vx = xx * v_mix + sx * (1 - v_mix)
             rx = xx * r_mix + sx * (1 - r_mix)
 
-            r = torch.sigmoid(rx @ rw)
-            k = kx @ kw
-            v = vx @ vw
+            r = torch.sigmoid(gemm(rx, rw))
+            k = gemm(kx, kw, output_dtype=torch.float32)
+            v = gemm(vx, vw, output_dtype=torch.float32)
             y, aa, bb, pp = cuda_wkv(T, C, t_decay, t_first, k, v, aa, bb, pp)
             
-            out = (r * y) @ ow
+            out = gemm(r * y.to(x.dtype), ow)
             return x + out, xx[-1,:], aa, bb, pp
 
         @MyFunction
         def cuda_att_seq_i8(self, x, sx, aa, bb, pp, ln_w, ln_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
             T, C = x.size()
             xx = F.layer_norm(x, (C,), weight=ln_w, bias=ln_b)
             sx = torch.cat((sx.unsqueeze(0), xx[:-1,:]))
@@ -556,24 +651,34 @@
 
     def forward(self, tokens, state, full_output=False):
         with torch.no_grad():
             w = self.w
             args = self.args
 
             if state == None:
-                state = [None] * args.n_layer * 5
-                for i in range(args.n_layer): # state: 0=att_xx 1=att_aa 2=att_bb 3=att_pp 4=ffn_xx
-                    dd = self.strategy[i]
-                    dev = dd.device
-                    atype = dd.atype
-                    state[i*5+0] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
-                    state[i*5+1] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous()
-                    state[i*5+2] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous()
-                    state[i*5+3] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous() - 1e30
-                    state[i*5+4] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
+                if self.version == 4:
+                    state = [None] * args.n_layer * 5
+                    for i in range(args.n_layer): # state: 0=att_xx 1=att_aa 2=att_bb 3=att_pp 4=ffn_xx
+                        dd = self.strategy[i]
+                        dev = dd.device
+                        atype = dd.atype
+                        state[i*5+0] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
+                        state[i*5+1] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous()
+                        state[i*5+2] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous()
+                        state[i*5+3] = torch.zeros(args.n_embd, dtype=torch.float, requires_grad=False, device=dev).contiguous() - 1e30
+                        state[i*5+4] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
+                elif self.version == 5:
+                    state = [None] * args.n_layer * 3
+                    for i in range(args.n_layer): # state: 0=att_xx 1=att_kv 2=ffn_xx
+                        dd = self.strategy[i]
+                        dev = dd.device
+                        atype = dd.atype
+                        state[i*3+0] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
+                        state[i*3+1] = torch.zeros((args.n_head, args.n_embd//args.n_head, args.n_embd//args.n_head), dtype=torch.float, requires_grad=False, device=dev).contiguous()
+                        state[i*3+2] = torch.zeros(args.n_embd, dtype=atype, requires_grad=False, device=dev).contiguous()
 
             seq_mode = len(tokens) > 1
 
             x = w['emb.weight'][tokens if seq_mode else tokens[0]]
 
             for i in range(args.n_layer):
                 bbb = f'blocks.{i}.'
@@ -584,17 +689,21 @@
                 atype = dd.atype
                 wtype = dd.wtype
                 if seq_mode:
                     if 'cuda' in str(dev) and os.environ["RWKV_CUDA_ON"] == '1':
                         ATT = self.cuda_att_seq if wtype != torch.uint8 else self.cuda_att_seq_i8
                     else:
                         ATT = self.att_seq if wtype != torch.uint8 else self.att_seq_i8
+                    if self.version == 5:
+                        ATT = self.att_seq_v5
                     FFN = self.ffn_seq if wtype != torch.uint8 else self.ffn_seq_i8
                 else:
                     ATT = self.att_one if wtype != torch.uint8 else self.att_one_i8
+                    if self.version == 5:
+                        ATT = self.att_one_v5
                     FFN = self.ffn_one if wtype != torch.uint8 else self.ffn_one_i8
 
                 x = x.to(dtype=atype, device=dev)
 
                 kw = w[f'{att}key.weight']
                 vw = w[f'{att}value.weight']
                 rw = w[f'{att}receptance.weight']
@@ -616,25 +725,39 @@
                 rrx = w[f'{att}receptance.weight_rx'] if wtype == torch.uint8 else x
                 rmy = w[f'{att}receptance.weight_my'] if wtype == torch.uint8 else x
                 rry = w[f'{att}receptance.weight_ry'] if wtype == torch.uint8 else x
                 omx = w[f'{att}output.weight_mx'] if wtype == torch.uint8 else x
                 orx = w[f'{att}output.weight_rx'] if wtype == torch.uint8 else x
                 omy = w[f'{att}output.weight_my'] if wtype == torch.uint8 else x
                 ory = w[f'{att}output.weight_ry'] if wtype == torch.uint8 else x
-                x, state[i*5+0], state[i*5+1], state[i*5+2], state[i*5+3] = ATT(
-                    x, state[i*5+0], state[i*5+1], state[i*5+2], state[i*5+3],
-                    w[f'{bbb}ln1.weight'], w[f'{bbb}ln1.bias'],
-                    w[f'{att}time_mix_k'], w[f'{att}time_mix_v'], w[f'{att}time_mix_r'],
-                    w[f'{att}time_decay'], w[f'{att}time_first'],
-                    kw, vw, rw, ow,
-                    kmx, krx, kmy, kry,
-                    vmx, vrx, vmy, vry,
-                    rmx, rrx, rmy, rry,
-                    omx, orx, omy, ory,
-                    )
+                if self.version == 4:
+                    x, state[i*5+0], state[i*5+1], state[i*5+2], state[i*5+3] = ATT(
+                        x, state[i*5+0], state[i*5+1], state[i*5+2], state[i*5+3],
+                        w[f'{bbb}ln1.weight'], w[f'{bbb}ln1.bias'],
+                        w[f'{att}time_mix_k'], w[f'{att}time_mix_v'], w[f'{att}time_mix_r'],
+                        w[f'{att}time_decay'], w[f'{att}time_first'],
+                        kw, vw, rw, ow,
+                        kmx, krx, kmy, kry,
+                        vmx, vrx, vmy, vry,
+                        rmx, rrx, rmy, rry,
+                        omx, orx, omy, ory,
+                        )
+                elif self.version == 5:
+                    x, state[i*3+0], state[i*3+1] = ATT(
+                        x, state[i*3+0], state[i*3+1],
+                        w[f'{bbb}ln1.weight'], w[f'{bbb}ln1.bias'],
+                        w[f'{att}ln_x.weight'], w[f'{att}ln_x.bias'],
+                        w[f'{att}time_mix_k'], w[f'{att}time_mix_v'], w[f'{att}time_mix_r'],
+                        w[f'{att}time_decay'], w[f'{att}time_first'],
+                        kw, vw, rw, ow,
+                        kmx, krx, kmy, kry,
+                        vmx, vrx, vmy, vry,
+                        rmx, rrx, rmy, rry,
+                        omx, orx, omy, ory,
+                        )
                 if dd.stream:
                     del kw, vw, rw, ow
 
                 kw = w[f'{ffn}key.weight']
                 vw = w[f'{ffn}value.weight']
                 rw = w[f'{ffn}receptance.weight']
                 if dd.stream:
@@ -648,17 +771,21 @@
                 vmx = w[f'{ffn}value.weight_mx'] if wtype == torch.uint8 else x
                 vrx = w[f'{ffn}value.weight_rx'] if wtype == torch.uint8 else x
                 vmy = w[f'{ffn}value.weight_my'] if wtype == torch.uint8 else x
                 vry = w[f'{ffn}value.weight_ry'] if wtype == torch.uint8 else x
                 rmx = w[f'{ffn}receptance.weight_mx'] if wtype == torch.uint8 else x
                 rrx = w[f'{ffn}receptance.weight_rx'] if wtype == torch.uint8 else x
                 rmy = w[f'{ffn}receptance.weight_my'] if wtype == torch.uint8 else x
-                rry = w[f'{ffn}receptance.weight_ry'] if wtype == torch.uint8 else x                    
-                x, state[i*5+4] = FFN(
-                    x, state[i*5+4],
+                rry = w[f'{ffn}receptance.weight_ry'] if wtype == torch.uint8 else x
+                if self.version == 4:
+                    offset = i*5+4
+                elif self.version == 5:
+                    offset = i*3+2
+                x, state[offset] = FFN(
+                    x, state[offset],
                     w[f'{bbb}ln2.weight'], w[f'{bbb}ln2.bias'],
                     w[f'{ffn}time_mix_k'], w[f'{ffn}time_mix_r'],
                     kw, vw, rw,
                     kmx, krx, kmy, kry,
                     vmx, vrx, vmy, vry,
                     rmx, rrx, rmy, rry,                    
                     )
```

### Comparing `rwkv-0.8.0/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.5/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.5/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.0/src/rwkv/utils.py` & `rwkv-0.8.5/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.0/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.5/src/rwkv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.0
+Version: 0.8.5
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -76,15 +76,15 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
-                     alpha_decay=0.996, # gradually decay the penalty
+                     alpha_decay = 0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
```

