# Comparing `tmp/mypy-boto3-iotwireless-1.28.15.tar.gz` & `tmp/mypy-boto3-iotwireless-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotwireless-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
+gzip compressed data, was "mypy-boto3-iotwireless-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:23 2023, max compression
```

## Comparing `mypy-boto3-iotwireless-1.28.15.tar` & `mypy-boto3-iotwireless-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.553299 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72150 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    72034 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-28 20:28:47.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   101165 2023-07-28 20:28:52.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   101072 2023-07-28 20:28:50.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25736 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:02.000000 mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.557299 mypy-boto3-iotwireless-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:28:46.000000 mypy-boto3-iotwireless-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24233 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.549198 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72698 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72582 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-29 09:48:19.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   101300 2023-07-29 09:48:24.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101207 2023-07-29 09:48:22.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:03:23.000000 mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:23.557198 mypy-boto3-iotwireless-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:48:18.000000 mypy-boto3-iotwireless-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-iotwireless-1.28.15/LICENSE` & `mypy-boto3-iotwireless-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15/PKG-INFO` & `mypy-boto3-iotwireless-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.28.15/README.md` & `mypy-boto3-iotwireless-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/__main__.py` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTWireless 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.IoTWireless 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.py` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,18 +95,22 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     LoRaWANDeviceProfileTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANFuotaTaskTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     LoRaWANMulticastSessionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
@@ -125,15 +129,17 @@
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -291,15 +297,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_destination)
         """
 
     def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
+        LoRaWAN: Union[LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -382,30 +388,30 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceTypeDef = ...,
+        LoRaWAN: Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_wireless_device)
         """
 
     def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayTypeDef,
+        LoRaWAN: Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef],
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -1187,15 +1193,18 @@
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_fuota_task)
         """
 
     def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
+        self,
+        *,
+        Id: str,
+        LoRaWAN: Union[LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_multicast_group_session)
         """
@@ -1308,16 +1317,20 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
 
     def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[
+            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
+        ] = ...,
+        WirelessGatewayLogOptions: Sequence[
+            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/client.pyi` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -95,18 +95,22 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     LoRaWANDeviceProfileTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANFuotaTaskTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     LoRaWANMulticastSessionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
@@ -125,15 +129,17 @@
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -275,15 +281,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_destination)
         """
     def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
+        LoRaWAN: Union[LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -361,29 +367,29 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceTypeDef = ...,
+        LoRaWAN: Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#create_wireless_device)
         """
     def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayTypeDef,
+        LoRaWAN: Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef],
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -1089,15 +1095,18 @@
         """
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_fuota_task)
         """
     def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
+        self,
+        *,
+        Id: str,
+        LoRaWAN: Union[LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef]
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#start_multicast_group_session)
         """
@@ -1201,16 +1210,20 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_fuota_task)
         """
     def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[
+            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
+        ] = ...,
+        WirelessGatewayLogOptions: Sequence[
+            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
+        ] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/client/#update_log_levels_by_resource_types)
         """
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.py` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/literals.pyi` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.py` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3597,16 +3597,20 @@
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
+        "WirelessDeviceLogOptions": Sequence[
+            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
+        ],
+        "WirelessGatewayLogOptions": Sequence[
+            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless/type_defs.pyi` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3512,16 +3512,20 @@
     },
 )
 
 UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
+        "WirelessDeviceLogOptions": Sequence[
+            Union[WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef]
+        ],
+        "WirelessGatewayLogOptions": Sequence[
+            Union[WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef]
+        ],
     },
     total=False,
 )
 
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/PKG-INFO` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotwireless
-Version: 1.28.15
-Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotwireless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotwireless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotwireless-1.28.15/mypy_boto3_iotwireless.egg-info/SOURCES.txt` & `mypy-boto3-iotwireless-1.28.15.post1/mypy_boto3_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotwireless-1.28.15/setup.py` & `mypy-boto3-iotwireless-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotwireless",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.IoTWireless 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

