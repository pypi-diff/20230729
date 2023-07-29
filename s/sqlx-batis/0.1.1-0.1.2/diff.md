# Comparing `tmp/sqlx-batis-0.1.1.tar.gz` & `tmp/sqlx-batis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.1.tar", last modified: Fri Jul 28 02:50:40 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.2.tar", last modified: Sat Jul 29 08:11:08 2023, max compression
```

## Comparing `sqlx-batis-0.1.1.tar` & `sqlx-batis-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/
--rw-rw-rw-   0        0        0     3373 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-28 02:50:31.000000 sqlx-batis-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlbatis/
--rw-rw-rw-   0        0        0      834 2023-07-26 14:53:18.000000 sqlx-batis-0.1.1/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.1/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.1/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     4411 2023-07-28 02:00:07.000000 sqlx-batis-0.1.1/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.1/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.1/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.1/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.1/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.1/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.1/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.1/sqlbatis/support.py
--rw-rw-rw-   0        0        0      606 2023-07-28 01:56:21.000000 sqlx-batis-0.1.1/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3373 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 02:50:40.000000 sqlx-batis-0.1.1/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/
+-rw-rw-rw-   0        0        0     3373 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-29 08:10:36.000000 sqlx-batis-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.2/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.2/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.2/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     5051 2023-07-29 07:30:33.000000 sqlx-batis-0.1.2/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.2/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.2/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.2/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.2/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.2/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.2/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.2/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1631 2023-07-29 06:24:56.000000 sqlx-batis-0.1.2/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3373 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.1/PKG-INFO` & `sqlx-batis-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.1
+Version: 0.1.2
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.1.1/README.rst` & `sqlx-batis-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/setup.py` & `sqlx-batis-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.2.5',
+        'sqlx-exec>=1.2.9',
     ],
-    version='0.1.1',
+    version='0.1.2',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.1/sqlbatis/constant.py` & `sqlx-batis-0.1.2/sqlbatis/constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from sqlexec.constant import MYSQL, POSTGRESQL
+from sqlexec.constant import MYSQL, POSTGRESQL, SQLITE
 
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 CACHE_SIZE = 256
 
 MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
 
+SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
+
 MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
                         FROM information_schema.columns WHERE table_schema = (SELECT DATABASE()) AND table_name = ? LIMIT ?'''
 
 POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
                           WHERE table_schema='public' and table_name = ? LIMIT ?'''
 
 DYNAMIC_REGEX = '{%|{{|}}|%}'
```

### Comparing `sqlx-batis-0.1.1/sqlbatis/db.py` & `sqlx-batis-0.1.2/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/dbx.py` & `sqlx-batis-0.1.2/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/engine.py` & `sqlx-batis-0.1.2/sqlbatis/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 import re
-from sqlexec import get
 from typing import Sequence
 from .support import DBError
+from sqlexec import get, query
 from functools import lru_cache
 from .log_support import logger
 from sqlexec.engine import Engine as BaseEngine
 from .sql_support import require_limit, get_page_start
-from .constant import MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL, MYSQL_SELECT_KEY, LIMIT_1, MYSQL, POSTGRESQL, DEFAULT_KEY_FIELD, CACHE_SIZE
+from .constant import MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL, MYSQL_SELECT_KEY, LIMIT_1, MYSQL, POSTGRESQL, DEFAULT_KEY_FIELD, CACHE_SIZE, SQLITE, \
+    SQLITE_SELECT_KEY
 
 
 # Engin = Enum('Engin', ['MYSQL', 'POSTGRESQL', 'OTHER'])
 # class Engin(Enum):
 #     MYSQL = 'MySQL'
 #     POSTGRESQL = 'PostgreSQL'
 #     OTHER = 'Other'
 
 
 class Engine(BaseEngine):
-    def __init__(self, name=None):
-        super().__init__(name)
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_page_sql_args(sql, page_num, page_size, *args)
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_page_sql_args(sql, page_num, page_size, *args)
+        elif Engine.current_engine() == SQLITE:
+            return SQLiteEngine.get_page_sql_args(sql, page_num, page_size, *args)
         raise NotImplementedError(f"Not implement method 'get_page_sql_args' for {Engine.current_engine()}.")
 
     @staticmethod
     def get_select_key(*args, **kwargs):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_select_key()
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_select_key(*args, **kwargs)
+        elif Engine.current_engine() == SQLITE:
+            return SQLiteEngine.get_select_key()
         raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}.")
 
     @staticmethod
     def get_table_columns(table: str):
         if Engine.current_engine() == MYSQL:
             return MySqlEngine.get_table_columns(table)
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_table_columns(table)
+        elif Engine.current_engine() == SQLITE:
+            return SQLiteEngine.get_table_columns(table)
         raise "*"
 
 
-
 class MySqlEngine(Engine):
-    def __init__(self, engin):
-        super().__init__(engin)
-
-    @classmethod
-    def init(cls, name=MYSQL):
-        super().init(name)
-
     @staticmethod
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
         return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
@@ -72,21 +69,14 @@
         return get(MYSQL_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key():
         return MYSQL_SELECT_KEY
 
 class PostgresEngine(Engine):
-    def __init__(self, engin):
-        super().__init__(engin)
-
-    @classmethod
-    def init(cls, name=POSTGRESQL):
-        super().init(name)
-
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
         start = get_page_start(page_num, page_size)
         if require_limit(sql):
             sql = '{} LIMIT ? OFFSET ?'.format(sql)
         args = [*args, page_size, start]
         return sql, args
@@ -116,7 +106,25 @@
     @staticmethod
     @lru_cache(maxsize=CACHE_SIZE)
     def _get_key_seq_from_sql(sql: str):
         table = re.search('(?<=into )\w+', sql, re.I)
         key_seq = PostgresEngine.build_key_seq(table.group())
         logger.warning("'key_seq' is None, will use default '{}' from sql.".format(key_seq))
         return key_seq
+
+
+class SQLiteEngine(PostgresEngine):
+    @staticmethod
+    def get_table_columns(table: str):
+        results = query(f'PRAGMA table_info({table})')
+        return ','.join([result['name'] for result in results])
+
+    @staticmethod
+    def get_select_key():
+        return SQLITE_SELECT_KEY
+
+    def before_execute(self, function: str, sql: str, *args):
+        if self.show_sql:
+            logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+        if '%' in sql and 'like' in sql.lower():
+            sql = sql.replace('%', '%%').replace('%%%%', '%%')
+        return sql
```

### Comparing `sqlx-batis-0.1.1/sqlbatis/log_support.py` & `sqlx-batis-0.1.2/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/orm.py` & `sqlx-batis-0.1.2/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/snowflake.py` & `sqlx-batis-0.1.2/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.2/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.2/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlbatis/sql_support.py` & `sqlx-batis-0.1.2/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.1/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.2/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.1
+Version: 0.1.2
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

