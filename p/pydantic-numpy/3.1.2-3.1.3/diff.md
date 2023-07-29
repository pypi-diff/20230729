# Comparing `tmp/pydantic_numpy-3.1.2.tar.gz` & `tmp/pydantic_numpy-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-3.1.2.tar", max compression
+gzip compressed data, was "pydantic_numpy-3.1.3.tar", max compression
```

## Comparing `pydantic_numpy-3.1.2.tar` & `pydantic_numpy-3.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.2/LICENSE
--rw-r--r--   0        0        0     2703 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.2/README.md
--rw-r--r--   0        0        0      130 2023-07-27 08:24:24.004488 pydantic_numpy-3.1.2/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.2/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0     5502 2023-07-26 16:19:01.494117 pydantic_numpy-3.1.2/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0     3891 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0      118 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/__init__.py
--rw-r--r--   0        0        0     1116 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/multi_array.py
--rw-r--r--   0        0        0     8605 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/np_model.py
--rw-r--r--   0        0        0      474 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     2284 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     2036 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     2859 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     2578 2023-07-25 16:46:39.934073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0     1621 2023-07-26 16:19:01.494117 pydantic_numpy-3.1.2/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1206 2023-07-27 08:24:29.314455 pydantic_numpy-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.3/LICENSE
+-rw-r--r--   0        0        0     2703 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.3/README.md
+-rw-r--r--   0        0        0      130 2023-07-29 08:53:31.052028 pydantic_numpy-3.1.3/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.3/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0     5502 2023-07-26 16:19:01.494117 pydantic_numpy-3.1.3/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0     3891 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0      118 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/model/__init__.py
+-rw-r--r--   0        0        0     1116 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/model/multi_array.py
+-rw-r--r--   0        0        0     8605 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/model/np_model.py
+-rw-r--r--   0        0        0      474 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     2288 2023-07-29 12:17:57.081596 pydantic_numpy-3.1.3/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     2288 2023-07-29 12:17:57.081596 pydantic_numpy-3.1.3/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     2287 2023-07-29 12:17:57.082596 pydantic_numpy-3.1.3/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     2039 2023-07-29 12:17:57.082596 pydantic_numpy-3.1.3/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     2863 2023-07-29 12:17:57.082596 pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     2869 2023-07-29 12:17:57.082596 pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     2868 2023-07-29 12:17:57.082596 pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     2581 2023-07-29 12:17:57.083596 pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2023-07-29 10:09:21.466067 pydantic_numpy-3.1.3/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1206 2023-07-29 12:17:57.103596 pydantic_numpy-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.3/PKG-INFO
```

### Comparing `pydantic_numpy-3.1.2/LICENSE` & `pydantic_numpy-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/README.md` & `pydantic_numpy-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-3.1.3/pydantic_numpy/helper/annotation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/helper/validation.py` & `pydantic_numpy-3.1.3/pydantic_numpy/helper/validation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/model/multi_array.py` & `pydantic_numpy-3.1.3/pydantic_numpy/model/multi_array.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/model/np_model.py` & `pydantic_numpy-3.1.3/pydantic_numpy/model/np_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/i_dimensional.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 Np1DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=1)
 
 Np1DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=1)
 Np1DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=1)
 Np1DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=1)
 Np1DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=1)
 
-Np1DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=1)
+Np1DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble, dimensions=1)
 Np1DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=1)
 Np1DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=1)
 Np1DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=1)
 
-Np1DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.complex256, dimensions=1)
+Np1DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.clongdouble, dimensions=1)
 Np1DArrayComplex128 = np_array_pydantic_annotated_typing(data_type=np.complex128, dimensions=1)
 Np1DArrayComplex64 = np_array_pydantic_annotated_typing(data_type=np.complex64, dimensions=1)
 
 Np1DArrayBool = np_array_pydantic_annotated_typing(data_type=bool, dimensions=1)
 
 
 # Non-number types
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/ii_dimensional.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 Np2DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=2)
 
 Np2DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=2)
 Np2DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=2)
 Np2DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=2)
 Np2DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=2)
 
