# Comparing `tmp/pyhyypapihawkmod-1.2.0b7.tar.gz` & `tmp/pyhyypapihawkmod-1.2.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.2.0b7.tar", last modified: Sat Jul 29 10:05:39 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.2.0b8.tar", last modified: Sat Jul 29 11:10:06 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.2.0b7.tar` & `pyhyypapihawkmod-1.2.0b8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:39.096887 pyhyypapihawkmod-1.2.0b7/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-29 10:05:39.084385 pyhyypapihawkmod-1.2.0b7/PKG-INFO
--rw-rw-rw-   0        0        0     2415 2023-07-28 18:20:05.000000 pyhyypapihawkmod-1.2.0b7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:38.996303 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12205 2023-07-29 09:48:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29646 2023-07-29 09:54:15.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4084 2023-07-29 09:36:17.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-29 10:05:39.071354 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-29 10:05:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-29 10:05:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 10:05:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-29 10:05:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 10:05:38.000000 pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 10:05:39.097880 pyhyypapihawkmod-1.2.0b7/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-29 09:31:18.000000 pyhyypapihawkmod-1.2.0b7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.896834 pyhyypapihawkmod-1.2.0b8/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-29 11:10:06.896330 pyhyypapihawkmod-1.2.0b8/PKG-INFO
+-rw-rw-rw-   0        0        0     2459 2023-07-29 11:05:28.000000 pyhyypapihawkmod-1.2.0b8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.882316 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12205 2023-07-29 11:08:57.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29649 2023-07-29 11:05:40.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4084 2023-07-29 09:36:17.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-07-28 18:18:42.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:10:06.893824 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-29 11:10:06.000000 pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:10:06.897337 pyhyypapihawkmod-1.2.0b8/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-29 11:05:05.000000 pyhyypapihawkmod-1.2.0b8/setup.py
```

### Comparing `pyhyypapihawkmod-1.2.0b7/LICENSE.md` & `pyhyypapihawkmod-1.2.0b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/PKG-INFO` & `pyhyypapihawkmod-1.2.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b7
+Version: 1.2.0b8
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b7/README.md` & `pyhyypapihawkmod-1.2.0b8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.2.0b8
+- Added additional debug checks
+
 1.2.0b2
 - Added additional checks for openviolated and tampered information when not received
 
 1.2.0b1
 - Version bump for semantic versioning 
 
 1.1.7b3
```

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,17 +320,17 @@
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             _LOGGER.warning(f"Error getting zone state info from api: {_json_result['error']}")
-            raise HyypApiError(
-                f"Error getting zone state info from api: {_json_result['error']}"
-            )
+            #raise HyypApiError(
+            #    f"Error getting zone state info from api: {_json_result['error']}"
+            #)
 
         if json_key is None:
             return _json_result
 
         return _json_result[json_key]
```

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.2.0b7
+Version: 1.2.0b8
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.2.0b7/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.2.0b8/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.2.0b7/setup.py` & `pyhyypapihawkmod-1.2.0b8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.2.0b7",
+    version="1.2.0b8",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

