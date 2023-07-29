# Comparing `tmp/bt_data-0.0.1-py3-none-any.whl.zip` & `tmp/bt_data-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,21 @@
-Zip file size: 1577 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 16:28 bt_data/__init__.py
--rw-r--r--  2.0 unx       67 b- defN 23-Jul-12 16:28 bt_data/data.py
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-12 16:28 bt_data-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 16:28 bt_data-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-12 16:28 bt_data-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      439 b- defN 23-Jul-12 16:28 bt_data-0.0.1.dist-info/RECORD
-6 files, 1148 bytes uncompressed, 775 bytes compressed:  32.5%
+Zip file size: 6512 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 16:51 bt_data/__init__.py
+-rw-r--r--  2.0 unx       67 b- defN 23-Jul-29 16:51 bt_data/data.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Jul-29 16:51 bt_data/db/DbAdapter.py
+-rw-r--r--  2.0 unx     2065 b- defN 23-Jul-29 16:51 bt_data/db/PostgresqlAdapter.py
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-29 16:51 bt_data/db/__init__.py
+-rw-r--r--  2.0 unx      103 b- defN 23-Jul-29 16:51 bt_data/enum/SyncType.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 16:51 bt_data/enum/__init__.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-29 16:51 bt_data/model/Df.py
+-rw-r--r--  2.0 unx     3250 b- defN 23-Jul-29 16:51 bt_data/model/Instrument.py
+-rw-r--r--  2.0 unx      426 b- defN 23-Jul-29 16:51 bt_data/model/Model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 16:51 bt_data/model/__init__.py
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-29 16:51 bt_data/model/akshare/AKShareStockInfoACodeName.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 16:51 bt_data/model/akshare/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 16:51 bt_data/test/__init__.py
+-rw-r--r--  2.0 unx      133 b- defN 23-Jul-29 16:51 bt_data/test/test.py
+-rw-r--r--  2.0 unx      656 b- defN 23-Jul-29 16:51 bt_data-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 16:51 bt_data-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-29 16:51 bt_data-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1505 b- defN 23-Jul-29 16:51 bt_data-0.0.2.dist-info/RECORD
+19 files, 9003 bytes uncompressed, 4034 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -1,19 +1,58 @@
 Filename: bt_data/__init__.py
 Comment: 
 
 Filename: bt_data/data.py
 Comment: 
 
-Filename: bt_data-0.0.1.dist-info/METADATA
+Filename: bt_data/db/DbAdapter.py
 Comment: 
 
-Filename: bt_data-0.0.1.dist-info/WHEEL
+Filename: bt_data/db/PostgresqlAdapter.py
 Comment: 
 
-Filename: bt_data-0.0.1.dist-info/top_level.txt
+Filename: bt_data/db/__init__.py
 Comment: 
 
-Filename: bt_data-0.0.1.dist-info/RECORD
+Filename: bt_data/enum/SyncType.py
+Comment: 
+
+Filename: bt_data/enum/__init__.py
+Comment: 
+
+Filename: bt_data/model/Df.py
+Comment: 
+
+Filename: bt_data/model/Instrument.py
+Comment: 
+
+Filename: bt_data/model/Model.py
+Comment: 
+
+Filename: bt_data/model/__init__.py
+Comment: 
+
+Filename: bt_data/model/akshare/AKShareStockInfoACodeName.py
+Comment: 
+
+Filename: bt_data/model/akshare/__init__.py
+Comment: 
+
+Filename: bt_data/test/__init__.py
+Comment: 
+
+Filename: bt_data/test/test.py
+Comment: 
+
+Filename: bt_data-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: bt_data-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: bt_data-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: bt_data-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bt_data-0.0.1.dist-info/METADATA` & `bt_data-0.0.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: bt-data
-Version: 0.0.1
+Version: 0.0.2
 Summary: BotTrader Data Package
 Home-page: https://dev.azure.com/enfuture/BotTrader/_git/bt-data
 Author: heian0224
 Author-email: heian0224@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://dev.azure.com/enfuture/BotTrader/_git/bt-data/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: SQLAlchemy
+Requires-Dist: psycopg2-binary
+Requires-Dist: sqlalchemy2-stubs
+Requires-Dist: sqlmodel
 
 UNKNOWN
```

