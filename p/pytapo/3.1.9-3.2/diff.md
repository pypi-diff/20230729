# Comparing `tmp/pytapo-3.1.9.tar.gz` & `tmp/pytapo-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytapo-3.1.9.tar", last modified: Mon Apr  3 12:42:38 2023, max compression
+gzip compressed data, was "pytapo-3.2.tar", last modified: Fri Jul 28 23:48:30 2023, max compression
```

## Comparing `pytapo-3.1.9.tar` & `pytapo-3.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jurajnyiri   (501) staff       (20)        0 2023-04-03 12:42:38.733887 pytapo-3.1.9/
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     1069 2020-10-01 16:27:56.000000 pytapo-3.1.9/LICENSE
--rw-r--r--   0 jurajnyiri   (501) staff       (20)       16 2020-10-05 17:18:33.000000 pytapo-3.1.9/MANIFEST.in
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     5513 2023-04-03 12:42:38.733345 pytapo-3.1.9/PKG-INFO
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     5076 2023-02-19 14:19:57.000000 pytapo-3.1.9/README.md
-drwxr-xr-x   0 jurajnyiri   (501) staff       (20)        0 2023-04-03 12:42:38.719347 pytapo-3.1.9/pytapo/
--rw-r--r--   0 jurajnyiri   (501) staff       (20)    39055 2023-04-03 12:41:17.000000 pytapo-3.1.9/pytapo/__init__.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)      523 2023-04-03 10:49:34.000000 pytapo-3.1.9/pytapo/const.py
-drwxr-xr-x   0 jurajnyiri   (501) staff       (20)        0 2023-04-03 12:42:38.732028 pytapo-3.1.9/pytapo/media_stream/
--rw-r--r--   0 jurajnyiri   (501) staff       (20)        0 2022-11-24 13:18:53.000000 pytapo-3.1.9/pytapo/media_stream/__init__.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     1977 2023-02-18 20:12:52.000000 pytapo-3.1.9/pytapo/media_stream/_utils.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     4295 2023-02-19 16:33:44.000000 pytapo-3.1.9/pytapo/media_stream/convert.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     2626 2023-02-17 23:16:54.000000 pytapo-3.1.9/pytapo/media_stream/crypto.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     8385 2023-02-24 11:56:12.000000 pytapo-3.1.9/pytapo/media_stream/downloader.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)      607 2022-11-24 13:18:53.000000 pytapo-3.1.9/pytapo/media_stream/error.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     3241 2023-02-18 20:28:53.000000 pytapo-3.1.9/pytapo/media_stream/pes.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)      659 2023-02-18 20:21:47.000000 pytapo-3.1.9/pytapo/media_stream/response.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)    19229 2023-02-18 22:06:34.000000 pytapo-3.1.9/pytapo/media_stream/session.py
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     5222 2023-02-18 20:30:07.000000 pytapo-3.1.9/pytapo/media_stream/tsReader.py
-drwxr-xr-x   0 jurajnyiri   (501) staff       (20)        0 2023-04-03 12:42:38.722253 pytapo-3.1.9/pytapo.egg-info/
--rw-r--r--   0 jurajnyiri   (501) staff       (20)     5513 2023-04-03 12:42:38.000000 pytapo-3.1.9/pytapo.egg-info/PKG-INFO
--rw-r--r--   0 jurajnyiri   (501) staff       (20)      530 2023-04-03 12:42:38.000000 pytapo-3.1.9/pytapo.egg-info/SOURCES.txt
--rw-r--r--   0 jurajnyiri   (501) staff       (20)        1 2023-04-03 12:42:38.000000 pytapo-3.1.9/pytapo.egg-info/dependency_links.txt
--rw-r--r--   0 jurajnyiri   (501) staff       (20)       34 2023-04-03 12:42:38.000000 pytapo-3.1.9/pytapo.egg-info/requires.txt
--rw-r--r--   0 jurajnyiri   (501) staff       (20)        7 2023-04-03 12:42:38.000000 pytapo-3.1.9/pytapo.egg-info/top_level.txt
--rw-r--r--   0 jurajnyiri   (501) staff       (20)       38 2023-04-03 12:42:38.734037 pytapo-3.1.9/setup.cfg
--rw-r--r--   0 jurajnyiri   (501) staff       (20)      778 2023-04-03 12:40:50.000000 pytapo-3.1.9/setup.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-07-28 23:48:30.456170 pytapo-3.2/
+-rw-r--r--   0 jnyiri     (501) staff       (20)     1069 2023-04-19 11:02:05.000000 pytapo-3.2/LICENSE
+-rw-r--r--   0 jnyiri     (501) staff       (20)       16 2023-04-19 11:02:05.000000 pytapo-3.2/MANIFEST.in
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5531 2023-07-28 23:48:30.456010 pytapo-3.2/PKG-INFO
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5076 2023-04-19 11:02:05.000000 pytapo-3.2/README.md
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-07-28 23:48:30.451531 pytapo-3.2/pytapo/
+-rw-r--r--   0 jnyiri     (501) staff       (20)      687 2023-07-28 23:39:41.000000 pytapo-3.2/pytapo/TlsAdapter.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)    41727 2023-07-28 23:45:22.000000 pytapo-3.2/pytapo/__init__.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      571 2023-07-06 15:09:24.000000 pytapo-3.2/pytapo/const.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-07-28 23:48:30.455217 pytapo-3.2/pytapo/media_stream/
+-rw-r--r--   0 jnyiri     (501) staff       (20)        0 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/__init__.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     1977 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/_utils.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     4346 2023-05-04 14:22:22.000000 pytapo-3.2/pytapo/media_stream/convert.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     2626 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/crypto.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     8467 2023-07-06 15:42:38.000000 pytapo-3.2/pytapo/media_stream/downloader.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      607 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/error.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     3241 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/pes.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)      659 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/response.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)    19229 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/session.py
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5222 2023-04-19 11:02:05.000000 pytapo-3.2/pytapo/media_stream/tsReader.py
+drwxr-xr-x   0 jnyiri     (501) staff       (20)        0 2023-07-28 23:48:30.452253 pytapo-3.2/pytapo.egg-info/
+-rw-r--r--   0 jnyiri     (501) staff       (20)     5531 2023-07-28 23:48:30.000000 pytapo-3.2/pytapo.egg-info/PKG-INFO
+-rw-r--r--   0 jnyiri     (501) staff       (20)      551 2023-07-28 23:48:30.000000 pytapo-3.2/pytapo.egg-info/SOURCES.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)        1 2023-07-28 23:48:30.000000 pytapo-3.2/pytapo.egg-info/dependency_links.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)       34 2023-07-28 23:48:30.000000 pytapo-3.2/pytapo.egg-info/requires.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)        7 2023-07-28 23:48:30.000000 pytapo-3.2/pytapo.egg-info/top_level.txt
+-rw-r--r--   0 jnyiri     (501) staff       (20)       38 2023-07-28 23:48:30.456386 pytapo-3.2/setup.cfg
+-rw-r--r--   0 jnyiri     (501) staff       (20)      776 2023-07-28 23:44:29.000000 pytapo-3.2/setup.py
```

### Comparing `pytapo-3.1.9/LICENSE` & `pytapo-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/PKG-INFO` & `pytapo-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pytapo
-Version: 3.1.9
+Version: 3.2
 Summary: Python library for communication with Tapo Cameras
 Home-page: https://github.com/JurajNyiri/pytapo
 Author: Juraj Nyíri
 Author-email: juraj.nyiri@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTapo
