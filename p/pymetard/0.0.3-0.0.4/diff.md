# Comparing `tmp/pymetard-0.0.3.tar.gz` & `tmp/pymetard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetard-0.0.3.tar", last modified: Mon Jul 17 04:21:46 2023, max compression
+gzip compressed data, was "pymetard-0.0.4.tar", last modified: Sat Jul 29 07:31:03 2023, max compression
```

## Comparing `pymetard-0.0.3.tar` & `pymetard-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 04:21:36.000000 pymetard-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 04:21:46.566873 pymetard-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 04:21:36.000000 pymetard-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/meteo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/station.py
--rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-17 04:21:36.000000 pymetard-0.0.3/pymetard/metar/stations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.562873 pymetard-0.0.3/pymetard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 04:21:46.000000 pymetard-0.0.3/pymetard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 04:21:36.000000 pymetard-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 04:21:46.566873 pymetard-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-17 04:21:36.000000 pymetard-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/pymetard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:46.566873 pymetard-0.0.3/tests/pymetard/metar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/metar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-17 04:21:36.000000 pymetard-0.0.3/tests/pymetard/metar/test_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-29 07:30:54.000000 pymetard-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-29 07:31:03.322148 pymetard-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-29 07:30:54.000000 pymetard-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.318148 pymetard-0.0.4/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/metar/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/metar/meteo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/metar/station.py
+-rw-r--r--   0 runner    (1001) docker     (123)   814165 2023-07-29 07:30:54.000000 pymetard-0.0.4/pymetard/metar/stations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/pymetard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 07:31:03.000000 pymetard-0.0.4/pymetard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-29 07:30:54.000000 pymetard-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 07:31:03.322148 pymetard-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-29 07:30:54.000000 pymetard-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:30:54.000000 pymetard-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/tests/pymetard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:30:54.000000 pymetard-0.0.4/tests/pymetard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 07:31:03.322148 pymetard-0.0.4/tests/pymetard/metar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 07:30:54.000000 pymetard-0.0.4/tests/pymetard/metar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-29 07:30:54.000000 pymetard-0.0.4/tests/pymetard/metar/test_station.py
```

### Comparing `pymetard-0.0.3/LICENSE` & `pymetard-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.3/PKG-INFO` & `pymetard-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download parsed METAR data.
 Home-page: https://github.com/ai4time/pymetard
 Author: AI4Time
 Author-email: huang.yipeng@hotmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,12 +17,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# AWC METAR Downloader
+# PyMetarD: METAR Data Downloader
 Download parsed METAR data (real-time and historical) from NOAA sites like Aviation Weather Center and Weather.gov.
 
-[![ci](https://github.com/ai4time/pymetard/actions/workflows/ci.yml/badge.svg)](https://github.com/ai4time/pymetard/actions/workflows/ci.yml)
-[![dist](https://github.com/ai4time/pymetard/actions/workflows/dist.yaml/badge.svg)](https://github.com/ai4time/pymetard/actions/workflows/dist.yaml)
+<p>
+    <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
+    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10|3.11-blue.svg" />
+    <img src ="https://img.shields.io/github/actions/workflow/status/ai4time/pymetard/ci.yml?branch=master&label=ci"/>
+    <img src ="https://img.shields.io/github/actions/workflow/status/ai4time/pymetard/dist.yaml?label=dist"/>
+</p>
```

### Comparing `pymetard-0.0.3/pymetard/cli.py` & `pymetard-0.0.4/pymetard/cli.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.3/pymetard/metar/downloader.py` & `pymetard-0.0.4/pymetard/metar/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
     def _fetch_data_from_raw_metar(
         self,
         metar_raw: str,
         year: Optional[int] = None,
         month: Optional[int] = None,
     ) -> Optional[Dict[str, str]]:
         logger.debug(f"Parsing raw METAR: {metar_raw}")
+        metar_raw = self._clean_raw_metar(metar_raw)
         metar_decoded = Metar.Metar(
             metar_raw,
             year=year,
             month=month,
             strict=False,
         )
         station = self.stations[metar_decoded.station_id]
@@ -191,14 +192,17 @@
             f"rh={round(data['relativehumidity'] * 100)}%," if data['relativehumidity'] else ""
             f"wind={round(data['winddirection_deg'])}° " if data['winddirection_deg'] else ""
             f"at {data['windspeed_kt']} knots" if data['windspeed_kt'] else ""
         )
 
         return data
 
+    def _clean_raw_metar(self, metar_raw: str) -> str:
+        return metar_raw.replace("\x00", "")
+
     def _metar_valid(self, metar: Metar.Metar) -> bool:
         return metar.time is not None
 
     def _temperature(self, metar: Metar.Metar) -> Optional[float]:
         if metar.temp is None:
             return None
         return metar.temp.value(units="C")
```

### Comparing `pymetard-0.0.3/pymetard/metar/station.py` & `pymetard-0.0.4/pymetard/metar/station.py`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.3/pymetard/metar/stations.txt` & `pymetard-0.0.4/pymetard/metar/stations.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.3/pymetard.egg-info/PKG-INFO` & `pymetard-0.0.4/pymetard.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download parsed METAR data.
 Home-page: https://github.com/ai4time/pymetard
 Author: AI4Time
 Author-email: huang.yipeng@hotmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,12 +17,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# AWC METAR Downloader
+# PyMetarD: METAR Data Downloader
 Download parsed METAR data (real-time and historical) from NOAA sites like Aviation Weather Center and Weather.gov.
 
-[![ci](https://github.com/ai4time/pymetard/actions/workflows/ci.yml/badge.svg)](https://github.com/ai4time/pymetard/actions/workflows/ci.yml)
-[![dist](https://github.com/ai4time/pymetard/actions/workflows/dist.yaml/badge.svg)](https://github.com/ai4time/pymetard/actions/workflows/dist.yaml)
+<p>
+    <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
+    <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10|3.11-blue.svg" />
+    <img src ="https://img.shields.io/github/actions/workflow/status/ai4time/pymetard/ci.yml?branch=master&label=ci"/>
+    <img src ="https://img.shields.io/github/actions/workflow/status/ai4time/pymetard/dist.yaml?label=dist"/>
+</p>
```

### Comparing `pymetard-0.0.3/pymetard.egg-info/SOURCES.txt` & `pymetard-0.0.4/pymetard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymetard-0.0.3/setup.py` & `pymetard-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import setuptools
 
 
-CLIENT_VERSION = "0.0.3"
+CLIENT_VERSION = "0.0.4"
 PACKAGE_NAME = "pymetard"
 
 try:
     with io.open("README.md", encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
```

### Comparing `pymetard-0.0.3/tests/pymetard/metar/test_station.py` & `pymetard-0.0.4/tests/pymetard/metar/test_station.py`

 * *Files identical despite different names*

