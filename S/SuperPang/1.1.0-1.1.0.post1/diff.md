# Comparing `tmp/SuperPang-1.1.0.tar.gz` & `tmp/SuperPang-1.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperPang-1.1.0.tar", last modified: Thu Jul 27 10:43:04 2023, max compression
+gzip compressed data, was "SuperPang-1.1.0.post1.tar", last modified: Sat Jul 29 18:57:32 2023, max compression
```

## Comparing `SuperPang-1.1.0.tar` & `SuperPang-1.1.0.post1.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.336078 SuperPang-1.1.0/
--rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-1.1.0/LICENSE
--rw-rw-r--   0 fer       (1000) fer       (1000)       31 2023-07-07 12:28:07.000000 SuperPang-1.1.0/MANIFEST.in
--rw-rw-r--   0 fer       (1000) fer       (1000)     8251 2023-07-27 10:43:04.336078 SuperPang-1.1.0/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)     5730 2023-07-10 19:19:29.000000 SuperPang-1.1.0/README.md
--rw-rw-r--   0 fer       (1000) fer       (1000)     1759 2023-07-07 12:28:07.000000 SuperPang-1.1.0/pyproject.toml
--rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-27 10:43:04.336078 SuperPang-1.1.0/setup.cfg
--rw-rw-r--   0 fer       (1000) fer       (1000)      774 2023-07-10 19:19:21.000000 SuperPang-1.1.0/setup.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.324078 SuperPang-1.1.0/src/
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.328078 SuperPang-1.1.0/src/SuperPang.egg-info/
--rw-rw-r--   0 fer       (1000) fer       (1000)     8251 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/PKG-INFO
--rw-rw-r--   0 fer       (1000) fer       (1000)     1165 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/SOURCES.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/dependency_links.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)      172 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/entry_points.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/requires.txt
--rw-rw-r--   0 fer       (1000) fer       (1000)       16 2023-07-27 10:43:04.000000 SuperPang-1.1.0/src/SuperPang.egg-info/top_level.txt
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.328078 SuperPang-1.1.0/src/superpang/
--rw-rw-r--   0 fer       (1000) fer       (1000)        6 2023-07-26 08:30:54.000000 SuperPang-1.1.0/src/superpang/VERSION
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/__init__.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.328078 SuperPang-1.1.0/src/superpang/lib/
--rw-rw-r--   0 fer       (1000) fer       (1000)    59803 2023-07-25 17:51:07.000000 SuperPang-1.1.0/src/superpang/lib/Assembler.py
--rw-rw-r--   0 fer       (1000) fer       (1000)  1199685 2023-07-27 10:43:03.000000 SuperPang-1.1.0/src/superpang/lib/Compressor.c
--rw-rw-r--   0 fer       (1000) fer       (1000)     3971 2023-07-27 09:24:05.000000 SuperPang-1.1.0/src/superpang/lib/Compressor.pyx
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/lib/__init__.py
--rw-rw-r--   0 fer       (1000) fer       (1000)  1100082 2023-07-27 10:43:03.000000 SuperPang-1.1.0/src/superpang/lib/cutils.c
--rw-rw-r--   0 fer       (1000) fer       (1000)     5151 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/lib/cutils.pyx
--rw-rw-r--   0 fer       (1000) fer       (1000)     3038 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/lib/utils.py
--rw-rw-r--   0 fer       (1000) fer       (1000)  1149237 2023-07-27 10:43:03.000000 SuperPang-1.1.0/src/superpang/lib/vtools.c
--rw-rw-r--   0 fer       (1000) fer       (1000)     2920 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/lib/vtools.pyx
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.328078 SuperPang-1.1.0/src/superpang/scripts/
--rwxrwxr-x   0 fer       (1000) fer       (1000)    17576 2023-07-26 09:25:32.000000 SuperPang-1.1.0/src/superpang/scripts/SuperPang.py
--rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/scripts/__init__.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)    12655 2023-07-27 07:48:19.000000 SuperPang-1.1.0/src/superpang/scripts/condense-edges.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)    16726 2023-07-21 10:24:20.000000 SuperPang-1.1.0/src/superpang/scripts/homogenize.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)     1589 2023-07-14 14:46:06.000000 SuperPang-1.1.0/src/superpang/scripts/test-SuperPang.py
--rwxrwxr-x   0 fer       (1000) fer       (1000)     1589 2023-07-14 14:46:06.000000 SuperPang-1.1.0/src/superpang/scripts/test_SuperPang.py
-drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-27 10:43:04.336078 SuperPang-1.1.0/src/superpang/test_data/
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2430301 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2636415981.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2266131 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2636416036.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2274047 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2636416061.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2402610 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2636416062.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2207567 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2639762512.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2184834 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2639762514.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2317227 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2639762515.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2202772 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2639762516.fna
--rwxrwxr-x   0 fer       (1000) fer       (1000)  2210266 2023-07-07 12:28:07.000000 SuperPang-1.1.0/src/superpang/test_data/2844342787.fna
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/
+-rw-r--r--   0 fer       (1000) fer       (1000)     1532 2022-07-05 08:49:46.000000 SuperPang-1.1.0.post1/LICENSE
+-rw-rw-r--   0 fer       (1000) fer       (1000)       31 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/MANIFEST.in
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5730 2023-07-28 09:11:39.000000 SuperPang-1.1.0.post1/README.md
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1759 2023-07-28 09:09:52.000000 SuperPang-1.1.0.post1/pyproject.toml
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/setup.cfg
+-rw-rw-r--   0 fer       (1000) fer       (1000)      798 2023-07-28 10:51:10.000000 SuperPang-1.1.0.post1/setup.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/SuperPang.egg-info/
+-rw-rw-r--   0 fer       (1000) fer       (1000)     8257 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/PKG-INFO
+-rw-rw-r--   0 fer       (1000) fer       (1000)     1080 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/SOURCES.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)        1 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/dependency_links.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)      172 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/entry_points.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       38 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/requires.txt
+-rw-rw-r--   0 fer       (1000) fer       (1000)       10 2023-07-29 18:57:32.000000 SuperPang-1.1.0.post1/src/SuperPang.egg-info/top_level.txt
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/
+-rw-rw-r--   0 fer       (1000) fer       (1000)       12 2023-07-27 16:14:09.000000 SuperPang-1.1.0.post1/src/superpang/VERSION
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/__init__.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/lib/
+-rw-rw-r--   0 fer       (1000) fer       (1000)    59803 2023-07-27 18:42:42.000000 SuperPang-1.1.0.post1/src/superpang/lib/Assembler.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     3485 2023-07-27 17:26:50.000000 SuperPang-1.1.0.post1/src/superpang/lib/Compressor.pyx
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/__init__.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     5630 2023-07-28 09:05:45.000000 SuperPang-1.1.0.post1/src/superpang/lib/cutils.pyx
+-rw-rw-r--   0 fer       (1000) fer       (1000)     3038 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/utils.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)     2920 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/lib/vtools.pyx
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.660153 SuperPang-1.1.0.post1/src/superpang/scripts/
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    17576 2023-07-26 09:25:32.000000 SuperPang-1.1.0.post1/src/superpang/scripts/SuperPang.py
+-rw-rw-r--   0 fer       (1000) fer       (1000)        0 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/scripts/__init__.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    12655 2023-07-27 07:48:19.000000 SuperPang-1.1.0.post1/src/superpang/scripts/condense-edges.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)    16722 2023-07-28 09:06:48.000000 SuperPang-1.1.0.post1/src/superpang/scripts/homogenize.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post1/src/superpang/scripts/test-SuperPang.py
+-rwxrwxr-x   0 fer       (1000) fer       (1000)     1568 2023-07-28 09:34:05.000000 SuperPang-1.1.0.post1/src/superpang/scripts/test_SuperPang.py
+drwxrwxr-x   0 fer       (1000) fer       (1000)        0 2023-07-29 18:57:32.672153 SuperPang-1.1.0.post1/src/superpang/test_data/
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2430301 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636415981.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2266131 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416036.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2274047 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416061.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2402610 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2636416062.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2207567 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762512.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2184834 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762514.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2317227 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762515.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2202772 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2639762516.fna
+-rwxrwxr-x   0 fer       (1000) fer       (1000)  2210266 2023-07-07 12:28:07.000000 SuperPang-1.1.0.post1/src/superpang/test_data/2844342787.fna
```

### Comparing `SuperPang-1.1.0/LICENSE` & `SuperPang-1.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/PKG-INFO` & `SuperPang-1.1.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperPang
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Non-redundant pangenome assemblies from multiple genomes or bins
 Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Fernando Puente-Sánchez
         All rights reserved.
