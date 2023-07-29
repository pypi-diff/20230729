# Comparing `tmp/apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:30 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar", last modified: Sat Jul 29 12:08:41 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.262299 apache-airflow-providers-microsoft-mssql-3.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.263458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11330 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.188032 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.189095 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.190231 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.224205 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.230075 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-06-19 10:14:19.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.235908 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.259868 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1948 2023-06-20 11:42:30.265458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.821562 apache-airflow-providers-microsoft-mssql-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:08:41.822228 apache-airflow-providers-microsoft-mssql-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.743542 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.744691 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.745962 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.780244 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-29 12:01:19.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.786324 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4199 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.792105 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-16 17:25:26.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:41.818364 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:41.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-29 12:08:41.824371 apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-29 12:08:40.000000 apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-microsoft-mssql:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-mssql",
         "name": "Microsoft SQL Server (MSSQL)",
         "description": "`Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.2",
             "3.4.1",
             "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,43 +22,45 @@
 
 import pymssql
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 
 class MsSqlHook(DbApiHook):
-    """Interact with Microsoft SQL Server."""
+    """
+    Interact with Microsoft SQL Server.
+
+    :param args: passed to DBApiHook
+    :param sqlalchemy_scheme: Scheme sqlalchemy connection.  Default is ``mssql+pymssql`` Only used for
+      ``get_sqlalchemy_engine`` and ``get_sqlalchemy_connection`` methods.
+    :param kwargs: passed to DbApiHook
+    """
 
     conn_name_attr = "mssql_conn_id"
     default_conn_name = "mssql_default"
     conn_type = "mssql"
     hook_name = "Microsoft SQL Server"
     supports_autocommit = True
     DEFAULT_SQLALCHEMY_SCHEME = "mssql+pymssql"
 
     def __init__(
         self,
         *args,
         sqlalchemy_scheme: str | None = None,
         **kwargs,
     ) -> None:
-        """
-        :param args: passed to DBApiHook
-        :param sqlalchemy_scheme: Scheme sqlalchemy connection.  Default is ``mssql+pymssql`` Only used for
-          ``get_sqlalchemy_engine`` and ``get_sqlalchemy_connection`` methods.
-        :param kwargs: passed to DbApiHook
-        """
         super().__init__(*args, **kwargs)
         self.schema = kwargs.pop("schema", None)
         self._sqlalchemy_scheme = sqlalchemy_scheme
 
     @property
     def connection_extra_lower(self) -> dict:
         """
         ``connection.extra_dejson`` but where keys are converted to lower case.
+
         This is used internally for case-insensitive access of mssql params.
         """
         conn = self.get_connection(self.mssql_conn_id)  # type: ignore[attr-defined]
         return {k.lower(): v for k, v in conn.extra_dejson.items()}
 
     @property
     def sqlalchemy_scheme(self) -> str:
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         :ref:`howto/operator:MsSqlOperator`
 
     This operator may use one of two hooks, depending on the ``conn_type`` of the connection.
 
     If conn_type is ``'odbc'``, then :py:class:`~airflow.providers.odbc.hooks.odbc.OdbcHook`
     is used.  Otherwise, :py:class:`~airflow.providers.microsoft.mssql.hooks.mssql.MsSqlHook` is used.
 
+    This class is deprecated.
+
+    Please use :class:`airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
+
     :param sql: the sql code to be executed (templated)
     :param mssql_conn_id: reference to a specific mssql database
     :param parameters: (optional) the parameters to render the SQL query with.
     :param autocommit: if True, each command is automatically committed.
         (default value: False)
     :param database: name of database which overwrite defined one in connection
     """
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py` & `apache-airflow-providers-microsoft-mssql-3.4.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-mssql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.1"
+version = "3.4.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-mssql setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

