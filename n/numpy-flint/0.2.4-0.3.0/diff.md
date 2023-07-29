# Comparing `tmp/numpy-flint-0.2.4.tar.gz` & `tmp/numpy-flint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy-flint-0.2.4.tar", last modified: Sun Apr 30 22:18:35 2023, max compression
+gzip compressed data, was "numpy-flint-0.3.0.tar", last modified: Sat Jul 29 19:24:22 2023, max compression
```

## Comparing `numpy-flint-0.2.4.tar` & `numpy-flint-0.3.0.tar`

### file list

```diff
@@ -1,145 +1,148 @@
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.892894 numpy-flint-0.2.4/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.797894 numpy-flint-0.2.4/.venv/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.797894 numpy-flint-0.2.4/.venv/lib/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.798894 numpy-flint-0.2.4/.venv/lib/python3.9/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.807894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.816894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/
--rw-r--r--   0 jef       (1000) jef       (1000)     3908 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h
--rw-r--r--   0 jef       (1000) jef       (1000)    14800 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h
--rw-r--r--   0 jef       (1000) jef       (1000)    17680 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_embedding.h
--rw-r--r--   0 jef       (1000) jef       (1000)     5976 2023-04-04 22:13:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.799894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.799894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.800894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.817894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/
--rw-r--r--   0 jef       (1000) jef       (1000)  2138822 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_cython.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.825894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/
--rw-r--r--   0 jef       (1000) jef       (1000)   956390 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c
--rw-r--r--   0 jef       (1000) jef       (1000)       84 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/release_mem.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.801894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.825894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/
--rw-r--r--   0 jef       (1000) jef       (1000)    22335 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/python.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.828894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/
--rw-r--r--   0 jef       (1000) jef       (1000)     1902 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/attach.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1198 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/stdafx.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1035 2023-04-30 17:41:40.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/targetver.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.805894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.802894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.845894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/
--rw-r--r--   0 jef       (1000) jef       (1000)    62712 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)    12614 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1877 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h
--rw-r--r--   0 jef       (1000) jef       (1000)      971 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h
--rw-r--r--   0 jef       (1000) jef       (1000)      282 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)     3818 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h
--rw-r--r--   0 jef       (1000) jef       (1000)    19943 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1959 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.845894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/
--rw-r--r--   0 jef       (1000) jef       (1000)    80138 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h
--rw-r--r--   0 jef       (1000) jef       (1000)    10191 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)    68688 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h
--rw-r--r--   0 jef       (1000) jef       (1000)     6830 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h
--rw-r--r--   0 jef       (1000) jef       (1000)     4327 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)    15990 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h
--rw-r--r--   0 jef       (1000) jef       (1000)    39015 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h
--rw-r--r--   0 jef       (1000) jef       (1000)     4603 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h
--rw-r--r--   0 jef       (1000) jef       (1000)     2786 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1948 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h
--rw-r--r--   0 jef       (1000) jef       (1000)    19874 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h
--rw-r--r--   0 jef       (1000) jef       (1000)      678 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1120 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h
--rw-r--r--   0 jef       (1000) jef       (1000)     2943 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h
--rw-r--r--   0 jef       (1000) jef       (1000)     6405 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h
--rw-r--r--   0 jef       (1000) jef       (1000)      899 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.847894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/
--rw-r--r--   0 jef       (1000) jef       (1000)      488 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/bitgen.h
--rw-r--r--   0 jef       (1000) jef       (1000)     9865 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h
--rw-r--r--   0 jef       (1000) jef       (1000)    11895 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1185 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.803894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.847894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/
--rw-r--r--   0 jef       (1000) jef       (1000)      344 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/limited_api.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.804894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.876894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/
--rw-r--r--   0 jef       (1000) jef       (1000)      818 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c
--rw-r--r--   0 jef       (1000) jef       (1000)      432 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimddp.c
--rw-r--r--   0 jef       (1000) jef       (1000)      529 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c
--rw-r--r--   0 jef       (1000) jef       (1000)      379 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdhp.c
--rw-r--r--   0 jef       (1000) jef       (1000)      779 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      749 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      842 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      948 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1004 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c
--rw-r--r--   0 jef       (1000) jef       (1000)      956 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1132 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1010 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      759 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c
--rw-r--r--   0 jef       (1000) jef       (1000)      755 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c
--rw-r--r--   0 jef       (1000) jef       (1000)      868 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c
--rw-r--r--   0 jef       (1000) jef       (1000)      817 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      301 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma4.c
--rw-r--r--   0 jef       (1000) jef       (1000)      600 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c
--rw-r--r--   0 jef       (1000) jef       (1000)      251 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_fp16.c
--rw-r--r--   0 jef       (1000) jef       (1000)      609 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1049 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c
--rw-r--r--   0 jef       (1000) jef       (1000)      686 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c
--rw-r--r--   0 jef       (1000) jef       (1000)      697 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      689 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      675 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c
--rw-r--r--   0 jef       (1000) jef       (1000)      692 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c
--rw-r--r--   0 jef       (1000) jef       (1000)      705 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      478 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      263 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      250 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx3.c
--rw-r--r--   0 jef       (1000) jef       (1000)      305 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx4.c
--rw-r--r--   0 jef       (1000) jef       (1000)      461 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vx.c
--rw-r--r--   0 jef       (1000) jef       (1000)      788 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c
--rw-r--r--   0 jef       (1000) jef       (1000)      624 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c
--rw-r--r--   0 jef       (1000) jef       (1000)      234 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_xop.c
--rw-r--r--   0 jef       (1000) jef       (1000)      636 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c
--rw-r--r--   0 jef       (1000) jef       (1000)      504 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512dq_mask.c
--rw-r--r--   0 jef       (1000) jef       (1000)     1595 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c
--rw-r--r--   0 jef       (1000) jef       (1000)      499 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx4_mma.c
--rw-r--r--   0 jef       (1000) jef       (1000)      945 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c
--rw-r--r--   0 jef       (1000) jef       (1000)       16 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/test_flags.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.877894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/
--rw-r--r--   0 jef       (1000) jef       (1000)       77 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/gfortran_vs2003_hack.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.805894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.879894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/
--rw-r--r--   0 jef       (1000) jef       (1000)    46010 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c
--rw-r--r--   0 jef       (1000) jef       (1000)     5835 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.806894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.806894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.880894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/
--rw-r--r--   0 jef       (1000) jef       (1000)     7299 2023-04-02 14:57:18.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.808894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.808894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.880894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/cffi/
--rw-r--r--   0 jef       (1000) jef       (1000)     2623 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.884894 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/
--rw-r--r--   0 jef       (1000) jef       (1000)      116 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/getpid_compat.h
--rw-r--r--   0 jef       (1000) jef       (1000)      522 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h
--rw-r--r--   0 jef       (1000) jef       (1000)     1625 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/mutex.h
--rw-r--r--   0 jef       (1000) jef       (1000)      284 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/pyversion_compat.h
--rw-r--r--   0 jef       (1000) jef       (1000)     3184 2023-04-30 17:41:38.000000 numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h
--rw-r--r--   0 jef       (1000) jef       (1000)      852 2023-04-02 17:20:31.000000 numpy-flint-0.2.4/MANIFEST.in
--rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-30 22:18:35.891894 numpy-flint-0.2.4/PKG-INFO
--rw-r--r--   0 jef       (1000) jef       (1000)     7642 2023-04-02 14:09:32.000000 numpy-flint-0.2.4/copying.lesser.md
--rw-r--r--   0 jef       (1000) jef       (1000)    34916 2023-04-02 14:09:32.000000 numpy-flint-0.2.4/copying.md
--rw-r--r--   0 jef       (1000) jef       (1000)     1507 2023-04-30 19:41:17.000000 numpy-flint-0.2.4/pyproject.toml
--rw-r--r--   0 jef       (1000) jef       (1000)    12282 2023-04-05 01:28:05.000000 numpy-flint-0.2.4/readme.md
--rw-r--r--   0 jef       (1000) jef       (1000)       38 2023-04-30 22:18:35.892894 numpy-flint-0.2.4/setup.cfg
--rw-r--r--   0 jef       (1000) jef       (1000)     1540 2023-04-03 01:00:19.000000 numpy-flint-0.2.4/setup.py
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.886894 numpy-flint-0.2.4/src/
--rw-r--r--   0 jef       (1000) jef       (1000)    36625 2023-04-04 21:55:07.000000 numpy-flint-0.2.4/src/flint.h
--rw-r--r--   0 jef       (1000) jef       (1000)    61889 2023-04-30 18:58:53.000000 numpy-flint-0.2.4/src/numpy_flint.c
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.890894 numpy-flint-0.2.4/src/numpy_flint.egg-info/
--rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/PKG-INFO
--rw-r--r--   0 jef       (1000) jef       (1000)     6947 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/SOURCES.txt
--rw-r--r--   0 jef       (1000) jef       (1000)        1 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/dependency_links.txt
--rw-r--r--   0 jef       (1000) jef       (1000)       12 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/requires.txt
--rw-r--r--   0 jef       (1000) jef       (1000)        6 2023-04-30 22:18:35.000000 numpy-flint-0.2.4/src/numpy_flint.egg-info/top_level.txt
-drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-04-30 22:18:35.891894 numpy-flint-0.2.4/tests/
--rw-r--r--   0 jef       (1000) jef       (1000)    30312 2023-04-30 19:40:38.000000 numpy-flint-0.2.4/tests/test_flint.py
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.454350 numpy-flint-0.3.0/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.847350 numpy-flint-0.3.0/.venv/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.847350 numpy-flint-0.3.0/.venv/lib/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.848350 numpy-flint-0.3.0/.venv/lib/python3.9/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.854350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.008350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/
+-rw-r--r--   0 jef       (1000) jef       (1000)     3908 2023-04-04 22:13:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    14800 2023-04-04 22:13:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    17680 2023-04-04 22:13:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_embedding.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     5976 2023-04-04 22:13:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.848350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.849350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.849350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.013350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/
+-rw-r--r--   0 jef       (1000) jef       (1000)  2138822 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_cython.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.087350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/
+-rw-r--r--   0 jef       (1000) jef       (1000)   956390 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c
+-rw-r--r--   0 jef       (1000) jef       (1000)       84 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/release_mem.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.850350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.089350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/
+-rw-r--r--   0 jef       (1000) jef       (1000)    22335 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/python.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.112350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/
+-rw-r--r--   0 jef       (1000) jef       (1000)     1902 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/attach.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1198 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/stdafx.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1035 2023-04-30 17:41:40.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/targetver.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.853350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.852350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.852350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.217350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/
+-rw-r--r--   0 jef       (1000) jef       (1000)    62712 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    12614 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1877 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      971 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      282 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     3818 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    19943 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1959 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.221350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/
+-rw-r--r--   0 jef       (1000) jef       (1000)    80138 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    10191 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    68688 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     6830 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     4327 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    15990 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    39015 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     4603 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     2786 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1948 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    19874 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      678 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1120 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     2943 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     6405 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      899 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.239350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/
+-rw-r--r--   0 jef       (1000) jef       (1000)      488 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/bitgen.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     9865 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    11895 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1185 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.852350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/tests/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.853350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.247350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/
+-rw-r--r--   0 jef       (1000) jef       (1000)      344 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/tests/examples/limited_api/limited_api.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.853350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.323350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/
+-rw-r--r--   0 jef       (1000) jef       (1000)      818 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      432 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimddp.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      529 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      379 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdhp.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      779 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      749 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      842 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      948 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1004 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      956 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1132 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1010 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      759 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      755 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      868 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      817 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      301 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      600 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      251 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_fp16.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      609 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1049 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      686 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      697 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      689 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      675 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      692 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      705 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      478 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      263 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      250 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx3.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      305 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vsx4.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      461 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vx.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      788 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      624 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      234 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_xop.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      636 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      504 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512dq_mask.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     1595 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      499 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx4_mma.c
+-rw-r--r--   0 jef       (1000) jef       (1000)      945 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c
+-rw-r--r--   0 jef       (1000) jef       (1000)       16 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/test_flags.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.325350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/
+-rw-r--r--   0 jef       (1000) jef       (1000)       77 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/mingw/gfortran_vs2003_hack.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.853350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.354350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/src/
+-rw-r--r--   0 jef       (1000) jef       (1000)    46010 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     5835 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.854350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/tests/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.854350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.400350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/
+-rw-r--r--   0 jef       (1000) jef       (1000)     7299 2023-04-02 14:57:18.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.854350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.854350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/backend/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.404350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/backend/cffi/
+-rw-r--r--   0 jef       (1000) jef       (1000)     2623 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.426350 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/
+-rw-r--r--   0 jef       (1000) jef       (1000)      116 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/getpid_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      522 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     1625 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/mutex.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      284 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/pyversion_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)     3184 2023-04-30 17:41:38.000000 numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h
+-rw-r--r--   0 jef       (1000) jef       (1000)      852 2023-04-02 17:20:31.000000 numpy-flint-0.3.0/MANIFEST.in
+-rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-07-29 19:24:22.452350 numpy-flint-0.3.0/PKG-INFO
+-rw-r--r--   0 jef       (1000) jef       (1000)     7642 2023-04-02 14:09:32.000000 numpy-flint-0.3.0/copying.lesser.md
+-rw-r--r--   0 jef       (1000) jef       (1000)    34916 2023-04-02 14:09:32.000000 numpy-flint-0.3.0/copying.md
+-rw-r--r--   0 jef       (1000) jef       (1000)     1522 2023-07-22 22:16:40.000000 numpy-flint-0.3.0/pyproject.toml
+-rw-r--r--   0 jef       (1000) jef       (1000)    12282 2023-04-05 01:28:05.000000 numpy-flint-0.3.0/readme.md
+-rw-r--r--   0 jef       (1000) jef       (1000)       38 2023-07-29 19:24:22.455350 numpy-flint-0.3.0/setup.cfg
+-rw-r--r--   0 jef       (1000) jef       (1000)     1607 2023-07-27 01:54:34.000000 numpy-flint-0.3.0/setup.py
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:21.855350 numpy-flint-0.3.0/src/
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.440350 numpy-flint-0.3.0/src/flint/
+-rw-r--r--   0 jef       (1000) jef       (1000)     1027 2023-07-28 21:57:48.000000 numpy-flint-0.3.0/src/flint/__init__.py
+-rw-r--r--   0 jef       (1000) jef       (1000)    36625 2023-04-04 21:55:07.000000 numpy-flint-0.3.0/src/flint/flint.h
+-rw-r--r--   0 jef       (1000) jef       (1000)    61901 2023-07-27 23:35:52.000000 numpy-flint-0.3.0/src/flint/numpy_flint.c
+-rw-r--r--   0 jef       (1000) jef       (1000)     2653 2023-07-27 23:48:01.000000 numpy-flint-0.3.0/src/flint/numpy_flint.h
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.445350 numpy-flint-0.3.0/src/numpy_flint.egg-info/
+-rw-r--r--   0 jef       (1000) jef       (1000)    12575 2023-07-29 19:24:21.000000 numpy-flint-0.3.0/src/numpy_flint.egg-info/PKG-INFO
+-rw-r--r--   0 jef       (1000) jef       (1000)     7005 2023-07-29 19:24:21.000000 numpy-flint-0.3.0/src/numpy_flint.egg-info/SOURCES.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)        1 2023-07-29 19:24:21.000000 numpy-flint-0.3.0/src/numpy_flint.egg-info/dependency_links.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)       12 2023-07-29 19:24:21.000000 numpy-flint-0.3.0/src/numpy_flint.egg-info/requires.txt
+-rw-r--r--   0 jef       (1000) jef       (1000)        6 2023-07-29 19:24:21.000000 numpy-flint-0.3.0/src/numpy_flint.egg-info/top_level.txt
+drwxr-xr-x   0 jef       (1000) jef       (1000)        0 2023-07-29 19:24:22.446350 numpy-flint-0.3.0/tests/
+-rw-r--r--   0 jef       (1000) jef       (1000)    30312 2023-04-30 19:40:38.000000 numpy-flint-0.3.0/tests/test_flint.py
```

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_cffi_errors.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_cffi_include.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/_embedding.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/_embedding.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/cffi/parse_c_type.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_cython.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_cython.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/pydevd_frame_evaluator.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/python.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/common/python.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/attach.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/attach.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/stdafx.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/stdafx.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/targetver.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/debugpy/_vendored/pydevd/pydevd_attach_to_process/windows/targetver.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__multiarray_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/__ufunc_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_neighborhood_iterator_imp.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/_numpyconfig.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/experimental_dtype_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/halffloat.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/libdivide/libdivide.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/noprefix.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_1_7_deprecated_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_3kcompat.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_common.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_cpu.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_endian.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_interrupt.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_no_deprecated_api.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/npy_os.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/numpyconfig.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/old_defines.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/oldnumeric.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/random/distributions.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/core/include/numpy/utils.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimd.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_asimdfhm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_clx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_cnl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_icl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knl.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_knm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512_skx.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512cd.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_avx512f.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_f16c.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_fma3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_neon_vfpv4.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_popcnt.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse41.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_sse42.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_ssse3.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/cpu_vxe2.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512bw_mask.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_avx512f_reduce.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/distutils/checks/extra_vsx_asm.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/src/fortranobject.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/mutex.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/.venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h` & `numpy-flint-0.3.0/.venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/MANIFEST.in` & `numpy-flint-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/PKG-INFO` & `numpy-flint-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-flint
-Version: 0.2.4
+Version: 0.3.0
 Summary: Add a rounded floating point interval (flint) dtype to NumPy
 Author-email: Jef Wagner <jefwagner@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: copying.lesser.md
 License-File: copying.md
```