```

### Comparing `SuperPang-1.1.0/README.md` & `SuperPang-1.1.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/pyproject.toml` & `SuperPang-1.1.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/SuperPang.egg-info/PKG-INFO` & `SuperPang-1.1.0.post1/src/SuperPang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SuperPang
-Version: 1.1.0
+Version: 1.1.0.post1
 Summary: Non-redundant pangenome assemblies from multiple genomes or bins
 Author-email: Fernando Puente-Sánchez <fernando.puente.sanchez@slu.se>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Fernando Puente-Sánchez
         All rights reserved.
```

### Comparing `SuperPang-1.1.0/src/SuperPang.egg-info/SOURCES.txt` & `SuperPang-1.1.0.post1/src/SuperPang.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 src/SuperPang.egg-info/dependency_links.txt
 src/SuperPang.egg-info/entry_points.txt
 src/SuperPang.egg-info/requires.txt
 src/SuperPang.egg-info/top_level.txt
 src/superpang/VERSION
 src/superpang/__init__.py
 src/superpang/lib/Assembler.py
-src/superpang/lib/Compressor.c
 src/superpang/lib/Compressor.pyx
 src/superpang/lib/__init__.py
-src/superpang/lib/cutils.c
 src/superpang/lib/cutils.pyx
 src/superpang/lib/utils.py