-Np2DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=2)
+Np2DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble, dimensions=2)
 Np2DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=2)
 Np2DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=2)
 Np2DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=2)
 
-Np2DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.complex256, dimensions=2)
+Np2DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.clongdouble, dimensions=2)
 Np2DArrayComplex128 = np_array_pydantic_annotated_typing(data_type=np.complex128, dimensions=2)
 Np2DArrayComplex64 = np_array_pydantic_annotated_typing(data_type=np.complex64, dimensions=2)
 
 Np2DArrayBool = np_array_pydantic_annotated_typing(data_type=bool, dimensions=2)
 
 
 # Non-number types
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/iii_dimensional.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 Np3DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=3)
 
 Np3DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=3)
 Np3DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=3)
 Np3DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=3)
 Np3DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=3)
 
-Np3DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=3)
+Np3DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble, dimensions=3)
 Np3DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=3)
 Np3DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=3)
 Np3DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=3)
 
-Np3DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.complex256, dimensions=3)
+Np3DArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.clongdouble, dimensions=3)
 Np3DArrayComplex128 = np_array_pydantic_annotated_typing(data_type=np.complex128, dimensions=3)
 Np3DArrayComplex64 = np_array_pydantic_annotated_typing(data_type=np.complex64, dimensions=3)
 
 Np3DArrayBool = np_array_pydantic_annotated_typing(data_type=bool, dimensions=3)
 
 
 # Non-number types
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/n_dimensional.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 NpNDArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8)
 
 NpNDArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64)
 NpNDArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32)
 NpNDArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16)
 NpNDArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8)
 
-NpNDArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128)
+NpNDArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble)
 NpNDArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64)
 NpNDArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32)
 NpNDArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16)
 
-NpNDArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.complex256)
+NpNDArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.clongdouble)
 NpNDArrayComplex128 = np_array_pydantic_annotated_typing(data_type=np.complex128)
 NpNDArrayComplex64 = np_array_pydantic_annotated_typing(data_type=np.complex64)
 
 NpNDArrayBool = np_array_pydantic_annotated_typing(data_type=bool)
 
 
 # Non-number types
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 NpStrict1DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=1, strict_data_typing=True)
 
 NpStrict1DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=1, strict_data_typing=True)
 
-NpStrict1DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=1, strict_data_typing=True)
+NpStrict1DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=1, strict_data_typing=True)
 NpStrict1DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=1, strict_data_typing=True)
 
 NpStrict1DArrayComplex256 = np_array_pydantic_annotated_typing(
-    data_type=np.complex256, dimensions=1, strict_data_typing=True
+    data_type=np.clongdouble, dimensions=1, strict_data_typing=True
 )
 NpStrict1DArrayComplex128 = np_array_pydantic_annotated_typing(
     data_type=np.complex128, dimensions=1, strict_data_typing=True
 )
 NpStrict1DArrayComplex64 = np_array_pydantic_annotated_typing(
     data_type=np.complex64, dimensions=1, strict_data_typing=True
 )
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 NpStrict2DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=2, strict_data_typing=True)
 
 NpStrict2DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=2, strict_data_typing=True)
 NpStrict2DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=2, strict_data_typing=True)
 NpStrict2DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=2, strict_data_typing=True)
 NpStrict2DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=2, strict_data_typing=True)
 
-NpStrict2DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=2, strict_data_typing=True)
+NpStrict2DArrayFp128 = np_array_pydantic_annotated_typing(
+    data_type=np.longdouble, dimensions=2, strict_data_typing=True
+)
 NpStrict2DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=2, strict_data_typing=True)
 NpStrict2DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=2, strict_data_typing=True)
 NpStrict2DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=2, strict_data_typing=True)
 
 NpStrict2DArrayComplex256 = np_array_pydantic_annotated_typing(
-    data_type=np.complex256, dimensions=2, strict_data_typing=True
+    data_type=np.clongdouble, dimensions=2, strict_data_typing=True
 )
 NpStrict2DArrayComplex128 = np_array_pydantic_annotated_typing(
     data_type=np.complex128, dimensions=2, strict_data_typing=True
 )
 NpStrict2DArrayComplex64 = np_array_pydantic_annotated_typing(
     data_type=np.complex64, dimensions=2, strict_data_typing=True
 )
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 NpStrict3DArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, dimensions=3, strict_data_typing=True)
 
 NpStrict3DArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, dimensions=3, strict_data_typing=True)
 NpStrict3DArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, dimensions=3, strict_data_typing=True)
 NpStrict3DArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, dimensions=3, strict_data_typing=True)
 NpStrict3DArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, dimensions=3, strict_data_typing=True)
 
