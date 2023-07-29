# Comparing `tmp/sqlx-exec-1.2.6.tar.gz` & `tmp/sqlx-exec-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.6.tar", last modified: Fri Jul 28 03:10:34 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.8.tar", last modified: Sat Jul 29 03:34:26 2023, max compression
```

## Comparing `sqlx-exec-1.2.6.tar` & `sqlx-exec-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     2737 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2023-07-28 01:49:35.000000 sqlx-exec-1.2.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-28 03:10:31.000000 sqlx-exec-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlexec/
--rw-rw-rw-   0        0        0      350 2023-07-27 11:09:15.000000 sqlx-exec-1.2.6/sqlexec/constant.py
--rw-rw-rw-   0        0        0     1461 2023-07-28 01:52:46.000000 sqlx-exec-1.2.6/sqlexec/engine.py
--rw-rw-rw-   0        0        0    10215 2023-07-28 01:52:28.000000 sqlx-exec-1.2.6/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.6/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.6/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.6/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.6/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.6/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.6/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 03:09:51.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2737 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 03:10:34.000000 sqlx-exec-1.2.6/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0     2734 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.2.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-29 03:32:42.000000 sqlx-exec-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlexec/
+-rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.2.8/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     1461 2023-07-28 01:52:46.000000 sqlx-exec-1.2.8/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11333 2023-07-29 02:44:36.000000 sqlx-exec-1.2.8/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.8/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.8/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.2.8/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.8/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.8/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.8/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2734 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.6/LICENSE` & `sqlx-exec-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/PKG-INFO` & `sqlx-exec-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.6
+Version: 1.2.8
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.2.6/README.rst` & `sqlx-exec-1.2.8/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

### Comparing `sqlx-exec-1.2.6/setup.py` & `sqlx-exec-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.6',
+    version='1.2.8',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.2.6/sqlexec/engine.py` & `sqlx-exec-1.2.8/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/sqlexec/exec.py` & `sqlx-exec-1.2.8/sqlexec/exec.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,36 +6,59 @@
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
 _SHOW_SQL = False
 
 
-def init_db(driver='', pool_size=0, show_sql=False, debug=False, **kwargs):
+def init_db(*args, **kwargs):
+    """
+    Compliant with the Python DB API 2.0 (PEP-249).
+
+    from sqlexec import init_db
+    init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+    or
+    init_db(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
+
+    Addition parameters:
+    :param driver: str, import driver, 'import pymysql'
+    :param pool_size: int, size of connection pool
+    :param show_sql: bool, if True, print sql
+    :param debug: bool, if True, print debug context
+
+    Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
+    """
+
     global _DB_CTX, _SHOW_SQL
-    if debug:
+    driver = kwargs.pop('driver') if 'driver' in kwargs else None
+    pool_size = kwargs.pop('pool_size') if 'pool_size' in kwargs else 0
+    if 'show_sql' in kwargs:
+        _SHOW_SQL = kwargs.pop('show_sql')
+    if 'debug' in kwargs and kwargs.pop('debug'):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     prepared = MYSQL_CONNECTOR == driver
     engine, driver, creator = import_driver(driver)
-    if pool_size <= 0:
-        connect = lambda: creator.connect(**kwargs)
-    elif prepared:
+
+    pool_args = ['mincached', 'maxcached', 'maxshared', 'maxconnections', 'blocking', 'maxusage', 'setsession', 'reset', 'failures', 'ping']
+    pool_kwargs = {key: kwargs.pop(key) for key in pool_args if key in kwargs}
+
+    if prepared:
         # mysql.connector 用自带连接池
         kwargs['pool_size'] = pool_size
-        connect = lambda: creator.connect(**kwargs)
-    else:
+    connect = lambda: creator.connect(*args, **kwargs)
+
+    if pool_size >= 1 and not prepared:
         from .pooling import pooled_connect
-        connect = pooled_connect(creator, pool_size, **kwargs)
+        connect = pooled_connect(connect, pool_size, **pool_kwargs)
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-        _SHOW_SQL = show_sql
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
     Engine.init(engine)
     if pool_size > 0:
         logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
         logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
```

### Comparing `sqlx-exec-1.2.6/sqlexec/init_import.py` & `sqlx-exec-1.2.8/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/sqlexec/log_support.py` & `sqlx-exec-1.2.8/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/sqlexec/sql_support.py` & `sqlx-exec-1.2.8/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/sqlexec/support.py` & `sqlx-exec-1.2.8/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.6/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.8/sqlx_exec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.6
+Version: 1.2.8
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 ''''''''''''
 
 .. code:: python
 
    import sqlexec
 
    if __name__ == '__main__':
-       sqlexec.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
+       sqlexec.init_db(host='127.0.0.1', port='3306', user='xxx', password='xxx', database='test', show_sql=True, driver='pymysql')
 
        # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
```

