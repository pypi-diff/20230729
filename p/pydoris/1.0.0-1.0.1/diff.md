# Comparing `tmp/pydoris-1.0.0.tar.gz` & `tmp/pydoris-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoris-1.0.0.tar", last modified: Mon Jul 17 07:55:03 2023, max compression
+gzip compressed data, was "pydoris-1.0.1.tar", last modified: Sat Jul 29 14:48:15 2023, max compression
```

## Comparing `pydoris-1.0.0.tar` & `pydoris-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-17 07:55:03.857727 pydoris-1.0.0/
--rw-r--r--   0 liujiwen   (501) staff       (20)    11357 2023-07-17 04:04:30.000000 pydoris-1.0.0/LICENSE
--rw-r--r--   0 liujiwen   (501) staff       (20)     2523 2023-07-17 07:55:03.857565 pydoris-1.0.0/PKG-INFO
--rw-r--r--   0 liujiwen   (501) staff       (20)     1780 2023-07-17 07:48:55.000000 pydoris-1.0.0/README.md
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-17 07:55:03.855432 pydoris-1.0.0/pydoris/
--rw-r--r--   0 liujiwen   (501) staff       (20)      829 2023-07-17 07:48:55.000000 pydoris-1.0.0/pydoris/__init__.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-17 07:55:03.857124 pydoris-1.0.0/pydoris/sqlalchemy/
--rw-r--r--   0 liujiwen   (501) staff       (20)      922 2023-07-17 07:43:44.000000 pydoris-1.0.0/pydoris/sqlalchemy/__init__.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     3649 2023-07-17 07:23:14.000000 pydoris-1.0.0/pydoris/sqlalchemy/datatype.py
--rw-r--r--   0 liujiwen   (501) staff       (20)     5943 2023-07-17 07:53:00.000000 pydoris-1.0.0/pydoris/sqlalchemy/dialect.py
-drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-17 07:55:03.856480 pydoris-1.0.0/pydoris.egg-info/
--rw-r--r--   0 liujiwen   (501) staff       (20)     2523 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/PKG-INFO
--rw-r--r--   0 liujiwen   (501) staff       (20)      356 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/SOURCES.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/dependency_links.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)       72 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/entry_points.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-07-17 06:56:17.000000 pydoris-1.0.0/pydoris.egg-info/not-zip-safe
--rw-r--r--   0 liujiwen   (501) staff       (20)       72 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/requires.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)        8 2023-07-17 07:55:03.000000 pydoris-1.0.0/pydoris.egg-info/top_level.txt
--rw-r--r--   0 liujiwen   (501) staff       (20)       38 2023-07-17 07:55:03.857771 pydoris-1.0.0/setup.cfg
--rw-r--r--   0 liujiwen   (501) staff       (20)     2528 2023-07-17 07:41:43.000000 pydoris-1.0.0/setup.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-29 14:48:15.260834 pydoris-1.0.1/
+-rw-r--r--   0 liujiwen   (501) staff       (20)    11357 2023-07-17 04:04:30.000000 pydoris-1.0.1/LICENSE
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2536 2023-07-29 14:48:15.260687 pydoris-1.0.1/PKG-INFO
+-rw-r--r--   0 liujiwen   (501) staff       (20)     1780 2023-07-17 07:48:55.000000 pydoris-1.0.1/README.md
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-29 14:48:15.258507 pydoris-1.0.1/pydoris/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      829 2023-07-28 10:49:42.000000 pydoris-1.0.1/pydoris/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3552 2023-07-28 10:49:05.000000 pydoris-1.0.1/pydoris/doris_client.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-29 14:48:15.260428 pydoris-1.0.1/pydoris/sqlalchemy/
+-rw-r--r--   0 liujiwen   (501) staff       (20)      922 2023-07-19 10:53:08.000000 pydoris-1.0.1/pydoris/sqlalchemy/__init__.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     3649 2023-07-17 07:23:14.000000 pydoris-1.0.1/pydoris/sqlalchemy/datatype.py
+-rw-r--r--   0 liujiwen   (501) staff       (20)     5889 2023-07-29 14:43:55.000000 pydoris-1.0.1/pydoris/sqlalchemy/dialect.py
+drwxr-xr-x   0 liujiwen   (501) staff       (20)        0 2023-07-29 14:48:15.259774 pydoris-1.0.1/pydoris.egg-info/
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2536 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/PKG-INFO
+-rw-r--r--   0 liujiwen   (501) staff       (20)      380 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/SOURCES.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/dependency_links.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)      120 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/entry_points.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)        1 2023-07-27 09:40:53.000000 pydoris-1.0.1/pydoris.egg-info/not-zip-safe
+-rw-r--r--   0 liujiwen   (501) staff       (20)       72 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/requires.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)        8 2023-07-29 14:48:15.000000 pydoris-1.0.1/pydoris.egg-info/top_level.txt
+-rw-r--r--   0 liujiwen   (501) staff       (20)       38 2023-07-29 14:48:15.260870 pydoris-1.0.1/setup.cfg
+-rw-r--r--   0 liujiwen   (501) staff       (20)     2603 2023-07-29 14:45:25.000000 pydoris-1.0.1/setup.py
```

### Comparing `pydoris-1.0.0/LICENSE` & `pydoris-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoris-1.0.0/PKG-INFO` & `pydoris-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydoris
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface to Doris
 Home-page: https://github.com/apache/doris
