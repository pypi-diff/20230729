# Comparing `tmp/apache-airflow-providers-exasol-4.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-exasol-4.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-exasol-4.2.1rc1.tar", last modified: Tue Jun 20 11:42:00 2023, max compression
+gzip compressed data, was "apache-airflow-providers-exasol-4.2.2rc1.tar", last modified: Sat Jul 29 12:08:24 2023, max compression
```

## Comparing `apache-airflow-providers-exasol-4.2.1rc1.tar` & `apache-airflow-providers-exasol-4.2.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.090548 apache-airflow-providers-exasol-4.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:42:00.091679 apache-airflow-providers-exasol-4.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11516 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.010967 apache-airflow-providers-exasol-4.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.012178 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.051802 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.057572 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10925 2023-06-05 12:50:36.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.063339 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.087791 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-20 11:42:00.093634 apache-airflow-providers-exasol-4.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.194316 apache-airflow-providers-exasol-4.2.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5702 2023-07-29 12:08:24.194905 apache-airflow-providers-exasol-4.2.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.124786 apache-airflow-providers-exasol-4.2.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.125874 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.157247 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.162968 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11648 2023-07-26 06:59:50.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.168963 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:24.192073 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5702 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:24.000000 apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-exasol-4.2.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-07-29 12:08:24.196761 apache-airflow-providers-exasol-4.2.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-29 12:08:23.000000 apache-airflow-providers-exasol-4.2.2rc1/setup.py
```

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/LICENSE` & `apache-airflow-providers-exasol-4.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in` & `apache-airflow-providers-exasol-4.2.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.2.1"
+__version__ = "4.2.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-exasol:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-exasol",
         "name": "Exasol",
         "description": "`Exasol <https://docs.exasol.com/home.htm>`__\n",
         "suspended": False,
         "versions": [
+            "4.2.2",
             "4.2.1",
             "4.2.0",
             "4.1.3",
             "4.1.2",
             "4.1.1",
             "4.1.0",
             "4.0.1",
```

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/hooks/exasol.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from contextlib import closing
-from typing import Any, Callable, Iterable, Mapping, Sequence
+from typing import Any, Callable, Iterable, Mapping, Sequence, TypeVar, overload
 
 import pandas as pd
 import pyexasol
 from pyexasol import ExaConnection, ExaStatement
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook, return_single_query_results
 
+T = TypeVar("T")
+
 
 class ExasolHook(DbApiHook):
     """Interact with Exasol.
 
     You can specify the pyexasol ``compression``, ``encryption``, ``json_lib``
     and ``client_name``  parameters in the extra field of your connection
     as ``{"compression": True, "json_lib": "rapidjson", etc}``.
@@ -62,15 +64,17 @@
         for arg_name, arg_val in conn.extra_dejson.items():
             if arg_name in ["compression", "encryption", "json_lib", "client_name"]:
                 conn_args[arg_name] = arg_val
 
         conn = pyexasol.connect(**conn_args)
         return conn
 
-    def get_pandas_df(self, sql: str, parameters: dict | None = None, **kwargs) -> pd.DataFrame:
+    def get_pandas_df(
+        self, sql, parameters: Iterable | Mapping[str, Any] | None = None, **kwargs
+    ) -> pd.DataFrame:
         """Execute the SQL and return a Pandas dataframe.
 
         :param sql: The sql statement to be executed (str) or a list of
             sql statements to execute.
         :param parameters: The parameters to render the SQL query with.
 
         Other keyword arguments are all forwarded into
@@ -79,27 +83,27 @@
         with closing(self.get_conn()) as conn:
             df = conn.export_to_pandas(sql, query_params=parameters, **kwargs)
             return df
 
     def get_records(
         self,
         sql: str | list[str],
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
     ) -> list[dict | tuple[Any, ...]]:
         """Execute the SQL and return a set of records.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         with closing(self.get_conn()) as conn:
             with closing(conn.execute(sql, parameters)) as cur:
                 return cur.fetchall()
 
-    def get_first(self, sql: str | list[str], parameters: Iterable | Mapping | None = None) -> Any:
+    def get_first(self, sql: str | list[str], parameters: Iterable | Mapping[str, Any] | None = None) -> Any:
         """Execute the SQL and return the first resulting row.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         with closing(self.get_conn()) as conn:
@@ -153,23 +157,47 @@
                     v.get("precision", None),
                     v.get("scale", None),
                     True,
                 )
             )
         return cols
 
+    @overload
+    def run(
+        self,
+        sql: str | Iterable[str],
+        autocommit: bool = ...,
+        parameters: Iterable | Mapping[str, Any] | None = ...,
+        handler: None = ...,
+        split_statements: bool = ...,
+        return_last: bool = ...,
+    ) -> None:
+        ...
+
+    @overload
+    def run(
+        self,
+        sql: str | Iterable[str],
+        autocommit: bool = ...,
+        parameters: Iterable | Mapping[str, Any] | None = ...,
+        handler: Callable[[Any], T] = ...,
+        split_statements: bool = ...,
+        return_last: bool = ...,
+    ) -> T | list[T]:
+        ...
+
     def run(
         self,
         sql: str | Iterable[str],
         autocommit: bool = False,
-        parameters: Iterable | Mapping | None = None,
-        handler: Callable | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
+        handler: Callable[[Any], T] | None = None,
         split_statements: bool = False,
         return_last: bool = True,
-    ) -> Any | list[Any] | None:
+    ) -> T | list[T] | None:
         """Run a command or a list of commands.
 
         Pass a list of SQL statements to the SQL parameter to get them to
         execute sequentially.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
```

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py` & `apache-airflow-providers-exasol-4.2.2rc1/airflow/providers/exasol/operators/exasol.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt` & `apache-airflow-providers-exasol-4.2.2rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml` & `apache-airflow-providers-exasol-4.2.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/setup.cfg` & `apache-airflow-providers-exasol-4.2.2rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-exasol-4.2.1rc1/setup.py` & `apache-airflow-providers-exasol-4.2.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-exasol package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.2.1"
+version = "4.2.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-exasol setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

