# Comparing `tmp/dalinicus.aiolyric-1.1.2.tar.gz` & `tmp/dalinicus.aiolyric-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalinicus.aiolyric-1.1.2.tar", last modified: Sat Jul 29 19:23:17 2023, max compression
+gzip compressed data, was "dalinicus.aiolyric-1.1.3.tar", last modified: Sat Jul 29 20:18:09 2023, max compression
```

## Comparing `dalinicus.aiolyric-1.1.2.tar` & `dalinicus.aiolyric-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 19:23:17.393910 dalinicus.aiolyric-1.1.2/
--rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      819 2023-07-29 19:23:17.393406 dalinicus.aiolyric-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 19:23:17.382382 dalinicus.aiolyric-1.1.2/aiolyric/
--rw-rw-rw-   0        0        0     6178 2023-07-29 19:22:47.000000 dalinicus.aiolyric-1.1.2/aiolyric/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:23:17.382382 dalinicus.aiolyric-1.1.2/aiolyric/client/
--rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/client/__init__.py
--rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/const.py
--rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:23:17.386900 dalinicus.aiolyric-1.1.2/aiolyric/objects/
--rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/objects/__init__.py
--rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/objects/base.py
--rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/objects/device.py
--rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.2/aiolyric/objects/location.py
--rw-rw-rw-   0        0        0     2259 2023-07-29 17:54:44.000000 dalinicus.aiolyric-1.1.2/aiolyric/objects/priority.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:23:17.392402 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/
--rw-rw-rw-   0        0        0      819 2023-07-29 19:23:17.000000 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-29 19:23:17.000000 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 19:23:17.000000 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 19:23:17.000000 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 19:23:17.000000 dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 19:23:17.393910 dalinicus.aiolyric-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-07-29 19:21:58.000000 dalinicus.aiolyric-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:18:09.396237 dalinicus.aiolyric-1.1.3/
+-rw-rw-rw-   0        0        0     1095 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:18:09.395736 dalinicus.aiolyric-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 20:18:09.380729 dalinicus.aiolyric-1.1.3/aiolyric/
+-rw-rw-rw-   0        0        0     6211 2023-07-29 20:16:36.000000 dalinicus.aiolyric-1.1.3/aiolyric/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:18:09.381729 dalinicus.aiolyric-1.1.3/aiolyric/client/
+-rw-rw-rw-   0        0        0     2743 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/client/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/const.py
+-rw-rw-rw-   0        0        0      230 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:18:09.385729 dalinicus.aiolyric-1.1.3/aiolyric/objects/
+-rw-rw-rw-   0        0        0       20 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/objects/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/objects/base.py
+-rw-rw-rw-   0        0        0     8043 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/objects/device.py
+-rw-rw-rw-   0        0        0     5115 2023-07-27 20:43:58.000000 dalinicus.aiolyric-1.1.3/aiolyric/objects/location.py
+-rw-rw-rw-   0        0        0     2269 2023-07-29 20:17:07.000000 dalinicus.aiolyric-1.1.3/aiolyric/objects/priority.py
+drwxrwxrwx   0        0        0        0 2023-07-29 20:18:09.394738 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-07-29 20:18:09.000000 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-29 20:18:09.000000 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 20:18:09.000000 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-29 20:18:09.000000 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 20:18:09.000000 dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 20:18:09.396237 dalinicus.aiolyric-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-29 20:18:00.000000 dalinicus.aiolyric-1.1.3/setup.py
```

### Comparing `dalinicus.aiolyric-1.1.2/LICENSE` & `dalinicus.aiolyric-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.2/PKG-INFO` & `dalinicus.aiolyric-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.2
+Version: 1.1.3
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.2/aiolyric/__init__.py` & `dalinicus.aiolyric-1.1.3/aiolyric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from aiohttp import ClientResponse
 
 from .const import BASE_URL
 from .objects.base import LyricBase
 from .objects.device import LyricDevice
 from .objects.location import LyricLocation
-from .objects.priority import LyricPriority, Rooms
+from .objects.priority import LyricPriority, LyricRooms
 
 
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
-    def rooms_dict(self) -> dict:
+    def rooms_dict(self) -> dict[str, LyricRooms]:
         return self._rooms_dict
 
     async def get_devices(
         self,
         location_id: int,
     ) -> None:
         """Get Devices."""
@@ -89,15 +89,15 @@
         """Get Priority, which contains accessory information."""
         response: ClientResponse = await self._client.get(
             f"{BASE_URL}/devices/thermostats/{device_id}/priority?apikey={self.client_id}&locationId={location_id}"
         )
         json = await response.json()
         self.logger.debug(json)
         
-        priority = LyricPriority(self._client, json)
+        priority = LyricPriority(self._client, attributes=json)
 
         self._rooms_dict[priority.deviceId]: dict = {}
         for room in priority.currentPriority.rooms:
             self._rooms_dict[device_id][room.id] = room
 
     async def update_thermostat(
         self,
```

### Comparing `dalinicus.aiolyric-1.1.2/aiolyric/client/__init__.py` & `dalinicus.aiolyric-1.1.3/aiolyric/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.2/aiolyric/objects/device.py` & `dalinicus.aiolyric-1.1.3/aiolyric/objects/device.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.2/aiolyric/objects/location.py` & `dalinicus.aiolyric-1.1.3/aiolyric/objects/location.py`

 * *Files identical despite different names*

### Comparing `dalinicus.aiolyric-1.1.2/aiolyric/objects/priority.py` & `dalinicus.aiolyric-1.1.3/aiolyric/objects/priority.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return self.attributes.get("status", "")
 
     @property
     def detectMotion(self):
         return self.attributes.get("detectMotion", False)
 
 
-class Rooms(LyricBase):
+class LyricRooms(LyricBase):
 
     @property
     def id(self):
         return self.attributes.get("id", None)
 
     @property
     def roomName(self):
@@ -73,15 +73,15 @@
 
     @property
     def selectedRooms(self):
         return self.attributes.get("selectedRooms", [])
 
     @property
     def rooms(self):
-        return [Rooms(x) for x in self.attributes.get("rooms", [])]
+        return [LyricRooms(x) for x in self.attributes.get("rooms", [])]
 
 
 class LyricPriority(LyricBase):
 
     @property
     def deviceId(self):
         return self.attributes.get("deviceId", "")
```

### Comparing `dalinicus.aiolyric-1.1.2/dalinicus.aiolyric.egg-info/PKG-INFO` & `dalinicus.aiolyric-1.1.3/dalinicus.aiolyric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalinicus.aiolyric
-Version: 1.1.2
+Version: 1.1.3
 Summary: AIO package for the Honeywell Lyric Platform.
 Home-page: https://github.com/timmo001/aiolyric
 Author: Aidan Timson (Timmo)
 Author-email: contact@timmo.xyz
 License: MIT
 Keywords: honeywell lyric thermostat
 License-File: LICENSE
```

### Comparing `dalinicus.aiolyric-1.1.2/setup.py` & `dalinicus.aiolyric-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import io
 
 from setuptools import find_packages, setup
 
-version = "1.1.2"
+version = "1.1.3"
 
 setup(
     name="dalinicus.aiolyric",
     version=version,
     description="AIO package for the Honeywell Lyric Platform.",
     long_description=io.open("README.md", encoding="UTF-8").read(),
     keywords="honeywell lyric thermostat",
```