@@ -127,7 +128,9 @@
 Author is in no way affiliated with Tp-Link or Tapo.
 
 All the api requests used within the library are available and published on the internet (examples linked above) and this module is purely just a wrapper around those https requests.
 
 Author does not guarantee functionality of this library and is not responsible for any damage.
 
 All product names, trademarks and registered trademarks in this repository, are property of their respective owners.
+
+
```

### Comparing `pytapo-3.1.9/README.md` & `pytapo-3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/__init__.py` & `pytapo-3.2/pytapo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 #
 # Author: See contributors at https://github.com/JurajNyiri/pytapo/graphs/contributors
 #
 
 import hashlib
 import json
-
 import requests
-import urllib3
+from datetime import datetime
 from warnings import warn
 
 from .const import ERROR_CODES, MAX_LOGIN_RETRIES
 from .media_stream.session import HttpMediaSession
-from datetime import datetime
-
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+from .TlsAdapter import TlsAdapter
 
 
 class Tapo:
     def __init__(
         self, host, user, password, cloudPassword="", superSecretKey="", childID=None
     ):
         self.host = host
         self.user = user
         self.password = password
         self.cloudPassword = cloudPassword
         self.superSecretKey = superSecretKey
         self.stok = False
         self.userID = False
         self.childID = childID
