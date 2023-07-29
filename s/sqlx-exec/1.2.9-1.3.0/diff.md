# Comparing `tmp/sqlx-exec-1.2.9.tar.gz` & `tmp/sqlx-exec-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.9.tar", last modified: Sat Jul 29 07:49:14 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.3.0.tar", last modified: Sat Jul 29 08:44:50 2023, max compression
```

## Comparing `sqlx-exec-1.2.9.tar` & `sqlx-exec-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.9/LICENSE
--rw-rw-rw-   0        0        0     2759 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.2.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-29 07:49:09.000000 sqlx-exec-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlexec/
--rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.2.9/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2551 2023-07-29 07:25:18.000000 sqlx-exec-1.2.9/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11488 2023-07-29 07:44:50.000000 sqlx-exec-1.2.9/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.9/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.9/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.2.9/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.9/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.9/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.9/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2759 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2759 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.3.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-29 08:44:45.000000 sqlx-exec-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlexec/
+-rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.3.0/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2551 2023-07-29 07:25:18.000000 sqlx-exec-1.3.0/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11488 2023-07-29 07:44:50.000000 sqlx-exec-1.3.0/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1308 2023-07-29 08:32:47.000000 sqlx-exec-1.3.0/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.3.0/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.3.0/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.3.0/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.3.0/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.3.0/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2759 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 08:44:50.000000 sqlx-exec-1.3.0/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.9/LICENSE` & `sqlx-exec-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/PKG-INFO` & `sqlx-exec-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.9
+Version: 1.3.0
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.2.9/README.rst` & `sqlx-exec-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/setup.py` & `sqlx-exec-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.9',
+    version='1.3.0',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.2.9/sqlexec/engine.py` & `sqlx-exec-1.3.0/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlexec/exec.py` & `sqlx-exec-1.3.0/sqlexec/exec.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlexec/init_import.py` & `sqlx-exec-1.3.0/sqlexec/init_import.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from .support import DBError
 from .log_support import logger
 from .constant import DRIVERS, UNKNOW
 
 
 def import_driver(driver):
     creator = None
+    curr_engine = Engine.current_engine()
     if driver:
         if driver not in DRIVERS:
             logger.warning(f"Driver '{driver}' not support now, may be you should adapte it youself.")
         engine = DRIVERS.get(driver)
         creator = do_import(driver, engine)
+        engine = engine if engine else curr_engine
     else:
-        curr_engine = Engine.current_engine()
         drivers = dict(filter(lambda x: x[1] == curr_engine, DRIVERS.items())) if curr_engine and curr_engine != UNKNOW else DRIVERS
         for driver, engine in drivers.items():
             try:
                 creator = importlib.import_module(driver)
                 break
             except ModuleNotFoundError:
                 pass
```

### Comparing `sqlx-exec-1.2.9/sqlexec/log_support.py` & `sqlx-exec-1.3.0/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlexec/pooling.py` & `sqlx-exec-1.3.0/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlexec/sql_support.py` & `sqlx-exec-1.3.0/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlexec/support.py` & `sqlx-exec-1.3.0/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.9/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.3.0/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.9
+Version: 1.3.0
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
```

