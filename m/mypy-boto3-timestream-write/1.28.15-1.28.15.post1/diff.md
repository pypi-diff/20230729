# Comparing `tmp/mypy-boto3-timestream-write-1.28.15.tar.gz` & `tmp/mypy-boto3-timestream-write-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:22 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.28.15.tar` & `mypy-boto3-timestream-write-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.249994 mypy-boto3-timestream-write-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-28 20:43:53.245994 mypy-boto3-timestream-write-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.229994 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-28 20:40:39.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-28 20:40:39.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.245994 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:53.000000 mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:53.249994 mypy-boto3-timestream-write-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:40:38.000000 mypy-boto3-timestream-write-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23667 2023-07-29 10:00:51.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:04:22.000000 mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:22.309444 mypy-boto3-timestream-write-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-29 10:00:50.000000 mypy-boto3-timestream-write-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.28.15/LICENSE` & `mypy-boto3-timestream-write-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/PKG-INFO` & `mypy-boto3-timestream-write-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.15
-Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-write-1.28.15/README.md` & `mypy-boto3-timestream-write-1.28.15.post1/README.md`

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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/__main__.py` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamWrite 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.TimestreamWrite 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
 
     session = Session()
     client: TimestreamWriteClient = session.client("timestream-write")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -33,14 +34,15 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
@@ -105,15 +107,17 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
+        DataModelConfiguration: Union[
+            DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+        ] = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_batch_load_task)
@@ -133,15 +137,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -289,15 +293,15 @@
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,24 @@
     from boto3.session import Session
     from mypy_boto3_timestream_write.client import TimestreamWriteClient
 
     session = Session()
     client: TimestreamWriteClient = session.client("timestream-write")
     ```
 """
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -33,14 +34,15 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
@@ -99,15 +101,17 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
+        DataModelConfiguration: Union[
+            DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+        ] = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_batch_load_task)
@@ -125,15 +129,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -265,15 +269,15 @@
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: Union[SchemaTypeDef, SchemaOutputTypeDef] = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.28.15
-Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.TimestreamWrite 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
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
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-timestream-write-1.28.15/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.28.15.post1/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.28.15/setup.py` & `mypy-boto3-timestream-write-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.TimestreamWrite 1.28.15 service generated with"
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

