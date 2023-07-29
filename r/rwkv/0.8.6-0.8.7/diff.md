# Comparing `tmp/rwkv-0.8.6.tar.gz` & `tmp/rwkv-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.8.6.tar", last modified: Sat Jul 29 02:42:05 2023, max compression
+gzip compressed data, was "rwkv-0.8.7.tar", last modified: Sat Jul 29 09:30:59 2023, max compression
```

## Comparing `rwkv-0.8.6.tar` & `rwkv-0.8.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.6/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.6/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 02:42:05.000000 rwkv-0.8.6/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.6/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-29 02:33:02.000000 rwkv-0.8.6/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 02:42:05.000000 rwkv-0.8.6/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.6/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     2934 2023-07-24 21:43:08.000000 rwkv-0.8.6/src/rwkv/cuda/gemm_fp16_cublas.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.6/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4897 2023-07-24 21:43:08.000000 rwkv-0.8.6/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    39410 2023-07-29 02:38:18.000000 rwkv-0.8.6/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.6/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.6/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.6/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 02:42:05.000000 rwkv-0.8.6/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.7/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.7/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 09:30:59.000000 rwkv-0.8.7/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.7/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-29 09:26:39.000000 rwkv-0.8.7/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 09:30:59.000000 rwkv-0.8.7/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.7/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3621 2023-07-29 09:25:30.000000 rwkv-0.8.7/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.7/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5002 2023-07-29 09:25:30.000000 rwkv-0.8.7/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    40726 2023-07-29 09:29:04.000000 rwkv-0.8.7/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.7/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.7/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.7/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.8.6/LICENSE` & `rwkv-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/PKG-INFO` & `rwkv-0.8.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.6
+Version: 0.8.7
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-0.8.6/README.md` & `rwkv-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/src/rwkv/cuda/gemm_fp16_cublas.cpp` & `rwkv-0.8.7/src/rwkv/cuda/gemm_fp16_cublas.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #include <cublas_v2.h>
 #include <cuda.h>
 #include <cuda_fp16.h>
 #include <cuda_runtime.h>
 #include <torch/extension.h>
 
-#define CUBLAS_CHECK(condition)                                             \
-  for (cublasStatus_t _cublas_check_status = (condition);                   \
-       _cublas_check_status != CUBLAS_STATUS_SUCCESS;)                      \
+#define CUBLAS_CHECK(condition)                                                \
+  for (cublasStatus_t _cublas_check_status = (condition);                      \
+       _cublas_check_status != CUBLAS_STATUS_SUCCESS;)                         \
     throw std::runtime_error("cuBLAS error " +                                 \
-                             std::to_string(_cublas_check_status) +         \
-                             " at " + std::to_string(__LINE__));
+                             std::to_string(_cublas_check_status) + " at " +   \
+                             std::to_string(__LINE__));
 