+        self.timeCorrection = False
         self.headers = {
             "Host": self.host,
             "Referer": "https://{host}".format(host=self.host),
             "Accept": "application/json",
             "Accept-Encoding": "gzip, deflate",
             "User-Agent": "Tapo CameraClient Android",
             "Connection": "close",
             "requestByApp": "true",
             "Content-Type": "application/json; charset=UTF-8",
         }
         self.hashedPassword = hashlib.md5(password.encode("utf8")).hexdigest().upper()
         self.hashedCloudPassword = (
             hashlib.md5(cloudPassword.encode("utf8")).hexdigest().upper()
         )
+        self.session = requests.session()
+        self.session.mount("https://", TlsAdapter())
 
         self.basicInfo = self.getBasicInfo()
         self.presets = self.isSupportingPresets()
         if not self.presets:
             self.presets = {}
 
     def isSupportingPresets(self):
@@ -72,17 +72,18 @@
             "method": "login",
             "params": {
                 "hashed": True,
                 "password": self.hashedPassword,
                 "username": self.user,
             },
         }
-        res = requests.post(
-            url, data=json.dumps(data), headers=self.headers, verify=False
+        res = self.session.request(
+            "POST", url, data=json.dumps(data), headers=self.headers, verify=False
         )
+
         if res.status_code == 401:
             try:
                 data = res.json()
                 if data["result"]["data"]["code"] == -40411:
                     raise Exception("Invalid authentication data")
             except Exception as e:
                 if str(e) == "Invalid authentication data":
@@ -160,17 +161,23 @@
                             },
                         }
                     ]
                 },
             }
         else:
             fullRequest = requestData
