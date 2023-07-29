# Comparing `tmp/mypy-boto3-mediaconnect-1.28.12.tar.gz` & `tmp/mypy-boto3-mediaconnect-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconnect-1.28.12.tar", last modified: Thu Jul 27 05:35:00 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconnect-1.28.15.tar", last modified: Fri Jul 28 20:43:15 2023, max compression
```

## Comparing `mypy-boto3-mediaconnect-1.28.12.tar` & `mypy-boto3-mediaconnect-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.136444 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-27 05:25:56.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-27 05:25:56.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-07-27 05:25:57.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66488 2023-07-27 05:25:57.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:00.140444 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 05:35:00.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:59.000000 mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:00.144444 mypy-boto3-mediaconnect-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:25:54.000000 mypy-boto3-mediaconnect-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.997470 mypy-boto3-mediaconnect-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-07-28 20:43:14.997470 mypy-boto3-mediaconnect-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.997470 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-28 20:31:01.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64946 2023-07-28 20:31:03.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64855 2023-07-28 20:31:02.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:14.997470 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22043 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:14.000000 mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:14.997470 mypy-boto3-mediaconnect-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:31:00.000000 mypy-boto3-mediaconnect-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/LICENSE` & `mypy-boto3-mediaconnect-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,169 +398,164 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
+    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
-    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
-    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
-    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
-    EncryptionOutputTypeDef,
-    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    GatewayNetworkOutputTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
-    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
-    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
-    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
+    DeleteFlowResponseTypeDef,
+    DeleteGatewayResponseTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
+    RemoveFlowOutputResponseTypeDef,
+    RemoveFlowSourceResponseTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
+    UpdateBridgeStateResponseTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
+    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
+    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
-    EntitlementTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    GatewayTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
+    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
-    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/README.md` & `mypy-boto3-mediaconnect-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,169 +366,164 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
+    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
-    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
-    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
-    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
-    EncryptionOutputTypeDef,
-    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    GatewayNetworkOutputTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
-    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
-    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
-    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
+    DeleteFlowResponseTypeDef,
+    DeleteGatewayResponseTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
+    RemoveFlowOutputResponseTypeDef,
+    RemoveFlowSourceResponseTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
+    UpdateBridgeStateResponseTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
+    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
+    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
-    EntitlementTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    GatewayTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
+    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
-    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__init__.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/__main__.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConnect 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaConnect 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/client.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/literals.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,103 +70,103 @@
 class ListBridgesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBridgesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
         """
 
 
 class ListEntitlementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitlementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
         """
 
 
 class ListFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
         """
 
 
 class ListGatewayInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewayInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
         """
 
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
         """
 
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
         """
 
 
 class ListReservationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/paginator.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,97 +67,97 @@
 class ListBridgesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBridgesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListBridges.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listbridgespaginator)
         """
 
 class ListEntitlementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEntitlementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listentitlementspaginator)
         """
 
 class ListFlowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFlowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listflowspaginator)
         """
 
 class ListGatewayInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
     """
 
     def paginate(
-        self, *, FilterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FilterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewayInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGatewayInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayinstancespaginator)
         """
 
 class ListGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewaysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listgatewayspaginator)
         """
 
 class ListOfferingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listofferingspaginator)
         """
 
 class ListReservationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReservationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/paginators/#listreservationspaginator)
         """
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,169 +51,164 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "VpcInterfaceAttachmentTypeDef",
     "AddBridgeNetworkOutputRequestTypeDef",
     "AddBridgeNetworkSourceRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
-    "VpcInterfaceAttachmentOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
-    "DeleteBridgeResponseTypeDef",
     "DeleteFlowRequestRequestTypeDef",
-    "DeleteFlowResponseTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
-    "DeleteGatewayResponseTypeDef",
     "DeregisterGatewayInstanceRequestRequestTypeDef",
-    "DeregisterGatewayInstanceResponseTypeDef",
     "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
     "DescribeGatewayInstanceRequestRequestTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
-    "EncryptionOutputTypeDef",
-    "SourcePriorityOutputTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
-    "GatewayNetworkOutputTypeDef",
-    "ListBridgesRequestListBridgesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
-    "ListFlowsRequestListFlowsPaginateTypeDef",
     "ListFlowsRequestRequestTypeDef",
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
     "ListGatewayInstancesRequestRequestTypeDef",
     "ListedGatewayInstanceTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
     "ListedGatewayTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RemoveBridgeOutputRequestRequestTypeDef",
-    "RemoveBridgeOutputResponseTypeDef",
     "RemoveBridgeSourceRequestRequestTypeDef",
-    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
-    "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
-    "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
-    "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
-    "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBridgeNetworkOutputRequestTypeDef",
     "UpdateBridgeNetworkSourceRequestTypeDef",
     "UpdateEgressGatewayBridgeRequestTypeDef",
     "UpdateIngressGatewayBridgeRequestTypeDef",
     "UpdateBridgeStateRequestRequestTypeDef",
-    "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
-    "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
+    "DeleteFlowResponseTypeDef",
+    "DeleteGatewayResponseTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
+    "RemoveFlowMediaStreamResponseTypeDef",
+    "RemoveFlowOutputResponseTypeDef",
+    "RemoveFlowSourceResponseTypeDef",
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    "RevokeFlowEntitlementResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
+    "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
-    "BridgeFlowSourceTypeDef",
-    "GatewayBridgeSourceTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
+    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
-    "EntitlementTypeDef",
-    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
-    "GatewayTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
     "AddBridgeSourceRequestTypeDef",
+    "BridgeSourceTypeDef",
     "UpdateBridgeSourceRequestRequestTypeDef",
     "AddBridgeOutputsRequestRequestTypeDef",
+    "GrantFlowEntitlementsResponseTypeDef",
+    "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
-    "BridgeSourceTypeDef",
     "AddBridgeOutputsResponseTypeDef",
     "UpdateBridgeOutputResponseTypeDef",
     "DescribeGatewayInstanceResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
-    "GrantFlowEntitlementsResponseTypeDef",
-    "UpdateFlowEntitlementResponseTypeDef",
     "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
-    "CreateGatewayResponseTypeDef",
-    "DescribeGatewayResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "AddBridgeSourcesRequestRequestTypeDef",
     "CreateBridgeRequestRequestTypeDef",
@@ -272,14 +267,25 @@
         "Name": str,
         "NetworkName": str,
         "Port": int,
         "Protocol": ProtocolType,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 AddEgressGatewayBridgeRequestTypeDef = TypedDict(
     "AddEgressGatewayBridgeRequestTypeDef",
     {
         "MaxBitrate": int,
     },
 )
 
@@ -366,22 +372,14 @@
     {
         "FlowArn": str,
         "FlowSourceArn": str,
         "Name": str,
     },
 )
 
