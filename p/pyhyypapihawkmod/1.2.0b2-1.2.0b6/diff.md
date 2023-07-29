# Comparing `tmp/pyhyypapihawkmod-1.2.0b2.tar.gz` & `tmp/pyhyypapihawkmod-1.2.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.2.0b2.tar", last modified: Fri Jul 28 17:50:47 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.2.0b6.tar", last modified: Fri Jul 28 19:54:11 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.2.0b2.tar` & `pyhyypapihawkmod-1.2.0b6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.713806 pyhyypapihawkmod-1.2.0b2/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-28 17:50:47.712798 pyhyypapihawkmod-1.2.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     2415 2023-07-28 17:49:31.000000 pyhyypapihawkmod-1.2.0b2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.697681 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    11363 2023-07-28 17:47:18.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29480 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4026 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-07-28 17:10:49.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-28 17:50:47.711310 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 17:50:47.000000 pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 17:50:47.714311 pyhyypapihawkmod-1.2.0b2/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-28 17:11:42.000000 pyhyypapihawkmod-1.2.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:54:11.606672 pyhyypapihawkmod-1.2.0b6/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-28 19:54:11.605680 pyhyypapihawkmod-1.2.0b6/PKG-INFO
+-rw-rw-rw-   0        0        0     2415 2023-07-28 18:20:05.000000 pyhyypapihawkmod-1.2.0b6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 19:54:11.591246 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12096 2023-07-28 19:50:15.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29564 2023-07-28 18:42:49.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4026 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:54:11.603154 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-28 19:54:11.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-28 19:54:11.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 19:54:11.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-28 19:54:11.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 19:54:11.000000 pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:54:11.606672 pyhyypapihawkmod-1.2.0b6/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-28 19:42:50.000000 pyhyypapihawkmod-1.2.0b6/setup.py
```

### Comparing `pyhyypapihawkmod-1.2.0b2/LICENSE.md` & `pyhyypapihawkmod-1.2.0b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/PKG-INFO` & `pyhyypapihawkmod-1.2.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b2
+Version: 1.2.0b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b2/README.md` & `pyhyypapihawkmod-1.2.0b6/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/alarm_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 from datetime import datetime
 import time
 from .constants import EventNumber, STD_PARAMS
 import logging
+import threading as thread
 
 _LOGGER = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from .client import HyypClient
 
@@ -43,14 +44,16 @@
             
         
     def get_zone_state_info_for_site(self, site):
         current_siteinfo = None
         for siteinfo in self._zone_state_info:
             if site in siteinfo:
                 current_siteinfo = siteinfo[site]
+                if current_siteinfo is None:
+                    return None
                 if "status" not in current_siteinfo:
                     return None
                 if current_siteinfo["status"] != "SUCCESS":
                     return None
         return current_siteinfo
     
             
@@ -266,33 +269,45 @@
         self._fetch_data()
         formatted_data: dict[Any, Any] = self._format_data()
 
         return formatted_data
 
 
 
-    def debug_notifications(self) -> dict[Any, Any]:
-        """Pull notifications for debug purposes."""
-        # The API returns data from site level.
-
-        """
-        self._fetch_data()
-        site_ids = {site["id"]: site for site in self._sync_info["sites"]}
+    def debug_thread(self):
+        while 1:
         
-        for site in site_ids:
-            self._fetch_notifications(site_id=site)
-            site_ids[site] = self._notifications
-
-
-        return site_ids
-        """
+            _LOGGER.setLevel(logging.DEBUG)
+            time.sleep(1.5)
+            syncinfo = self._client.get_sync_info()
+            time.sleep(1)
+            stateinfo = self._client.get_state_info()
+            time.sleep(2)
+            site = syncinfo["sites"][0]["id"]
+            time.sleep(2)
+            notificationinfo = self._client.site_notifications(site_id=site)
+            time.sleep(2)
+            zoneinfo = self._client.get_zone_state_info(site_id=site)
+            
+            message = {"Syncinfo" : syncinfo,
+                    "Stateinfo" : stateinfo,
+                    "notifications" : notificationinfo,
+                    "zoneinfo" : zoneinfo,
+                        }
+            
+            _LOGGER.debug('------------------------------')
+            _LOGGER.debug('--------Start of debug--------')
+            
+            _LOGGER.debug(message)
+            
+            _LOGGER.debug('--------End of debug--------')
+            _LOGGER.debug('-----------------------------')
+            time.sleep(30)
+    
 
 
-        self._fetch_data()
-        fb = self.get_zone_state_info_for_site(108781)
-        message = {"rand" : "1147",
-                    "raw" : self._zone_state_info,
-                   "forsite" : fb
-                    }
-        
+    def get_debug_info(self) -> dict[Any, Any]:
+        """Pull notifications for debug purposes."""
+        # The API returns data from site level.
+        thread.Thread(target=self.debug_thread).start()
         
-        return fb
+
```

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,17 @@
         return _json_result
 
     def load_alarm_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
 
         return HyypAlarmInfos(self).status()
 
-    def get_debug_notifications(self) -> dict[Any, Any]:
+    def get_debug_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
-        return HyypAlarmInfos(self).debug_notifications()
+        return HyypAlarmInfos(self).get_debug_info()
 
     def site_notifications(
         self, site_id: int, timestamp: int | None = None, json_key: int | None = None
     ) -> Any:
         """Get site notifications from API."""
 
         _params: dict[str, Any] = STD_PARAMS.copy()
@@ -318,14 +318,15 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
+            _LOGGER.warning(f"Error getting zone state info from api: {_json_result['error']}")
             raise HyypApiError(
                 f"Error getting zone state info from api: {_json_result['error']}"
             )
 
         if json_key is None:
             return _json_result
```

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b2
+Version: 1.2.0b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b2/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.2.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b2/setup.py` & `pyhyypapihawkmod-1.2.0b6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.2.0b2",
+    version="1.2.0b6",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

