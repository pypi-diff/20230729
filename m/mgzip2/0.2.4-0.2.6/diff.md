# Comparing `tmp/mgzip2-0.2.4.tar.gz` & `tmp/mgzip2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgzip2-0.2.4.tar", last modified: Sat Jul 29 02:42:34 2023, max compression
+gzip compressed data, was "mgzip2-0.2.6.tar", last modified: Sat Jul 29 14:05:18 2023, max compression
```

## Comparing `mgzip2-0.2.4.tar` & `mgzip2-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 02:42:34.846496 mgzip2-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-29 02:42:25.000000 mgzip2-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 02:42:34.846496 mgzip2-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 02:42:25.000000 mgzip2-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 02:42:34.846496 mgzip2-0.2.4/mgzip/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-29 02:42:25.000000 mgzip2-0.2.4/mgzip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-29 02:42:25.000000 mgzip2-0.2.4/mgzip/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27317 2023-07-29 02:42:25.000000 mgzip2-0.2.4/mgzip/multiProcGzip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 02:42:34.846496 mgzip2-0.2.4/mgzip2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 02:42:34.000000 mgzip2-0.2.4/mgzip2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-29 02:42:34.000000 mgzip2-0.2.4/mgzip2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 02:42:34.000000 mgzip2-0.2.4/mgzip2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 02:42:34.000000 mgzip2-0.2.4/mgzip2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 02:42:34.846496 mgzip2-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-29 02:42:25.000000 mgzip2-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:18.177385 mgzip2-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-29 14:05:07.000000 mgzip2-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 14:05:18.177385 mgzip2-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-29 14:05:07.000000 mgzip2-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:18.173384 mgzip2-0.2.6/mgzip/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-29 14:05:07.000000 mgzip2-0.2.6/mgzip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-29 14:05:07.000000 mgzip2-0.2.6/mgzip/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27531 2023-07-29 14:05:07.000000 mgzip2-0.2.6/mgzip/multiProcGzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:05:18.173384 mgzip2-0.2.6/mgzip2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-29 14:05:18.000000 mgzip2-0.2.6/mgzip2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-29 14:05:18.000000 mgzip2-0.2.6/mgzip2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:05:18.000000 mgzip2-0.2.6/mgzip2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 14:05:18.000000 mgzip2-0.2.6/mgzip2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:05:18.177385 mgzip2-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-29 14:05:07.000000 mgzip2-0.2.6/setup.py
```

### Comparing `mgzip2-0.2.4/LICENSE` & `mgzip2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mgzip2-0.2.4/PKG-INFO` & `mgzip2-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgzip2
-Version: 0.2.4
+Version: 0.2.6
 Summary: A multi-threading implementation of Python gzip module
 Home-page: https://github.com/MichalRIcar/mgzip2
 Author: Vincent Li | Michal Ricar
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mgzip2-0.2.4/README.md` & `mgzip2-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mgzip2-0.2.4/mgzip/__main__.py` & `mgzip2-0.2.6/mgzip/__main__.py`

 * *Files identical despite different names*

### Comparing `mgzip2-0.2.4/mgzip/multiProcGzip.py` & `mgzip2-0.2.6/mgzip/multiProcGzip.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import builtins
 import struct
 import zlib
 import io
 from gzip import GzipFile, write32u, _GzipReader, _PaddedFile, READ, WRITE, FEXTRA, FNAME, FCOMMENT, FHCRC
 from multiprocessing.dummy import Pool
 
-__version__ = "0.2.4"
+__version__ = "0.2.6"
 
 SID = b'IG' # Subfield ID of indexed gzip file
 
 def open(filename, mode="rb", compresslevel=9,
          encoding=None, errors=None, newline=None,
          thread=None, blocksize=10**8):
     """Open a gzip-compressed file in binary or text mode.
@@ -448,15 +448,21 @@
                 self._buffer.close()
         finally:
             self.fileobj = None
             myfileobj = self.myfileobj
             if myfileobj:
                 self.myfileobj = None
                 myfileobj.close()
-
+                     
+            if self.mode == WRITE:
+                self.pool.close()
+                self.pool.join()
+            elif self.mode == READ:
+                self.raw.close()
+                     
     def flush(self):
         self._check_not_closed()
         if self.mode == WRITE:
             self._flush_pool(force=True)
             self.fileobj.flush()
 
 class _MulitGzipReader(_GzipReader):
```

### Comparing `mgzip2-0.2.4/mgzip2.egg-info/PKG-INFO` & `mgzip2-0.2.6/mgzip2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgzip2
-Version: 0.2.4
+Version: 0.2.6
 Summary: A multi-threading implementation of Python gzip module
 Home-page: https://github.com/MichalRIcar/mgzip2
 Author: Vincent Li | Michal Ricar
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mgzip2-0.2.4/setup.py` & `mgzip2-0.2.6/setup.py`

 * *Files identical despite different names*

