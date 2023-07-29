# Comparing `tmp/pgsqlx-generator-1.7.0.tar.gz` & `tmp/pgsqlx-generator-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-generator-1.7.0.tar", last modified: Fri Jul 28 02:53:37 2023, max compression
+gzip compressed data, was "dist\pgsqlx-generator-1.7.1.tar", last modified: Sat Jul 29 08:49:35 2023, max compression
```

## Comparing `pgsqlx-generator-1.7.0.tar` & `pgsqlx-generator-1.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx/
--rw-rw-rw-   0        0        0     6450 2023-07-28 02:01:22.000000 pgsqlx-generator-1.7.0/pgsqlx/generator.py
--rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.7.0/pgsqlx/generator.tpl
--rw-rw-rw-   0        0        0      511 2023-07-28 02:01:22.000000 pgsqlx-generator-1.7.0/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2868 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2868 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.7.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-28 02:53:37.000000 pgsqlx-generator-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-07-28 02:53:31.000000 pgsqlx-generator-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx/
+-rw-rw-rw-   0        0        0     7649 2023-07-29 03:22:49.000000 pgsqlx-generator-1.7.1/pgsqlx/generator.py
+-rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.7.1/pgsqlx/generator.tpl
+-rw-rw-rw-   0        0        0     1505 2023-07-29 08:25:34.000000 pgsqlx-generator-1.7.1/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2868 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2868 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.7.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:49:35.000000 pgsqlx-generator-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-07-29 08:48:18.000000 pgsqlx-generator-1.7.1/setup.py
```

### Comparing `pgsqlx-generator-1.7.0/pgsqlx/generator.py` & `pgsqlx-generator-1.7.1/pgsqlx/generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,35 +14,63 @@
     comma2 = '，'
     sql = '''SELECT column_name as "COLUMN_NAME", udt_name as "DATA_TYPE", column_default 
              FROM information_schema.columns WHERE table_schema='public' AND table_name = ?'''
     key_sql = '''SELECT a.attname FROM pg_index i
                  JOIN pg_attribute a ON a.attrelid = i.indrelid AND a.attnum = any(i.indkey)
                  WHERE i.indrelid = ?::regclass AND i.indisprimary LIMIT 1'''
 
-    def __init__(self, pool_size=0, **kwargs):
+    def __init__(self, *args, **kwargs):
+        """
+        Compliant with the Python DB API 2.0 (PEP-249).
+
+        from pgsqlx.generator import Generator
+        coder = Generator("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2')
+        or
+        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
+
+        Addition parameters:
+        :param driver: str, import driver, 'import pymysql'
+        :param pool_size: int, size of connection pool
+        :param show_sql: bool, if True, print sql
+        :param debug: bool, if True, print debug context
+
+        Other parameters of connection pool refer to DBUtils: https://webwareforpython.github.io/DBUtils/main.html#pooleddb-pooled-db
+        """
+
         PostgresEngine.init()
-        init_db(pool_size=pool_size, **kwargs)
+        init_db(*args, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
+        """
+        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
+        coder.generate_with_schema('testdb', 'models.py')
+        """
+
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
         self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
 
     def generate_with_tables(self, tables: Union[str, Iterable[str]], path: str = None, *args, **kwargs):
+        """
+        coder = Generator(user='root', password='xxx', host='127.0.0.1', port=3306, database='testdb', driver='pymysql')
+        coder.generate_with_tables(['user', 'person'], 'models.py')
+        """
+
         metas = None
         only_one_table = False
         if not args:
             args = COMMON_COLS
         if not kwargs:
             kwargs = ATTRIBUTES
 
         columns = [v for v in kwargs.values()]
         if args:
+            args = list(args)
             args.reverse()
             for i in range(0, len(args)):
                 columns.insert(1, args[i])
 
             # 去重
             base_columns = list(set(columns))
             # 保持原有顺序
```

### Comparing `pgsqlx-generator-1.7.0/pgsqlx/generator.tpl` & `pgsqlx-generator-1.7.1/pgsqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.7.0/pgsqlx_generator.egg-info/PKG-INFO` & `pgsqlx-generator-1.7.1/pgsqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.7.0
+Version: 1.7.1
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.7.0/PKG-INFO` & `pgsqlx-generator-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.7.0
+Version: 1.7.1
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.7.0/README.rst` & `pgsqlx-generator-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.7.0/setup.py` & `pgsqlx-generator-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 setup(
     name='pgsqlx-generator',
     packages=['pgsqlx'],
     description="pgsqlx-generator is a model code generator from tables for PgSqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'pgsqlx>=1.6.9',
+        'pgsqlx>=1.7.0',
     ],
-    version='1.7.0',
+    version='1.7.1',
     url='https://gitee.com/summry/pgsqlx/blob/master/generator.md',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['PostgreSQL', 'PgSqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

