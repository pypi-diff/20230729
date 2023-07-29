# Comparing `tmp/mypy-boto3-meteringmarketplace-1.28.15.tar.gz` & `tmp/mypy-boto3-meteringmarketplace-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
+gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:41 2023, max compression
```

## Comparing `mypy-boto3-meteringmarketplace-1.28.15.tar` & `mypy-boto3-meteringmarketplace-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.353516 mypy-boto3-meteringmarketplace-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 20:43:18.349516 mypy-boto3-meteringmarketplace-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.337516 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.349516 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.353516 mypy-boto3-meteringmarketplace-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.793289 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-29 09:51:30.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 10:03:41.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:41.801289 mypy-boto3-meteringmarketplace-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-29 09:51:29.000000 mypy-boto3-meteringmarketplace-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/LICENSE` & `mypy-boto3-meteringmarketplace-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.15
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/README.md` & `mypy-boto3-meteringmarketplace-1.28.15.post1/README.md`

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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__main__.py` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceMetering 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.MarketplaceMetering 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.py` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
+    UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
+    UsageRecordOutputTypeDef,
     UsageRecordTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -73,15 +75,18 @@
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#exceptions)
         """
 
     def batch_meter_usage(
-        self, *, UsageRecords: Sequence[UsageRecordTypeDef], ProductCode: str
+        self,
+        *,
+        UsageRecords: Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
+        ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#batch_meter_usage)
@@ -121,15 +126,17 @@
         self,
         *,
         ProductCode: str,
         Timestamp: Union[datetime, str],
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[UsageAllocationTypeDef] = ...
+        UsageAllocations: Sequence[
+            Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
+        ] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#meter_usage)
         """
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.pyi` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .type_defs import (
     BatchMeterUsageResultTypeDef,
     MeterUsageResultTypeDef,
     RegisterUsageResultTypeDef,
     ResolveCustomerResultTypeDef,
+    UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
+    UsageRecordOutputTypeDef,
     UsageRecordTypeDef,
 )
 
 __all__ = ("MarketplaceMeteringClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -69,15 +71,18 @@
         """
         MarketplaceMeteringClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#exceptions)
         """
     def batch_meter_usage(
-        self, *, UsageRecords: Sequence[UsageRecordTypeDef], ProductCode: str
+        self,
+        *,
+        UsageRecords: Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
+        ProductCode: str
     ) -> BatchMeterUsageResultTypeDef:
         """
         `BatchMeterUsage` is called from a SaaS application listed on AWS Marketplace to
         post metering records for a set of customers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.batch_meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#batch_meter_usage)
@@ -113,15 +118,17 @@
         self,
         *,
         ProductCode: str,
         Timestamp: Union[datetime, str],
         UsageDimension: str,
         UsageQuantity: int = ...,
         DryRun: bool = ...,
-        UsageAllocations: Sequence[UsageAllocationTypeDef] = ...
+        UsageAllocations: Sequence[
+            Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]
+        ] = ...
     ) -> MeterUsageResultTypeDef:
         """
         API to emit metering records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client.meter_usage)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/client/#meter_usage)
         """
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.py` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.pyi` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.py` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     },
 )
 _OptionalMeterUsageRequestRequestTypeDef = TypedDict(
     "_OptionalMeterUsageRequestRequestTypeDef",
     {
         "UsageQuantity": int,
         "DryRun": bool,
-        "UsageAllocations": Sequence[UsageAllocationTypeDef],
+        "UsageAllocations": Sequence[Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]],
     },
     total=False,
 )
 
 
 class MeterUsageRequestRequestTypeDef(
     _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
@@ -236,15 +236,15 @@
     },
     total=False,
 )
 
 BatchMeterUsageRequestRequestTypeDef = TypedDict(
     "BatchMeterUsageRequestRequestTypeDef",
     {
-        "UsageRecords": Sequence[UsageRecordTypeDef],
+        "UsageRecords": Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
         "ProductCode": str,
     },
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.pyi` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     },
 )
 _OptionalMeterUsageRequestRequestTypeDef = TypedDict(
     "_OptionalMeterUsageRequestRequestTypeDef",
     {
         "UsageQuantity": int,
         "DryRun": bool,
-        "UsageAllocations": Sequence[UsageAllocationTypeDef],
+        "UsageAllocations": Sequence[Union[UsageAllocationTypeDef, UsageAllocationOutputTypeDef]],
     },
     total=False,
 )
 
 class MeterUsageRequestRequestTypeDef(
     _RequiredMeterUsageRequestRequestTypeDef, _OptionalMeterUsageRequestRequestTypeDef
 ):
@@ -223,15 +223,15 @@
     },
     total=False,
 )
 
 BatchMeterUsageRequestRequestTypeDef = TypedDict(
     "BatchMeterUsageRequestRequestTypeDef",
     {
-        "UsageRecords": Sequence[UsageRecordTypeDef],
+        "UsageRecords": Sequence[Union[UsageRecordTypeDef, UsageRecordOutputTypeDef]],
         "ProductCode": str,
     },
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.15
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt` & `mypy-boto3-meteringmarketplace-1.28.15.post1/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.15/setup.py` & `mypy-boto3-meteringmarketplace-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-meteringmarketplace",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with"
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

