# Comparing `tmp/sqlx-exec-1.2.8.tar.gz` & `tmp/sqlx-exec-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.2.8.tar", last modified: Sat Jul 29 03:34:26 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.9.tar", last modified: Sat Jul 29 07:49:14 2023, max compression
```

## Comparing `sqlx-exec-1.2.8.tar` & `sqlx-exec-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     2734 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.2.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-29 03:32:42.000000 sqlx-exec-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlexec/
--rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.2.8/sqlexec/constant.py
--rw-rw-rw-   0        0        0     1461 2023-07-28 01:52:46.000000 sqlx-exec-1.2.8/sqlexec/engine.py
--rw-rw-rw-   0        0        0    11333 2023-07-29 02:44:36.000000 sqlx-exec-1.2.8/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.8/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.8/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.2.8/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.8/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.8/sqlexec/support.py
--rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.8/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2734 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 03:34:26.000000 sqlx-exec-1.2.8/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     2759 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2226 2023-07-29 03:34:20.000000 sqlx-exec-1.2.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-07-29 07:49:09.000000 sqlx-exec-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlexec/
+-rw-rw-rw-   0        0        0      489 2023-07-29 03:31:34.000000 sqlx-exec-1.2.9/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2551 2023-07-29 07:25:18.000000 sqlx-exec-1.2.9/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    11488 2023-07-29 07:44:50.000000 sqlx-exec-1.2.9/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     1260 2023-07-28 01:52:28.000000 sqlx-exec-1.2.9/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.9/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.2.9/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1138 2023-07-28 01:49:35.000000 sqlx-exec-1.2.9/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.9/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.9/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2759 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 07:49:14.000000 sqlx-exec-1.2.9/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.2.8/LICENSE` & `sqlx-exec-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/PKG-INFO` & `sqlx-exec-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.8
+Version: 1.2.9
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: sql,MySQL,PostgreSQL,python
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
```

### Comparing `sqlx-exec-1.2.8/README.rst` & `sqlx-exec-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/setup.py` & `sqlx-exec-1.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.8',
+    version='1.2.9',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
-    keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
+    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
     include_package_data=True,
     python_requires='>=3.5',
     zip_safe=False
```

### Comparing `sqlx-exec-1.2.8/sqlexec/engine.py` & `sqlx-exec-1.2.9/sqlexec/engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 from typing import Sequence
 from functools import lru_cache
+from .log_support import logger
 from .constant import CACHE_SIZE, UNKNOW
 
 _ENGINE = None
 
 
 class Engine:
-    def __init__(self, name=UNKNOW):
+    def __init__(self, name, transform_placeholder, show_sql = False):
         self.name = name
+        self.show_sql = show_sql
+        self.transform_placeholder = transform_placeholder
 
     @classmethod
-    def init(cls, name=UNKNOW):
+    def init(cls, name=UNKNOW, transform_placeholder=None):
+        cls.init0(name, transform_placeholder, show_sql=False)
+
+    @classmethod
+    def init0(cls, name, transform_placeholder, show_sql):
         global _ENGINE
         if _ENGINE:
-            if _ENGINE.name == UNKNOW and name != UNKNOW:
+            _ENGINE.show_sql = show_sql
+            if _ENGINE.name is None or _ENGINE.name == UNKNOW:
                 _ENGINE.name = name
+            if _ENGINE.transform_placeholder is None:
+                _ENGINE.transform_placeholder = transform_placeholder
         else:
-            _ENGINE = cls(name)
+            _ENGINE = cls(name, transform_placeholder, show_sql)
 
     @staticmethod
     def current_engine():
         global _ENGINE
         if _ENGINE:
             return _ENGINE.name
         return None
@@ -39,10 +49,23 @@
         return _ENGINE.get_select_key(*args, **kwargs)
 
     @staticmethod
     def get_table_columns_intf(table: str):
         return _ENGINE.get_table_columns(table)
 
     @staticmethod
+    def before_execute_intf(function: str, sql: str, *args):
+        return _ENGINE.before_execute(function, sql, *args)
+
+    @staticmethod
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('{}'.format(col), '?') for col in cols])
         return 'INSERT INTO {}({}) VALUES({})'.format(table, ', '.join(columns), ','.join(placeholders))
+
+    def before_execute(self, function: str, sql: str, *args):
+        if self.show_sql:
+            logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+        if '%' in sql and 'like' in sql.lower():
+            sql = sql.replace('%', '%%').replace('%%%%', '%%')
+        if self.transform_placeholder:
+            sql = sql.replace('?', '%s')
+        return sql
```

### Comparing `sqlx-exec-1.2.8/sqlexec/exec.py` & `sqlx-exec-1.2.9/sqlexec/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 import functools
 from . import sql_support
 from .engine import Engine
-from .constant import MYSQL_CONNECTOR
 from .init_import import import_driver
