# Comparing `tmp/mysqlx-1.6.8.tar.gz` & `tmp/mysqlx-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.8.tar", last modified: Fri Jul 28 02:54:54 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.9.tar", last modified: Sat Jul 29 08:48:36 2023, max compression
```

## Comparing `mysqlx-1.6.8.tar` & `mysqlx-1.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/
-drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx/
--rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.6.8/mysqlx/db.py
--rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.6.8/mysqlx/dbx.py
--rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.6.8/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.8/mysqlx/orm.py
--rw-rw-rw-   0        0        0      491 2023-07-28 02:04:25.000000 mysqlx-1.6.8/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4511 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      279 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 02:54:54.000000 mysqlx-1.6.8/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4511 2023-07-28 02:54:54.000000 mysqlx-1.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-28 02:54:54.000000 mysqlx-1.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-28 02:54:38.000000 mysqlx-1.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:48:36.000000 mysqlx-1.6.9/
+drwxrwxrwx   0        0        0        0 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx/
+-rw-rw-rw-   0        0        0      665 2023-07-28 02:04:41.000000 mysqlx-1.6.9/mysqlx/db.py
+-rw-rw-rw-   0        0        0      535 2023-07-28 02:37:55.000000 mysqlx-1.6.9/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      592 2023-07-28 02:20:31.000000 mysqlx-1.6.9/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     6082 2023-07-27 04:32:45.000000 mysqlx-1.6.9/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     1487 2023-07-29 08:47:09.000000 mysqlx-1.6.9/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 08:48:36.000000 mysqlx-1.6.9/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4511 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      279 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 08:48:35.000000 mysqlx-1.6.9/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4511 2023-07-29 08:48:36.000000 mysqlx-1.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 08:48:36.000000 mysqlx-1.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-29 08:47:34.000000 mysqlx-1.6.9/setup.py
```

### Comparing `mysqlx-1.6.8/mysqlx/db.py` & `mysqlx-1.6.9/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.8/mysqlx/dbx.py` & `mysqlx-1.6.9/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.8/mysqlx/log_support.py` & `mysqlx-1.6.9/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.8/mysqlx/orm.py` & `mysqlx-1.6.9/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.8/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.9/mysqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.8
+Version: 1.6.9
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.8/PKG-INFO` & `mysqlx-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.8
+Version: 1.6.9
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.8/README.rst` & `mysqlx-1.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.8/setup.py` & `mysqlx-1.6.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.1.1',
+        'sqlx-batis>=0.1.3',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.8',
+    version='1.6.9',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

