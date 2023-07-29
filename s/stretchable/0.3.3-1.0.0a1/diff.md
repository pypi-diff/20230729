# Comparing `tmp/stretchable-0.3.3-cp37-abi3-win_arm64.whl.zip` & `tmp/stretchable-1.0.0a1-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 158897 bytes, number of entries: 9
--rw-r--r--  4.6 unx     1711 b- defN 23-Jul-29 14:18 stretchable-0.3.3.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-29 14:18 stretchable-0.3.3.dist-info/WHEEL
--rw-r--r--  4.6 unx     1106 b- defN 23-Jul-29 14:18 stretchable-0.3.3.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     1505 b- defN 23-Jul-29 14:18 stretchable/layout.py
--rw-r--r--  4.6 unx     6115 b- defN 23-Jul-29 14:18 stretchable/node.py
--rw-r--r--  4.6 unx    11744 b- defN 23-Jul-29 14:18 stretchable/style.py
--rw-r--r--  4.6 unx     1211 b- defN 23-Jul-29 14:18 stretchable/__init__.py
--rwxr-xr-x  4.6 unx   337920 b- defN 23-Jul-29 14:18 stretchable/stretch.pyd
--rw-r--r--  4.6 unx      718 b- defN 23-Jul-29 14:18 stretchable-0.3.3.dist-info/RECORD
-9 files, 362124 bytes uncompressed, 157675 bytes compressed:  56.5%
+Zip file size: 159104 bytes, number of entries: 9
+-rw-r--r--  4.6 unx     2319 b- defN 23-Jul-29 15:31 stretchable-1.0.0a1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-29 15:31 stretchable-1.0.0a1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1106 b- defN 23-Jul-29 15:31 stretchable-1.0.0a1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     1505 b- defN 23-Jul-29 15:31 stretchable/layout.py
+-rw-r--r--  4.6 unx     6686 b- defN 23-Jul-29 15:31 stretchable/node.py
+-rw-r--r--  4.6 unx    11699 b- defN 23-Jul-29 15:31 stretchable/style.py
+-rw-r--r--  4.6 unx      608 b- defN 23-Jul-29 15:31 stretchable/__init__.py
+-rwxr-xr-x  4.6 unx   337920 b- defN 23-Jul-29 15:31 stretchable/stretch.pyd
+-rw-r--r--  4.6 unx      725 b- defN 23-Jul-29 15:31 stretchable-1.0.0a1.dist-info/RECORD
+9 files, 362662 bytes uncompressed, 157866 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: stretchable-0.3.3.dist-info/METADATA
+Filename: stretchable-1.0.0a1.dist-info/METADATA
 Comment: 
 
-Filename: stretchable-0.3.3.dist-info/WHEEL
+Filename: stretchable-1.0.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: stretchable-0.3.3.dist-info/license_files/LICENSE
+Filename: stretchable-1.0.0a1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: stretchable/layout.py
 Comment: 
 
 Filename: stretchable/node.py
 Comment: 
@@ -18,11 +18,11 @@
 
 Filename: stretchable/__init__.py
 Comment: 
 
 Filename: stretchable/stretch.pyd
 Comment: 
 
-Filename: stretchable-0.3.3.dist-info/RECORD
+Filename: stretchable-1.0.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stretchable/node.py

```diff
@@ -1,22 +1,43 @@
 import math
 from typing import Callable, List, Optional
 
-from . import Stretch, _bindings
 from .layout import Layout
+from .stretch import _bindings
 from .style import _NAN, Size, Style
 
 # ========================================================================= #
 # NODE                                                                      #
 # ========================================================================= #
 
 
 MeasureFunc = Callable[[Size], Size]
 
 
+class Stretch:
+    _PRIVATE_PTR: int = None
+
+    def __init__(self):
+        raise Exception(
+            "You should not be accessing or attempting to create an instance of this class."
+        )
+
+    @staticmethod
+    def get_ptr():
+        if Stretch._PRIVATE_PTR is None:
+            Stretch._PRIVATE_PTR = _bindings.stretch_init()
+        return Stretch._PRIVATE_PTR
+
+    @staticmethod
+    def reset():
+        if not Stretch._PRIVATE_PTR is None:
+            _bindings.stretch_free(Stretch._PRIVATE_PTR)
+            Stretch._PRIVATE_PTR = None
+
+
 def reset():
     Stretch.reset()
 
 
 class Node:
     def __init__(
         self,
```

## stretchable/style.py

```diff
@@ -1,13 +1,11 @@
 from enum import IntEnum
 from typing import Generic, Optional, TypeVar
 
-from . import _bindings
-
-# from multiprocessing.sharedctypes import Value
+from .stretch import _bindings
 
 # ========================================================================= #
 # STYLE - ENUMS                                                             #
 # ========================================================================= #
 
 
 class AlignItems(IntEnum):
```

## stretchable/__init__.py

```diff
@@ -3,15 +3,14 @@
 
 # Stretch is an implementation of CSS Flexbox written in Rust:
 # https://github.com/vislyhq/stretch
 
 # import bindings etc.
 from .layout import Layout
 from .node import Node, reset
-from .stretch import _bindings
 from .style import (
     AlignContent,
     AlignItems,
     AlignSelf,
     Dimension,
     DimensionValue,
     Direction,
@@ -26,27 +25,7 @@
     Style,
     auto,
     pct,
     pt,
     undef,
 )
 
-
-class Stretch:
-    _PRIVATE_PTR: int = None
-
-    def __init__(self):
-        raise Exception(
-            "You should not be accessing or attempting to create an instance of this class."
-        )
-
-    @staticmethod
-    def get_ptr():
-        if Stretch._PRIVATE_PTR is None:
-            Stretch._PRIVATE_PTR = _bindings.stretch_init()
-        return Stretch._PRIVATE_PTR
-
-    @staticmethod
-    def reset():
-        if not Stretch._PRIVATE_PTR is None:
-            _bindings.stretch_free(Stretch._PRIVATE_PTR)
-            Stretch._PRIVATE_PTR = None
```

