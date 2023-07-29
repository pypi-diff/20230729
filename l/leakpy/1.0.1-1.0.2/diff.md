# Comparing `tmp/leakpy-1.0.1-py3-none-any.whl.zip` & `tmp/leakpy-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3627 bytes, number of entries: 5
--rwxrwxr-x  2.0 unx     5938 b- defN 23-Mar-04 23:15 leakpy-1.0.1.data/scripts/leakpy
--rw-rw-r--  2.0 unx     1131 b- defN 23-Mar-04 23:15 leakpy-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-04 23:15 leakpy-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Mar-04 23:15 leakpy-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      382 b- defN 23-Mar-04 23:15 leakpy-1.0.1.dist-info/RECORD
-5 files, 7544 bytes uncompressed, 2913 bytes compressed:  61.4%
+Zip file size: 3327 bytes, number of entries: 5
+-rwxr-xr-x  2.0 unx     4655 b- defN 23-Jul-29 17:38 leakpy-1.0.2.data/scripts/leakpy
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      382 b- defN 23-Jul-29 17:38 leakpy-1.0.2.dist-info/RECORD
+5 files, 6261 bytes uncompressed, 2613 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: leakpy-1.0.1.data/scripts/leakpy
+Filename: leakpy-1.0.2.data/scripts/leakpy
 Comment: 
 
-Filename: leakpy-1.0.1.dist-info/METADATA
+Filename: leakpy-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: leakpy-1.0.1.dist-info/WHEEL
+Filename: leakpy-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: leakpy-1.0.1.dist-info/top_level.txt
+Filename: leakpy-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: leakpy-1.0.1.dist-info/RECORD
+Filename: leakpy-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `leakpy-1.0.1.dist-info/METADATA` & `leakpy-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leakpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: LeakIX API Client 
 Home-page: https://github.com/Chocapikk/LeakPy
 Author: Valentin Lobstein
 Author-email: balgogan@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