-#define CUDA_CHECK(condition)                                               \
-  for (cudaError_t _cuda_check_status = (condition);                        \
-       _cuda_check_status != cudaSuccess;)                                  \
+#define CUDA_CHECK(condition)                                                  \
+  for (cudaError_t _cuda_check_status = (condition);                           \
+       _cuda_check_status != cudaSuccess;)                                     \
     throw std::runtime_error(                                                  \
-        "CUDA error " +                                                        \
-        std::string(cudaGetErrorString(_cuda_check_status)) + " at " +      \
-        std::to_string(__LINE__));
+        "CUDA error " + std::string(cudaGetErrorString(_cuda_check_status)) +  \
+        " at " + std::to_string(__LINE__));
 
 cublasHandle_t get_cublas_handle() {
   static cublasHandle_t cublas_handle = []() {
     cublasHandle_t handle = nullptr;
     CUBLAS_CHECK(cublasCreate(&handle));
 #if CUDA_VERSION < 11000
     CUBLAS_CHECK(cublasSetMathMode(handle, CUBLAS_TENSOR_OP_MATH));
@@ -44,28 +43,44 @@
       c.dtype() == torch::kFloat32 ? CUDA_R_32F : CUDA_R_16F;
   const auto compute_type = CUDA_R_32F;
   const float sp_alpha = 1.f;
   // swap a and b, and use CUBLAS_OP_N. see the notes above
   std::swap(a, b);
   const cublasOperation_t cublas_trans_a = CUBLAS_OP_N;
   const cublasOperation_t cublas_trans_b = CUBLAS_OP_N;
-  // m = (B^T).size(0) = B.size(1), and = A.size(1) after swap
-  const int m = a.size(1);
-  const int k = a.size(0);
-  const int n = b.size(0);
+  // m = (B^T).size(0) = B.size(1), and = A.size(1) after swap,
+  // negative axis is used because of the existence of batch matmul.
+  const int m = a.size(-1);
+  const int k = a.size(-2);
+  const int n = b.size(-2);
   const int cublas_lda = m;
   const int cublas_ldb = k;
   const int cublas_ldc = m;
   cublasHandle_t cublas_handle = get_cublas_handle();
 
 #if CUDA_VERSION >= 11000
   cublasGemmAlgo_t algo = CUBLAS_GEMM_DEFAULT;
 #else
   cublasGemmAlgo_t algo = CUBLAS_GEMM_DFALT_TENSOR_OP;
 #endif
   const float sp_beta = 0.f;
-  CUBLAS_CHECK(cublasGemmEx(
-      cublas_handle, cublas_trans_a, cublas_trans_b, m, n, k, &sp_alpha,
-      a.data_ptr(), cuda_data_type, cublas_lda, b.data_ptr(), cuda_data_type,
-      cublas_ldb, &sp_beta, c.data_ptr(), cuda_c_data_type, cublas_ldc,
-      compute_type, algo));
+  if (a.dense_dim() == 2 && b.dense_dim() == 2) {
+    CUBLAS_CHECK(cublasGemmEx(
+        cublas_handle, cublas_trans_a, cublas_trans_b, m, n, k, &sp_alpha,
+        a.data_ptr(), cuda_data_type, cublas_lda, b.data_ptr(), cuda_data_type,
+        cublas_ldb, &sp_beta, c.data_ptr(), cuda_c_data_type, cublas_ldc,
+        compute_type, algo));
+  } else {
+    // batch matmul
+    assert(a.dense_dim() == 3 && b.dense_dim() == 3);
+
+    const long long int cublas_stride_a = m * k;
+    const long long int cublas_stride_b = k * n;
+    const long long int cublas_stride_c = m * n;
+    CUBLAS_CHECK(cublasGemmStridedBatchedEx(
+        cublas_handle, cublas_trans_a, cublas_trans_b, m,
+        n, k, &sp_alpha, a.data_ptr(), cuda_data_type, cublas_lda,
+        cublas_stride_a, b.data_ptr(), cuda_data_type, cublas_ldb, cublas_stride_b,
+        &sp_beta, c.data_ptr(), cuda_c_data_type, cublas_ldc, cublas_stride_c,
+        a.size(0), compute_type, algo));
+  }
 }
```

### Comparing `rwkv-0.8.6/src/rwkv/cuda/operators.cu` & `rwkv-0.8.7/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.7/src/rwkv/cuda/wrapper.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -114,22 +114,28 @@
     default:
         assert(false && "Only FP16 and FP32 are currently supported");
     }
 }
 
 using torch::Tensor;
 
+#ifndef DISABLE_CUBLAS_GEMM
 void gemm_fp16_cublas(Tensor a, Tensor b, Tensor c);
+#endif
 
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
     m.def("wkv_forward", &wkv_forward, "wkv forward");
     m.def("mm8_seq", &mm8_seq, "mm8 seq");
     m.def("mm8_one", &mm8_one, "mm8 one");
+#ifndef DISABLE_CUBLAS_GEMM
     m.def("gemm_fp16_cublas", &gemm_fp16_cublas, "gemv fp16 cublas");
+#endif
 }
 
 TORCH_LIBRARY(rwkv, m) {
     m.def("wkv_forward", wkv_forward);
     m.def("mm8_seq", mm8_seq);
     m.def("mm8_one", mm8_one);
+#ifndef DISABLE_CUBLAS_GEMM
     m.def("gemm_fp16_cublas", gemm_fp16_cublas);
+#endif
 }
```

### Comparing `rwkv-0.8.6/src/rwkv/model.py` & `rwkv-0.8.7/src/rwkv/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,32 @@
     def __nop(ob):
         return ob
     MyFunction = __nop
     MyStatic = __nop
 
 if os.environ.get('RWKV_CUDA_ON') == '1':
     from torch.utils.cpp_extension import load