-        res = requests.post(
-            url, data=json.dumps(fullRequest), headers=self.headers, verify=False
+
+        res = self.session.request(
+            "POST",
+            url,
+            data=json.dumps(fullRequest),
+            headers=self.headers,
+            verify=False,
         )
+
         if not self.responseIsOK(res):
             data = json.loads(res.text)
             #  -40401: Invalid Stok
             if (
                 data
                 and "error_code" in data
                 and data["error_code"] == -40401
@@ -212,20 +219,78 @@
             {
                 "method": "getChildDeviceList",
                 "params": {"childControl": {"start_index": 0}},
             }
         )
         return childDevices["result"]["child_device_list"]
 
+    def getTimeCorrection(self):
+        if self.timeCorrection is False:
+            currentTime = self.getTime()
+
+            timeReturned = (
+                "system" in currentTime
+                and "clock_status" in currentTime["system"]
+                and "seconds_from_1970" in currentTime["system"]["clock_status"]
+            )
+            if timeReturned:
+                nowTS = int(datetime.timestamp(datetime.now()))
+                self.timeCorrection = (
+                    nowTS - currentTime["system"]["clock_status"]["seconds_from_1970"]
+                )
+        return self.timeCorrection
+
+    def getEvents(self, startTime=False, endTime=False):
+        timeCorrection = self.getTimeCorrection()
+        if timeCorrection is False:
+            raise Exception("Failed to get correct camera time.")
+
+        nowTS = int(datetime.timestamp(datetime.now()))
+        if startTime is False:
+            startTime = nowTS + (-1 * timeCorrection) - (10 * 60)
+        if endTime is False:
+            endTime = nowTS + (-1 * timeCorrection) + 60
+
+        responseData = self.executeFunction(
+            "searchDetectionList",
+            {
+                "playback": {
+                    "search_detection_list": {
+                        "start_index": 0,
+                        "channel": 0,
+                        "start_time": startTime,
+                        "end_time": endTime,
+                        "end_index": 999,
+                    }
+                }
+            },
+        )
+        events = []
+
+        detectionsReturned = (
+            "playback" in responseData
+            and "search_detection_list" in responseData["playback"]
+        )
+
+        if detectionsReturned:
+            for event in responseData["playback"]["search_detection_list"]:
+                event["start_time"] = event["start_time"] + timeCorrection
+                event["end_time"] = event["end_time"] + timeCorrection
+                event["startRelative"] = nowTS - event["start_time"]
+                event["endRelative"] = nowTS - event["end_time"]
+                events.append(event)
+        return events
+
     # returns empty response for child devices
     def getOsd(self):
         # no, asking for all does not work...
         if self.childID:
             return self.executeFunction(
-                "getOsd", {"OSD": {"name": ["logo", "date", "label"]}},
+                "getOsd",
+                {"OSD": {"name": ["logo", "date", "label"]}},
             )
         else:
             return self.executeFunction(
                 "getOsd",
                 {"OSD": {"name": ["date", "week", "font"], "table": ["label_info"]}},
             )
 
@@ -299,21 +364,23 @@
     def getModuleSpec(self):
         return self.performRequest(
             {"method": "get", "function": {"name": ["module_spec"]}}
         )
 
     def getPrivacyMode(self):
         data = self.executeFunction(
-            "getLensMaskConfig", {"lens_mask": {"name": ["lens_mask_info"]}},
+            "getLensMaskConfig",
+            {"lens_mask": {"name": ["lens_mask_info"]}},
         )
         return data["lens_mask"]["lens_mask_info"]
 
     def getMediaEncrypt(self):
         data = self.executeFunction(
-            "getMediaEncrypt", {"cet": {"name": ["media_encrypt"]}},
+            "getMediaEncrypt",
+            {"cet": {"name": ["media_encrypt"]}},
         )
         return data["cet"]["media_encrypt"]
 
     def getAlarm(self):
         # ensure reverse compatibility, simulate the same response for children devices
         if self.childID:
             data = self.getAlarmConfig()
@@ -326,15 +393,16 @@
                 "alarm_type": "0",
                 "light_type": "0",
                 "enabled": data[0]["result"]["enabled"],
                 "alarm_mode": data[0]["result"]["alarm_mode"],
             }
         else:
             return self.executeFunction(
-                "getLastAlarmInfo", {"msg_alarm": {"name": ["chn1_msg_alarm_info"]}},
+                "getLastAlarmInfo",
+                {"msg_alarm": {"name": ["chn1_msg_alarm_info"]}},
             )["msg_alarm"]["chn1_msg_alarm_info"]
 
     def getAlarmConfig(self):
         return self.executeFunction(
             "multipleRequest",
             {
                 "requests": [
@@ -345,19 +413,23 @@
                     {"method": "getSirenStatus", "params": {"msg_alarm": {}}},
                 ]
             },
         )
 
     def getRotationStatus(self):
         return self.executeFunction(
-            "getRotationStatus", {"image": {"name": ["switch"]}},
+            "getRotationStatus",
+            {"image": {"name": ["switch"]}},
         )
 
     def getLED(self):