-Author: liujiwen-up
+Author: liujiwen-up,bingquanzhao
 Author-email: wen15580974595@163.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `pydoris-1.0.0/README.md` & `pydoris-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pydoris-1.0.0/pydoris/__init__.py` & `pydoris-1.0.1/pydoris/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

### Comparing `pydoris-1.0.0/pydoris/sqlalchemy/__init__.py` & `pydoris-1.0.1/pydoris/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `pydoris-1.0.0/pydoris/sqlalchemy/datatype.py` & `pydoris-1.0.1/pydoris/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `pydoris-1.0.0/pydoris/sqlalchemy/dialect.py` & `pydoris-1.0.1/pydoris/sqlalchemy/dialect.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,22 +49,22 @@
         assert schema is not None
 
         quote = self.identifier_preparer.quote_identifier
         full_name = quote(table_name)
         if schema:
             full_name = "{}.{}".format(quote(schema), full_name)
 
-        res = connection.execute(f"DESCRIBE {full_name}") # 获取元数据信息
+        res = connection.execute(f"DESCRIBE {full_name}")
         return res.first() is not None
 
     def get_schema_names(self, connection, **kw):
-        rp = connection.exec_driver_sql("SHOW schemas") # 获取库名
+        rp = connection.exec_driver_sql("SHOW schemas")
         return [r[0] for r in rp]
 
-    def get_table_names(self, connection, schema=None, **kw): # 获取表名
+    def get_table_names(self, connection, schema=None, **kw):
         """Return a Unicode SHOW TABLES from a given schema."""
         if schema is not None:
             current_schema = schema
         else:
             current_schema = self.default_schema_name
 
         charset = self._connection_charset
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydoris-1.0.0/pydoris.egg-info/PKG-INFO` & `pydoris-1.0.1/pydoris.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydoris
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python interface to Doris
 Home-page: https://github.com/apache/doris
-Author: liujiwen-up
+Author: liujiwen-up,bingquanzhao
 Author-email: wen15580974595@163.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `pydoris-1.0.0/setup.py` & `pydoris-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 setup(
     name=package_name,
     version=version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
-    author="liujiwen-up",
+    author="liujiwen-up,bingquanzhao",
     author_email="wen15580974595@163.com",
     url="https://github.com/apache/doris",
     classifiers=[
 	"Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
@@ -62,10 +62,11 @@
     packages=find_packages(include=["pydoris", "pydoris.*"]),
     package_data={"": ["LICENSE", "README.md"]},
     include_package_data=True,
     zip_safe=False,
     entry_points={
         'sqlalchemy.dialects': [
             'pydoris = pydoris.sqlalchemy.dialect:DorisDialect',
+            'doris = pydoris.sqlalchemy.dialect:DorisDialect'
         ]
     },
 )
```

