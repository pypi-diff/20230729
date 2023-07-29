# Comparing `tmp/stress_injector-0.7-py3-none-any.whl.zip` & `tmp/stress_injector-0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12735 bytes, number of entries: 12
--rw-r--r--  2.0 unx      248 b- defN 23-Apr-16 19:29 stressinjector/__init__.py
--rw-r--r--  2.0 unx     4968 b- defN 23-Apr-16 19:29 stressinjector/cpu.py
--rw-r--r--  2.0 unx      614 b- defN 23-Apr-16 19:29 stressinjector/helper.py
--rw-r--r--  2.0 unx     4832 b- defN 23-Apr-16 19:29 stressinjector/memory.py
--rw-r--r--  2.0 unx     1388 b- defN 23-Apr-16 19:29 stressinjector/models.py
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-16 19:29 stressinjector/requirements.txt
--rw-r--r--  2.0 unx     5495 b- defN 23-Apr-16 19:29 stressinjector/url.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     8973 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      982 b- defN 23-Apr-16 19:29 stress_injector-0.7.dist-info/RECORD
-12 files, 28734 bytes uncompressed, 11081 bytes compressed:  61.4%
+Zip file size: 12749 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      248 b- defN 23-Jul-29 05:49 stressinjector/__init__.py
+-rw-r--r--  2.0 unx     4968 b- defN 23-Jul-29 05:49 stressinjector/cpu.py
+-rw-r--r--  2.0 unx      614 b- defN 23-Jul-29 05:49 stressinjector/helper.py
+-rw-r--r--  2.0 unx     4881 b- defN 23-Jul-29 05:49 stressinjector/memory.py
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jul-29 05:49 stressinjector/models.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-29 05:49 stressinjector/requirements.txt
+-rw-r--r--  2.0 unx     5495 b- defN 23-Jul-29 05:49 stressinjector/url.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Jul-29 05:49 stress_injector-0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8973 b- defN 23-Jul-29 05:49 stress_injector-0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 05:49 stress_injector-0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-29 05:49 stress_injector-0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      982 b- defN 23-Jul-29 05:49 stress_injector-0.8.dist-info/RECORD
+12 files, 28783 bytes uncompressed, 11095 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: stressinjector/requirements.txt
 Comment: 
 
 Filename: stressinjector/url.py
 Comment: 
 
-Filename: stress_injector-0.7.dist-info/LICENSE
+Filename: stress_injector-0.8.dist-info/LICENSE
 Comment: 
 
-Filename: stress_injector-0.7.dist-info/METADATA
+Filename: stress_injector-0.8.dist-info/METADATA
 Comment: 
 
-Filename: stress_injector-0.7.dist-info/WHEEL
+Filename: stress_injector-0.8.dist-info/WHEEL
 Comment: 
 
-Filename: stress_injector-0.7.dist-info/top_level.txt
+Filename: stress_injector-0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: stress_injector-0.7.dist-info/RECORD
+Filename: stress_injector-0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stressinjector/__init__.py

```diff
@@ -1,6 +1,6 @@
 from stressinjector.cpu import CPUStress  # noqa: F401
 from stressinjector.memory import MemoryStress  # noqa: F401
 from stressinjector.models import RequestType  # noqa: F401
 from stressinjector.url import URLStress  # noqa: F401
 
-version = "0.7"
+version = "0.8"
```

## stressinjector/memory.py

```diff
@@ -1,20 +1,22 @@
 import logging
 import math
-import resource
 import time
 from typing import Union
 
 import psutil
 from numpy.random import bytes
 from tqdm import tqdm
 
 from .helper import flush_screen
 from .models import LOGGER, operating_system, settings
 
+if settings.os != operating_system.windows:
+    import resource
+
 
 def _size_converter(byte_size: Union[int, float]) -> str:
     """Gets the current memory consumed and converts it to human friendly format.
 
     Args:
         byte_size: Receives byte size as argument.
```

## Comparing `stress_injector-0.7.dist-info/LICENSE` & `stress_injector-0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stress_injector-0.7.dist-info/METADATA` & `stress_injector-0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stress-injector
-Version: 0.7
+Version: 0.8
 Summary: Python module, to inject memory and CPU stress, and URL load test
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Vignesh Sivanandha Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -154,15 +154,15 @@
 **Requirement**
 ```shell
 python -m pip install changelog-generator
 ```
 
 **Usage**
 ```shell
-changelog reverse -f release_notes.rst -t 'Release Notes'
+changelog reverse -f release_notes.rst -t "Release Notes"
 ```
 
 #### Linting
 `PreCommit` will ensure linting, and the doc creation are run on every commit.
 
 **Requirement**
 <br>
```

## Comparing `stress_injector-0.7.dist-info/RECORD` & `stress_injector-0.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-stressinjector/__init__.py,sha256=-9gH5SzeHoezc3pf1SSmygOE4Y3m6stsdHxifY88Ros,248
+stressinjector/__init__.py,sha256=Dp5yzc5OC6OUbc1u3RhlaIzFbdW_AZ6CSaaevBzMEwc,248
 stressinjector/cpu.py,sha256=LmkAwKTRjJoOUDwnfHUbN_ZmbgR2abnn9weKo5NxSFg,4968
 stressinjector/helper.py,sha256=ZWo7Sa9UlrZM8XvOCgiSsyr_F2BfKWtHjnOW6ffwn0s,614
-stressinjector/memory.py,sha256=NJ27Mup3yKYP9f_ff-93EKMqE4YI9T_Pn4tsZkI1GrI,4832
+stressinjector/memory.py,sha256=_-9XiUO2eGLnWDNEAxEmuA4ntlTKEmx5y-t_iEHIvks,4881
 stressinjector/models.py,sha256=r0qifwX0a1IIlKw05yF4w_Vs_hnT1EHOpPv5h2Vn7e0,1388
 stressinjector/requirements.txt,sha256=o0WLVFGoHLyK73BX_BCqQVYXYt88PYxKZy7MLq9X-Qs,49
 stressinjector/url.py,sha256=tPSK5TAs_Ka92frwGzuLwpYMNJ0_pI1fVq-iqXfXtUU,5495
-stress_injector-0.7.dist-info/LICENSE,sha256=9GP7w3y3dz_gc9ZHCmL88lkaKLeQCj8rj5-_oCIeYWo,1078
-stress_injector-0.7.dist-info/METADATA,sha256=dVET85OuWsUR5rm0RpD7D7SrVsgXC7Pjb9FGm-Qwuv4,8973
-stress_injector-0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-stress_injector-0.7.dist-info/top_level.txt,sha256=2j2pqoZNB0Ruvn7YWu9h8L-ktGLncCvZendmHtkG83Q,15
-stress_injector-0.7.dist-info/RECORD,,
+stress_injector-0.8.dist-info/LICENSE,sha256=9GP7w3y3dz_gc9ZHCmL88lkaKLeQCj8rj5-_oCIeYWo,1078
+stress_injector-0.8.dist-info/METADATA,sha256=kHifrkzgEsimJntxoiB5nVa3ARxa0MMjQpylKLiK5zY,8973
+stress_injector-0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+stress_injector-0.8.dist-info/top_level.txt,sha256=2j2pqoZNB0Ruvn7YWu9h8L-ktGLncCvZendmHtkG83Q,15
+stress_injector-0.8.dist-info/RECORD,,
```