### Comparing `numpy-flint-0.2.4/copying.lesser.md` & `numpy-flint-0.3.0/copying.lesser.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/copying.md` & `numpy-flint-0.3.0/copying.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/pyproject.toml` & `numpy-flint-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 
 [build-system]
 requires = ["setuptools>=59", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "numpy-flint"
-version = "0.2.4"
 authors = [{name="Jef Wagner", email="jefwagner@gmail.com"}]
 readme = "readme.md"
-# license = "LGPL-3.0-or-later"
 requires-python = ">=3.7"
 dependencies = ["numpy>=1.17"]
 description = "Add a rounded floating point interval (flint) dtype to NumPy"
+dynamic = ["version"]
 
 [tool.setuptools]
-# packages = ["flint"]
 license-files = ["copying*"]
 
+[tool.setuptools.dynamic]
+version = {attr = "flint.__version__"}
+
 [tool.cibuildwheel]
 # Build for cpython only
 # build = "cp310-win_amd64" # for quick local testing
 skip =  "pp*"
 # Test the wheels
 test-requires = "pytest"
 test-command = "pytest {project} -v --log-level=DEBUG"
```

### Comparing `numpy-flint-0.2.4/readme.md` & `numpy-flint-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/setup.py` & `numpy-flint-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,19 +26,20 @@
 
 from setuptools import setup, Extension
 import numpy as np
 
 setup_args = dict(
     ext_modules = [
         Extension(
-            name='flint',
-            sources=['src/numpy_flint.c'],
+            name='flint.numpy_flint',
+            sources=['src/flint/numpy_flint.c'],
             depends=[
-                'src/flint.h',
-                'src/numpy_flint.c',
+                'src/flint/flint.h',
+                'src/flint/numpy_flint.h',
+                'src/flint/numpy_flint.c',
             ],
-            include_dirs=[np.get_include(),'src'],
+            include_dirs=[np.get_include()],
         )
     ]
 )
 
 setup(**setup_args)
```

### Comparing `numpy-flint-0.2.4/src/flint.h` & `numpy-flint-0.3.0/src/flint/flint.h`

 * *Files identical despite different names*

### Comparing `numpy-flint-0.2.4/src/numpy_flint.c` & `numpy-flint-0.3.0/src/flint/numpy_flint.c`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,17 @@
 #include <numpy/npy_math.h>
 // #include <numpy/halffloat.h>
 #include <numpy/ufuncobject.h>
 #include "structmember.h"
 
 #include "flint.h"
 
-/// @brief A python flint object
-/// @param obval The internal c representation of the flint object
-typedef struct {
-    PyObject_HEAD
-    flint obval;
-} PyFlint;
+#define NUMPY_FLINT_MODULE
+#include "numpy_flint.h"
 
-/// @brief The flint PyTypeObject
-static PyTypeObject PyFlint_Type;
 
 /// @brief The array of data members of the flint object
 PyMemberDef pyflint_members[] = {
     {"a", T_DOUBLE, offsetof(PyFlint, obval.a), READONLY,
         "The lower bound of the floating point interval"},
     {"b", T_DOUBLE, offsetof(PyFlint, obval.b), READONLY,
         "The upper bound of the floating point interval"},
@@ -52,32 +46,14 @@
 
 // ###############################
 // ---- Convenience functions ----
 // ###############################
 // This section contains some convenience functions that are used by the method
 // implementations below.
 
-/// @brief Check if an object is a flint
-/// @param ob The PyObject to check
-/// @return 1 if the object is a flint, 0 otherwise
-static inline int PyFlint_Check(PyObject* ob) {
-    return PyObject_IsInstance(ob, (PyObject*) &PyFlint_Type);
-}
-
-/// @brief Create a PyFlint object from a c flint struct.
-/// @param f The c flint struct
-/// @return A new PyFlint object that contains a copy of f
-static inline PyObject* PyFlint_FromFlint(flint f) {
-    PyFlint* p = (PyFlint*) PyFlint_Type.tp_alloc(&PyFlint_Type, 0);
-    if (p) {
-        p->obval = f;
-    }
-    return (PyObject*) p;
-}
-
 /// @brief A macro to check if an object is a PyFlint and grab the c struct.
 /// @param f The c flint struct to copy the data into
 /// @param F The python PyObject to check
 /// @return If F is not a PyFlint, this forces an early return with NULL
 #define PyFlint_CheckedGetFlint(f, F) \
     if (PyFlint_Check(F)) { \
         f = ((PyFlint*) F)->obval; \
@@ -1320,28 +1296,29 @@
 
 // ###########################
 // ---- Module definition ----
 // ###########################
 /// @brief Struct with minimum needed components for the module definition
 static struct PyModuleDef moduledef = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "flint",
+    .m_name = "numpy_flint",
     .m_doc = "Rounded floating point intervals (flints)",
     .m_size = -1
 };
 
 /// @brief The module initialization function
-PyMODINIT_FUNC PyInit_flint(void) {
+PyMODINIT_FUNC PyInit_numpy_flint(void) {
     PyObject* m;
     PyObject* numpy;
     PyObject* numpy_dict;
     PyArray_Descr* npyflint_descr;
-    int NPY_FLINT;
     PyArray_Descr* from_descr;
     int arg_types[3];
+    static void* PyFlint_API[2];
+    PyObject* c_api_object;
     // Create the new module
     m = PyModule_Create(&moduledef);
     if (m==NULL) {
         PyErr_Print();
         PyErr_SetString(PyExc_SystemError, "Could not create flint module.");
         return NULL;
     }
@@ -1544,14 +1521,32 @@
     REGISTER_UFUNC(hypot, hypot)
     REGISTER_UFUNC(arctan2, atan2)
     // Finally register the new type with the module
     if (PyModule_AddObject(m, "flint", (PyObject *) &PyFlint_Type) < 0) {
         Py_DECREF(&PyFlint_Type);
         Py_DECREF(m);
         PyErr_Print();
-        PyErr_SetString(PyExc_SystemError, "Could not add flint.flint type to module flint.");
+        PyErr_SetString(PyExc_SystemError, "Could not add numpy_flint.flint type to module flint.");
+        return NULL;
+    }
+    // Register PyFlint_Type and NPY_FLINT with the c api
+    PyFlint_API[0] = (void*) get_pyflint_type;
+    PyFlint_API[1] = (void*) get_npy_flint;
+    c_api_object = PyCapsule_New((void*) PyFlint_API, "flint.numpy_flint.c_api", NULL);
+    if (c_api_object == NULL) {
+        Py_XDECREF(c_api_object);
+        Py_DECREF(m);
+        PyErr_Print();
+        PyErr_SetString(PyExc_SystemError, "Could create the c_api_object.");
+        return NULL;
+    }
+    if (PyModule_AddObject(m, "c_api", c_api_object) < 0) {
+        Py_XDECREF(c_api_object);
+        Py_DECREF(m);
+        PyErr_Print();
+        PyErr_SetString(PyExc_SystemError, "Could not add numpy_flint.c_api to flint module.");
         return NULL;
     }
 
     return m;
 }
```

### Comparing `numpy-flint-0.2.4/src/numpy_flint.egg-info/PKG-INFO` & `numpy-flint-0.3.0/src/numpy_flint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpy-flint
-Version: 0.2.4
+Version: 0.3.0
 Summary: Add a rounded floating point interval (flint) dtype to NumPy
 Author-email: Jef Wagner <jefwagner@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: copying.lesser.md
 License-File: copying.md
```

### Comparing `numpy-flint-0.2.4/src/numpy_flint.egg-info/SOURCES.txt` & `numpy-flint-0.3.0/src/numpy_flint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,17 @@
 .venv/lib/python3.9/site-packages/numpy/f2py/tests/src/array_from_pyobj/wrapmodule.c
 .venv/lib/python3.9/site-packages/zmq/backend/cffi/_cdefs.h
 .venv/lib/python3.9/site-packages/zmq/utils/getpid_compat.h
 .venv/lib/python3.9/site-packages/zmq/utils/ipcmaxlen.h
 .venv/lib/python3.9/site-packages/zmq/utils/mutex.h
 .venv/lib/python3.9/site-packages/zmq/utils/pyversion_compat.h
 .venv/lib/python3.9/site-packages/zmq/utils/zmq_compat.h
-src/flint.h
-src/numpy_flint.c
+src/flint/__init__.py
+src/flint/flint.h
+src/flint/numpy_flint.c
+src/flint/numpy_flint.h
 src/numpy_flint.egg-info/PKG-INFO
 src/numpy_flint.egg-info/SOURCES.txt
 src/numpy_flint.egg-info/dependency_links.txt
 src/numpy_flint.egg-info/requires.txt
 src/numpy_flint.egg-info/top_level.txt
 tests/test_flint.py
```

### Comparing `numpy-flint-0.2.4/tests/test_flint.py` & `numpy-flint-0.3.0/tests/test_flint.py`

 * *Files identical despite different names*

