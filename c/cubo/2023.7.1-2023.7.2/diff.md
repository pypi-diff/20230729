# Comparing `tmp/cubo-2023.7.1.tar.gz` & `tmp/cubo-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubo-2023.7.1.tar", last modified: Wed Jul 26 14:25:17 2023, max compression
+gzip compressed data, was "cubo-2023.7.2.tar", last modified: Sat Jul 29 14:16:07 2023, max compression
```

## Comparing `cubo-2023.7.1.tar` & `cubo-2023.7.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.367131 cubo-2023.7.1/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 12:31:14.000000 cubo-2023.7.1/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-26 14:25:17.367131 cubo-2023.7.1/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7050 2023-07-09 12:31:14.000000 cubo-2023.7.1/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.363797 cubo-2023.7.1/cubo/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      178 2023-07-26 14:11:23.000000 cubo-2023.7.1/cubo/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4006 2023-07-26 14:05:48.000000 cubo-2023.7.1/cubo/cubo.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2401 2023-07-09 12:31:14.000000 cubo-2023.7.1/cubo/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.363797 cubo-2023.7.1/cubo.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      110 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-26 14:25:17.367131 cubo-2023.7.1/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1340 2023-07-26 14:11:30.000000 cubo-2023.7.1/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-29 14:16:07.245395 cubo-2023.7.2/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 12:31:14.000000 cubo-2023.7.2/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-29 14:16:07.245395 cubo-2023.7.2/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7050 2023-07-09 12:31:14.000000 cubo-2023.7.2/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-29 14:16:07.245395 cubo-2023.7.2/cubo/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      178 2023-07-29 14:12:34.000000 cubo-2023.7.2/cubo/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4156 2023-07-28 20:31:45.000000 cubo-2023.7.2/cubo/cubo.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3228 2023-07-28 20:30:02.000000 cubo-2023.7.2/cubo/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-29 14:16:07.245395 cubo-2023.7.2/cubo.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-29 14:16:07.000000 cubo-2023.7.2/cubo.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-07-29 14:16:07.000000 cubo-2023.7.2/cubo.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-29 14:16:07.000000 cubo-2023.7.2/cubo.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      110 2023-07-29 14:16:07.000000 cubo-2023.7.2/cubo.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-07-29 14:16:07.000000 cubo-2023.7.2/cubo.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-29 14:16:07.245395 cubo-2023.7.2/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1340 2023-07-29 14:12:16.000000 cubo-2023.7.2/setup.py
```

### Comparing `cubo-2023.7.1/LICENSE` & `cubo-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cubo-2023.7.1/PKG-INFO` & `cubo-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cubo Version: 2023.7.1 Summary: Easily create EO
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.2 Summary: Easily create EO
 mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
```

### Comparing `cubo-2023.7.1/README.md` & `cubo-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `cubo-2023.7.1/cubo/cubo.py` & `cubo-2023.7.2/cubo/cubo.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import pandas as pd
 import planetary_computer as pc
 import pystac_client
 import rasterio.features
 import stackstac
 import xarray as xr
 
-from .utils import _central_pixel_bbox
+from .utils import _central_pixel_bbox, _compute_distance_to_center
 
 
 def create(
     lat: Union[float, int],
     lon: Union[float, int],
-    collection: str,    
+    collection: str,
     start_date: str,
     end_date: str,
     bands: Optional[Union[str, List[str]]] = None,
     edge_size: Union[float, int] = 128.0,
     resolution: Union[float, int] = 10.0,
     stac: str = "https://planetarycomputer.microsoft.com/api/stac/v1",
     **kwargs,
@@ -134,11 +134,15 @@
         central_lon=lon,
         central_y=utm_coords[1],
         central_x=utm_coords[0],
         time_coverage_start=start_date,
         time_coverage_end=end_date,
     )
 
+    cube = cube.assign_coords(
+        {"cubo:distance_from_center": (["y", "x"], _compute_distance_to_center(cube))}
+    )
+
     # New name
     cube.name = collection
 
     return cube
```

### Comparing `cubo-2023.7.1/cubo.egg-info/PKG-INFO` & `cubo-2023.7.2/cubo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cubo Version: 2023.7.1 Summary: Easily create EO
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.2 Summary: Easily create EO
 mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
```

### Comparing `cubo-2023.7.1/setup.py` & `cubo-2023.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="cubo",
-    version="2023.7.1",
+    version="2023.7.2",
     url="https://github.com/davemlz/cubo",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Easily create EO mini cubes from STAC in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

