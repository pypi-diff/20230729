# Comparing `tmp/pgsqlx-1.6.9.tar.gz` & `tmp/pgsqlx-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.9.tar", last modified: Fri Jul 28 02:53:01 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.7.0.tar", last modified: Sat Jul 29 08:49:17 2023, max compression
```

## Comparing `pgsqlx-1.6.9.tar` & `pgsqlx-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx/
--rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.9/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.6.9/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.6.9/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.6.9/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.6.9/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.6.9/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      511 2023-07-28 02:01:22.000000 pgsqlx-1.6.9/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4612 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4612 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-28 02:53:01.000000 pgsqlx-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-28 02:51:58.000000 pgsqlx-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx/
+-rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.0/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.0/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1250 2023-07-28 02:45:27.000000 pgsqlx-1.7.0/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.0/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.0/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.0/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1505 2023-07-29 08:25:34.000000 pgsqlx-1.7.0/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4612 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4612 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.7.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:49:17.000000 pgsqlx-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-29 08:48:18.000000 pgsqlx-1.7.0/setup.py
```

### Comparing `pgsqlx-1.6.9/pgsqlx/db.py` & `pgsqlx-1.7.0/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/pgsqlx/dbx.py` & `pgsqlx-1.7.0/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/pgsqlx/log_support.py` & `pgsqlx-1.7.0/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/pgsqlx/orm.py` & `pgsqlx-1.7.0/pgsqlx/orm.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/pgsqlx/sql_mapper.py` & `pgsqlx-1.7.0/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.7.0/pgsqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.9
+Version: 1.7.0
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.9/PKG-INFO` & `pgsqlx-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.9
+Version: 1.7.0
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.9/README.rst` & `pgsqlx-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.9/setup.py` & `pgsqlx-1.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
-        'sqlx-batis>=0.1.1',
+        'sqlx-batis>=0.1.3',
     ],
-    version='1.6.9',
+    version='1.7.0',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

