# Comparing `tmp/pyapriltags-3.3.0.post1-py3-none-win_amd64.whl.zip` & `tmp/pyapriltags-3.3.0.post2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 1377121 bytes, number of entries: 8
+Zip file size: 1377384 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       91 b- defN 22-Dec-02 20:22 pyapriltags/__init__.py
--rw-r--r--  2.0 unx    19558 b- defN 22-Dec-02 23:01 pyapriltags/apriltags.py
--rwxr-xr-x  2.0 unx  2169263 b- defN 22-Dec-02 23:07 pyapriltags/libapriltag.dll
--rw-r--r--  2.0 unx     3044 b- defN 22-Dec-02 23:07 pyapriltags-3.3.0.post1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    12769 b- defN 22-Dec-02 23:07 pyapriltags-3.3.0.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 22-Dec-02 23:07 pyapriltags-3.3.0.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Dec-02 23:07 pyapriltags-3.3.0.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      687 b- defN 22-Dec-02 23:07 pyapriltags-3.3.0.post1.dist-info/RECORD
-8 files, 2205522 bytes uncompressed, 1375919 bytes compressed:  37.6%
+-rw-r--r--  2.0 unx    19603 b- defN 22-Dec-02 23:30 pyapriltags/apriltags.py
+-rwxr-xr-x  2.0 unx  2169263 b- defN 22-Dec-03 09:38 pyapriltags/libapriltag.dll
+-rw-r--r--  2.0 unx       97 b- defN 22-Dec-02 20:22 pyapriltags/py.typed
+-rw-r--r--  2.0 unx     3044 b- defN 22-Dec-03 09:38 pyapriltags-3.3.0.post2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    12769 b- defN 22-Dec-03 09:38 pyapriltags-3.3.0.post2.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 22-Dec-03 09:38 pyapriltags-3.3.0.post2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Dec-03 09:38 pyapriltags-3.3.0.post2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      762 b- defN 22-Dec-03 09:38 pyapriltags-3.3.0.post2.dist-info/RECORD
+9 files, 2205739 bytes uncompressed, 1376066 bytes compressed:  37.6%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: pyapriltags/apriltags.py
 Comment: 
 
 Filename: pyapriltags/libapriltag.dll
 Comment: 
 
-Filename: pyapriltags-3.3.0.post1.dist-info/LICENSE.md
+Filename: pyapriltags/py.typed
 Comment: 
 
-Filename: pyapriltags-3.3.0.post1.dist-info/METADATA
+Filename: pyapriltags-3.3.0.post2.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyapriltags-3.3.0.post1.dist-info/WHEEL
+Filename: pyapriltags-3.3.0.post2.dist-info/METADATA
 Comment: 
 
-Filename: pyapriltags-3.3.0.post1.dist-info/top_level.txt
+Filename: pyapriltags-3.3.0.post2.dist-info/WHEEL
 Comment: 
 
-Filename: pyapriltags-3.3.0.post1.dist-info/RECORD
+Filename: pyapriltags-3.3.0.post2.dist-info/top_level.txt
+Comment: 
+
+Filename: pyapriltags-3.3.0.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyapriltags/apriltags.py

```diff
@@ -11,15 +11,15 @@
 Apriltags 3 version: Aleksandar Petrov, Spring 2019
 Current maintainer: Will Barber
 
 """
 import ctypes
 import os
 import sys
-from typing import Any, Dict, List, NamedTuple, Optional, Union
+from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 
 import numpy
 
 dir_path = os.path.dirname(os.path.realpath(__file__))
 
 
 ######################################################################
@@ -356,15 +356,15 @@
                     self.libc.tagStandard41h12_destroy(tf)
                 elif 'tagStandard52h13' == family:
                     self.libc.tagStandard52h13_destroy.restype = None
                     self.libc.tagStandard52h13_destroy(tf)
 
     def detect(
         self, img: numpy.ndarray, estimate_tag_pose: bool = False,
-        camera_params: Optional[numpy.ndarray] = None,
+        camera_params: Union[numpy.ndarray, Tuple[float, float, float, float], None] = None,
         tag_size: Union[float, None, Dict[int, float]] = None,
     ) -> List[Detection]:
         """
         Run detectons on the provided image. The image must be a grayscale
         image of type numpy.uint8.
         """
         assert len(img.shape) == 2
```

## pyapriltags/libapriltag.dll

### objdump

```diff
@@ -5,15 +5,15 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Fri Dec  2 23:06:37 2022
+Time/Date		Sat Dec  3 09:37:53 2022
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	38
 SizeOfCode		0000000000036600
 SizeOfInitializedData	000000000017c600
 SizeOfUninitializedData	0000000000000e00
 AddressOfEntryPoint	0000000000001350
@@ -26,15 +26,15 @@
 MajorImageVersion	3
 MinorImageVersion	3
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		0020a000
 SizeOfHeaders		00000600
-CheckSum		0021b543
+CheckSum		0021dd2c
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -156,15 +156,15 @@
  00180028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2c6a9d000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		638a84fd
+Time/Date stamp 		638b18f1
 Major/Minor 			0/0
 Name 				000000000017dd2a libapriltag.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000014d
 	[Name Pointer/Ordinal] Table	0000014d
 Table Addresses
@@ -579967,16 +579967,16 @@
 	...
 
 Disassembly of section .edata:
 
 00000002c6a9d000 <.edata>:
    2c6a9d000:	add    %al,(%rax)
    2c6a9d002:	add    %al,(%rax)
-   2c6a9d004:	std
-   2c6a9d005:	test   %cl,0x63(%rdx)
+   2c6a9d004:	int1
+   2c6a9d005:	sbb    %cl,0x63(%rbx)
    2c6a9d00b:	add    %ch,(%rdx)
    2c6a9d00d:	fstl   (%rdi)
    2c6a9d00f:	add    %al,(%rcx)
    2c6a9d011:	add    %al,(%rax)
    2c6a9d013:	add    %cl,0x1(%rbp)
    2c6a9d016:	add    %al,(%rax)
    2c6a9d018:	add    %r8,(%r8)
```

## Comparing `pyapriltags-3.3.0.post1.dist-info/LICENSE.md` & `pyapriltags-3.3.0.post2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyapriltags-3.3.0.post1.dist-info/METADATA` & `pyapriltags-3.3.0.post2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapriltags
-Version: 3.3.0.post1
+Version: 3.3.0.post2
 Summary: Python bindings for the Apriltags library
 Home-page: https://github.com/WillB97/pyapriltags
 Author: Aleksandar Petrov
 Author-email: alpetrov@ethz.ch
 Maintainer: Will Barber
 License: BSD
 Platform: UNKNOWN
```

