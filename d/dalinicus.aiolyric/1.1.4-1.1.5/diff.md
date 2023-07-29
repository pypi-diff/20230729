# Comparing `tmp/dalinicus.aiolyric-1.1.4.tar.gz` & `tmp/dalinicus.aiolyric-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalinicus.aiolyric-1.1.4.tar", last modified: Sat Jul 29 20:30:19 2023, max compression
+gzip compressed data, was "dalinicus.aiolyric-1.1.5.tar", last modified: Sat Jul 29 20:32:59 2023, max compression
```

## Comparing `dalinicus.aiolyric-1.1.4.tar` & `dalinicus.aiolyric-1.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 20:30:19.282512 dalinicus.aiolyric-1.1.4/
--rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      819 2023-07-29 20:30:19.282512 dalinicus.aiolyric-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 20:30:19.267494 dalinicus.aiolyric-1.1.4/aiolyric/
--rw-rw-rw-   0        0        0     6186 2023-07-29 20:29:35.000000 dalinicus.aiolyric-1.1.4/aiolyric/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:30:19.267994 dalinicus.aiolyric-1.1.4/aiolyric/client/
--rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/client/__init__.py
--rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/const.py
--rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:30:19.272504 dalinicus.aiolyric-1.1.4/aiolyric/objects/
--rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/objects/__init__.py
--rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/objects/base.py
--rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/objects/device.py
--rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.4/aiolyric/objects/location.py
--rw-rw-rw-   0        0        0     2268 2023-07-29 20:30:10.000000 dalinicus.aiolyric-1.1.4/aiolyric/objects/priority.py
-drwxrwxrwx   0        0        0        0 2023-07-29 20:30:19.281514 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/
--rw-rw-rw-   0        0        0      819 2023-07-29 20:30:19.000000 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-29 20:30:19.000000 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 20:30:19.000000 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 20:30:19.000000 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 20:30:19.000000 dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 20:30:19.283012 dalinicus.aiolyric-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-29 20:29:51.000000 dalinicus.aiolyric-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.020167 dalinicus.aiolyric-1.1.5/
+-rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:32:59.019666 dalinicus.aiolyric-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.005597 dalinicus.aiolyric-1.1.5/aiolyric/
+-rw-rw-rw-   0        0        0     6184 2023-07-29 20:32:40.000000 dalinicus.aiolyric-1.1.5/aiolyric/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.006596 dalinicus.aiolyric-1.1.5/aiolyric/client/
+-rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/client/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/const.py
+-rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.010159 dalinicus.aiolyric-1.1.5/aiolyric/objects/
+-rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/base.py
+-rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/device.py
+-rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/location.py
+-rw-rw-rw-   0        0        0     2267 2023-07-29 20:32:15.000000 dalinicus.aiolyric-1.1.5/aiolyric/objects/priority.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:32:59.018158 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 20:32:58.000000 dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 20:32:59.020167 dalinicus.aiolyric-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-29 20:32:53.000000 dalinicus.aiolyric-1.1.5/setup.py
```

### Comparing `dalinicus.aiolyric-1.1.4/LICENSE` & `dalinicus.aiolyric-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.4/PKG-INFO` & `dalinicus.aiolyric-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.4
+Version: 1.1.5
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.4/aiolyric/__init__.py` & `dalinicus.aiolyric-1.1.5/aiolyric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from aiohttp import ClientResponse
 
 from .const import BASE_URL
 from .objects.base import LyricBase
 from .objects.device import LyricDevice
 from .objects.location import LyricLocation
-from .objects.priority import LyricPriority, LyricRooms
+from .objects.priority import LyricPriority, LyricRoom
 
 
 class Lyric(LyricBase):
     """Handles authentication refresh tokens."""
 
     def __init__(
         self,
@@ -45,15 +45,15 @@
         return self._locations
 
     @property
     def locations_dict(self) -> dict:
         return self._locations_dict
 
     @property
-    def rooms_dict(self) -> dict[str, LyricRooms]:
+    def rooms_dict(self) -> dict[str, LyricRoom]:
         return self._rooms_dict
 
     async def get_devices(
         self,
         location_id: int,
     ) -> None:
         """Get Devices."""
```

### Comparing `dalinicus.aiolyric-1.1.4/aiolyric/client/__init__.py` & `dalinicus.aiolyric-1.1.5/aiolyric/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.4/aiolyric/objects/device.py` & `dalinicus.aiolyric-1.1.5/aiolyric/objects/device.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.4/aiolyric/objects/location.py` & `dalinicus.aiolyric-1.1.5/aiolyric/objects/location.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.4/aiolyric/objects/priority.py` & `dalinicus.aiolyric-1.1.5/aiolyric/objects/priority.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     @property
     def selectedRooms(self):
         return self.attributes.get("selectedRooms", [])
 
     @property
     def rooms(self):
-        return [LyricRooms(x) for x in self.attributes.get("rooms", [])]
+        return [LyricRoom(x) for x in self.attributes.get("rooms", [])]
 
 
 class LyricPriority(LyricBase):
 
     @property
     def deviceId(self):
         return self.attributes.get("deviceId", "")
```

### Comparing `dalinicus.aiolyric-1.1.4/dalinicus.aiolyric.egg-info/PKG-INFO` & `dalinicus.aiolyric-1.1.5/dalinicus.aiolyric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.4
+Version: 1.1.5
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.4/setup.py` & `dalinicus.aiolyric-1.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import io
 
 from setuptools import find_packages, setup
 
-version = "1.1.4"
+version = "1.1.5"
 
 setup(
     name="dalinicus.aiolyric",
     version=version,
     description="AIO package for the Honeywell Lyric Platform.",
     long_description=io.open("README.md", encoding="UTF-8").read(),
     keywords="honeywell lyric thermostat",
```

