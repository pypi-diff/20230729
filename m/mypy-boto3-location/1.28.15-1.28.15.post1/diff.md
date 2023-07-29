# Comparing `tmp/mypy-boto3-location-1.28.15.tar.gz` & `tmp/mypy-boto3-location-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-location-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
+gzip compressed data, was "mypy-boto3-location-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:33 2023, max compression
```

## Comparing `mypy-boto3-location-1.28.15.tar` & `mypy-boto3-location-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.021416 mypy-boto3-location-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/mypy_boto3_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45468 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65922 2023-07-28 20:30:27.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65809 2023-07-28 20:30:26.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:25.000000 mypy-boto3-location-1.28.15/mypy_boto3_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.013415 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:10.000000 mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.021416 mypy-boto3-location-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:30:24.000000 mypy-boto3-location-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.761251 mypy-boto3-location-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45733 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45658 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-29 09:50:03.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65922 2023-07-29 09:50:05.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65809 2023-07-29 09:50:04.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:33.757251 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:33.000000 mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:33.761251 mypy-boto3-location-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:50:00.000000 mypy-boto3-location-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-location-1.28.15/LICENSE` & `mypy-boto3-location-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/PKG-INFO` & `mypy-boto3-location-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.15
-Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.28.15/README.md` & `mypy-boto3-location-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/__init__.pyi` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/__main__.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LocationService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.LocationService 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/client.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
@@ -56,14 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
@@ -293,15 +295,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_geofence_collection)
         """
 
     def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsTypeDef,
+        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef],
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
@@ -689,15 +691,15 @@
         """
 
     def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryTypeDef,
+        Geometry: Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef],
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -798,15 +800,15 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef] = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
```

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/client.pyi` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
@@ -56,14 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
@@ -276,15 +278,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#create_geofence_collection)
         """
     def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsTypeDef,
+        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef],
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
@@ -635,15 +637,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#list_trackers)
         """
     def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryTypeDef,
+        Geometry: Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef],
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -737,15 +739,15 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: Union[datetime, str] = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef] = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/client/#update_key)
         """
```

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/literals.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/literals.pyi` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/paginator.pyi` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.py` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location/type_defs.pyi` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/PKG-INFO` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-location
-Version: 1.28.15
-Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LocationService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/
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
 [mypy-boto3-location docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_location/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-location-1.28.15/mypy_boto3_location.egg-info/SOURCES.txt` & `mypy-boto3-location-1.28.15.post1/mypy_boto3_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-location-1.28.15/setup.py` & `mypy-boto3-location-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-location",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LocationService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

