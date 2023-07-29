# Comparing `tmp/airtouch5py-0.2.4.tar.gz` & `tmp/airtouch5py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.4.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.5.tar", max compression
```

## Comparing `airtouch5py-0.2.4.tar` & `airtouch5py-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/LICENSE
--rw-r--r--   0        0        0       47 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/README.md
--rw-r--r--   0        0        0     4853 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     8614 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2192 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15561 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-26 21:34:08.044325 airtouch5py-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/README.md
+-rw-r--r--   0        0        0     4853 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     8614 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2208 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15561 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.5/PKG-INFO
```

### Comparing `airtouch5py-0.2.4/LICENSE` & `airtouch5py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.5/airtouch5py/airtouch5_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.5/airtouch5py/airtouch5_simple_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.5/airtouch5py/data_packet_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 class DataPacketFactory:
     _id: int
 
     def __init__(self):
         self._id = 0x01
 
     def zone_control(self, zones: list[ZoneControlZone]) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(ADDRESS, self._id, ZoneControlData(zones))
 
     def zone_status_request(self) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(ADDRESS, self._id, ZoneStatusData([]))
 
     def ac_control(self, ac: list[AcControl]) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(ADDRESS, self._id, AcControlData(ac))
 
     def ac_status_request(self) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(ADDRESS, self._id, AcStatusData([]))
 
     def ac_ability_request(self, ac_number: int | None = None) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(EXTENDED_ADDRESS, self._id, AcAbilityRequestData(ac_number))
 
     def ac_error_information_request(self, ac_number: int) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(
             EXTENDED_ADDRESS, self._id, AcErrorInformationRequestData(ac_number)
         )
 
     def zone_name_request(self, zone_number: int | None = None) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(EXTENDED_ADDRESS, self._id, ZoneNameRequestData(zone_number))
 
     def console_version_request(self) -> DataPacket:
-        self._id = self._id + 1 % 256
+        self._id = (self._id + 1) % 256
         return DataPacket(EXTENDED_ADDRESS, self._id, ConsoleVersionRequestData())
```

### Comparing `airtouch5py-0.2.4/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.5/airtouch5py/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.5/airtouch5py/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packet_reader.py` & `airtouch5py-0.2.5/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.5/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.5/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.5/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.5/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.5/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.4/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.5/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