-src/superpang/lib/vtools.c
 src/superpang/lib/vtools.pyx
 src/superpang/scripts/SuperPang.py
 src/superpang/scripts/__init__.py
 src/superpang/scripts/condense-edges.py
 src/superpang/scripts/homogenize.py
 src/superpang/scripts/test-SuperPang.py
 src/superpang/scripts/test_SuperPang.py
```

### Comparing `SuperPang-1.1.0/src/superpang/lib/Assembler.py` & `SuperPang-1.1.0.post1/src/superpang/lib/Assembler.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/lib/Compressor.pyx` & `SuperPang-1.1.0.post1/src/superpang/lib/Compressor.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #cython: language_level=3
 #cython: boundscheck=False
 #cython: wraparound=False
 #cython: cdivision=True
+#cython: cpow=True
 
 from cpython.array cimport array
 import numpy as np
 cimport numpy as np
 DTYPE = np.uint8
 ctypedef np.uint8_t DTYPE_t
 
@@ -29,84 +30,74 @@
         self.clength = self.com + self.rem
         
     def compress(self, const unsigned char [:] seq):
         cdef Py_ssize_t i, j
         cdef const unsigned char [:] tetra
         cdef DTYPE_t [1000] cseq
         cdef int ctetra
-        cdef unsigned int exp # unsigned int to avoid power operation to be casted to a double
         for i in range(self.com):
             # Each tetranucleotide is stored as an 8-bit binary
             # A: 00, C: 01, G: 10, T: 11 
             tetra = seq[i*4:(i*4)+4]
             ctetra = 0
             for j in range(3,-1,-1):
                 if tetra[3-j] == b'A':
                     pass
                 elif tetra[3-j] == b'C':
-                    exp = (2*j)
-                    ctetra += 10**exp
+                    ctetra += 10**(2*j)
                 elif tetra[3-j] == b'G':
-                    exp = (2*j)+1
-                    ctetra += 10**exp
+                    ctetra += 10**((2*j)+1)
                 elif tetra[3-j] == b'T':
-                    exp = (2*j)+1
-                    ctetra += 10**exp
-                    esp = (2*j)
-                    ctetra += 10**exp
+                    ctetra += 10**((2*j)+1)
+                    ctetra += 10**(2*j)
             # Transform the 8-bit into a 1-byte decimal
             cseq[i] = self.change_base(ctetra, 2, 10)
         # For the remainder, just store each base as a byte
         for i in range(self.rem):
             cseq[self.com+i] = seq[4*self.com+i] # this directly casts the char into into DTYPE_t
 
         return cseq[0:self.clength]
 
 
     def decompress(self, const unsigned char[:] cseq):
         cdef Py_ssize_t i, j
         cdef int dec
         cdef int ctetra
-        cdef unsigned int exp # unsigned int to avoid power operation to be casted to a double
         seq = array('u', '0'*self.ksize)
         for i in range(self.com):
             dec = cseq[i]
             # Get the 8-bit binary from the decimal byte
             ctetra = self.change_base(dec, 10, 2)
             # Reconstruc the tetranucleotide
             for j in range(3,-1,-1):
                 if ctetra // 10**((2*j)+1):
                     if ( ctetra - 10**((2*j)+1) ) // 10**((2*j)):
                         seq[(i*4)+(3-j)] = 'T'