+from .constant import MYSQL_CONNECTOR, SQLITE
 from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
-_SHOW_SQL = False
 
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
 
-    from sqlexec import init_db
-    init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+    from sqlexec
+    sqlexec.init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
     or
-    init_db(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
+    sqlexec.init_db("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+    or
+    sqlexec.init_db(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql', pool_size=5, show_sql=True, debug=True)
 
     Addition parameters:
-    :param driver: str, import driver, 'import pymysql'
-    :param pool_size: int, size of connection pool
-    :param show_sql: bool, if True, print sql
-    :param debug: bool, if True, print debug context
+    :param driver=None: str, import driver, 'import pymysql'
+    :param pool_size=0: int, default 0, size of connection pool
+    :param show_sql=False: bool,  if True, print sql
+    :param debug=False: bool, if True, print debug context
+    :param transform_placeholder=True: bool, if True, sql placeholder '?' --> '%s'
 
     Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
     """
 
-    global _DB_CTX, _SHOW_SQL
+    global _DB_CTX
     driver = kwargs.pop('driver') if 'driver' in kwargs else None
     pool_size = kwargs.pop('pool_size') if 'pool_size' in kwargs else 0
-    if 'show_sql' in kwargs:
-        _SHOW_SQL = kwargs.pop('show_sql')
+    show_sql = kwargs.pop('show_sql') if 'show_sql' in kwargs else False
+    transform_placeholder = kwargs.pop('transform_placeholder') if 'transform_placeholder' in kwargs else True
+
     if 'debug' in kwargs and kwargs.pop('debug'):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
-    prepared = MYSQL_CONNECTOR == driver
     engine, driver, creator = import_driver(driver)
+    prepared = MYSQL_CONNECTOR == driver
 
     pool_args = ['mincached', 'maxcached', 'maxshared', 'maxconnections', 'blocking', 'maxusage', 'setsession', 'reset', 'failures', 'ping']
     pool_kwargs = {key: kwargs.pop(key) for key in pool_args if key in kwargs}
 
     if prepared:
         # mysql.connector 用自带连接池
         kwargs['pool_size'] = pool_size
@@ -53,15 +56,17 @@
         connect = pooled_connect(connect, pool_size, **pool_kwargs)
 
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
-    Engine.init(engine)
+    if SQLITE == engine:
+        transform_placeholder = False
+    Engine.init0(engine, transform_placeholder, show_sql)
     if pool_size > 0:
         logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
         logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
 
 
 def connection():
@@ -125,15 +130,15 @@
 def execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('execute', sql.strip(), *args)
+    sql = Engine.before_execute_intf('execute', sql.strip(), *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
@@ -174,15 +179,15 @@
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s" % ('save_sql', select_key, sql, args))
-    sql = _before_execute('save_sql', sql, *args)
+    sql = Engine.before_execute_intf('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(select_key)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -212,15 +217,15 @@
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
     if isinstance(args[0], dict):
         sql, args = sql_support.batch_named_sql_args(sql, *args)
-    sql = _before_execute('batch_execute', sql.strip(), *args)
+    sql = Engine.before_execute_intf('batch_execute', sql.strip(), *args)
     args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
@@ -250,15 +255,15 @@
 def select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('select', sql.strip(), *args)
+    sql = Engine.before_execute_intf('select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
@@ -268,15 +273,15 @@
 def select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('select_one', sql.strip(), *args)
+    sql = Engine.before_execute_intf('select_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
@@ -292,15 +297,15 @@
 def query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('query', sql.strip(), *args)
+    sql = Engine.before_execute_intf('query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in results]
@@ -315,15 +320,15 @@
 def query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = _before_execute('query_one', sql.strip(), *args)
+    sql = Engine.before_execute_intf('query_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
@@ -339,15 +344,7 @@
 #     return query(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
     _DB_CTX.try_init()
     return _DB_CTX.connection
-
-
-def _before_execute(function: str, sql: str, *args):
-    if _SHOW_SQL:
-        logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
-    if '%' in sql and 'like' in sql.lower():
-        sql = sql.replace('%', '%%').replace('%%%%', '%%')
-    return sql.replace('?', '%s')
```

### Comparing `sqlx-exec-1.2.8/sqlexec/init_import.py` & `sqlx-exec-1.2.9/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/sqlexec/log_support.py` & `sqlx-exec-1.2.9/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/sqlexec/pooling.py` & `sqlx-exec-1.2.9/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/sqlexec/sql_support.py` & `sqlx-exec-1.2.9/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/sqlexec/support.py` & `sqlx-exec-1.2.9/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.2.8/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.9/sqlx_exec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.2.8
+Version: 1.2.9
 Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
-Keywords: sql,MySQL,PostgreSQL,python
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Usage Sample
 ''''''''''''
```