-    load(
-        name=f"wkv_cuda",
-        sources=[f"{current_path}/cuda/wrapper.cpp", f"{current_path}/cuda/operators.cu", f"{current_path}/cuda/gemm_fp16_cublas.cpp"],
-        verbose=True,
-        extra_cuda_cflags=["-t 4", "-std=c++17", "--use_fast_math", "-O3", "--extra-device-vectorization"],
-        is_python_module=False)
+    try:
+        load(
+            name=f"wkv_cuda",
+            sources=[f"{current_path}/cuda/wrapper.cpp", f"{current_path}/cuda/operators.cu", f"{current_path}/cuda/gemm_fp16_cublas.cpp"],
+            verbose=True,
+            extra_cuda_cflags=["-t 4", "-std=c++17", "--use_fast_math", "-O3", "--extra-device-vectorization"],
+            is_python_module=False)
+        DISABLE_CUBLAS_GEMM = False
+    except:
+        print("Failed to build cuBLAS matmul, falling back to torch.matmul. Small model with fp16 will overflow.")
+        load(
+            name=f"wkv_cuda",
+            sources=[f"{current_path}/cuda/wrapper.cpp", f"{current_path}/cuda/operators.cu"],
+            verbose=True,
+            extra_cuda_cflags=["-t 4", "-std=c++17", "--use_fast_math", "-O3", "--extra-device-vectorization"],
+            extra_cflags=["-DDISABLE_CUBLAS_GEMM"],
+            is_python_module=False)
+        DISABLE_CUBLAS_GEMM = True
 
     @MyStatic
     def cuda_wkv(T: int, C: int, w, u, k, v, aa, bb, pp):
         assert 1 * C % min(C, 32) == 0
         assert k.dtype == v.dtype == torch.float16 or k.dtype == v.dtype == torch.float32
         assert w.dtype == u.dtype == aa.dtype == bb.dtype == pp.dtype == torch.float32
         w = w.contiguous()
@@ -66,31 +78,40 @@
         assert x.shape == (N,)
         assert w.shape == (N, M)
         assert rx.shape == mx.shape == (M,)
         assert ry.shape == my.shape == (N, 1)
         y = torch.zeros((M,), device=w.device, dtype=torch.float32)
         torch.ops.rwkv.mm8_one(N, M, x, w, mx, rx, my, ry, y)
         return y.to(dtype=x.dtype)
+else:
+    os.environ["RWKV_CUDA_ON"] = '0'
+
+if os.environ.get('RWKV_CUDA_ON') == '1' and not DISABLE_CUBLAS_GEMM:
     @MyStatic
     def gemm(a, b, output_dtype: Optional[torch.dtype]=None):
         if output_dtype is None:
             output_dtype = a.dtype
         if a.dtype == b.dtype == torch.float16 and a.device.type == 'cuda':
-            assert len(b.shape) == 2
             if len(a.shape) == 1:
+                assert len(b.shape) == 2
                 c = torch.empty((b.shape[-1],), dtype=output_dtype, device=a.device)
                 a = a.unsqueeze(0)
             else:
-                c = torch.empty((a.shape[0], b.shape[-1]), dtype=output_dtype, device=a.device)
+                assert len(a.shape) == len(b.shape)
+                assert len(a.shape) == 2 or len(a.shape) == 3
+                # torch.empty((*a.shape[:-1], b.shape[-1])) doesn't work with jit
+                if len(a.shape) == 2:
+                    c = torch.empty((a.shape[0], b.shape[-1]), dtype=output_dtype, device=a.device)
+                else:
+                    c = torch.empty((a.shape[0], a.shape[1], b.shape[-1]), dtype=output_dtype, device=a.device)
             torch.ops.rwkv.gemm_fp16_cublas(a, b, c)
             return c
         else:
             return (a @ b).to(output_dtype)
 else:
-    os.environ["RWKV_CUDA_ON"] = '0'
     def gemm(a, b, output_dtype: Optional[torch.dtype]=None):
         if output_dtype is None:
             output_dtype = a.dtype
         return (a @ b).to(output_dtype)
 
 ########################################################################################################
 