-                        exp = (2*j)+1
-                        ctetra -= 10**exp
-                        exp = (2*j)
-                        ctetra -= 10**exp
+                        ctetra -= 10**((2*j)+1)
+                        ctetra -= 10**(2*j)
                     else:
                         seq[(i*4)+(3-j)] = 'G'
-                        exp = (2*j)+1
-                        ctetra -= 10**exp
+                        ctetra -= 10**((2*j)+1)
                 else:
                     if ctetra // 10**((2*j)):
                         seq[(i*4)+(3-j)] = 'C'
-                        exp = (2*j)
-                        ctetra -= 10**exp
+                        ctetra -= 10**(2*j)
                     else:
                         seq[(i*4)+(3-j)] = 'A'
 
         # For the remainder, just transform the byte into a character
         for i in range(self.rem):
             dec = cseq[self.com+i]
             seq[4*self.com+i] = chr(dec)
         
         return seq.tounicode()
 
     
     cdef inline int change_base(self, int num, int base0, int base1):
         # This expects 8-bit binary numbers and decimals no larger than 255!
-        cdef unsigned int i # unsigned int to avoid power operation to be casted to a double
+        cdef Py_ssize_t i
         cdef int res = 0
         for i in range(7,-1,-1):
             if num // base1**i:
                 num -= base1**i
                 res += base0**i
         return res
```

### Comparing `SuperPang-1.1.0/src/superpang/lib/cutils.pyx` & `SuperPang-1.1.0.post1/src/superpang/lib/cutils.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #cython: language_level=3
 #cython: boundscheck=False
 #cython: wraparound=False
 #cython: cdivision=True
 
-from libc.stdlib cimport malloc, atoi
+from libc.stdlib cimport malloc, strtol
 from cpython.array cimport array, clone
 
 cdef Py_ssize_t MAX_RC_LEN = 50000000
 cdef char *seq_dest = <char *>malloc(MAX_RC_LEN + 1)
 seq_dest[MAX_RC_LEN] = b'\0'
 cdef char *seq_destC = <char *>malloc(MAX_RC_LEN + 1)
 seq_destC[MAX_RC_LEN] = b'\0'
@@ -30,49 +30,52 @@
 
 
 cpdef parse_cigar(str cigar):
     cdef bytes py_bytes = cigar.encode('UTF-8')
     cdef Py_ssize_t cLen = len(py_bytes)
     cdef char *cigar_src = py_bytes
     cdef char c
-    cdef char [10] buf
+    cdef char [10] buf = [0]*10 # Explicitly initialize to 0.
+                                # Using conda compilers (but not base ubuntu compilers, even when versions were equal)
+                                #  caused trailing characters being passed to strtol in some instances (buf seemed to have more than 10 elements)
+                                #  so if those characters could be parsed as a number, the result from strtol was wront. Initializing to 0 from the starts apparently fixes this
     cdef Py_ssize_t i, j, bsize = 0, nOps = 0, idlen = 0
     cdef float mlen = 0
-    cdef unsigned int [:] Larray
+    cdef long [:] Larray
     cdef char [:] oparray
     cdef double iden
-    Larray  = clone(array('I'), 100000, False)
+    Larray  = clone(array('l'), 100000, False)
     oparray = clone(array('b'), 100000, False)
     for i in range(cLen):
         c = cigar_src[i]
         if c >= 48 and c <= 57:
             buf[bsize] = c
             bsize += 1
         else:
             for j in range(bsize): # shift to the end
                 buf[9-j] = buf[bsize-j-1]
             for j in range(10-bsize):
                 buf[j] = 48 # "0"
             bsize = 0
-            Larray[nOps] = atoi(buf)
+            Larray[nOps] = strtol(buf, NULL, 10)
             oparray[nOps] = c
             if c == 61: # "="
                 mlen  += Larray[nOps]
                 idlen += Larray[nOps]
             elif c == 88: # "X":
                 idlen += Larray[nOps]
             nOps += 1
     if idlen > 0:
         iden = mlen/idlen
     else:
         iden = 0
     return Larray[:nOps], oparray[:nOps], idlen, iden
 
 
-cpdef correct_query(str query, Py_ssize_t queryStart, Py_ssize_t queryEnd, str target, Py_ssize_t targetStart, Py_ssize_t targetEnd, unsigned int [:] cigLengths, char[:] cigOps, bint isRC, int mismatch_size_threshold, int indel_size_threshold):
+cpdef correct_query(str query, Py_ssize_t queryStart, Py_ssize_t queryEnd, str target, Py_ssize_t targetStart, Py_ssize_t targetEnd, long [:] cigLengths, char[:] cigOps, bint isRC, int mismatch_size_threshold, int indel_size_threshold):
   
     query = query if not isRC else reverse_complement(query)
 
     cdef bytes q_bytes = query.encode('UTF-8')
     cdef bytes t_bytes = target.encode('UTF-8')
     cdef char *query_src  = q_bytes
     cdef char *target_src = t_bytes