-NpStrict3DArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, dimensions=3, strict_data_typing=True)
+NpStrict3DArrayFp128 = np_array_pydantic_annotated_typing(
+    data_type=np.longdouble, dimensions=3, strict_data_typing=True
+)
 NpStrict3DArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, dimensions=3, strict_data_typing=True)
 NpStrict3DArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, dimensions=3, strict_data_typing=True)
 NpStrict3DArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, dimensions=3, strict_data_typing=True)
 
 NpStrict3DArrayComplex256 = np_array_pydantic_annotated_typing(
-    data_type=np.complex256, dimensions=3, strict_data_typing=True
+    data_type=np.clongdouble, dimensions=3, strict_data_typing=True
 )
 NpStrict3DArrayComplex128 = np_array_pydantic_annotated_typing(
     data_type=np.complex128, dimensions=3, strict_data_typing=True
 )
 NpStrict3DArrayComplex64 = np_array_pydantic_annotated_typing(
     data_type=np.complex64, dimensions=3, strict_data_typing=True
 )
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-3.1.3/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 NpStrictNDArrayInt8 = np_array_pydantic_annotated_typing(data_type=np.int8, strict_data_typing=True)
 
 NpStrictNDArrayUint64 = np_array_pydantic_annotated_typing(data_type=np.uint64, strict_data_typing=True)
 NpStrictNDArrayUint32 = np_array_pydantic_annotated_typing(data_type=np.uint32, strict_data_typing=True)
 NpStrictNDArrayUint16 = np_array_pydantic_annotated_typing(data_type=np.uint16, strict_data_typing=True)
 NpStrictNDArrayUint8 = np_array_pydantic_annotated_typing(data_type=np.uint8, strict_data_typing=True)
 
-NpStrictNDArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.float128, strict_data_typing=True)
+NpStrictNDArrayFp128 = np_array_pydantic_annotated_typing(data_type=np.longdouble, strict_data_typing=True)
 NpStrictNDArrayFp64 = np_array_pydantic_annotated_typing(data_type=np.float64, strict_data_typing=True)
 NpStrictNDArrayFp32 = np_array_pydantic_annotated_typing(data_type=np.float32, strict_data_typing=True)
 NpStrictNDArrayFp16 = np_array_pydantic_annotated_typing(data_type=np.float16, strict_data_typing=True)
 
-NpStrictNDArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.complex256, strict_data_typing=True)
+NpStrictNDArrayComplex256 = np_array_pydantic_annotated_typing(data_type=np.clongdouble, strict_data_typing=True)
 NpStrictNDArrayComplex128 = np_array_pydantic_annotated_typing(data_type=np.complex128, strict_data_typing=True)
 NpStrictNDArrayComplex64 = np_array_pydantic_annotated_typing(data_type=np.complex64, strict_data_typing=True)
 
 NpStrictNDArrayBool = np_array_pydantic_annotated_typing(data_type=bool, strict_data_typing=True)
 
 
 # Non-number types
```

### Comparing `pydantic_numpy-3.1.2/pydantic_numpy/util.py` & `pydantic_numpy-3.1.3/pydantic_numpy/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.2/pyproject.toml` & `pydantic_numpy-3.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "3.1.2"
+version = "3.1.3"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
```

### Comparing `pydantic_numpy-3.1.2/PKG-INFO` & `pydantic_numpy-3.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 3.1.2
+Version: 3.1.3
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
```

