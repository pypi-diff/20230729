# Comparing `tmp/rwkv-0.8.5.tar.gz` & `tmp/rwkv-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.8.5.tar", last modified: Sat Jul 29 01:20:39 2023, max compression
+gzip compressed data, was "rwkv-0.8.6.tar", last modified: Sat Jul 29 02:42:05 2023, max compression
```

## Comparing `rwkv-0.8.5.tar` & `rwkv-0.8.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.5/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.5/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 01:20:39.000000 rwkv-0.8.5/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.5/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-27 23:10:42.000000 rwkv-0.8.5/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 01:20:39.000000 rwkv-0.8.5/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.5/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     2934 2023-07-24 21:43:08.000000 rwkv-0.8.5/src/rwkv/cuda/gemm_fp16_cublas.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.5/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4897 2023-07-24 21:43:08.000000 rwkv-0.8.5/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    39350 2023-07-29 01:08:41.000000 rwkv-0.8.5/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.5/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.5/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.5/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 01:20:39.000000 rwkv-0.8.5/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.6/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.6/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 02:42:05.000000 rwkv-0.8.6/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.6/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-29 02:33:02.000000 rwkv-0.8.6/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 02:42:05.000000 rwkv-0.8.6/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.6/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     2934 2023-07-24 21:43:08.000000 rwkv-0.8.6/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.6/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4897 2023-07-24 21:43:08.000000 rwkv-0.8.6/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    39410 2023-07-29 02:38:18.000000 rwkv-0.8.6/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.6/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.6/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.6/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.8.5/LICENSE` & `rwkv-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/PKG-INFO` & `rwkv-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.5
+Version: 0.8.6
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-0.8.5/README.md` & `rwkv-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/cuda/gemm_fp16_cublas.cpp` & `rwkv-0.8.6/src/rwkv/cuda/gemm_fp16_cublas.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/cuda/operators.cu` & `rwkv-0.8.6/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.6/src/rwkv/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/model.py` & `rwkv-0.8.6/src/rwkv/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,21 +593,22 @@
         wb = wk.transpose(-2, -1).flip(1)
         w = torch.cat([w[:, 1:], u], dim=1)
         w = F.pad(w, (0, T))
         w = torch.tile(w, [T])
         w = w[:, :-T].reshape(-1, T, 2 * T - 1)
         w = w[:, :, T-1:].reshape(H, T, T)
 
-        r = gemm(rx, rw).view(T, H, S).transpose(0, 1)
-        k = gemm(kx, kw).view(T, H, S).transpose(0, 1).transpose(-2, -1)
-        v = gemm(vx, vw).view(T, H, S).transpose(0, 1)
+        r = gemm(rx, rw).view(T, H, S).transpose(0, 1).float()
+        k = gemm(kx, kw).view(T, H, S).transpose(0, 1).transpose(-2, -1).float()
+        v = gemm(vx, vw).view(T, H, S).transpose(0, 1).float()
 
         out = ((r @ k) * w) @ v + (r @ s) * wb
         s = ws * s + (k * wk) @ v
         
+        out = out.to(dtype=x.dtype)
         out = out.transpose(0, 1).contiguous().reshape(T, H*S)
         out = F.group_norm(out, num_groups=H, weight=lx_w, bias=lx_b)
         out = gemm(out, ow)
 
         return x + out, xx[-1,:], s
 
     ########################################################################################################
```

### Comparing `rwkv-0.8.5/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.6/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.6/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv/utils.py` & `rwkv-0.8.6/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.5/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.6/src/rwkv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.5
+Version: 0.8.6
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

