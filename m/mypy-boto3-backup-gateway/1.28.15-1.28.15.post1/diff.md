# Comparing `tmp/mypy-boto3-backup-gateway-1.28.15.tar.gz` & `tmp/mypy-boto3-backup-gateway-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-gateway-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-gateway-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:34 2023, max compression
```

## Comparing `mypy-boto3-backup-gateway-1.28.15.tar` & `mypy-boto3-backup-gateway-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.340696 mypy-boto3-backup-gateway-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-28 20:42:19.332697 mypy-boto3-backup-gateway-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.332697 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-28 20:20:07.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-28 20:20:07.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-07-28 20:20:07.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20338 2023-07-28 20:20:07.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:06.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.332697 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:19.000000 mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.340696 mypy-boto3-backup-gateway-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:20:05.000000 mypy-boto3-backup-gateway-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.749022 mypy-boto3-backup-gateway-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20415 2023-07-29 09:38:59.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:34.745022 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 10:02:34.000000 mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:34.749022 mypy-boto3-backup-gateway-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-29 09:38:58.000000 mypy-boto3-backup-gateway-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/LICENSE` & `mypy-boto3-backup-gateway-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.28.15
-Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/README.md` & `mypy-boto3-backup-gateway-1.28.15.post1/README.md`

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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__init__.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__init__.pyi` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/__main__.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupGateway 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.BackupGateway 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/client.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,22 @@
     from mypy_boto3_backup_gateway.client import BackupGatewayClient
 
     session = Session()
     client: BackupGatewayClient = session.client("backup-gateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
@@ -276,15 +277,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#list_virtual_machines)
         """
 
     def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
+        BandwidthRateLimitIntervals: Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/client.pyi` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,22 @@
     from mypy_boto3_backup_gateway.client import BackupGatewayClient
 
     session = Session()
     client: BackupGatewayClient = session.client("backup-gateway")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
@@ -253,15 +254,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#list_virtual_machines)
         """
     def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
+        BandwidthRateLimitIntervals: Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/literals.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/literals.pyi` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/paginator.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/paginator.pyi` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/type_defs.py` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
     data: AssociateGatewayToServerInputRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -617,15 +617,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
         "GatewayArn": str,
     },
 )
 
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway/type_defs.pyi` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
     data: AssociateGatewayToServerInputRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -602,15 +602,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": Sequence[
+            Union[BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef]
+        ],
         "GatewayArn": str,
     },
 )
 
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.28.15
-Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
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
 [mypy-boto3-backup-gateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-backup-gateway-1.28.15/mypy_boto3_backup_gateway.egg-info/SOURCES.txt` & `mypy-boto3-backup-gateway-1.28.15.post1/mypy_boto3_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.28.15/setup.py` & `mypy-boto3-backup-gateway-1.28.15.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup-gateway",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.BackupGateway 1.28.15 service generated with mypy-boto3-builder"
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