-        return self.executeFunction("getLedStatus", {"led": {"name": ["config"]}},)[
+        return self.executeFunction(
+            "getLedStatus",
+            {"led": {"name": ["config"]}},
+        )[
             "led"
         ]["config"]
 
     def getAutoTrackTarget(self):
         return self.executeFunction(
             "getTargetTrackConfig", {"target_track": {"name": ["target_track_info"]}}
         )["target_track"]["target_track_info"]
@@ -554,15 +626,16 @@
             elif sensitivity == "low":
                 return "20"
             else:
                 raise Exception("Invalid sensitivity, can be low, normal or high")
 
     def getMotionDetection(self):
         return self.executeFunction(
-            "getDetectionConfig", {"motion_detection": {"name": ["motion_det"]}},
+            "getDetectionConfig",
+            {"motion_detection": {"name": ["motion_det"]}},
         )["motion_detection"]["motion_det"]
 
     def setMotionDetection(self, enabled, sensitivity=False):
         data = {
             "motion_detection": {"motion_det": {"enabled": "on" if enabled else "off"}},
         }
         if sensitivity:
@@ -578,64 +651,69 @@
             data["motion_detection"]["motion_det"]["digital_sensitivity"] = currentData[
                 "digital_sensitivity"
             ]
         return self.executeFunction("setDetectionConfig", data)
 
     def getPersonDetection(self):
         return self.executeFunction(
-            "getPersonDetectionConfig", {"people_detection": {"name": ["detection"]}},
+            "getPersonDetectionConfig",
+            {"people_detection": {"name": ["detection"]}},
         )["people_detection"]["detection"]
 
     def setPersonDetection(self, enabled, sensitivity=False):
         data = {
             "people_detection": {"detection": {"enabled": "on" if enabled else "off"}}
         }
         if sensitivity:
             data["people_detection"]["detection"][
                 "sensitivity"
             ] = self.__getSensitivityNumber(sensitivity)
         return self.executeFunction("setPersonDetectionConfig", data)
 
     def getVehicleDetection(self):
         return self.executeFunction(
-            "getVehicleDetectionConfig", {"vehicle_detection": {"name": ["detection"]}},
+            "getVehicleDetectionConfig",
+            {"vehicle_detection": {"name": ["detection"]}},
         )["vehicle_detection"]["detection"]
 
     def setVehicleDetection(self, enabled, sensitivity=False):
         data = {
             "vehicle_detection": {"detection": {"enabled": "on" if enabled else "off"}}
         }
         if sensitivity:
             data["vehicle_detection"]["detection"][
                 "sensitivity"
             ] = self.__getSensitivityNumber(sensitivity)
         return self.executeFunction("setVehicleDetectionConfig", data)
 
     def getPetDetection(self):
         return self.executeFunction(
-            "getPetDetectionConfig", {"pet_detection": {"name": ["detection"]}},
+            "getPetDetectionConfig",
+            {"pet_detection": {"name": ["detection"]}},
         )["pet_detection"]["detection"]
 
     def setPetDetection(self, enabled, sensitivity=False):
         data = {"pet_detection": {"detection": {"enabled": "on" if enabled else "off"}}}
         if sensitivity:
             data["pet_detection"]["detection"][
                 "sensitivity"
             ] = self.__getSensitivityNumber(sensitivity)
 
         return self.executeFunction("setPetDetectionConfig", data)
 
     def getBarkDetection(self):
         return self.executeFunction(
-            "getBarkDetectionConfig", {"bark_detection": {"name": ["detection"]}},
+            "getBarkDetectionConfig",
+            {"bark_detection": {"name": ["detection"]}},
         )["bark_detection"]["detection"]
 
     def getMeowDetection(self):
         return self.executeFunction(
-            "getMeowDetectionConfig", {"meow_detection": {"name": ["detection"]}},
+            "getMeowDetectionConfig",
+            {"meow_detection": {"name": ["detection"]}},
         )["meow_detection"]["detection"]
 
     def setBarkDetection(self, enabled, sensitivity=False):
         data = {
             "bark_detection": {"detection": {"enabled": "on" if enabled else "off"}}
         }
         if sensitivity:
@@ -654,15 +732,16 @@
                 "sensitivity"
             ] = self.__getSensitivityNumber(sensitivity)
 
         return self.executeFunction("setMeowDetectionConfig", data)
 
     def getGlassBreakDetection(self):
         return self.executeFunction(
-            "getGlassDetectionConfig", {"glass_detection": {"name": ["detection"]}},
+            "getGlassDetectionConfig",
+            {"glass_detection": {"name": ["detection"]}},
         )["glass_detection"]["detection"]
 
     def setGlassBreakDetection(self, enabled, sensitivity=False):
         data = {
             "glass_detection": {"detection": {"enabled": "on" if enabled else "off"}}
         }
         if sensitivity:
@@ -670,15 +749,16 @@
                 "sensitivity"
             ] = self.__getSensitivityNumber(sensitivity)
 
         return self.executeFunction("setGlassDetectionConfig", data)
 
     def getTamperDetection(self):
         return self.executeFunction(
-            "getTamperDetectionConfig", {"tamper_detection": {"name": "tamper_det"}},
+            "getTamperDetectionConfig",
+            {"tamper_detection": {"name": "tamper_det"}},
         )["tamper_detection"]["tamper_det"]
 
     def setTamperDetection(self, enabled, sensitivity=False):
         data = {
             "tamper_detection": {"tamper_det": {"enabled": "on" if enabled else "off"}}
         }
         if sensitivity:
@@ -688,15 +768,16 @@
                 sensitivity = "medium"
             data["tamper_detection"]["tamper_det"]["sensitivity"] = sensitivity
 
         return self.executeFunction("setTamperDetectionConfig", data)
 
     def getBabyCryDetection(self):
         return self.executeFunction(
-            "getBCDConfig", {"sound_detection": {"name": ["bcd"]}},
+            "getBCDConfig",
+            {"sound_detection": {"name": ["bcd"]}},
         )["sound_detection"]["bcd"]
 
     def getCruise(self):
         data = self.executeFunction(
             "getPatrolAction", {"patrol": {"get_patrol_action": {}}}
         )
         return data
@@ -723,18 +804,22 @@
         )
 
     def setCruise(self, enabled, coord=False):
         if coord not in ["x", "y"] and coord is not False:
             raise Exception("Invalid coord parameter. Can be 'x' or 'y'.")
         if enabled and coord is not False:
             return self.executeFunction(
-                "cruiseMove", {"motor": {"cruise": {"coord": coord}}},
+                "cruiseMove",
+                {"motor": {"cruise": {"coord": coord}}},
             )
         else:
-            return self.executeFunction("cruiseStop", {"motor": {"cruise_stop": {}}},)
+            return self.executeFunction(
+                "cruiseStop",
+                {"motor": {"cruise_stop": {}}},
+            )
 
     def reboot(self):
         return self.executeFunction("rebootDevice", {"system": {"reboot": "null"}})
 
     def getPresets(self):
         data = self.executeFunction("getPresetConfig", {"preset": {"name": ["preset"]}})
         self.presets = {
@@ -835,15 +920,16 @@
         if self.childID:
             return self.setRotationStatus("center" if enable else "off")
         else:
             return self.__setImageSwitch("flip_type", "center" if enable else "off")
 
     def setRotationStatus(self, flip_type):
         return self.executeFunction(
-            "setRotationStatus", {"image": {"switch": {"flip_type": flip_type}}},
+            "setRotationStatus",
+            {"image": {"switch": {"flip_type": flip_type}}},
         )
 
     def getForceWhitelampState(self) -> bool:
         return self.__getImageSwitch("force_wtl_state") == "on"
 
     def setForceWhitelampState(self, enable: bool):
         return self.__setImageSwitch("force_wtl_state", "on" if enable else "off")
@@ -877,21 +963,27 @@
                 "Light frequency mode must be one of {}".format(allowed_modes)
             )
         return self.__setImageCommon("light_freq_mode", mode)
 
     # does not work for child devices, function discovery needed
     def startManualAlarm(self):
         return self.performRequest(
-            {"method": "do", "msg_alarm": {"manual_msg_alarm": {"action": "start"}},}
+            {
+                "method": "do",
+                "msg_alarm": {"manual_msg_alarm": {"action": "start"}},
+            }
         )
 
     # does not work for child devices, function discovery needed
     def stopManualAlarm(self):
         return self.performRequest(
-            {"method": "do", "msg_alarm": {"manual_msg_alarm": {"action": "stop"}},}
+            {
+                "method": "do",
+                "msg_alarm": {"manual_msg_alarm": {"action": "stop"}},
+            }
         )
 
     @staticmethod
     def getErrorMessage(errorCode):
         if str(errorCode) in ERROR_CODES:
             return str(ERROR_CODES[str(errorCode)])
         else:
