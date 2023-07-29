# Comparing `tmp/apache-airflow-providers-oracle-3.7.1rc1.tar.gz` & `tmp/apache-airflow-providers-oracle-3.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-oracle-3.7.1rc1.tar", last modified: Tue Jun 20 11:42:47 2023, max compression
+gzip compressed data, was "apache-airflow-providers-oracle-3.7.2rc1.tar", last modified: Sat Jul 29 12:08:52 2023, max compression
```

## Comparing `apache-airflow-providers-oracle-3.7.1rc1.tar` & `apache-airflow-providers-oracle-3.7.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.127364 apache-airflow-providers-oracle-3.7.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14005 2023-06-20 11:42:47.128474 apache-airflow-providers-oracle-3.7.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12428 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.026099 apache-airflow-providers-oracle-3.7.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.027356 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.070602 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.077652 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/example_oracle.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.084818 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.092233 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.099114 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.125104 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14005 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-oracle-3.7.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:42:47.130389 apache-airflow-providers-oracle-3.7.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 11:42:45.000000 apache-airflow-providers-oracle-3.7.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.296187 apache-airflow-providers-oracle-3.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-29 12:08:52.296949 apache-airflow-providers-oracle-3.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.199591 apache-airflow-providers-oracle-3.7.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.200703 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.239182 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.245825 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.254024 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.261930 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-07-16 17:25:26.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.268432 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-06-28 06:26:40.000000 apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:52.293630 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:52.000000 apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-oracle-3.7.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-07-29 12:08:52.299039 apache-airflow-providers-oracle-3.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-29 12:08:51.000000 apache-airflow-providers-oracle-3.7.2rc1/setup.py
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/LICENSE` & `apache-airflow-providers-oracle-3.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/MANIFEST.in` & `apache-airflow-providers-oracle-3.7.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.7.1"
+__version__ = "3.7.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-oracle:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/example_oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/example_dags/example_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/get_provider_info.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-oracle",
         "name": "Oracle",
         "description": "`Oracle <https://www.oracle.com/en/database/>`__\n",
         "suspended": False,
         "versions": [
+            "3.7.2",
             "3.7.1",
             "3.7.0",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/operators/oracle.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     from airflow.utils.context import Context
 
 
 class OracleOperator(SQLExecuteQueryOperator):
     """
     Executes sql code in a specific Oracle database.
 
+    This class is deprecated.
+
+    Please use :class:`airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
+
     :param sql: the sql code to be executed. Can receive a str representing a sql statement,
         a list of str (sql statements), or reference to a template file.
         Template reference are recognized by str ending in '.sql'
         (templated)
     :param oracle_conn_id: The :ref:`Oracle connection id <howto/connection:oracle>`
         reference to a specific Oracle database.
     :param parameters: (optional, templated) the parameters to render the SQL query with.
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/__init__.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache-airflow-providers-oracle-3.7.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     from airflow.utils.context import Context
 
 
 class OracleToOracleOperator(BaseOperator):
     """
     Moves data from Oracle to Oracle.
 
-
     :param oracle_destination_conn_id: destination Oracle connection.
     :param destination_table: destination table to insert rows.
     :param oracle_source_conn_id: :ref:`Source Oracle connection <howto/connection:oracle>`.
     :param source_sql: SQL query to execute against the source Oracle
         database. (templated)
     :param source_sql_params: Parameters to use in sql query. (templated)
     :param rows_chunk: number of rows per chunk to commit.
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt` & `apache-airflow-providers-oracle-3.7.2rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/pyproject.toml` & `apache-airflow-providers-oracle-3.7.2rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
 
@@ -35,15 +37,16 @@
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi",
-    "airflow/migrations/versions/*.py"
+    "airflow/migrations/versions/*.py",
+    "tests/dags/test_imports.py",
 ]
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
@@ -67,14 +70,16 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+namespace-packages = ["airflow/providers"]
+
 [tool.pytest.ini_options]
 # * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
 # * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
 # * And we focus on use native pytest capabilities rather than adopt another frameworks.
 addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
 norecursedirs = [
     ".eggs",
@@ -93,54 +98,28 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
-# TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
-known-third-party = [
-    "asana",
-    "atlassian",
-    "celery",
-    "cloudant",
-    "databricks",
-    "datadog",
-    "docker",
-    "elasticsearch",
-    "github",
-    "google",
-    "grpc",
-    "jenkins",
-    "mysql",
-    "neo4j",
-    "papermill",
-    "redis",
-    "sendgrid",
-    "snowflake",
-    "telegram",
-    "trino",
-]
-
 [tool.ruff.per-file-ignores]
 "airflow/models/__init__.py" = ["F401"]
 "airflow/models/sqla_models.py" = ["F401"]
 
-
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
 "airflow/serialization/pydantic/*.py" = ["I002"]
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/setup.cfg` & `apache-airflow-providers-oracle-3.7.2rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-oracle-3.7.1rc1/setup.py` & `apache-airflow-providers-oracle-3.7.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-oracle package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.7.1"
+version = "3.7.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-oracle setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"], "numpy": ["numpy"]},
```

