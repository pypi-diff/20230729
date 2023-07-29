# Comparing `tmp/qpandas-1.0.1.tar.gz` & `tmp/qpandas-1.0.2.tar.gz`

## Comparing `qpandas-1.0.1.tar` & `qpandas-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 qpandas-1.0.1/README.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 qpandas-1.0.1/TODO.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 qpandas-1.0.1/publish.sh
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 qpandas-1.0.1/requirements.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/workflows/install.yml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qpandas-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/__init__.py
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/qpandas.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/births.csv
--rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/births_by_month.csv
--rw-r--r--   0        0        0    62608 2020-02-02 00:00:00.000000 qpandas-1.0.1/src/qpandas/data/meat.csv
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_pandasql.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_qpandas.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 qpandas-1.0.1/tests/test_utils.py
--rw-r--r--   0        0        0   147456 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/.mode
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/csv_sqlite3.sh
--rw-r--r--   0        0        0   286720 2020-02-02 00:00:00.000000 qpandas-1.0.1/util/x.db
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 qpandas-1.0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 qpandas-1.0.1/LICENSE
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 qpandas-1.0.1/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 qpandas-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 qpandas-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 qpandas-1.0.2/README.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 qpandas-1.0.2/TODO.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 qpandas-1.0.2/publish.sh
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 qpandas-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 qpandas-1.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 qpandas-1.0.2/.github/workflows/install.yml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qpandas-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 qpandas-1.0.2/src/qpandas/__init__.py
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 qpandas-1.0.2/src/qpandas/qpandas.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 qpandas-1.0.2/src/qpandas/data/births.csv
+-rw-r--r--   0        0        0    11028 2020-02-02 00:00:00.000000 qpandas-1.0.2/src/qpandas/data/births_by_month.csv
+-rw-r--r--   0        0        0    62608 2020-02-02 00:00:00.000000 qpandas-1.0.2/src/qpandas/data/meat.csv
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 qpandas-1.0.2/tests/test_pandasql.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 qpandas-1.0.2/tests/test_qpandas.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 qpandas-1.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0   147456 2020-02-02 00:00:00.000000 qpandas-1.0.2/util/.mode
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 qpandas-1.0.2/util/csv_sqlite3.sh
+-rw-r--r--   0        0        0   286720 2020-02-02 00:00:00.000000 qpandas-1.0.2/util/x.db
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 qpandas-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 qpandas-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 qpandas-1.0.2/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 qpandas-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 qpandas-1.0.2/PKG-INFO
```

### Comparing `qpandas-1.0.1/README.py` & `qpandas-1.0.2/README.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/TODO.md` & `qpandas-1.0.2/TODO.md`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/.github/workflows/install.yml` & `qpandas-1.0.2/.github/workflows/install.yml`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/.github/workflows/test.yml` & `qpandas-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/src/qpandas/__init__.py` & `qpandas-1.0.2/src/qpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/src/qpandas/qpandas.py` & `qpandas-1.0.2/src/qpandas/qpandas.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/src/qpandas/data/births.csv` & `qpandas-1.0.2/src/qpandas/data/births.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/src/qpandas/data/births_by_month.csv` & `qpandas-1.0.2/src/qpandas/data/births_by_month.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/src/qpandas/data/meat.csv` & `qpandas-1.0.2/src/qpandas/data/meat.csv`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/tests/test_pandasql.py` & `qpandas-1.0.2/tests/test_pandasql.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/tests/test_utils.py` & `qpandas-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/util/.mode` & `qpandas-1.0.2/util/.mode`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/util/x.db` & `qpandas-1.0.2/util/x.db`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/.gitignore` & `qpandas-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/LICENSE` & `qpandas-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/README.md` & `qpandas-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qpandas-1.0.1/pyproject.toml` & `qpandas-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qpandas"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="yrom1", email="ryanm.inbox@gmail.com" },
 ]
 description = "Query Panadas DataFrames with SQL"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "sqlalchemy",
     "pandas",
-    "mysqlclient",
+    "sqlglot",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/yrom1/qpandas"
 "Bug Tracker" = "https://github.com/yrom1/qpandas/issues"
 
 [tool.pytest.ini_options]
```

### Comparing `qpandas-1.0.1/PKG-INFO` & `qpandas-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qpandas
-Version: 1.0.1
+Version: 1.0.2
 Summary: Query Panadas DataFrames with SQL
 Project-URL: Homepage, https://github.com/yrom1/qpandas
 Project-URL: Bug Tracker, https://github.com/yrom1/qpandas/issues
 Author-email: yrom1 <ryanm.inbox@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: mysqlclient
 Requires-Dist: pandas
 Requires-Dist: sqlalchemy
+Requires-Dist: sqlglot
 Description-Content-Type: text/markdown
 
 # qpandas
 
 
 ---
```

