# Comparing `tmp/sqlx-batis-0.1.2.tar.gz` & `tmp/sqlx-batis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.2.tar", last modified: Sat Jul 29 08:11:08 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.1.3.tar", last modified: Sat Jul 29 08:45:27 2023, max compression
```

## Comparing `sqlx-batis-0.1.2.tar` & `sqlx-batis-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/
--rw-rw-rw-   0        0        0     3373 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-29 08:10:36.000000 sqlx-batis-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.2/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.2/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.2/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     5051 2023-07-29 07:30:33.000000 sqlx-batis-0.1.2/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.2/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.2/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.2/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.2/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.2/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.2/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.2/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1631 2023-07-29 06:24:56.000000 sqlx-batis-0.1.2/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3373 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 08:11:08.000000 sqlx-batis-0.1.2/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/
+-rw-rw-rw-   0        0        0     3373 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.1.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-29 08:45:23.000000 sqlx-batis-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlbatis/
+-rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.3/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8673 2023-07-28 01:55:39.000000 sqlx-batis-0.1.3/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6831 2023-07-28 02:15:36.000000 sqlx-batis-0.1.3/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     5051 2023-07-29 07:30:33.000000 sqlx-batis-0.1.3/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     4084 2023-07-28 02:13:59.000000 sqlx-batis-0.1.3/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.3/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.3/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.3/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5242 2023-07-28 01:56:29.000000 sqlx-batis-0.1.3/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1848 2023-07-27 03:50:25.000000 sqlx-batis-0.1.3/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.3/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1631 2023-07-29 06:24:56.000000 sqlx-batis-0.1.3/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3373 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-29 08:45:27.000000 sqlx-batis-0.1.3/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.2/PKG-INFO` & `sqlx-batis-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.2
+Version: 0.1.3
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.1.2/README.rst` & `sqlx-batis-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/setup.py` & `sqlx-batis-0.1.3/setup.py`

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
-        'sqlx-exec>=1.2.9',
+        'sqlx-exec>=1.3.0',
     ],
-    version='0.1.2',
+    version='0.1.3',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.2/sqlbatis/constant.py` & `sqlx-batis-0.1.3/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/db.py` & `sqlx-batis-0.1.3/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/dbx.py` & `sqlx-batis-0.1.3/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/engine.py` & `sqlx-batis-0.1.3/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/log_support.py` & `sqlx-batis-0.1.3/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/orm.py` & `sqlx-batis-0.1.3/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/snowflake.py` & `sqlx-batis-0.1.3/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/sql_holder.py` & `sqlx-batis-0.1.3/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/sql_mapper.py` & `sqlx-batis-0.1.3/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/sql_support.py` & `sqlx-batis-0.1.3/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlbatis/__init__.py` & `sqlx-batis-0.1.3/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.2/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.1.3/sqlx_batis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.2
+Version: 0.1.3
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