@@ -257,14 +278,16 @@
                         elif self.version == 5:
                             w[x] = torch.exp(-torch.exp(w[x].float())).reshape(-1,1,1)
                     elif '.time_first' in x: # need fp32 for this
                         if self.version == 4:
                             w[x] = w[x].float()
                         elif self.version == 5:
                             w[x] = torch.exp(w[x].float()).reshape(-1,1,1)
+                    elif '.ln_x' in x: # need fp32 for group_norm
+                        w[x] = w[x].float()
                     else:
                         if (len(w[x].shape) == 2) and ('emb' not in x):
                             if WTYPE != torch.uint8:
                                 w[x] = w[x].to(dtype=WTYPE)
                             else:
                                 w[x] = w[x].float()
 
@@ -554,24 +577,25 @@
         kx = xx * k_mix + sx * (1 - k_mix)
         vx = xx * v_mix + sx * (1 - v_mix)
         rx = xx * r_mix + sx * (1 - r_mix)
 
         H = t_decay.shape[0]
         S = x.shape[-1] // H
 
-        r = gemm(rx, rw).view(H, 1, S)
-        k = gemm(kx, kw).view(H, S, 1)
-        v = gemm(vx, vw).view(H, 1, S)
+        r = gemm(rx, rw, output_dtype=torch.float32).view(H, 1, S)
+        k = gemm(kx, kw, output_dtype=torch.float32).view(H, S, 1)
+        v = gemm(vx, vw, output_dtype=torch.float32).view(H, 1, S)
         
-        a = (k @ v).float()
-        out = r @ (t_first * a + s).to(dtype=r.dtype)
+        a = gemm(k, v)
+        out = r @ (t_first * a + s)
         s = a + t_decay * s
 
         out = out.flatten()
         out = F.group_norm(out.unsqueeze(0), num_groups=H, weight=lx_w, bias=lx_b).squeeze(0)
+        out = out.to(dtype=x.dtype)
         out = gemm(out, ow)
 
         return x + out, xx, s
 
     @MyFunction
     def att_seq_v5(self, x, sx, s, ln_w, ln_b, lx_w, lx_b, k_mix, v_mix, r_mix, t_decay, t_first, kw, vw, rw, ow, kmx, krx, kmy, kry, vmx, vrx, vmy, vry, rmx, rrx, rmy, rry, omx, orx, omy, ory):
         xx = F.layer_norm(x, (x.shape[-1],), weight=ln_w, bias=ln_b)
@@ -593,24 +617,24 @@
         wb = wk.transpose(-2, -1).flip(1)
         w = torch.cat([w[:, 1:], u], dim=1)
         w = F.pad(w, (0, T))
         w = torch.tile(w, [T])
         w = w[:, :-T].reshape(-1, T, 2 * T - 1)
         w = w[:, :, T-1:].reshape(H, T, T)
 
-        r = gemm(rx, rw).view(T, H, S).transpose(0, 1).float()
-        k = gemm(kx, kw).view(T, H, S).transpose(0, 1).transpose(-2, -1).float()
-        v = gemm(vx, vw).view(T, H, S).transpose(0, 1).float()
+        r = gemm(rx, rw, output_dtype=torch.float32).view(T, H, S).transpose(0, 1)
+        k = gemm(kx, kw, output_dtype=torch.float32).view(T, H, S).transpose(0, 1).transpose(-2, -1)
+        v = gemm(vx, vw, output_dtype=torch.float32).view(T, H, S).transpose(0, 1)
 
         out = ((r @ k) * w) @ v + (r @ s) * wb
         s = ws * s + (k * wk) @ v
         
-        out = out.to(dtype=x.dtype)
         out = out.transpose(0, 1).contiguous().reshape(T, H*S)
         out = F.group_norm(out, num_groups=H, weight=lx_w, bias=lx_b)
+        out = out.to(dtype=x.dtype)
         out = gemm(out, ow)
 
         return x + out, xx[-1,:], s
 
     ########################################################################################################
 
     if os.environ["RWKV_CUDA_ON"] == '1':
```

### Comparing `rwkv-0.8.6/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.7/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.7/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/src/rwkv/utils.py` & `rwkv-0.8.7/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.6/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.7/src/rwkv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.6
+Version: 0.8.7
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