-VpcInterfaceAttachmentOutputTypeDef = TypedDict(
-    "VpcInterfaceAttachmentOutputTypeDef",
-    {
-        "VpcInterfaceName": str,
-    },
-    total=False,
-)
-
 BridgeNetworkOutputTypeDef = TypedDict(
     "BridgeNetworkOutputTypeDef",
     {
         "IpAddress": str,
         "Name": str,
         "NetworkName": str,
         "Port": int,
@@ -475,53 +473,28 @@
 DeleteBridgeRequestRequestTypeDef = TypedDict(
     "DeleteBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
-DeleteBridgeResponseTypeDef = TypedDict(
-    "DeleteBridgeResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-DeleteFlowResponseTypeDef = TypedDict(
-    "DeleteFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DeleteGatewayResponseTypeDef = TypedDict(
-    "DeleteGatewayResponseTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
     {
         "GatewayInstanceArn": str,
     },
 )
 _OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
@@ -536,23 +509,14 @@
 class DeregisterGatewayInstanceRequestRequestTypeDef(
     _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
     _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
 
-DeregisterGatewayInstanceResponseTypeDef = TypedDict(
-    "DeregisterGatewayInstanceResponseTypeDef",
-    {
-        "GatewayInstanceArn": str,
-        "InstanceState": InstanceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBridgeRequestRequestTypeDef = TypedDict(
     "DescribeBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
@@ -617,21 +581,14 @@
 InterfaceTypeDef = TypedDict(
     "InterfaceTypeDef",
     {
         "Name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncodingParametersRequestTypeDef = TypedDict(
     "EncodingParametersRequestTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
@@ -640,48 +597,14 @@
     "EncodingParametersTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
 
-_RequiredEncryptionOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOutputTypeDef",
-    {
-        "RoleArn": str,
-    },
-)
-_OptionalEncryptionOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOutputTypeDef",
-    {
-        "Algorithm": AlgorithmType,
-        "ConstantInitializationVector": str,
-        "DeviceId": str,
-        "KeyType": KeyTypeType,
-        "Region": str,
-        "ResourceId": str,
-        "SecretArn": str,
-        "Url": str,
-    },
-    total=False,
-)
-
-
-class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
-    pass
-
-
-SourcePriorityOutputTypeDef = TypedDict(
-    "SourcePriorityOutputTypeDef",
-    {
-        "PrimarySource": str,
-    },
-    total=False,
-)
-
 SourcePriorityTypeDef = TypedDict(
     "SourcePriorityTypeDef",
     {
         "PrimarySource": str,
     },
     total=False,
 )
@@ -721,27 +644,20 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
-GatewayNetworkOutputTypeDef = TypedDict(
-    "GatewayNetworkOutputTypeDef",
-    {
-        "CidrBlock": str,
-        "Name": str,
-    },
-)
-
-ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
-    "ListBridgesRequestListBridgesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBridgesRequestRequestTypeDef = TypedDict(
     "ListBridgesRequestRequestTypeDef",
     {
@@ -759,22 +675,14 @@
         "BridgeState": BridgeStateType,
         "BridgeType": str,
         "Name": str,
         "PlacementArn": str,
     },
 )
 
-ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -798,40 +706,23 @@
 
 class ListedEntitlementTypeDef(
     _RequiredListedEntitlementTypeDef, _OptionalListedEntitlementTypeDef
 ):
     pass
 
 
-ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFlowsRequestRequestTypeDef = TypedDict(
     "ListFlowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewayInstancesRequestRequestTypeDef = TypedDict(
     "ListGatewayInstancesRequestRequestTypeDef",
     {
         "FilterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -857,22 +748,14 @@
 
 class ListedGatewayInstanceTypeDef(
     _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
 ):
     pass
 
 
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -883,39 +766,23 @@
     {
         "GatewayArn": str,
         "GatewayState": GatewayStateType,
         "Name": str,
     },
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -924,22 +791,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceSpecificationTypeDef = TypedDict(
     "_RequiredResourceSpecificationTypeDef",
     {
         "ResourceType": Literal["Mbps_Outbound_Bandwidth"],
     },
 )
 _OptionalResourceSpecificationTypeDef = TypedDict(
@@ -983,24 +842,14 @@
 )
 
 
 class TransportTypeDef(_RequiredTransportTypeDef, _OptionalTransportTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurchaseOfferingRequestRequestTypeDef = TypedDict(
     "PurchaseOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
@@ -1010,169 +859,76 @@
     "RemoveBridgeOutputRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "OutputName": str,
     },
 )
 
-RemoveBridgeOutputResponseTypeDef = TypedDict(
-    "RemoveBridgeOutputResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "OutputName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
     "RemoveBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
 
-RemoveBridgeSourceResponseTypeDef = TypedDict(
-    "RemoveBridgeSourceResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "SourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
 
-RemoveFlowMediaStreamResponseTypeDef = TypedDict(
-    "RemoveFlowMediaStreamResponseTypeDef",
-    {
-        "FlowArn": str,
-        "MediaStreamName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowOutputRequestRequestTypeDef = TypedDict(
     "RemoveFlowOutputRequestRequestTypeDef",
     {
         "FlowArn": str,
         "OutputArn": str,
     },
 )
 
-RemoveFlowOutputResponseTypeDef = TypedDict(
-    "RemoveFlowOutputResponseTypeDef",
-    {
-        "FlowArn": str,
-        "OutputArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowSourceRequestRequestTypeDef = TypedDict(
     "RemoveFlowSourceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "SourceArn": str,
     },
 )
 
-RemoveFlowSourceResponseTypeDef = TypedDict(
-    "RemoveFlowSourceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "SourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowVpcInterfaceRequestRequestTypeDef = TypedDict(
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaceName": str,
     },
 )
 
-RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "NonDeletedNetworkInterfaceIds": List[str],
-        "VpcInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RevokeFlowEntitlementRequestRequestTypeDef = TypedDict(
     "RevokeFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
 
-RevokeFlowEntitlementResponseTypeDef = TypedDict(
-    "RevokeFlowEntitlementResponseTypeDef",
-    {
-        "EntitlementArn": str,
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartFlowRequestRequestTypeDef = TypedDict(
     "StartFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1229,23 +985,14 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "DesiredState": DesiredStateType,
     },
 )
 
-UpdateBridgeStateResponseTypeDef = TypedDict(
-    "UpdateBridgeStateResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "DesiredState": DesiredStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -1286,23 +1033,14 @@
 class UpdateGatewayInstanceRequestRequestTypeDef(
     _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
     _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateGatewayInstanceResponseTypeDef = TypedDict(
-    "UpdateGatewayInstanceResponseTypeDef",
-    {
-        "BridgePlacement": BridgePlacementType,
-        "GatewayInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
     "_RequiredAddBridgeFlowSourceRequestTypeDef",
     {
         "FlowArn": str,
         "Name": str,
     },
 )
@@ -1317,14 +1055,56 @@
 
 class AddBridgeFlowSourceRequestTypeDef(
     _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
 ):
     pass
 
 
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "OutputArn": str,
+    },
+    total=False,
+)
+
+
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+):
+    pass
+
+
 _RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
     "_RequiredSetGatewayBridgeSourceRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
@@ -1364,94 +1144,225 @@
     "AddBridgeOutputRequestTypeDef",
     {
         "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
     },
     total=False,
 )
 
-AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
-    "AddFlowVpcInterfacesRequestRequestTypeDef",
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFlowResponseTypeDef = TypedDict(
+    "DeleteFlowResponseTypeDef",
     {
         "FlowArn": str,
-        "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddFlowVpcInterfacesResponseTypeDef = TypedDict(
-    "AddFlowVpcInterfacesResponseTypeDef",
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveFlowMediaStreamResponseTypeDef = TypedDict(
+    "RemoveFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
-        "VpcInterfaces": List[VpcInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MediaStreamName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGrantEntitlementRequestTypeDef = TypedDict(
-    "_RequiredGrantEntitlementRequestTypeDef",
+RemoveFlowOutputResponseTypeDef = TypedDict(
+    "RemoveFlowOutputResponseTypeDef",
     {
-        "Subscribers": Sequence[str],
+        "FlowArn": str,
+        "OutputArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGrantEntitlementRequestTypeDef = TypedDict(
-    "_OptionalGrantEntitlementRequestTypeDef",
+
+RemoveFlowSourceResponseTypeDef = TypedDict(
+    "RemoveFlowSourceResponseTypeDef",
     {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-        "Name": str,
+        "FlowArn": str,
+        "SourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "NonDeletedNetworkInterfaceIds": List[str],
+        "VpcInterfaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class GrantEntitlementRequestTypeDef(
-    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
-):
-    pass
+RevokeFlowEntitlementResponseTypeDef = TypedDict(
+    "RevokeFlowEntitlementResponseTypeDef",
+    {
+        "EntitlementArn": str,
+        "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredBridgeFlowSourceTypeDef = TypedDict(
-    "_RequiredBridgeFlowSourceTypeDef",
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
+    "AddFlowVpcInterfacesRequestRequestTypeDef",
+    {
+        "FlowArn": str,
+        "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
+    },
+)
+
+AddFlowVpcInterfacesResponseTypeDef = TypedDict(
+    "AddFlowVpcInterfacesResponseTypeDef",
     {
         "FlowArn": str,
+        "VpcInterfaces": List[VpcInterfaceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "EntitlementArn": str,
         "Name": str,
+        "Subscribers": List[str],
     },
 )
-_OptionalBridgeFlowSourceTypeDef = TypedDict(
-    "_OptionalBridgeFlowSourceTypeDef",
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
     {
-        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
-        "OutputArn": str,
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
     },
     total=False,
 )
 
 
-class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
 
-_RequiredGatewayBridgeSourceTypeDef = TypedDict(
-    "_RequiredGatewayBridgeSourceTypeDef",
+_RequiredGrantEntitlementRequestTypeDef = TypedDict(
+    "_RequiredGrantEntitlementRequestTypeDef",
     {
-        "BridgeArn": str,
+        "Subscribers": Sequence[str],
     },
 )
-_OptionalGatewayBridgeSourceTypeDef = TypedDict(
-    "_OptionalGatewayBridgeSourceTypeDef",
+_OptionalGrantEntitlementRequestTypeDef = TypedDict(
+    "_OptionalGrantEntitlementRequestTypeDef",
     {
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
+        "Name": str,
     },
     total=False,
 )
 
 
-class GatewayBridgeSourceTypeDef(
-    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+class GrantEntitlementRequestTypeDef(
+    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
 ):
     pass
 
 
 BridgeOutputTypeDef = TypedDict(
     "BridgeOutputTypeDef",
     {
@@ -1491,14 +1402,37 @@
     {
         "EgressCidrBlocks": Sequence[str],
         "Name": str,
         "Networks": Sequence[GatewayNetworkTypeDef],
     },
 )
 
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
+
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -1593,49 +1527,14 @@
     {
         "InputIp": str,
         "InputPort": int,
         "Interface": InterfaceTypeDef,
     },
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
-    {
-        "EntitlementArn": str,
-        "Name": str,
-        "Subscribers": List[str],
-    },
-)
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
-    {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionOutputTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-    },
-    total=False,
-)
-
-
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
-    pass
-
-
-FailoverConfigOutputTypeDef = TypedDict(
-    "FailoverConfigOutputTypeDef",
-    {
-        "FailoverMode": FailoverModeType,
-        "RecoveryWindow": int,
-        "SourcePriority": SourcePriorityOutputTypeDef,
-        "State": StateType,
-    },
-    total=False,
-)
-
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "FailoverMode": FailoverModeType,
         "RecoveryWindow": int,
         "SourcePriority": SourcePriorityTypeDef,
         "State": StateType,
@@ -1704,70 +1603,105 @@
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
 
-_RequiredGatewayTypeDef = TypedDict(
-    "_RequiredGatewayTypeDef",
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     {
-        "EgressCidrBlocks": List[str],
-        "GatewayArn": str,
-        "Name": str,
-        "Networks": List[GatewayNetworkOutputTypeDef],
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalGatewayTypeDef = TypedDict(
-    "_OptionalGatewayTypeDef",
+
+ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     {
-        "GatewayMessages": List[MessageDetailTypeDef],
-        "GatewayState": GatewayStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
-    pass
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewayInstancesResponseTypeDef = TypedDict(
     "ListGatewayInstancesResponseTypeDef",
     {
         "Instances": List[ListedGatewayInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "Gateways": List[ListedGatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
@@ -1854,14 +1788,23 @@
     {
         "FlowSource": AddBridgeFlowSourceRequestTypeDef,
         "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
     },
     total=False,
 )
 
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
+    {
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
@@ -1886,54 +1829,79 @@
     "AddBridgeOutputsRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
     },
 )
 
-GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
-    "GrantFlowEntitlementsRequestRequestTypeDef",
+GrantFlowEntitlementsResponseTypeDef = TypedDict(
+    "GrantFlowEntitlementsResponseTypeDef",
     {
-        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
+        "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BridgeSourceTypeDef = TypedDict(
-    "BridgeSourceTypeDef",
+UpdateFlowEntitlementResponseTypeDef = TypedDict(
+    "UpdateFlowEntitlementResponseTypeDef",
     {
-        "FlowSource": BridgeFlowSourceTypeDef,
-        "NetworkSource": BridgeNetworkSourceTypeDef,
+        "Entitlement": EntitlementTypeDef,
+        "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
+    "GrantFlowEntitlementsRequestRequestTypeDef",
+    {
+        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
+        "FlowArn": str,
     },
-    total=False,
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBridgeOutputResponseTypeDef = TypedDict(
     "UpdateBridgeOutputResponseTypeDef",
     {
         "BridgeArn": str,
         "Output": BridgeOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayInstanceResponseTypeDef = TypedDict(
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
@@ -2021,32 +1989,14 @@
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
 
-GrantFlowEntitlementsResponseTypeDef = TypedDict(
-    "GrantFlowEntitlementsResponseTypeDef",
-    {
-        "Entitlements": List[EntitlementTypeDef],
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFlowEntitlementResponseTypeDef = TypedDict(
-    "UpdateFlowEntitlementResponseTypeDef",
-    {
-        "Entitlement": EntitlementTypeDef,
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
@@ -2089,15 +2039,15 @@
 
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "Flows": List[ListedFlowTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddMediaStreamRequestTypeDef = TypedDict(
     "_RequiredAddMediaStreamRequestTypeDef",
     {
         "MediaStreamId": int,
@@ -2171,69 +2121,53 @@
 )
 
 
 class MediaStreamTypeDef(_RequiredMediaStreamTypeDef, _OptionalMediaStreamTypeDef):
     pass
 
 
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGatewayResponseTypeDef = TypedDict(
-    "DescribeGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddBridgeSourcesRequestRequestTypeDef = TypedDict(
     "AddBridgeSourcesRequestRequestTypeDef",
     {
         "BridgeArn": str,
@@ -2268,15 +2202,15 @@
 
 
 AddBridgeSourcesResponseTypeDef = TypedDict(
     "AddBridgeSourcesResponseTypeDef",
     {
         "BridgeArn": str,
         "Sources": List[BridgeSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBridgeTypeDef = TypedDict(
     "_RequiredBridgeTypeDef",
     {
         "BridgeArn": str,
@@ -2288,15 +2222,15 @@
 _OptionalBridgeTypeDef = TypedDict(
     "_OptionalBridgeTypeDef",
     {
         "BridgeMessages": List[MessageDetailTypeDef],
         "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
         "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
         "Outputs": List[BridgeOutputTypeDef],
-        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
+        "SourceFailoverConfig": FailoverConfigTypeDef,
         "Sources": List[BridgeSourceTypeDef],
     },
     total=False,
 )
 
 
 class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
@@ -2304,15 +2238,15 @@
 
 
 UpdateBridgeSourceResponseTypeDef = TypedDict(
     "UpdateBridgeSourceResponseTypeDef",
     {
         "BridgeArn": str,
         "Source": BridgeSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
@@ -2454,22 +2388,22 @@
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Destination": str,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
         "BridgeArn": str,
         "BridgePorts": List[int],
     },
     total=False,
 )
 
 
@@ -2484,15 +2418,15 @@
         "SourceArn": str,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
-        "Decryption": EncryptionOutputTypeDef,
+        "Decryption": EncryptionTypeDef,
         "Description": str,
         "EntitlementArn": str,
         "IngestIp": str,
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
@@ -2518,48 +2452,48 @@
 )
 
 AddFlowMediaStreamsResponseTypeDef = TypedDict(
     "AddFlowMediaStreamsResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowMediaStreamResponseTypeDef = TypedDict(
     "UpdateFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBridgeResponseTypeDef = TypedDict(
     "CreateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBridgeResponseTypeDef = TypedDict(
     "DescribeBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBridgeResponseTypeDef = TypedDict(
     "UpdateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
@@ -2605,33 +2539,33 @@
 
 
 AddFlowOutputsResponseTypeDef = TypedDict(
     "AddFlowOutputsResponseTypeDef",
     {
         "FlowArn": str,
         "Outputs": List[OutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowOutputResponseTypeDef = TypedDict(
     "UpdateFlowOutputResponseTypeDef",
     {
         "FlowArn": str,
         "Output": OutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddFlowSourcesResponseTypeDef = TypedDict(
     "AddFlowSourcesResponseTypeDef",
     {
         "FlowArn": str,
         "Sources": List[SourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowTypeDef = TypedDict(
     "_RequiredFlowTypeDef",
     {
         "AvailabilityZone": str,
@@ -2645,15 +2579,15 @@
 )
 _OptionalFlowTypeDef = TypedDict(
     "_OptionalFlowTypeDef",
     {
         "Description": str,
         "EgressIp": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
+        "SourceFailoverConfig": FailoverConfigTypeDef,
         "Sources": List[SourceTypeDef],
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "Maintenance": MaintenanceTypeDef,
     },
     total=False,
 )
 
@@ -2663,35 +2597,35 @@
 
 
 UpdateFlowSourceResponseTypeDef = TypedDict(
     "UpdateFlowSourceResponseTypeDef",
     {
         "FlowArn": str,
         "Source": SourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFlowResponseTypeDef = TypedDict(
     "CreateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
         "Messages": MessagesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/type_defs.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,169 +50,164 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "VpcInterfaceAttachmentTypeDef",
     "AddBridgeNetworkOutputRequestTypeDef",
     "AddBridgeNetworkSourceRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
     "VpcInterfaceTypeDef",
     "AddIngressGatewayBridgeRequestTypeDef",
     "AddMaintenanceTypeDef",
     "EncryptionTypeDef",
     "BridgeFlowOutputTypeDef",
-    "VpcInterfaceAttachmentOutputTypeDef",
     "BridgeNetworkOutputTypeDef",
     "BridgeNetworkSourceTypeDef",
     "EgressGatewayBridgeTypeDef",
     "IngressGatewayBridgeTypeDef",
     "MessageDetailTypeDef",
     "GatewayNetworkTypeDef",
     "DeleteBridgeRequestRequestTypeDef",
-    "DeleteBridgeResponseTypeDef",
     "DeleteFlowRequestRequestTypeDef",
-    "DeleteFlowResponseTypeDef",
     "DeleteGatewayRequestRequestTypeDef",
-    "DeleteGatewayResponseTypeDef",
     "DeregisterGatewayInstanceRequestRequestTypeDef",
-    "DeregisterGatewayInstanceResponseTypeDef",
     "DescribeBridgeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeFlowRequestRequestTypeDef",
     "MessagesTypeDef",
     "DescribeGatewayInstanceRequestRequestTypeDef",
     "DescribeGatewayRequestRequestTypeDef",
     "DescribeOfferingRequestRequestTypeDef",
     "DescribeReservationRequestRequestTypeDef",
     "InterfaceRequestTypeDef",
     "InterfaceTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EncodingParametersRequestTypeDef",
     "EncodingParametersTypeDef",
-    "EncryptionOutputTypeDef",
-    "SourcePriorityOutputTypeDef",
     "SourcePriorityTypeDef",
     "MaintenanceTypeDef",
     "FmtpRequestTypeDef",
     "FmtpTypeDef",
-    "GatewayNetworkOutputTypeDef",
-    "ListBridgesRequestListBridgesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBridgesRequestRequestTypeDef",
     "ListedBridgeTypeDef",
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     "ListEntitlementsRequestRequestTypeDef",
     "ListedEntitlementTypeDef",
-    "ListFlowsRequestListFlowsPaginateTypeDef",
     "ListFlowsRequestRequestTypeDef",
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
     "ListGatewayInstancesRequestRequestTypeDef",
     "ListedGatewayInstanceTypeDef",
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
     "ListGatewaysRequestRequestTypeDef",
     "ListedGatewayTypeDef",
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
     "ListOfferingsRequestRequestTypeDef",
-    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListReservationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ResourceSpecificationTypeDef",
     "TransportTypeDef",
-    "PaginatorConfigTypeDef",
     "PurchaseOfferingRequestRequestTypeDef",
     "RemoveBridgeOutputRequestRequestTypeDef",
-    "RemoveBridgeOutputResponseTypeDef",
     "RemoveBridgeSourceRequestRequestTypeDef",
-    "RemoveBridgeSourceResponseTypeDef",
     "RemoveFlowMediaStreamRequestRequestTypeDef",
-    "RemoveFlowMediaStreamResponseTypeDef",
     "RemoveFlowOutputRequestRequestTypeDef",
-    "RemoveFlowOutputResponseTypeDef",
     "RemoveFlowSourceRequestRequestTypeDef",
-    "RemoveFlowSourceResponseTypeDef",
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeFlowEntitlementRequestRequestTypeDef",
-    "RevokeFlowEntitlementResponseTypeDef",
     "StartFlowRequestRequestTypeDef",
-    "StartFlowResponseTypeDef",
     "StopFlowRequestRequestTypeDef",
-    "StopFlowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBridgeNetworkOutputRequestTypeDef",
     "UpdateBridgeNetworkSourceRequestTypeDef",
     "UpdateEgressGatewayBridgeRequestTypeDef",
     "UpdateIngressGatewayBridgeRequestTypeDef",
     "UpdateBridgeStateRequestRequestTypeDef",
-    "UpdateBridgeStateResponseTypeDef",
     "UpdateEncryptionTypeDef",
     "UpdateMaintenanceTypeDef",
     "UpdateGatewayInstanceRequestRequestTypeDef",
-    "UpdateGatewayInstanceResponseTypeDef",
     "AddBridgeFlowSourceRequestTypeDef",
+    "BridgeFlowSourceTypeDef",
+    "GatewayBridgeSourceTypeDef",
     "SetGatewayBridgeSourceRequestTypeDef",
     "UpdateBridgeFlowSourceRequestTypeDef",
     "UpdateGatewayBridgeSourceRequestTypeDef",
     "AddBridgeOutputRequestTypeDef",
+    "DeleteBridgeResponseTypeDef",
+    "DeleteFlowResponseTypeDef",
+    "DeleteGatewayResponseTypeDef",
+    "DeregisterGatewayInstanceResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RemoveBridgeOutputResponseTypeDef",
+    "RemoveBridgeSourceResponseTypeDef",
+    "RemoveFlowMediaStreamResponseTypeDef",
+    "RemoveFlowOutputResponseTypeDef",
+    "RemoveFlowSourceResponseTypeDef",
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    "RevokeFlowEntitlementResponseTypeDef",
+    "StartFlowResponseTypeDef",
+    "StopFlowResponseTypeDef",
+    "UpdateBridgeStateResponseTypeDef",
+    "UpdateGatewayInstanceResponseTypeDef",
     "AddFlowVpcInterfacesRequestRequestTypeDef",
     "AddFlowVpcInterfacesResponseTypeDef",
+    "EntitlementTypeDef",
     "GrantEntitlementRequestTypeDef",
-    "BridgeFlowSourceTypeDef",
-    "GatewayBridgeSourceTypeDef",
     "BridgeOutputTypeDef",
     "GatewayInstanceTypeDef",
     "CreateGatewayRequestRequestTypeDef",
+    "GatewayTypeDef",
     "DescribeFlowRequestFlowActiveWaitTypeDef",
     "DescribeFlowRequestFlowDeletedWaitTypeDef",
     "DescribeFlowRequestFlowStandbyWaitTypeDef",
     "DestinationConfigurationRequestTypeDef",
     "InputConfigurationRequestTypeDef",
     "DestinationConfigurationTypeDef",
     "InputConfigurationTypeDef",
-    "EntitlementTypeDef",
-    "FailoverConfigOutputTypeDef",
     "FailoverConfigTypeDef",
     "UpdateFailoverConfigTypeDef",
     "ListedFlowTypeDef",
     "MediaStreamAttributesRequestTypeDef",
     "MediaStreamAttributesTypeDef",
-    "GatewayTypeDef",
+    "ListBridgesRequestListBridgesPaginateTypeDef",
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    "ListReservationsRequestListReservationsPaginateTypeDef",
     "ListBridgesResponseTypeDef",
     "ListEntitlementsResponseTypeDef",
     "ListGatewayInstancesResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "OfferingTypeDef",
     "ReservationTypeDef",
     "UpdateBridgeOutputRequestRequestTypeDef",
     "UpdateFlowEntitlementRequestRequestTypeDef",
     "AddBridgeSourceRequestTypeDef",
+    "BridgeSourceTypeDef",
     "UpdateBridgeSourceRequestRequestTypeDef",
     "AddBridgeOutputsRequestRequestTypeDef",
+    "GrantFlowEntitlementsResponseTypeDef",
+    "UpdateFlowEntitlementResponseTypeDef",
     "GrantFlowEntitlementsRequestRequestTypeDef",
-    "BridgeSourceTypeDef",
     "AddBridgeOutputsResponseTypeDef",
     "UpdateBridgeOutputResponseTypeDef",
     "DescribeGatewayInstanceResponseTypeDef",
+    "CreateGatewayResponseTypeDef",
+    "DescribeGatewayResponseTypeDef",
     "MediaStreamOutputConfigurationRequestTypeDef",
     "MediaStreamSourceConfigurationRequestTypeDef",
     "MediaStreamOutputConfigurationTypeDef",
     "MediaStreamSourceConfigurationTypeDef",
-    "GrantFlowEntitlementsResponseTypeDef",
-    "UpdateFlowEntitlementResponseTypeDef",
     "UpdateBridgeRequestRequestTypeDef",
     "UpdateFlowRequestRequestTypeDef",
     "ListFlowsResponseTypeDef",
     "AddMediaStreamRequestTypeDef",
     "UpdateFlowMediaStreamRequestRequestTypeDef",
     "MediaStreamTypeDef",
-    "CreateGatewayResponseTypeDef",
-    "DescribeGatewayResponseTypeDef",
     "DescribeOfferingResponseTypeDef",
     "ListOfferingsResponseTypeDef",
     "DescribeReservationResponseTypeDef",
     "ListReservationsResponseTypeDef",
     "PurchaseOfferingResponseTypeDef",
     "AddBridgeSourcesRequestRequestTypeDef",
     "CreateBridgeRequestRequestTypeDef",
@@ -271,14 +266,25 @@
         "Name": str,
         "NetworkName": str,
         "Port": int,
         "Protocol": ProtocolType,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 AddEgressGatewayBridgeRequestTypeDef = TypedDict(
     "AddEgressGatewayBridgeRequestTypeDef",
     {
         "MaxBitrate": int,
     },
 )
 
@@ -361,22 +367,14 @@
     {
         "FlowArn": str,
         "FlowSourceArn": str,
         "Name": str,
     },
 )
 
-VpcInterfaceAttachmentOutputTypeDef = TypedDict(
-    "VpcInterfaceAttachmentOutputTypeDef",
-    {
-        "VpcInterfaceName": str,
-    },
-    total=False,
-)
-
 BridgeNetworkOutputTypeDef = TypedDict(
     "BridgeNetworkOutputTypeDef",
     {
         "IpAddress": str,
         "Name": str,
         "NetworkName": str,
         "Port": int,
@@ -464,53 +462,28 @@
 DeleteBridgeRequestRequestTypeDef = TypedDict(
     "DeleteBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
-DeleteBridgeResponseTypeDef = TypedDict(
-    "DeleteBridgeResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFlowRequestRequestTypeDef = TypedDict(
     "DeleteFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-DeleteFlowResponseTypeDef = TypedDict(
-    "DeleteFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayRequestRequestTypeDef = TypedDict(
     "DeleteGatewayRequestRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DeleteGatewayResponseTypeDef = TypedDict(
-    "DeleteGatewayResponseTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredDeregisterGatewayInstanceRequestRequestTypeDef",
     {
         "GatewayInstanceArn": str,
     },
 )
 _OptionalDeregisterGatewayInstanceRequestRequestTypeDef = TypedDict(
@@ -523,23 +496,14 @@
 
 class DeregisterGatewayInstanceRequestRequestTypeDef(
     _RequiredDeregisterGatewayInstanceRequestRequestTypeDef,
     _OptionalDeregisterGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
-DeregisterGatewayInstanceResponseTypeDef = TypedDict(
-    "DeregisterGatewayInstanceResponseTypeDef",
-    {
-        "GatewayInstanceArn": str,
-        "InstanceState": InstanceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBridgeRequestRequestTypeDef = TypedDict(
     "DescribeBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 
@@ -604,21 +568,14 @@
 InterfaceTypeDef = TypedDict(
     "InterfaceTypeDef",
     {
         "Name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EncodingParametersRequestTypeDef = TypedDict(
     "EncodingParametersRequestTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
@@ -627,46 +584,14 @@
     "EncodingParametersTypeDef",
     {
         "CompressionFactor": float,
         "EncoderProfile": EncoderProfileType,
     },
 )
 
-_RequiredEncryptionOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOutputTypeDef",
-    {
-        "RoleArn": str,
-    },
-)
-_OptionalEncryptionOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOutputTypeDef",
-    {
-        "Algorithm": AlgorithmType,
-        "ConstantInitializationVector": str,
-        "DeviceId": str,
-        "KeyType": KeyTypeType,
-        "Region": str,
-        "ResourceId": str,
-        "SecretArn": str,
-        "Url": str,
-    },
-    total=False,
-)
-
-class EncryptionOutputTypeDef(_RequiredEncryptionOutputTypeDef, _OptionalEncryptionOutputTypeDef):
-    pass
-
-SourcePriorityOutputTypeDef = TypedDict(
-    "SourcePriorityOutputTypeDef",
-    {
-        "PrimarySource": str,
-    },
-    total=False,
-)
-
 SourcePriorityTypeDef = TypedDict(
     "SourcePriorityTypeDef",
     {
         "PrimarySource": str,
     },
     total=False,
 )
@@ -706,27 +631,20 @@
         "Range": RangeType,
         "ScanMode": ScanModeType,
         "Tcs": TcsType,
     },
     total=False,
 )
 
-GatewayNetworkOutputTypeDef = TypedDict(
-    "GatewayNetworkOutputTypeDef",
-    {
-        "CidrBlock": str,
-        "Name": str,
-    },
-)
-
-ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
-    "ListBridgesRequestListBridgesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBridgesRequestRequestTypeDef = TypedDict(
     "ListBridgesRequestRequestTypeDef",
     {
@@ -744,22 +662,14 @@
         "BridgeState": BridgeStateType,
         "BridgeType": str,
         "Name": str,
         "PlacementArn": str,
     },
 )
 
-ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
-    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEntitlementsRequestRequestTypeDef = TypedDict(
     "ListEntitlementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -781,40 +691,23 @@
 )
 
 class ListedEntitlementTypeDef(
     _RequiredListedEntitlementTypeDef, _OptionalListedEntitlementTypeDef
 ):
     pass
 
-ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
-    "ListFlowsRequestListFlowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFlowsRequestRequestTypeDef = TypedDict(
     "ListFlowsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
-    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
-    {
-        "FilterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewayInstancesRequestRequestTypeDef = TypedDict(
     "ListGatewayInstancesRequestRequestTypeDef",
     {
         "FilterArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -838,22 +731,14 @@
 )
 
 class ListedGatewayInstanceTypeDef(
     _RequiredListedGatewayInstanceTypeDef, _OptionalListedGatewayInstanceTypeDef
 ):
     pass
 
-ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysRequestListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysRequestRequestTypeDef = TypedDict(
     "ListGatewaysRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -864,39 +749,23 @@
     {
         "GatewayArn": str,
         "GatewayState": GatewayStateType,
         "Name": str,
     },
 )
 
-ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
-    "ListOfferingsRequestListOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOfferingsRequestRequestTypeDef = TypedDict(
     "ListOfferingsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
-    "ListReservationsRequestListReservationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReservationsRequestRequestTypeDef = TypedDict(
     "ListReservationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -905,22 +774,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredResourceSpecificationTypeDef = TypedDict(
     "_RequiredResourceSpecificationTypeDef",
     {
         "ResourceType": Literal["Mbps_Outbound_Bandwidth"],
     },
 )
 _OptionalResourceSpecificationTypeDef = TypedDict(
@@ -960,24 +821,14 @@
     },
     total=False,
 )
 
 class TransportTypeDef(_RequiredTransportTypeDef, _OptionalTransportTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurchaseOfferingRequestRequestTypeDef = TypedDict(
     "PurchaseOfferingRequestRequestTypeDef",
     {
         "OfferingArn": str,
         "ReservationName": str,
         "Start": str,
     },
@@ -987,169 +838,76 @@
     "RemoveBridgeOutputRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "OutputName": str,
     },
 )
 
-RemoveBridgeOutputResponseTypeDef = TypedDict(
-    "RemoveBridgeOutputResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "OutputName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveBridgeSourceRequestRequestTypeDef = TypedDict(
     "RemoveBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
 
-RemoveBridgeSourceResponseTypeDef = TypedDict(
-    "RemoveBridgeSourceResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "SourceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowMediaStreamRequestRequestTypeDef = TypedDict(
     "RemoveFlowMediaStreamRequestRequestTypeDef",
     {
         "FlowArn": str,
         "MediaStreamName": str,
     },
 )
 
-RemoveFlowMediaStreamResponseTypeDef = TypedDict(
-    "RemoveFlowMediaStreamResponseTypeDef",
-    {
-        "FlowArn": str,
-        "MediaStreamName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowOutputRequestRequestTypeDef = TypedDict(
     "RemoveFlowOutputRequestRequestTypeDef",
     {
         "FlowArn": str,
         "OutputArn": str,
     },
 )
 
-RemoveFlowOutputResponseTypeDef = TypedDict(
-    "RemoveFlowOutputResponseTypeDef",
-    {
-        "FlowArn": str,
-        "OutputArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowSourceRequestRequestTypeDef = TypedDict(
     "RemoveFlowSourceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "SourceArn": str,
     },
 )
 
-RemoveFlowSourceResponseTypeDef = TypedDict(
-    "RemoveFlowSourceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "SourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveFlowVpcInterfaceRequestRequestTypeDef = TypedDict(
     "RemoveFlowVpcInterfaceRequestRequestTypeDef",
     {
         "FlowArn": str,
         "VpcInterfaceName": str,
     },
 )
 
-RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
-    "RemoveFlowVpcInterfaceResponseTypeDef",
-    {
-        "FlowArn": str,
-        "NonDeletedNetworkInterfaceIds": List[str],
-        "VpcInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 RevokeFlowEntitlementRequestRequestTypeDef = TypedDict(
     "RevokeFlowEntitlementRequestRequestTypeDef",
     {
         "EntitlementArn": str,
         "FlowArn": str,
     },
 )
 
-RevokeFlowEntitlementResponseTypeDef = TypedDict(
-    "RevokeFlowEntitlementResponseTypeDef",
-    {
-        "EntitlementArn": str,
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartFlowRequestRequestTypeDef = TypedDict(
     "StartFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-StartFlowResponseTypeDef = TypedDict(
-    "StartFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopFlowRequestRequestTypeDef = TypedDict(
     "StopFlowRequestRequestTypeDef",
     {
         "FlowArn": str,
     },
 )
 
-StopFlowResponseTypeDef = TypedDict(
-    "StopFlowResponseTypeDef",
-    {
-        "FlowArn": str,
-        "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1206,23 +964,14 @@
     "UpdateBridgeStateRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "DesiredState": DesiredStateType,
     },
 )
 
-UpdateBridgeStateResponseTypeDef = TypedDict(
-    "UpdateBridgeStateResponseTypeDef",
-    {
-        "BridgeArn": str,
-        "DesiredState": DesiredStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionTypeDef = TypedDict(
     "UpdateEncryptionTypeDef",
     {
         "Algorithm": AlgorithmType,
         "ConstantInitializationVector": str,
         "DeviceId": str,
         "KeyType": KeyTypeType,
@@ -1261,23 +1010,14 @@
 
 class UpdateGatewayInstanceRequestRequestTypeDef(
     _RequiredUpdateGatewayInstanceRequestRequestTypeDef,
     _OptionalUpdateGatewayInstanceRequestRequestTypeDef,
 ):
     pass
 
-UpdateGatewayInstanceResponseTypeDef = TypedDict(
-    "UpdateGatewayInstanceResponseTypeDef",
-    {
-        "BridgePlacement": BridgePlacementType,
-        "GatewayInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAddBridgeFlowSourceRequestTypeDef = TypedDict(
     "_RequiredAddBridgeFlowSourceRequestTypeDef",
     {
         "FlowArn": str,
         "Name": str,
     },
 )
@@ -1290,14 +1030,52 @@
 )
 
 class AddBridgeFlowSourceRequestTypeDef(
     _RequiredAddBridgeFlowSourceRequestTypeDef, _OptionalAddBridgeFlowSourceRequestTypeDef
 ):
     pass
 
+_RequiredBridgeFlowSourceTypeDef = TypedDict(
+    "_RequiredBridgeFlowSourceTypeDef",
+    {
+        "FlowArn": str,
+        "Name": str,
+    },
+)
+_OptionalBridgeFlowSourceTypeDef = TypedDict(
+    "_OptionalBridgeFlowSourceTypeDef",
+    {
+        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+        "OutputArn": str,
+    },
+    total=False,
+)
+
+class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+    pass
+
+_RequiredGatewayBridgeSourceTypeDef = TypedDict(
+    "_RequiredGatewayBridgeSourceTypeDef",
+    {
+        "BridgeArn": str,
+    },
+)
+_OptionalGatewayBridgeSourceTypeDef = TypedDict(
+    "_OptionalGatewayBridgeSourceTypeDef",
+    {
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
+    },
+    total=False,
+)
+
+class GatewayBridgeSourceTypeDef(
+    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+):
+    pass
+
 _RequiredSetGatewayBridgeSourceRequestTypeDef = TypedDict(
     "_RequiredSetGatewayBridgeSourceRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalSetGatewayBridgeSourceRequestTypeDef = TypedDict(
@@ -1335,89 +1113,222 @@
     "AddBridgeOutputRequestTypeDef",
     {
         "NetworkOutput": AddBridgeNetworkOutputRequestTypeDef,
     },
     total=False,
 )
 
-AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
-    "AddFlowVpcInterfacesRequestRequestTypeDef",
+DeleteBridgeResponseTypeDef = TypedDict(
+    "DeleteBridgeResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFlowResponseTypeDef = TypedDict(
+    "DeleteFlowResponseTypeDef",
     {
         "FlowArn": str,
-        "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddFlowVpcInterfacesResponseTypeDef = TypedDict(
-    "AddFlowVpcInterfacesResponseTypeDef",
+DeleteGatewayResponseTypeDef = TypedDict(
+    "DeleteGatewayResponseTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterGatewayInstanceResponseTypeDef = TypedDict(
+    "DeregisterGatewayInstanceResponseTypeDef",
+    {
+        "GatewayInstanceArn": str,
+        "InstanceState": InstanceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeOutputResponseTypeDef = TypedDict(
+    "RemoveBridgeOutputResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "OutputName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveBridgeSourceResponseTypeDef = TypedDict(
+    "RemoveBridgeSourceResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "SourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveFlowMediaStreamResponseTypeDef = TypedDict(
+    "RemoveFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
-        "VpcInterfaces": List[VpcInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MediaStreamName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGrantEntitlementRequestTypeDef = TypedDict(
-    "_RequiredGrantEntitlementRequestTypeDef",
+RemoveFlowOutputResponseTypeDef = TypedDict(
+    "RemoveFlowOutputResponseTypeDef",
     {
-        "Subscribers": Sequence[str],
+        "FlowArn": str,
+        "OutputArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGrantEntitlementRequestTypeDef = TypedDict(
-    "_OptionalGrantEntitlementRequestTypeDef",
+
+RemoveFlowSourceResponseTypeDef = TypedDict(
+    "RemoveFlowSourceResponseTypeDef",
     {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-        "Name": str,
+        "FlowArn": str,
+        "SourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class GrantEntitlementRequestTypeDef(
-    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
-):
-    pass
+RemoveFlowVpcInterfaceResponseTypeDef = TypedDict(
+    "RemoveFlowVpcInterfaceResponseTypeDef",
+    {
+        "FlowArn": str,
+        "NonDeletedNetworkInterfaceIds": List[str],
+        "VpcInterfaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredBridgeFlowSourceTypeDef = TypedDict(
-    "_RequiredBridgeFlowSourceTypeDef",
+RevokeFlowEntitlementResponseTypeDef = TypedDict(
+    "RevokeFlowEntitlementResponseTypeDef",
+    {
+        "EntitlementArn": str,
+        "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartFlowResponseTypeDef = TypedDict(
+    "StartFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopFlowResponseTypeDef = TypedDict(
+    "StopFlowResponseTypeDef",
+    {
+        "FlowArn": str,
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBridgeStateResponseTypeDef = TypedDict(
+    "UpdateBridgeStateResponseTypeDef",
+    {
+        "BridgeArn": str,
+        "DesiredState": DesiredStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInstanceResponseTypeDef = TypedDict(
+    "UpdateGatewayInstanceResponseTypeDef",
+    {
+        "BridgePlacement": BridgePlacementType,
+        "GatewayInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddFlowVpcInterfacesRequestRequestTypeDef = TypedDict(
+    "AddFlowVpcInterfacesRequestRequestTypeDef",
     {
         "FlowArn": str,
+        "VpcInterfaces": Sequence[VpcInterfaceRequestTypeDef],
+    },
+)
+
+AddFlowVpcInterfacesResponseTypeDef = TypedDict(
+    "AddFlowVpcInterfacesResponseTypeDef",
+    {
+        "FlowArn": str,
+        "VpcInterfaces": List[VpcInterfaceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredEntitlementTypeDef = TypedDict(
+    "_RequiredEntitlementTypeDef",
+    {
+        "EntitlementArn": str,
         "Name": str,
+        "Subscribers": List[str],
     },
 )
-_OptionalBridgeFlowSourceTypeDef = TypedDict(
-    "_OptionalBridgeFlowSourceTypeDef",
+_OptionalEntitlementTypeDef = TypedDict(
+    "_OptionalEntitlementTypeDef",
     {
-        "FlowVpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
-        "OutputArn": str,
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
     },
     total=False,
 )
 
-class BridgeFlowSourceTypeDef(_RequiredBridgeFlowSourceTypeDef, _OptionalBridgeFlowSourceTypeDef):
+class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
-_RequiredGatewayBridgeSourceTypeDef = TypedDict(
-    "_RequiredGatewayBridgeSourceTypeDef",
+_RequiredGrantEntitlementRequestTypeDef = TypedDict(
+    "_RequiredGrantEntitlementRequestTypeDef",
     {
-        "BridgeArn": str,
+        "Subscribers": Sequence[str],
     },
 )
-_OptionalGatewayBridgeSourceTypeDef = TypedDict(
-    "_OptionalGatewayBridgeSourceTypeDef",
+_OptionalGrantEntitlementRequestTypeDef = TypedDict(
+    "_OptionalGrantEntitlementRequestTypeDef",
     {
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "DataTransferSubscriberFeePercent": int,
+        "Description": str,
+        "Encryption": EncryptionTypeDef,
+        "EntitlementStatus": EntitlementStatusType,
+        "Name": str,
     },
     total=False,
 )
 
-class GatewayBridgeSourceTypeDef(
-    _RequiredGatewayBridgeSourceTypeDef, _OptionalGatewayBridgeSourceTypeDef
+class GrantEntitlementRequestTypeDef(
+    _RequiredGrantEntitlementRequestTypeDef, _OptionalGrantEntitlementRequestTypeDef
 ):
     pass
 
 BridgeOutputTypeDef = TypedDict(
     "BridgeOutputTypeDef",
     {
         "FlowOutput": BridgeFlowOutputTypeDef,
@@ -1454,14 +1365,35 @@
     {
         "EgressCidrBlocks": Sequence[str],
         "Name": str,
         "Networks": Sequence[GatewayNetworkTypeDef],
     },
 )
 
+_RequiredGatewayTypeDef = TypedDict(
+    "_RequiredGatewayTypeDef",
+    {
+        "EgressCidrBlocks": List[str],
+        "GatewayArn": str,
+        "Name": str,
+        "Networks": List[GatewayNetworkTypeDef],
+    },
+)
+_OptionalGatewayTypeDef = TypedDict(
+    "_OptionalGatewayTypeDef",
+    {
+        "GatewayMessages": List[MessageDetailTypeDef],
+        "GatewayState": GatewayStateType,
+    },
+    total=False,
+)
+
+class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
+    pass
+
 _RequiredDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
     "_RequiredDescribeFlowRequestFlowActiveWaitTypeDef",
     {
         "FlowArn": str,
     },
 )
 _OptionalDescribeFlowRequestFlowActiveWaitTypeDef = TypedDict(
@@ -1550,47 +1482,14 @@
     {
         "InputIp": str,
         "InputPort": int,
         "Interface": InterfaceTypeDef,
     },
 )
 
-_RequiredEntitlementTypeDef = TypedDict(
-    "_RequiredEntitlementTypeDef",
-    {
-        "EntitlementArn": str,
-        "Name": str,
-        "Subscribers": List[str],
-    },
-)
-_OptionalEntitlementTypeDef = TypedDict(
-    "_OptionalEntitlementTypeDef",
-    {
-        "DataTransferSubscriberFeePercent": int,
-        "Description": str,
-        "Encryption": EncryptionOutputTypeDef,
-        "EntitlementStatus": EntitlementStatusType,
-    },
-    total=False,
-)
-
-class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
-    pass
-
-FailoverConfigOutputTypeDef = TypedDict(
-    "FailoverConfigOutputTypeDef",
-    {
-        "FailoverMode": FailoverModeType,
-        "RecoveryWindow": int,
-        "SourcePriority": SourcePriorityOutputTypeDef,
-        "State": StateType,
-    },
-    total=False,
-)
-
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "FailoverMode": FailoverModeType,
         "RecoveryWindow": int,
         "SourcePriority": SourcePriorityTypeDef,
         "State": StateType,
@@ -1655,68 +1554,105 @@
 )
 
 class MediaStreamAttributesTypeDef(
     _RequiredMediaStreamAttributesTypeDef, _OptionalMediaStreamAttributesTypeDef
 ):
     pass
 
-_RequiredGatewayTypeDef = TypedDict(
-    "_RequiredGatewayTypeDef",
+ListBridgesRequestListBridgesPaginateTypeDef = TypedDict(
+    "ListBridgesRequestListBridgesPaginateTypeDef",
     {
-        "EgressCidrBlocks": List[str],
-        "GatewayArn": str,
-        "Name": str,
-        "Networks": List[GatewayNetworkOutputTypeDef],
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalGatewayTypeDef = TypedDict(
-    "_OptionalGatewayTypeDef",
+
+ListEntitlementsRequestListEntitlementsPaginateTypeDef = TypedDict(
+    "ListEntitlementsRequestListEntitlementsPaginateTypeDef",
     {
-        "GatewayMessages": List[MessageDetailTypeDef],
-        "GatewayState": GatewayStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class GatewayTypeDef(_RequiredGatewayTypeDef, _OptionalGatewayTypeDef):
-    pass
+ListFlowsRequestListFlowsPaginateTypeDef = TypedDict(
+    "ListFlowsRequestListFlowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef = TypedDict(
+    "ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef",
+    {
+        "FilterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysRequestListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysRequestListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOfferingsRequestListOfferingsPaginateTypeDef = TypedDict(
+    "ListOfferingsRequestListOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReservationsRequestListReservationsPaginateTypeDef = TypedDict(
+    "ListReservationsRequestListReservationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListBridgesResponseTypeDef = TypedDict(
     "ListBridgesResponseTypeDef",
     {
         "Bridges": List[ListedBridgeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitlementsResponseTypeDef = TypedDict(
     "ListEntitlementsResponseTypeDef",
     {
         "Entitlements": List[ListedEntitlementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewayInstancesResponseTypeDef = TypedDict(
     "ListGatewayInstancesResponseTypeDef",
     {
         "Instances": List[ListedGatewayInstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysResponseTypeDef = TypedDict(
     "ListGatewaysResponseTypeDef",
     {
         "Gateways": List[ListedGatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OfferingTypeDef = TypedDict(
     "OfferingTypeDef",
     {
         "CurrencyCode": str,
@@ -1799,14 +1735,23 @@
     {
         "FlowSource": AddBridgeFlowSourceRequestTypeDef,
         "NetworkSource": AddBridgeNetworkSourceRequestTypeDef,
     },
     total=False,
 )
 
+BridgeSourceTypeDef = TypedDict(
+    "BridgeSourceTypeDef",
+    {
+        "FlowSource": BridgeFlowSourceTypeDef,
+        "NetworkSource": BridgeNetworkSourceTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateBridgeSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeSourceRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "SourceName": str,
     },
 )
@@ -1829,54 +1774,79 @@
     "AddBridgeOutputsRequestRequestTypeDef",
     {
         "BridgeArn": str,
         "Outputs": Sequence[AddBridgeOutputRequestTypeDef],
     },
 )
 
-GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
-    "GrantFlowEntitlementsRequestRequestTypeDef",
+GrantFlowEntitlementsResponseTypeDef = TypedDict(
+    "GrantFlowEntitlementsResponseTypeDef",
     {
-        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
+        "Entitlements": List[EntitlementTypeDef],
         "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BridgeSourceTypeDef = TypedDict(
-    "BridgeSourceTypeDef",
+UpdateFlowEntitlementResponseTypeDef = TypedDict(
+    "UpdateFlowEntitlementResponseTypeDef",
     {
-        "FlowSource": BridgeFlowSourceTypeDef,
-        "NetworkSource": BridgeNetworkSourceTypeDef,
+        "Entitlement": EntitlementTypeDef,
+        "FlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GrantFlowEntitlementsRequestRequestTypeDef = TypedDict(
+    "GrantFlowEntitlementsRequestRequestTypeDef",
+    {
+        "Entitlements": Sequence[GrantEntitlementRequestTypeDef],
+        "FlowArn": str,
     },
-    total=False,
 )
 
 AddBridgeOutputsResponseTypeDef = TypedDict(
     "AddBridgeOutputsResponseTypeDef",
     {
         "BridgeArn": str,
         "Outputs": List[BridgeOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBridgeOutputResponseTypeDef = TypedDict(
     "UpdateBridgeOutputResponseTypeDef",
     {
         "BridgeArn": str,
         "Output": BridgeOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayInstanceResponseTypeDef = TypedDict(
     "DescribeGatewayInstanceResponseTypeDef",
     {
         "GatewayInstance": GatewayInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateGatewayResponseTypeDef = TypedDict(
+    "CreateGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGatewayResponseTypeDef = TypedDict(
+    "DescribeGatewayResponseTypeDef",
+    {
+        "Gateway": GatewayTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMediaStreamOutputConfigurationRequestTypeDef = TypedDict(
     "_RequiredMediaStreamOutputConfigurationRequestTypeDef",
     {
         "EncodingName": EncodingNameType,
@@ -1956,32 +1926,14 @@
 )
 
 class MediaStreamSourceConfigurationTypeDef(
     _RequiredMediaStreamSourceConfigurationTypeDef, _OptionalMediaStreamSourceConfigurationTypeDef
 ):
     pass
 
-GrantFlowEntitlementsResponseTypeDef = TypedDict(
-    "GrantFlowEntitlementsResponseTypeDef",
-    {
-        "Entitlements": List[EntitlementTypeDef],
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFlowEntitlementResponseTypeDef = TypedDict(
-    "UpdateFlowEntitlementResponseTypeDef",
-    {
-        "Entitlement": EntitlementTypeDef,
-        "FlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBridgeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBridgeRequestRequestTypeDef",
     {
         "BridgeArn": str,
     },
 )
 _OptionalUpdateBridgeRequestRequestTypeDef = TypedDict(
@@ -2020,15 +1972,15 @@
     pass
 
 ListFlowsResponseTypeDef = TypedDict(
     "ListFlowsResponseTypeDef",
     {
         "Flows": List[ListedFlowTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddMediaStreamRequestTypeDef = TypedDict(
     "_RequiredAddMediaStreamRequestTypeDef",
     {
         "MediaStreamId": int,
@@ -2096,69 +2048,53 @@
     },
     total=False,
 )
 
 class MediaStreamTypeDef(_RequiredMediaStreamTypeDef, _OptionalMediaStreamTypeDef):
     pass
 
-CreateGatewayResponseTypeDef = TypedDict(
-    "CreateGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeGatewayResponseTypeDef = TypedDict(
-    "DescribeGatewayResponseTypeDef",
-    {
-        "Gateway": GatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeOfferingResponseTypeDef = TypedDict(
     "DescribeOfferingResponseTypeDef",
     {
         "Offering": OfferingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOfferingsResponseTypeDef = TypedDict(
     "ListOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "Offerings": List[OfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReservationResponseTypeDef = TypedDict(
     "DescribeReservationResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReservationsResponseTypeDef = TypedDict(
     "ListReservationsResponseTypeDef",
     {
         "NextToken": str,
         "Reservations": List[ReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseOfferingResponseTypeDef = TypedDict(
     "PurchaseOfferingResponseTypeDef",
     {
         "Reservation": ReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddBridgeSourcesRequestRequestTypeDef = TypedDict(
     "AddBridgeSourcesRequestRequestTypeDef",
     {
         "BridgeArn": str,
@@ -2191,15 +2127,15 @@
     pass
 
 AddBridgeSourcesResponseTypeDef = TypedDict(
     "AddBridgeSourcesResponseTypeDef",
     {
         "BridgeArn": str,
         "Sources": List[BridgeSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBridgeTypeDef = TypedDict(
     "_RequiredBridgeTypeDef",
     {
         "BridgeArn": str,
@@ -2211,29 +2147,29 @@
 _OptionalBridgeTypeDef = TypedDict(
     "_OptionalBridgeTypeDef",
     {
         "BridgeMessages": List[MessageDetailTypeDef],
         "EgressGatewayBridge": EgressGatewayBridgeTypeDef,
         "IngressGatewayBridge": IngressGatewayBridgeTypeDef,
         "Outputs": List[BridgeOutputTypeDef],
-        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
+        "SourceFailoverConfig": FailoverConfigTypeDef,
         "Sources": List[BridgeSourceTypeDef],
     },
     total=False,
 )
 
 class BridgeTypeDef(_RequiredBridgeTypeDef, _OptionalBridgeTypeDef):
     pass
 
 UpdateBridgeSourceResponseTypeDef = TypedDict(
     "UpdateBridgeSourceResponseTypeDef",
     {
         "BridgeArn": str,
         "Source": BridgeSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddOutputRequestTypeDef = TypedDict(
     "_RequiredAddOutputRequestTypeDef",
     {
         "Protocol": ProtocolType,
@@ -2369,22 +2305,22 @@
 )
 _OptionalOutputTypeDef = TypedDict(
     "_OptionalOutputTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
         "Description": str,
         "Destination": str,
-        "Encryption": EncryptionOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
         "EntitlementArn": str,
         "ListenerAddress": str,
         "MediaLiveInputArn": str,
         "MediaStreamOutputConfigurations": List[MediaStreamOutputConfigurationTypeDef],
         "Port": int,
         "Transport": TransportTypeDef,
-        "VpcInterfaceAttachment": VpcInterfaceAttachmentOutputTypeDef,
+        "VpcInterfaceAttachment": VpcInterfaceAttachmentTypeDef,
         "BridgeArn": str,
         "BridgePorts": List[int],
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
@@ -2397,15 +2333,15 @@
         "SourceArn": str,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "DataTransferSubscriberFeePercent": int,
-        "Decryption": EncryptionOutputTypeDef,
+        "Decryption": EncryptionTypeDef,
         "Description": str,
         "EntitlementArn": str,
         "IngestIp": str,
         "IngestPort": int,
         "MediaStreamSourceConfigurations": List[MediaStreamSourceConfigurationTypeDef],
         "SenderControlPort": int,
         "SenderIpAddress": str,
@@ -2429,48 +2365,48 @@
 )
 
 AddFlowMediaStreamsResponseTypeDef = TypedDict(
     "AddFlowMediaStreamsResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowMediaStreamResponseTypeDef = TypedDict(
     "UpdateFlowMediaStreamResponseTypeDef",
     {
         "FlowArn": str,
         "MediaStream": MediaStreamTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBridgeResponseTypeDef = TypedDict(
     "CreateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBridgeResponseTypeDef = TypedDict(
     "DescribeBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBridgeResponseTypeDef = TypedDict(
     "UpdateBridgeResponseTypeDef",
     {
         "Bridge": BridgeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddFlowOutputsRequestRequestTypeDef = TypedDict(
     "AddFlowOutputsRequestRequestTypeDef",
     {
         "FlowArn": str,
@@ -2514,33 +2450,33 @@
     pass
 
 AddFlowOutputsResponseTypeDef = TypedDict(
     "AddFlowOutputsResponseTypeDef",
     {
         "FlowArn": str,
         "Outputs": List[OutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowOutputResponseTypeDef = TypedDict(
     "UpdateFlowOutputResponseTypeDef",
     {
         "FlowArn": str,
         "Output": OutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddFlowSourcesResponseTypeDef = TypedDict(
     "AddFlowSourcesResponseTypeDef",
     {
         "FlowArn": str,
         "Sources": List[SourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFlowTypeDef = TypedDict(
     "_RequiredFlowTypeDef",
     {
         "AvailabilityZone": str,
@@ -2554,15 +2490,15 @@
 )
 _OptionalFlowTypeDef = TypedDict(
     "_OptionalFlowTypeDef",
     {
         "Description": str,
         "EgressIp": str,
         "MediaStreams": List[MediaStreamTypeDef],
-        "SourceFailoverConfig": FailoverConfigOutputTypeDef,
+        "SourceFailoverConfig": FailoverConfigTypeDef,
         "Sources": List[SourceTypeDef],
         "VpcInterfaces": List[VpcInterfaceTypeDef],
         "Maintenance": MaintenanceTypeDef,
     },
     total=False,
 )
 
@@ -2570,35 +2506,35 @@
     pass
 
 UpdateFlowSourceResponseTypeDef = TypedDict(
     "UpdateFlowSourceResponseTypeDef",
     {
         "FlowArn": str,
         "Source": SourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFlowResponseTypeDef = TypedDict(
     "CreateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFlowResponseTypeDef = TypedDict(
     "DescribeFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
         "Messages": MessagesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowResponseTypeDef = TypedDict(
     "UpdateFlowResponseTypeDef",
     {
         "Flow": FlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.py` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect/waiter.pyi` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediaconnect)](https://pepy.tech/project/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,169 +398,164 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconnect.type_defs import (
     VpcInterfaceAttachmentTypeDef,
     AddBridgeNetworkOutputRequestTypeDef,
     AddBridgeNetworkSourceRequestTypeDef,
+    ResponseMetadataTypeDef,
     AddEgressGatewayBridgeRequestTypeDef,
     VpcInterfaceRequestTypeDef,
     VpcInterfaceTypeDef,
     AddIngressGatewayBridgeRequestTypeDef,
     AddMaintenanceTypeDef,
     EncryptionTypeDef,
     BridgeFlowOutputTypeDef,
-    VpcInterfaceAttachmentOutputTypeDef,
     BridgeNetworkOutputTypeDef,
     BridgeNetworkSourceTypeDef,
     EgressGatewayBridgeTypeDef,
     IngressGatewayBridgeTypeDef,
     MessageDetailTypeDef,
     GatewayNetworkTypeDef,
     DeleteBridgeRequestRequestTypeDef,
-    DeleteBridgeResponseTypeDef,
     DeleteFlowRequestRequestTypeDef,
-    DeleteFlowResponseTypeDef,
     DeleteGatewayRequestRequestTypeDef,
-    DeleteGatewayResponseTypeDef,
     DeregisterGatewayInstanceRequestRequestTypeDef,
-    DeregisterGatewayInstanceResponseTypeDef,
     DescribeBridgeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeFlowRequestRequestTypeDef,
     MessagesTypeDef,
     DescribeGatewayInstanceRequestRequestTypeDef,
     DescribeGatewayRequestRequestTypeDef,
     DescribeOfferingRequestRequestTypeDef,
     DescribeReservationRequestRequestTypeDef,
     InterfaceRequestTypeDef,
     InterfaceTypeDef,
-    EmptyResponseMetadataTypeDef,
     EncodingParametersRequestTypeDef,
     EncodingParametersTypeDef,
-    EncryptionOutputTypeDef,
-    SourcePriorityOutputTypeDef,
     SourcePriorityTypeDef,
     MaintenanceTypeDef,
     FmtpRequestTypeDef,
     FmtpTypeDef,
-    GatewayNetworkOutputTypeDef,
-    ListBridgesRequestListBridgesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBridgesRequestRequestTypeDef,
     ListedBridgeTypeDef,
-    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
     ListEntitlementsRequestRequestTypeDef,
     ListedEntitlementTypeDef,
-    ListFlowsRequestListFlowsPaginateTypeDef,
     ListFlowsRequestRequestTypeDef,
-    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
     ListGatewayInstancesRequestRequestTypeDef,
     ListedGatewayInstanceTypeDef,
-    ListGatewaysRequestListGatewaysPaginateTypeDef,
     ListGatewaysRequestRequestTypeDef,
     ListedGatewayTypeDef,
-    ListOfferingsRequestListOfferingsPaginateTypeDef,
     ListOfferingsRequestRequestTypeDef,
-    ListReservationsRequestListReservationsPaginateTypeDef,
     ListReservationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResourceSpecificationTypeDef,
     TransportTypeDef,
-    PaginatorConfigTypeDef,
     PurchaseOfferingRequestRequestTypeDef,
     RemoveBridgeOutputRequestRequestTypeDef,
-    RemoveBridgeOutputResponseTypeDef,
     RemoveBridgeSourceRequestRequestTypeDef,
-    RemoveBridgeSourceResponseTypeDef,
     RemoveFlowMediaStreamRequestRequestTypeDef,
-    RemoveFlowMediaStreamResponseTypeDef,
     RemoveFlowOutputRequestRequestTypeDef,
-    RemoveFlowOutputResponseTypeDef,
     RemoveFlowSourceRequestRequestTypeDef,
-    RemoveFlowSourceResponseTypeDef,
     RemoveFlowVpcInterfaceRequestRequestTypeDef,
-    RemoveFlowVpcInterfaceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RevokeFlowEntitlementRequestRequestTypeDef,
-    RevokeFlowEntitlementResponseTypeDef,
     StartFlowRequestRequestTypeDef,
-    StartFlowResponseTypeDef,
     StopFlowRequestRequestTypeDef,
-    StopFlowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBridgeNetworkOutputRequestTypeDef,
     UpdateBridgeNetworkSourceRequestTypeDef,
     UpdateEgressGatewayBridgeRequestTypeDef,
     UpdateIngressGatewayBridgeRequestTypeDef,
     UpdateBridgeStateRequestRequestTypeDef,
-    UpdateBridgeStateResponseTypeDef,
     UpdateEncryptionTypeDef,
     UpdateMaintenanceTypeDef,
     UpdateGatewayInstanceRequestRequestTypeDef,
-    UpdateGatewayInstanceResponseTypeDef,
     AddBridgeFlowSourceRequestTypeDef,
+    BridgeFlowSourceTypeDef,
+    GatewayBridgeSourceTypeDef,
     SetGatewayBridgeSourceRequestTypeDef,
     UpdateBridgeFlowSourceRequestTypeDef,
     UpdateGatewayBridgeSourceRequestTypeDef,
     AddBridgeOutputRequestTypeDef,
+    DeleteBridgeResponseTypeDef,
+    DeleteFlowResponseTypeDef,
+    DeleteGatewayResponseTypeDef,
+    DeregisterGatewayInstanceResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RemoveBridgeOutputResponseTypeDef,
+    RemoveBridgeSourceResponseTypeDef,
+    RemoveFlowMediaStreamResponseTypeDef,
+    RemoveFlowOutputResponseTypeDef,
+    RemoveFlowSourceResponseTypeDef,
+    RemoveFlowVpcInterfaceResponseTypeDef,
+    RevokeFlowEntitlementResponseTypeDef,
+    StartFlowResponseTypeDef,
+    StopFlowResponseTypeDef,
+    UpdateBridgeStateResponseTypeDef,
+    UpdateGatewayInstanceResponseTypeDef,
     AddFlowVpcInterfacesRequestRequestTypeDef,
     AddFlowVpcInterfacesResponseTypeDef,
+    EntitlementTypeDef,
     GrantEntitlementRequestTypeDef,
-    BridgeFlowSourceTypeDef,
-    GatewayBridgeSourceTypeDef,
     BridgeOutputTypeDef,
     GatewayInstanceTypeDef,
     CreateGatewayRequestRequestTypeDef,
+    GatewayTypeDef,
     DescribeFlowRequestFlowActiveWaitTypeDef,
     DescribeFlowRequestFlowDeletedWaitTypeDef,
     DescribeFlowRequestFlowStandbyWaitTypeDef,
     DestinationConfigurationRequestTypeDef,
     InputConfigurationRequestTypeDef,
     DestinationConfigurationTypeDef,
     InputConfigurationTypeDef,
-    EntitlementTypeDef,
-    FailoverConfigOutputTypeDef,
     FailoverConfigTypeDef,
     UpdateFailoverConfigTypeDef,
     ListedFlowTypeDef,
     MediaStreamAttributesRequestTypeDef,
     MediaStreamAttributesTypeDef,
-    GatewayTypeDef,
+    ListBridgesRequestListBridgesPaginateTypeDef,
+    ListEntitlementsRequestListEntitlementsPaginateTypeDef,
+    ListFlowsRequestListFlowsPaginateTypeDef,
+    ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef,
+    ListGatewaysRequestListGatewaysPaginateTypeDef,
+    ListOfferingsRequestListOfferingsPaginateTypeDef,
+    ListReservationsRequestListReservationsPaginateTypeDef,
     ListBridgesResponseTypeDef,
     ListEntitlementsResponseTypeDef,
     ListGatewayInstancesResponseTypeDef,
     ListGatewaysResponseTypeDef,
     OfferingTypeDef,
     ReservationTypeDef,
     UpdateBridgeOutputRequestRequestTypeDef,
     UpdateFlowEntitlementRequestRequestTypeDef,
     AddBridgeSourceRequestTypeDef,
+    BridgeSourceTypeDef,
     UpdateBridgeSourceRequestRequestTypeDef,
     AddBridgeOutputsRequestRequestTypeDef,
+    GrantFlowEntitlementsResponseTypeDef,
+    UpdateFlowEntitlementResponseTypeDef,
     GrantFlowEntitlementsRequestRequestTypeDef,
-    BridgeSourceTypeDef,
     AddBridgeOutputsResponseTypeDef,
     UpdateBridgeOutputResponseTypeDef,
     DescribeGatewayInstanceResponseTypeDef,
+    CreateGatewayResponseTypeDef,
+    DescribeGatewayResponseTypeDef,
     MediaStreamOutputConfigurationRequestTypeDef,
     MediaStreamSourceConfigurationRequestTypeDef,
     MediaStreamOutputConfigurationTypeDef,
     MediaStreamSourceConfigurationTypeDef,
-    GrantFlowEntitlementsResponseTypeDef,
-    UpdateFlowEntitlementResponseTypeDef,
     UpdateBridgeRequestRequestTypeDef,
     UpdateFlowRequestRequestTypeDef,
     ListFlowsResponseTypeDef,
     AddMediaStreamRequestTypeDef,
     UpdateFlowMediaStreamRequestRequestTypeDef,
     MediaStreamTypeDef,
-    CreateGatewayResponseTypeDef,
-    DescribeGatewayResponseTypeDef,
     DescribeOfferingResponseTypeDef,
     ListOfferingsResponseTypeDef,
     DescribeReservationResponseTypeDef,
     ListReservationsResponseTypeDef,
     PurchaseOfferingResponseTypeDef,
     AddBridgeSourcesRequestRequestTypeDef,
     CreateBridgeRequestRequestTypeDef,
```

### Comparing `mypy-boto3-mediaconnect-1.28.12/mypy_boto3_mediaconnect.egg-info/SOURCES.txt` & `mypy-boto3-mediaconnect-1.28.15/mypy_boto3_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.28.12/setup.py` & `mypy-boto3-mediaconnect-1.28.15/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconnect",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConnect 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MediaConnect 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

