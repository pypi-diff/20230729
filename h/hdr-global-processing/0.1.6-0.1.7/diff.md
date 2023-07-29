# Comparing `tmp/hdr_global_processing-0.1.6-py3-none-any.whl.zip` & `tmp/hdr_global_processing-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2720 bytes, number of entries: 6
+Zip file size: 2711 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-29 16:03 hdrglobal/__init__.py
--rw-rw-rw-  2.0 fat     3782 b- defN 23-Jul-29 15:55 hdrglobal/processor.py
--rw-rw-rw-  2.0 fat      330 b- defN 23-Jul-29 18:10 hdr_global_processing-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 18:10 hdr_global_processing-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-29 18:10 hdr_global_processing-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      507 b- defN 23-Jul-29 18:10 hdr_global_processing-0.1.6.dist-info/RECORD
-6 files, 4721 bytes uncompressed, 1788 bytes compressed:  62.1%
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-Jul-29 18:16 hdrglobal/processor.py
+-rw-rw-rw-  2.0 fat      330 b- defN 23-Jul-29 18:16 hdr_global_processing-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-29 18:16 hdr_global_processing-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-29 18:16 hdr_global_processing-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      507 b- defN 23-Jul-29 18:16 hdr_global_processing-0.1.7.dist-info/RECORD
+6 files, 4676 bytes uncompressed, 1779 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: hdrglobal/__init__.py
 Comment: 
 
 Filename: hdrglobal/processor.py
 Comment: 
 
-Filename: hdr_global_processing-0.1.6.dist-info/METADATA
+Filename: hdr_global_processing-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: hdr_global_processing-0.1.6.dist-info/WHEEL
+Filename: hdr_global_processing-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: hdr_global_processing-0.1.6.dist-info/top_level.txt
+Filename: hdr_global_processing-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hdr_global_processing-0.1.6.dist-info/RECORD
+Filename: hdr_global_processing-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hdrglobal/processor.py

```diff
@@ -1,12 +1,12 @@
-from hdrglobal.resources.crfio import CRF_importer, CRF_exporter
-from hdrglobal.resources.hdr_merge import merging
-from hdrglobal.resources.ldr_sharpen import LDR_sharpen
-from hdrglobal.resources.tonemaping import tonemaping
-from hdrglobal.resources.crf_calc import CRF_calculate
+from .resources.crfio import CRF_importer, CRF_exporter
+from .resources.hdr_merge import merging
+from .resources.ldr_sharpen import LDR_sharpen
+from .resources.tonemaping import tonemaping
+from .resources.crf_calc import CRF_calculate
 
 
 def processor(source, selector, gamma, saturation, sharpening_iteration, s, r, mode="processing",
               crf_bottom_path="../config/crf_bottom.npy", crf_perif_path="../config/crf_perif.npy"):
     """
     Processes a collection of images with specified parameters.
     The function handles multi-exposure image processing tasks.
```

