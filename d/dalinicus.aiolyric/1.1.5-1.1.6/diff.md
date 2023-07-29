# Comparing `tmp/dalinicus.aiolyric-1.1.5.tar.gz` & `tmp/dalinicus.aiolyric-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalinicus.aiolyric-1.1.5.tar", last modified: Sat Jul 29 20:32:59 2023, max compression
+gzip compressed data, was "dalinicus.aiolyric-1.1.6.tar", last modified: Sat Jul 29 20:35:45 2023, max compression
```

## Comparing `dalinicus.aiolyric-1.1.5.tar` & `dalinicus.aiolyric-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.020167 dalinicus.aiolyric-1.1.5/
--rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      819 2023-07-29 20:32:59.019666 dalinicus.aiolyric-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.005597 dalinicus.aiolyric-1.1.5/aiolyric/
--rw-rw-rw-   0        0        0     6184 2023-07-29 20:32:40.000000 dalinicus.aiolyric-1.1.5/aiolyric/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.006596 dalinicus.aiolyric-1.1.5/aiolyric/client/
--rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/client/__init__.py
--rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/const.py
--rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.010159 dalinicus.aiolyric-1.1.5/aiolyric/objects/
--rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/__init__.py
--rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/base.py
--rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/device.py
--rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/location.py
--rw-rw-rw-   0        0        0     2267 2023-07-29 20:32:15.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/priority.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.018158 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/
--rw-rw-rw-   0        0        0      819 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 20:32:59.020167 dalinicus.aiolyric-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-29 20:32:53.000000 dalinicus.aiolyric-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:35:45.225891 dalinicus.aiolyric-1.1.6/
+-rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:35:45.225891 dalinicus.aiolyric-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 20:35:45.209831 dalinicus.aiolyric-1.1.6/aiolyric/
+-rw-rw-rw-   0        0        0     6203 2023-07-29 20:35:16.000000 dalinicus.aiolyric-1.1.6/aiolyric/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:35:45.210831 dalinicus.aiolyric-1.1.6/aiolyric/client/
+-rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/client/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/const.py
+-rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:35:45.214841 dalinicus.aiolyric-1.1.6/aiolyric/objects/
+-rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/objects/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/objects/base.py
+-rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/objects/device.py
+-rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.6/aiolyric/objects/location.py
+-rw-rw-rw-   0        0        0     2267 2023-07-29 20:32:15.000000 dalinicus.aiolyric-1.1.6/aiolyric/objects/priority.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:35:45.224387 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:35:45.000000 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-29 20:35:45.000000 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 20:35:45.000000 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 20:35:45.000000 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 20:35:45.000000 dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 20:35:45.226391 dalinicus.aiolyric-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-29 20:35:38.000000 dalinicus.aiolyric-1.1.6/setup.py
```

### Comparing `dalinicus.aiolyric-1.1.5/LICENSE` & `dalinicus.aiolyric-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.5/PKG-INFO` & `dalinicus.aiolyric-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.5
+Version: 1.1.6
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.5/aiolyric/__init__.py` & `dalinicus.aiolyric-1.1.6/aiolyric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,18 @@
             f"{BASE_URL}/devices/thermostats/{device_id}/priority?apikey={self.client_id}&locationId={location_id}"
         )
         json = await response.json()
         self.logger.debug(json)
         
         priority = LyricPriority(json)
 
-        self._rooms_dict[priority.deviceId]: dict = {}
+        macId = priority.deviceId
+        self._rooms_dict[macId]: dict = {}
         for room in priority.currentPriority.rooms:
-            self._rooms_dict[device_id][room.id] = room
+            self._rooms_dict[macId][room.id] = room
 
     async def update_thermostat(
         self,
         location: LyricLocation,
         device: LyricDevice,
         mode=None,
         heatSetpoint=None,
```

### Comparing `dalinicus.aiolyric-1.1.5/aiolyric/client/__init__.py` & `dalinicus.aiolyric-1.1.6/aiolyric/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.5/aiolyric/objects/device.py` & `dalinicus.aiolyric-1.1.6/aiolyric/objects/device.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.5/aiolyric/objects/location.py` & `dalinicus.aiolyric-1.1.6/aiolyric/objects/location.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.5/aiolyric/objects/priority.py` & `dalinicus.aiolyric-1.1.6/aiolyric/objects/priority.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/PKG-INFO` & `dalinicus.aiolyric-1.1.6/dalinicus.aiolyric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.5
+Version: 1.1.6
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.5/setup.py` & `dalinicus.aiolyric-1.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import io
 
 from setuptools import find_packages, setup
 
-version = "1.1.5"
+version = "1.1.6"
 
 setup(
     name="dalinicus.aiolyric",
     version=version,
     description="AIO package for the Honeywell Lyric Platform.",
     long_description=io.open("README.md", encoding="UTF-8").read(),
     keywords="honeywell lyric thermostat",
```