```

### Comparing `pytapo-3.1.9/pytapo/const.py` & `pytapo-3.2/pytapo/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,9 +5,10 @@
     "-64324": "Privacy mode is ON, not able to execute",
     "-64302": "Preset ID not found",
     "-64321": "Preset ID was deleted so no longer exists",
     "-40106": "Parameter to get/do does not exist",
     "-40105": "Method does not exist",
     "-40101": "Parameter to set does not exist",
     "-40209": "Invalid login credentials",
+    "-64304": "Maximum Pan/Tilt range reached",
 }
 MAX_LOGIN_RETRIES = 2
```

### Comparing `pytapo-3.1.9/pytapo/media_stream/_utils.py` & `pytapo-3.2/pytapo/media_stream/_utils.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/convert.py` & `pytapo-3.2/pytapo/media_stream/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,20 @@
             file.write(self.writer.getvalue())
             file.close()
             tempAudioFileLocation = fileLocation + ".alaw"
             file = open(tempAudioFileLocation, "wb")
             file.write(self.audioWriter.getvalue())
             file.close()
 
-            cmd = 'ffmpeg -ss 00:00:00 -i "{inputVideoFile}" -f alaw -ar 8000 -i "{inputAudioFile}" -t {videoLength} -y -c:v copy -c:a aac -map 0:v:0 -map 1:a:0 "{outputFile}" >/dev/null 2>&1'.format(
+            cmd = 'ffmpeg -ss 00:00:00 -i "{inputVideoFile}" -f alaw -ar 8000 -i "{inputAudioFile}" -t {videoLength} -y -c:v copy -c:a aac -map 0:v:0 -map 1:a:0 "{outputFile}" >{devnull} 2>&1'.format(
                 inputVideoFile=tempVideoFileLocation,
                 inputAudioFile=tempAudioFileLocation,
                 outputFile=fileLocation,
                 videoLength=str(datetime.timedelta(seconds=fileLength)),
+                devnull=os.devnull
             )
             os.system(cmd)
 
             os.remove(tempVideoFileLocation)
             os.remove(tempAudioFileLocation)
         else:
             raise Exception("Method not supported")
@@ -54,15 +55,15 @@
         else:
             return self.addedChunks / 2
 
     # calculates real stream length, hard on processing since it has to go through all the frames
     def calculateLength(self):
         detectedLength = False
         try:
-            with tempfile.NamedTemporaryFile() as tmp:
+            with tempfile.NamedTemporaryFile(delete=False) as tmp:
                 tmp.write(self.writer.getvalue())
                 result = subprocess.run(
                     [
                         "ffprobe",
                         "-v",
                         "fatal",
                         "-show_entries",
@@ -73,15 +74,15 @@
                     ],
                     stdout=subprocess.PIPE,
                     stderr=subprocess.STDOUT,
                 )
                 detectedLength = float(result.stdout)
                 self.known_lengths[self.addedChunks] = detectedLength
                 self.lengthLastCalculatedAtChunk = self.addedChunks
-                tmp.close()
+            os.unlink(tmp.name)
         except Exception as e:
             print("")
             print(e)
             print("Warning: Could not calculate length from stream.")
             pass
         return detectedLength
```

### Comparing `pytapo-3.1.9/pytapo/media_stream/crypto.py` & `pytapo-3.2/pytapo/media_stream/crypto.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/downloader.py` & `pytapo-3.2/pytapo/media_stream/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 
 import json
 import os
 import hashlib
 
 
 class Downloader:
-    scriptStartTime = int(
-        datetime.now().timestamp()
-    )  # keeps track of when was class first imported in GMT
-
     FRESH_RECORDING_TIME_SECONDS = 60
 
     def __init__(
         self,
         tapo: Tapo,
         startTime: int,
         endTime: int,
+        timeCorrection: int,
         outputDirectory="./",
         padding=None,
         overwriteFiles=None,
         window_size=None,  # affects download speed, with higher values camera sometimes stops sending data
         fileName=None,
     ):
         self.tapo = tapo
         self.startTime = startTime
         self.endTime = endTime
         self.padding = padding
         self.fileName = fileName
+        self.timeCorrection = timeCorrection
         if padding is None:
             self.padding = 5
         else:
             self.padding = int(padding)
 
         self.outputDirectory = outputDirectory
         self.overwriteFiles = overwriteFiles
@@ -47,23 +45,23 @@
             with open(fileName, "rb") as f:
                 file_hash = hashlib.md5()
                 while chunk := f.read(8192):
                     file_hash.update(chunk)
             return file_hash.hexdigest()
         return False
 
-    async def downloadFile(self, logger=None):
-        if logger is not None:
-            logger.debug("Starting download")
+    async def downloadFile(self, callbackFunc=None):
+        if callbackFunc is not None:
+            callbackFunc("Starting download")
         async for status in self.download():
-            if logger is not None:
-                logger.debug(status)
+            if callbackFunc is not None:
+                callbackFunc(status)
             pass
-        if logger is not None:
-            logger.debug("Finished download")
+        if callbackFunc is not None:
+            callbackFunc("Finished download")
 
         md5Hash = self.md5(status["fileName"])
 
         status["md5"] = "" if md5Hash is False else md5Hash
 
         return status
 
@@ -80,15 +78,20 @@
             segmentLength = self.endTime - self.startTime
             if self.fileName is None:
                 fileName = (
                     self.outputDirectory + str(dateStart) + "-" + dateEnd + ".mp4"
                 )
             else:
                 fileName = self.outputDirectory + self.fileName
-            if self.scriptStartTime - self.FRESH_RECORDING_TIME_SECONDS < self.endTime:
+            if (
+                datetime.now().timestamp()
+                - self.FRESH_RECORDING_TIME_SECONDS
+                - self.timeCorrection
+                < self.endTime
+            ):
                 currentAction = "Recording in progress"
                 yield {
                     "currentAction": currentAction,
                     "fileName": fileName,
                     "progress": 0,
                     "total": 0,
                 }
```

### Comparing `pytapo-3.1.9/pytapo/media_stream/error.py` & `pytapo-3.2/pytapo/media_stream/error.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/pes.py` & `pytapo-3.2/pytapo/media_stream/pes.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/response.py` & `pytapo-3.2/pytapo/media_stream/response.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/session.py` & `pytapo-3.2/pytapo/media_stream/session.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo/media_stream/tsReader.py` & `pytapo-3.2/pytapo/media_stream/tsReader.py`

 * *Files identical despite different names*

### Comparing `pytapo-3.1.9/pytapo.egg-info/PKG-INFO` & `pytapo-3.2/pytapo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pytapo
-Version: 3.1.9
+Version: 3.2
 Summary: Python library for communication with Tapo Cameras
 Home-page: https://github.com/JurajNyiri/pytapo
 Author: Juraj Nyíri
 Author-email: juraj.nyiri@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyTapo
@@ -127,7 +128,9 @@
 Author is in no way affiliated with Tp-Link or Tapo.
 
 All the api requests used within the library are available and published on the internet (examples linked above) and this module is purely just a wrapper around those https requests.
 
 Author does not guarantee functionality of this library and is not responsible for any damage.
 
 All product names, trademarks and registered trademarks in this repository, are property of their respective owners.
+
+
```

### Comparing `pytapo-3.1.9/pytapo.egg-info/SOURCES.txt` & `pytapo-3.2/pytapo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+pytapo/TlsAdapter.py
 pytapo/__init__.py
 pytapo/const.py
 pytapo.egg-info/PKG-INFO
 pytapo.egg-info/SOURCES.txt
 pytapo.egg-info/dependency_links.txt
 pytapo.egg-info/requires.txt
 pytapo.egg-info/top_level.txt
```

### Comparing `pytapo-3.1.9/setup.py` & `pytapo-3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytapo",
-    version="3.1.9",
+    version="3.2",
     author="Juraj Nyíri",
     author_email="juraj.nyiri@gmail.com",
     description="Python library for communication with Tapo Cameras",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JurajNyiri/pytapo",
```