```

### Comparing `SuperPang-1.1.0/src/superpang/lib/utils.py` & `SuperPang-1.1.0.post1/src/superpang/lib/utils.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/lib/vtools.pyx` & `SuperPang-1.1.0.post1/src/superpang/lib/vtools.pyx`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/scripts/SuperPang.py` & `SuperPang-1.1.0.post1/src/superpang/scripts/SuperPang.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/scripts/condense-edges.py` & `SuperPang-1.1.0.post1/src/superpang/scripts/condense-edges.py`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/scripts/homogenize.py` & `SuperPang-1.1.0.post1/src/superpang/scripts/homogenize.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,16 @@
                 cigLengthsPy, cigOpsPy, idlenPy, idenPy = parse_cigar_py(cigar)
                 try:
                     assert list(cigLengths) == cigLengthsPy
                     assert list(cigOps) == cigOpsPy
                     assert idlen == idlenPy
                     assert round(iden, 2)  == round(idenPy, 2) or abs(1 - iden/idenPy) < 0.01
                 except:
-                    print(list(cigLengths)[1:10], cigLengthsPy[1:10])
-                    print(list(cigOps)[1:10], cigOpsPy[1:10])
+                    print(list(cigLengths)[:10], cigLengthsPy[:10])
+                    print(list(cigOps)[:10], cigOpsPy[:10])
                     print(idlen, idlenPy)
                     print(sum([L for L, op in zip(cigLengths, cigOps) if op == 61]), sum([L for L, op in zip(cigLengthsPy, cigOpsPy) if op == 61]))
                     print(round(iden, 6), round(idenPy, 6))
                     raise
             
             if cigLengths.size == 1 and chr(cigOps[0]) == '=':
                 continue # perfect match, ignore
```

### Comparing `SuperPang-1.1.0/src/superpang/scripts/test-SuperPang.py` & `SuperPang-1.1.0.post1/src/superpang/scripts/test-SuperPang.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         files = [f'{datapath}/2636415981.fna', f'{datapath}/2636416036.fna']
         iden = '-i0.95'
     else:
        files = glob(f'{datapath}/*fna')
        iden = '-i0.95'
 
     args = [sys.executable, superpath,'-f'] + files + ['--assume-complete',
-            iden, '-t12', '--assume-complete', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH,
+            iden, '-t12', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH,
             '--keep-temporary', '--keep-intermediate', '--debug']
     argss = ' '.join(args)
     print(f'Running SuperPang with command "{argss}"')
     ecode = call(args)
 
     if not ecode:
         print(f'\n\nAll went well, I hope! Test results should be present in {output_path}\n')
```

### Comparing `SuperPang-1.1.0/src/superpang/scripts/test_SuperPang.py` & `SuperPang-1.1.0.post1/src/superpang/scripts/test_SuperPang.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         files = [f'{datapath}/2636415981.fna', f'{datapath}/2636416036.fna']
         iden = '-i0.95'
     else:
        files = glob(f'{datapath}/*fna')
        iden = '-i0.95'
 
     args = [sys.executable, superpath,'-f'] + files + ['--assume-complete',
-            iden, '-t12', '--assume-complete', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH,
+            iden, '-t12', '--force-overwrite', '-o', output_path, '--minimap2-path', MINIMAP2_PATH,
             '--keep-temporary', '--keep-intermediate', '--debug']
     argss = ' '.join(args)
     print(f'Running SuperPang with command "{argss}"')
     ecode = call(args)
 
     if not ecode:
         print(f'\n\nAll went well, I hope! Test results should be present in {output_path}\n')
```

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2636415981.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2636415981.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2636416036.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2636416036.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2636416061.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2636416061.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2636416062.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2636416062.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2639762512.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2639762512.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2639762514.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2639762514.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2639762515.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2639762515.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2639762516.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2639762516.fna`

 * *Files identical despite different names*

### Comparing `SuperPang-1.1.0/src/superpang/test_data/2844342787.fna` & `SuperPang-1.1.0.post1/src/superpang/test_data/2844342787.fna`

 * *Files identical despite different names*

