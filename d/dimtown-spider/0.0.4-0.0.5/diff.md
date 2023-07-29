# Comparing `tmp/dimtown_spider-0.0.4.tar.gz` & `tmp/dimtown_spider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimtown_spider-0.0.4.tar", max compression
+gzip compressed data, was "dimtown_spider-0.0.5.tar", max compression
```

## Comparing `dimtown_spider-0.0.4.tar` & `dimtown_spider-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/LICENSE
--rw-r--r--   0        0        0     2028 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/README.md
--rw-r--r--   0        0        0     1584 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/AnimeAvatar.py
--rw-r--r--   0        0        0     1097 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/ArtAlbum.py
--rw-r--r--   0        0        0      912 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/CoupleAvatar.py
--rw-r--r--   0        0        0     1076 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/FemaleAvatar.py
--rw-r--r--   0        0        0     1005 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/Figure.py
--rw-r--r--   0        0        0     1085 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/MaleAvatar.py
--rw-r--r--   0        0        0     1329 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/SelectedIllustrations.py
--rw-r--r--   0        0        0     1273 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/SelectedPixiv.py
--rw-r--r--   0        0        0      922 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/__init__.py
--rw-r--r--   0        0        0     1125 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/cosplay.py
--rw-r--r--   0        0        0     1101 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/hanfu.py
--rw-r--r--   0        0        0     1066 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/jk.py
--rw-r--r--   0        0        0     1263 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/lolita.py
--rw-r--r--   0        0        0     1273 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/pcpic.py
--rw-r--r--   0        0        0     1327 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/phonepic.py
--rw-r--r--   0        0        0     4199 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/utils.py
--rw-r--r--   0        0        0      399 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 dimtown_spider-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2028 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/README.md
+-rw-r--r--   0        0        0     1584 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/AnimeAvatar.py
+-rw-r--r--   0        0        0     1097 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/ArtAlbum.py
+-rw-r--r--   0        0        0      912 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/CoupleAvatar.py
+-rw-r--r--   0        0        0     1076 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/FemaleAvatar.py
+-rw-r--r--   0        0        0     1005 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/Figure.py
+-rw-r--r--   0        0        0     1085 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/MaleAvatar.py
+-rw-r--r--   0        0        0     1329 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/SelectedIllustrations.py
+-rw-r--r--   0        0        0     1273 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/SelectedPixiv.py
+-rw-r--r--   0        0        0     1004 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/__init__.py
+-rw-r--r--   0        0        0     1125 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/cosplay.py
+-rw-r--r--   0        0        0     1101 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/hanfu.py
+-rw-r--r--   0        0        0     1066 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/jk.py
+-rw-r--r--   0        0        0     1263 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/lolita.py
+-rw-r--r--   0        0        0     1273 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/pcpic.py
+-rw-r--r--   0        0        0     1327 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/phonepic.py
+-rw-r--r--   0        0        0     1646 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/search.py
+-rw-r--r--   0        0        0     4199 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/dimtown/utils.py
+-rw-r--r--   0        0        0      399 2023-07-29 13:25:05.074493 dimtown_spider-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 dimtown_spider-0.0.5/PKG-INFO
```

### Comparing `dimtown_spider-0.0.4/LICENSE` & `dimtown_spider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/README.md` & `dimtown_spider-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/AnimeAvatar.py` & `dimtown_spider-0.0.5/dimtown/AnimeAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/ArtAlbum.py` & `dimtown_spider-0.0.5/dimtown/ArtAlbum.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/CoupleAvatar.py` & `dimtown_spider-0.0.5/dimtown/CoupleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/FemaleAvatar.py` & `dimtown_spider-0.0.5/dimtown/FemaleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/Figure.py` & `dimtown_spider-0.0.5/dimtown/Figure.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/MaleAvatar.py` & `dimtown_spider-0.0.5/dimtown/MaleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/SelectedIllustrations.py` & `dimtown_spider-0.0.5/dimtown/SelectedIllustrations.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/SelectedPixiv.py` & `dimtown_spider-0.0.5/dimtown/SelectedPixiv.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/__init__.py` & `dimtown_spider-0.0.5/dimtown/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,33 @@
 from .jk import JK
 from .lolita import Lolita
 from .MaleAvatar import MaleAvatar
 from .pcpic import PcPic
 from .phonepic import PhonePic
 from .SelectedIllustrations import SelectedIllustrations
 from .SelectedPixiv import SelectedPixiv
+from .search import Search
 
-__all__ = ['AnimeAvatar', 'ArtAlbum', 'CosPlay', 'CoupleAvatar', 'FemaleAvatar', 'Figure', 
-            'HanFu', 'JK', 'Lolita', 'MaleAvatar', 'PcPic', 'PhonePic', 'SelectedIllustrations', 
-            'SelectedPixiv']
-__title__ = 'dimtown'
-__description__ = 'A Spider for https://dimtown.com'
-__url__ = 'https://github.com/Cvandia/dimtown-spider'
-__version__ = '0.0.4'
-__author__ = 'Cvandia'
-__author_email__ = '1141538825@qq.com'
-__license__ = 'MIT License'
+__all__ = [
+    "AnimeAvatar",
+    "ArtAlbum",
+    "CosPlay",
+    "CoupleAvatar",
+    "FemaleAvatar",
+    "Figure",
+    "HanFu",
+    "JK",
+    "Lolita",
+    "MaleAvatar",
+    "PcPic",
+    "PhonePic",
+    "SelectedIllustrations",
+    "SelectedPixiv",
+    "Search",
+]
+__title__ = "dimtown"
+__description__ = "A Spider for https://dimtown.com"
+__url__ = "https://github.com/Cvandia/dimtown-spider"
+__version__ = "0.0.5"
+__author__ = "Cvandia"
+__author_email__ = "1141538825@qq.com"
+__license__ = "Apache License 2.0"
```

### Comparing `dimtown_spider-0.0.4/dimtown/cosplay.py` & `dimtown_spider-0.0.5/dimtown/cosplay.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/hanfu.py` & `dimtown_spider-0.0.5/dimtown/hanfu.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/jk.py` & `dimtown_spider-0.0.5/dimtown/jk.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/lolita.py` & `dimtown_spider-0.0.5/dimtown/lolita.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/pcpic.py` & `dimtown_spider-0.0.5/dimtown/pcpic.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/phonepic.py` & `dimtown_spider-0.0.5/dimtown/phonepic.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/dimtown/utils.py` & `dimtown_spider-0.0.5/dimtown/utils.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.4/PKG-INFO` & `dimtown_spider-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimtown-spider
-Version: 0.0.4
+Version: 0.0.5
 Summary: A spider for https://dimtown.com
 Author: divandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

