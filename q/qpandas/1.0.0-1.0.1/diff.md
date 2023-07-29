# Comparing `tmp/qpandas-1.0.0.tar.gz` & `tmp/qpandas-1.0.1.tar.gz`

## Comparing `qpandas-1.0.0.tar` & `qpandas-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 qpandas-1.0.0/README.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 qpandas-1.0.0/TODO.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 qpandas-1.0.0/publish.sh
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 qpandas-1.0.0/requirements.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 qpandas-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 qpandas-1.0.0/.github/workflows/install.yml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qpandas-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 qpandas-1.0.0/src/qpandas/__init__.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 qpandas-1.0.0/src/qpandas/sqldf.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 qpandas-1.0.0/src/qpandas/data/births.csv
--rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 qpandas-1.0.0/src/qpandas/data/births_by_month.csv
--rw-r--r--   0        0        0    62608 2020-02-02 00:00:00.000000 qpandas-1.0.0/src/qpandas/data/meat.csv
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 qpandas-1.0.0/tests/test_mypandas.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 qpandas-1.0.0/tests/test_pandasql.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 qpandas-1.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 qpandas-1.0.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 qpandas-1.0.0/LICENSE
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 qpandas-1.0.0/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 qpandas-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 qpandas-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 qpandas-1.0.1/README.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 qpandas-1.0.1/TODO.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 qpandas-1.0.1/publish.sh
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 qpandas-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/workflows/install.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/__init__.py
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/qpandas.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/births.csv
+-rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/births_by_month.csv
+-rw-r--r--   0        0        0    62608 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/meat.csv
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_pandasql.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_qpandas.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0   147456 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/.mode
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/csv_sqlite3.sh
+-rw-r--r--   0        0        0   286720 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/x.db
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 qpandas-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 qpandas-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 qpandas-1.0.1/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 qpandas-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 qpandas-1.0.1/PKG-INFO
```

### Comparing `qpandas-1.0.0/.github/workflows/install.yml` & `qpandas-1.0.1/.github/workflows/install.yml`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/.github/workflows/test.yml` & `qpandas-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/src/qpandas/sqldf.py` & `qpandas-1.0.1/src/qpandas/qpandas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 from __future__ import annotations
 
 import inspect
 import re
-import urllib
 from contextlib import contextmanager
 from functools import wraps
 from typing import Any, Callable
 from warnings import catch_warnings, filterwarnings, warn
 
 import pandas as pd
 from pandas.io.sql import read_sql
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Connection
 from sqlalchemy.event import listen
 from sqlalchemy.exc import DatabaseError, ResourceClosedError
 from sqlalchemy.pool import NullPool
+from sqlglot import transpile
 
-__all__ = ["MyPandas", "MyPandasException", "sqldf"]
+# __all__ = ["PandaSQL", "PandaSQLException", "sqldf"]
 
 _PRINT = False
-TEMP_DB_NAME = "__MYPANDAS_TEMP"
+_DIALECTS = """
+duckdb
+postgres
+spark
+trino
+bigquery
+hive
+presto
+sqlite
+tsql
+clickhouse
+mysql
+redshift
+starrocks
+dialect
+oracle
+snowflake
+tableau
+""".strip().splitlines()
 
 
 def _print(*args, **kwargs) -> None:
     if _PRINT:
         print(*args, **kwargs)
 
 
@@ -42,39 +60,33 @@
     for key, value in vars(cls).items():
         if callable(value):
             setattr(cls, key, _debug_func(value))
             continue
     return cls
 
 
-class MyPandasException(Exception):
+class PandaSQLException(Exception):
     pass
 
 
 @_debug
-class MyPandas:
-    def __init__(
-        self, db_uri: str = "sqlite:///:memory:", persist: bool = False
-    ) -> None:
+class PandaSQL:
+    def __init__(self, dialect: str, persist: bool = False) -> None:
         """
         Initialize with a specific database.
 
         :param db_uri: SQLAlchemy-compatible database URI.
         :param persist: keep tables in database between different calls on the same object of this class.
         """
-        self.engine = create_engine(db_uri, poolclass=NullPool)
+        if dialect not in _DIALECTS:
+            raise PandaSQLException("Unsupported database dialects.")
+        self.dialect = dialect
 
-        if self.engine.name not in ("sqlite", "postgresql", "mysql"):
-            raise MyPandasException("Unsupported database engine.")
-
-        if self.engine.name == "sqlite":
-            listen(self.engine, "connect", self._set_text_factory)
-
-        if self.engine.name == "mysql":
-            self._mysql_datbase = urllib.parse.urlsplit(db_uri).path.replace("/", "")  # type: ignore
+        self.engine = create_engine("sqlite:///:memory:", poolclass=NullPool)
+        listen(self.engine, "connect", self._set_text_factory)
 
         self.persist = persist
         self.loaded_tables: set[str] = set()
         if self.persist:
             self._conn = self.engine.connect()
             self._init_connection(self._conn)
 
@@ -84,14 +96,16 @@
         Automatically creates tables mentioned in the query from dataframes before executing.
 
         :param query: SQL query string, which can reference pandas dataframes as SQL tables.
         :param env: Variables environment - a dict mapping table names to pandas dataframes.
         If not specified use local and global variables of the caller.
         :return: Pandas dataframe with the result of the SQL query.
         """
+        query = transpile(query, read=self.dialect, write="sqlite")[0]
+
         if env is None:
             env = get_outer_frame_variables()
             assert env is not None
 
         with self.conn as conn:
             for table_name in extract_table_names(query):
                 if table_name not in env:
@@ -103,15 +117,15 @@
                 self.loaded_tables.add(table_name)
 
                 write_table(env[table_name], table_name, conn)
 
             try:
                 result = read_sql(query, conn)
             except DatabaseError as ex:
-                raise MyPandasException(ex)
+                raise PandaSQLException(ex)
             except ResourceClosedError:
                 # query returns nothing
                 result = None
 
         return result
 
     @property  # type: ignore
@@ -124,35 +138,22 @@
         else:
             conn = self.engine.connect()
             self._init_connection(conn)
             try:
                 yield conn
             finally:
                 _print("Closing conn")
-                if self.engine.name == "mysql" and self._mysql_datbase == "":
-                    conn.execute(f"DROP DATABASE {TEMP_DB_NAME};")
                 conn.close()
 
     def _init_connection(self, conn: Connection) -> None:
-        _print("Initing conn")
-        if self.engine.name == "postgresql":
-            conn.execute("SET search_path TO pg_temp")
-        if self.engine.name == "mysql":
-            _print("Before", (conn.execute("SELECT DATABASE();").fetchone()))
-            if self._mysql_datbase == "":
-                conn.execute(f"DROP DATABASE IF EXISTS {TEMP_DB_NAME};")
-                conn.execute(f"CREATE DATABASE {TEMP_DB_NAME};")
-                conn.execute(f"USE {TEMP_DB_NAME};")
-            _print("After", (conn.execute("SELECT DATABASE();").fetchone()))
-            # doesnt support BLOB/TEXT:
-            # conn.execute("SET default_storage_engine=MEMORY;")
-            # conn.execute("SET default_tmp_storage_engine=MEMORY;")
+        warn("This method does nothing remove call!")
 
     # TODO this connection_record is only used for testing but is useless?
     def _set_text_factory(self, dbapi_con, connection_record) -> None:
+        # TODO what exactly does this do for sqlite?
         # sqlite only
         dbapi_con.text_factory = str
 
 
 @_debug_func
 def get_outer_frame_variables() -> dict:
     """Get a dict of local and global variables of the first outer frame from another file."""
@@ -190,16 +191,14 @@
         try:
             df.to_sql(name=tablename, con=conn, index=False)
             # What?:
             # index=not any(name is None for name in df.index.names)
             # load index into db if all levels are named
         except Exception as e:
             _print(f"Exception: {e}")
-            _print(f"Table {tablename} already exists, dropping and readding!")
-            conn.execute(f"DROP TABLE {tablename};")
             df.to_sql(name=tablename, con=conn, index=False)
 
 
 @_debug_func
 def sqldf(
     query: str, env: dict[str, Any] | None = None, db_uri: str = "sqlite:///:memory:"
 ) -> pd.DataFrame:
@@ -234,8 +233,8 @@
     >>> sqldf("select * from df;", locals())
     >>> sqldf("select avg(x) from df;", locals())
     """
     warn(
         "sqldf is depricated, use of the MyPandas class is encouraged.",
         DeprecationWarning,
     )
-    return MyPandas(db_uri)(query, env)
+    return PandaSQL(db_uri)(query, env)
```

### Comparing `qpandas-1.0.0/src/qpandas/data/births.csv` & `qpandas-1.0.1/src/qpandas/data/births.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/src/qpandas/data/births_by_month.csv` & `qpandas-1.0.1/src/qpandas/data/births_by_month.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/src/qpandas/data/meat.csv` & `qpandas-1.0.1/src/qpandas/data/meat.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/tests/test_pandasql.py` & `qpandas-1.0.1/tests/test_pandasql.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/tests/test_utils.py` & `qpandas-1.0.1/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from qpandas.sqldf import extract_table_names, get_outer_frame_variables
+from qpandas.qpandas import extract_table_names, get_outer_frame_variables
 
 
 def test_get_vars():
     var_a = 123
     variable = {"a": "b", "c": "d"}
     assert get_outer_frame_variables()["var_a"] == var_a
     assert get_outer_frame_variables()["variable"] == variable
```

### Comparing `qpandas-1.0.0/.gitignore` & `qpandas-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/LICENSE` & `qpandas-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.0/pyproject.toml` & `qpandas-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qpandas"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="yrom1", email="ryanm.inbox@gmail.com" },
 ]
 description = "Query Panadas DataFrames with SQL"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
```

