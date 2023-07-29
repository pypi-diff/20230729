# Comparing `tmp/nsj_sql_utils_lib-0.0.3.tar.gz` & `tmp/nsj_sql_utils_lib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_sql_utils_lib-0.0.3.tar", last modified: Sat Jul 29 20:19:30 2023, max compression
+gzip compressed data, was "nsj_sql_utils_lib-0.0.4.tar", last modified: Sat Jul 29 21:23:00 2023, max compression
```

## Comparing `nsj_sql_utils_lib-0.0.3.tar` & `nsj_sql_utils_lib-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 20:19:29.999218 nsj_sql_utils_lib-0.0.3/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1215 2023-07-29 20:19:29.999218 nsj_sql_utils_lib-0.0.3/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      594 2023-07-22 22:08:44.000000 nsj_sql_utils_lib-0.0.3/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 20:19:29.999218 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      922 2023-07-22 22:06:27.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dao_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3722 2023-07-29 20:17:15.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dbadapter3.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dbconection_psycopg2.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 20:19:29.999218 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1215 2023-07-29 20:19:29.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      390 2023-07-29 20:19:29.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-29 20:19:29.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       42 2023-07-29 20:19:29.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2023-07-29 20:19:29.000000 nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-0.0.3/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      819 2023-07-29 20:19:30.003218 nsj_sql_utils_lib-0.0.3/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:23:00.414191 nsj_sql_utils_lib-0.0.4/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1215 2023-07-29 21:23:00.414191 nsj_sql_utils_lib-0.0.4/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      594 2023-07-22 22:08:44.000000 nsj_sql_utils_lib-0.0.4/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:23:00.414191 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-22 21:56:47.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      922 2023-07-22 22:06:27.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dao_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4500 2023-07-29 21:20:25.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dbadapter3.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      869 2023-07-22 22:02:23.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dbconection_psycopg2.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-29 21:23:00.414191 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1215 2023-07-29 21:23:00.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      390 2023-07-29 21:23:00.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-29 21:23:00.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       59 2023-07-29 21:23:00.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       18 2023-07-29 21:23:00.000000 nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-22 22:03:17.000000 nsj_sql_utils_lib-0.0.4/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      837 2023-07-29 21:23:00.414191 nsj_sql_utils_lib-0.0.4/setup.cfg
```

### Comparing `nsj_sql_utils_lib-0.0.3/PKG-INFO` & `nsj_sql_utils_lib-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_sql_utils_lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-0.0.3/README.md` & `nsj_sql_utils_lib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dao_util.py` & `nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dao_util.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dbadapter3.py` & `nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dbadapter3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+import re
+
 from sqlalchemy.engine.base import Connection as AlchemyConnection
+from sqlalchemy.exc import ResourceClosedError
+from sqlparams import SQLParams
 
 
 class DBAdapter3:
     """
     Adaptador de banco de dados para uso com o Psycopg2.
 
     Obs.: Esse adapter é simplificado, com relação ao DBAdapter2 e o DBAdapter, mas,
@@ -67,17 +71,32 @@
 
         if not isinstance(self.conn, AlchemyConnection):
             with self.conn.cursor() as cur:
                 cur.execute(sql, kwargs)
 
                 return self._handle_result(cur)
         else:
-            self.conn.execute(sql, kwargs)
+            return self._execute_sqlalchemy(sql, **kwargs)
 
-            return self._handle_result(cur)
+    def _execute_sqlalchemy(self, sql, **kwargs) -> tuple[list[dict[str, any]], int]:
+        sql2, pars2 = self._ajustar_query_sqlalchemy(sql, kwargs)
+
+        cur = None
+        try:
+            cur = self.conn.execute(sql2, pars2)
+
+            try:
+                result = [dict(rec.items()) for rec in cur.fetchall()]
+            except ResourceClosedError:
+                return ([], cur.rowcount)
+
+            return (result, cur.rowcount)
+        finally:
+            if cur is not None:
+                cur.close()
 
     def execute_many(
         self, sql, data: list[dict[str, any]]
     ) -> tuple[list[dict[str, any]], int]:
         """
         Executa uma query N vezes, de acordo com a lista de valores, em dicionários,
         recebidos no parâmetro "data"
@@ -97,7 +116,11 @@
                 "Execução de SQL com múltiplos valores ainda não suportada para conexões do SQL Alchemy."
             )
 
         with self.conn.cursor() as cur:
             cur.executemany(sql, data)
 
             return self._handle_result(cur)
+
+    def _ajustar_query_sqlalchemy(self, sql: str, pars: dict[str, any]):
+        sql = re.sub(r"%\(([^\(\)]+)\)s", r":\1", sql)
+        return SQLParams("named", "format").format(sql, pars)
```

### Comparing `nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib/dbconection_psycopg2.py` & `nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib/dbconection_psycopg2.py`

 * *Files identical despite different names*

### Comparing `nsj_sql_utils_lib-0.0.3/nsj_sql_utils_lib.egg-info/PKG-INFO` & `nsj_sql_utils_lib-0.0.4/nsj_sql_utils_lib.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-sql-utils-lib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 Home-page: https://github.com/Nasajon/nsj-sql-utils-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-sql-utils-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_sql_utils_lib-0.0.3/setup.cfg` & `nsj_sql_utils_lib-0.0.4/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_sql_utils_lib
-version = 0.0.3
+version = 0.0.4
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca de utilitários Python para facilitar a implementação de sistemas com acesso a banco de dados.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-sql-utils-lib
 project_urls = 
@@ -19,14 +19,15 @@
 package_dir = 
 	= ./
 packages = find:
 python_requires = >=3.4
 install_requires = 
 	psycopg2_binary>=2.9.6
 	SQLAlchemy>=1.4.32
+	sqlparams>=3.0.0
 
 [options.packages.find]
 where = ./
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

