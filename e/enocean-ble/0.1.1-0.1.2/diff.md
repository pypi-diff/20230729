# Comparing `tmp/enocean_ble-0.1.1.tar.gz` & `tmp/enocean_ble-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enocean_ble-0.1.1.tar", last modified: Mon Jul 10 21:04:12 2023, max compression
+gzip compressed data, was "enocean_ble-0.1.2.tar", last modified: Sat Jul 29 09:35:07 2023, max compression
```

## Comparing `enocean_ble-0.1.1.tar` & `enocean_ble-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-02 19:25:15.742226 enocean_ble-0.1.1/LICENSE
--rw-r--r--   0        0        0      137 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-02 19:25:15.742226 enocean_ble-0.1.1/enocean_ble/__init__.py
--rw-r--r--   0        0        0     1170 2023-07-10 21:00:55.929469 enocean_ble-0.1.1/enocean_ble/__main__.py
--rw-r--r--   0        0        0     5516 2023-07-10 21:00:30.589570 enocean_ble-0.1.1/enocean_ble/decoder.py
--rw-r--r--   0        0        0     2449 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/enocean_ble/parser.py
--rw-r--r--   0        0        0      652 2023-07-10 21:04:12.104970 enocean_ble-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3477 2023-07-02 19:25:15.758226 enocean_ble-0.1.1/tests/test_decoder.py
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 enocean_ble-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-02 19:25:15.742226 enocean_ble-0.1.2/LICENSE
+-rw-r--r--   0        0        0      137 2023-07-02 19:25:15.758226 enocean_ble-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 19:25:15.742226 enocean_ble-0.1.2/enocean_ble/__init__.py
+-rw-r--r--   0        0        0     1170 2023-07-10 21:00:55.929469 enocean_ble-0.1.2/enocean_ble/__main__.py
+-rw-r--r--   0        0        0     5516 2023-07-10 21:00:30.589570 enocean_ble-0.1.2/enocean_ble/decoder.py
+-rw-r--r--   0        0        0     2697 2023-07-29 09:32:52.676283 enocean_ble-0.1.2/enocean_ble/parser.py
+-rw-r--r--   0        0        0      652 2023-07-29 09:35:07.269292 enocean_ble-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 19:25:15.758226 enocean_ble-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3477 2023-07-02 19:25:15.758226 enocean_ble-0.1.2/tests/test_decoder.py
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 enocean_ble-0.1.2/PKG-INFO
```

### Comparing `enocean_ble-0.1.1/LICENSE` & `enocean_ble-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.1/enocean_ble/__main__.py` & `enocean_ble-0.1.2/enocean_ble/__main__.py`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.1/enocean_ble/decoder.py` & `enocean_ble-0.1.2/enocean_ble/decoder.py`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.1/enocean_ble/parser.py` & `enocean_ble-0.1.2/enocean_ble/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import logging
 from typing import Optional
 
 from bluetooth_data_tools import short_address
 from bluetooth_sensor_state_data import BluetoothData
 from home_assistant_bluetooth import BluetoothServiceInfo
+from sensor_state_data import BinarySensorDeviceClass
 
 from .decoder import PTM215BDecoder, TelegramType
 
 logger = logging.getLogger(__name__)
 
 MANUFACTURER_ID = 0x3DA
 
+class EnoecanDeviceClass(BinarySensorDeviceClass):
+    # On means button pressed
+    PRESSED = "pressed"
+
 
 class EnoceanBluetoothDeviceData(BluetoothData):
     """Data for Enocean BLE Switch"""
 
     def __init__(
         self, security_key: Optional[str] = None, validate_signature: bool = False
     ) -> None:
@@ -45,32 +50,32 @@
         self.set_device_type("Enocean Switch")
         self.set_device_manufacturer(data.manufacturer)
         self.set_device_name(f"Enocean PTM215b {identifier}")
 
         self.update_binary_sensor(
             f"a0_pressed",
             decoder.a0_action and decoder.is_press_action,
-            None,
+            EnoecanDeviceClass.PRESSED,
             "Channel A0",
         )
         self.update_binary_sensor(
             "a1_pressed",
             decoder.a1_action and decoder.is_press_action,
-            None,
+            EnoecanDeviceClass.PRESSED,
             "Channel A1",
         )
         self.update_binary_sensor(
             "b0_pressed",
             decoder.b0_action and decoder.is_press_action,
-            None,
+            EnoecanDeviceClass.PRESSED,
             "Channel B0",
         )
         self.update_binary_sensor(
             "b1_pressed",
             decoder.b1_action and decoder.is_press_action,
-            None,
+            EnoecanDeviceClass.PRESSED,
             "Channel B1",
         )
 
     def commission(self, data: BluetoothServiceInfo) -> str:
         # TODO: Build logic to retrieve security key from device in commission mode
         ...
```

### Comparing `enocean_ble-0.1.1/pyproject.toml` & `enocean_ble-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "enocean-ble"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [
     { name = "Christian Ohde", email = "christian.s1989@gmail.com" },
 ]
 dependencies = [
     "bleak>=0.20.2",
     "typer>=0.9.0",
```

### Comparing `enocean_ble-0.1.1/tests/test_decoder.py` & `enocean_ble-0.1.2/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `enocean_ble-0.1.1/PKG-INFO` & `enocean_ble-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean-ble
-Version: 0.1.1
+Version: 0.1.2
 Author-Email: Christian Ohde <christian.s1989@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: bleak>=0.20.2
 Requires-Dist: typer>=0.9.0
 Requires-Dist: bluetooth-sensor-state-data>=1.6.1
 Requires-Dist: bluetooth-data-tools>=1.2.0
```