## Comparing `stretchable-0.3.3.dist-info/METADATA` & `stretchable-1.0.0a1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 Metadata-Version: 2.1
 Name: stretchable
-Version: 0.3.3
+Version: 1.0.0a1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: maturin >=1.1, <2.0 ; extra == 'build'
 Requires-Dist: build ; extra == 'build'
 Requires-Dist: twine ; extra == 'build'
 Provides-Extra: build
 License-File: LICENSE
 Summary: Python bindings for Stretch (high performance flexbox implementation)
+Keywords: flexbox,stretch,css,layout
 Author: Kenneth Trelborg Vestergaard
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/mortencombat/stretchable
+Project-URL: repository, https://github.com/mortencombat/stretchable
 
 # Introduction
 
-This package enables target-agnostic layout operations using the CSS flexbox algorithm.
+This package enables target-agnostic layout operations using the CSS flexbox algorithm. For instance, it can be used for page layouts in reporting tools, etc.
 
-It implements Python bindings for [Stretch](https://vislyhq.github.io/stretch/), an implementation of Flexbox written in [Rust](https://www.rust-lang.org/).
-
-The project is based on the translation of the bindings from Swift to Python, from [stretched](https://github.com/nmichlo/stretched)
+It implements Python bindings for [Stretch](https://vislyhq.github.io/stretch/), an implementation of Flexbox written in [Rust](https://www.rust-lang.org/). The project is based on the translation of the bindings from Swift to Python, from [stretched](https://github.com/nmichlo/stretched).
 
 # Getting Started
 
 Helpful resources to getting started with CSS Flexbox include:
 
 - [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
 - [Flexbox Froggy](https://flexboxfroggy.com/)
 - [Yoga Playground](https://yogalayout.com/playground)
 
-# Build and Test
+# Usage
+
+See [demos](https://github.com/mortencombat/stretchable/tree/main/demos) for examples of basic usage. Keep in mind that the current version of Stretchable is early stage and the API can be expected to change (eg. improve).
+
+# Contributing
 
-Build and publish is handled automatically using Github Actions.
+Install Rust with [rustup](https://rustup.rs/) and use `maturin build [--release]` to build.
 
-# Contribute
+# License
 
-TODO: Explain how other users and developers can contribute.
+This work is released under the MIT license. A copy of the license is provided in the [LICENSE](https://github.com/mortencombat/stretchable/blob/main/LICENSE) file.
```

## Comparing `stretchable-0.3.3.dist-info/license_files/LICENSE` & `stretchable-1.0.0a1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `stretchable-0.3.3.dist-info/RECORD` & `stretchable-1.0.0a1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-stretchable-0.3.3.dist-info/METADATA,sha256=VaKHttwvB3LXNCekX8TXMNc7UKC7UxRUZElxICJNsS4,1711
-stretchable-0.3.3.dist-info/WHEEL,sha256=r2ZcmhlIh7eF2JLb1VlYcDTNryw-vUvm0cQuE_oUI8Y,94
-stretchable-0.3.3.dist-info/license_files/LICENSE,sha256=ICo42IBkViHgT3nUFDsRIWXd28vhSnpcw96zIBOeNGg,1106
+stretchable-1.0.0a1.dist-info/METADATA,sha256=d7YTu4GdJj4t9x6sKOPaH4jHDSwh2k8ltzBtBUv3ua0,2319
+stretchable-1.0.0a1.dist-info/WHEEL,sha256=r2ZcmhlIh7eF2JLb1VlYcDTNryw-vUvm0cQuE_oUI8Y,94
+stretchable-1.0.0a1.dist-info/license_files/LICENSE,sha256=ICo42IBkViHgT3nUFDsRIWXd28vhSnpcw96zIBOeNGg,1106
 stretchable/layout.py,sha256=p23MpKxbL1SXCMhVGiYyyhdcfNfZAaVbrH1lIaUMksI,1505
-stretchable/node.py,sha256=cceBUZ2Zu_lYOgtBewaEhM_NTlPabbpehBhJmESA8T4,6115
-stretchable/style.py,sha256=G1wfiG6DfnPvuXBxDLWxGcKg3IxOIgUO0DFO1x36WJk,11744
-stretchable/__init__.py,sha256=qeuAKzJVwiwnYdTnllGq9hqCmowUfKsZkDFiqm4TUDs,1211
-stretchable/stretch.pyd,sha256=XPaf0BDc2Qq_VZoesA4EcFAqtLnJ_QC7_ziW5Y7x77k,337920
-stretchable-0.3.3.dist-info/RECORD,,
+stretchable/node.py,sha256=nlT1EDzzoSPJPMW1LBJG28-ZJuDywu8w8EUVxWdIGTM,6686
+stretchable/style.py,sha256=gpwWZhhJsWC2jMjR25wwPpt31UEA9o2vgXB9Iva02Og,11699
+stretchable/__init__.py,sha256=bTJ-5Kj0l4K_r-RdPH-_nx_qaYnjC3c2dMzCzdYjgCw,608
+stretchable/stretch.pyd,sha256=8ydmuSY0cCBVa_iz0e7k1p7RZ2KifJLzItmSnyxW04s,337920
+stretchable-1.0.0a1.dist-info/RECORD,,
```

