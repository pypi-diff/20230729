# Comparing `tmp/apache-airflow-providers-presto-5.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-presto-5.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-presto-5.1.1rc1.tar", last modified: Tue Jun 20 11:42:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-presto-5.1.2rc1.tar", last modified: Sat Jul 29 12:08:57 2023, max compression
```

## Comparing `apache-airflow-providers-presto-5.1.1rc1.tar` & `apache-airflow-providers-presto-5.1.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.163627 apache-airflow-providers-presto-5.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.164703 apache-airflow-providers-presto-5.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12698 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.088803 apache-airflow-providers-presto-5.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.090015 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.122350 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.128435 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.136308 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.160935 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      210 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-presto-5.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 11:42:56.166648 apache-airflow-providers-presto-5.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.574103 apache-airflow-providers-presto-5.1.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-07-29 12:08:57.574694 apache-airflow-providers-presto-5.1.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.502162 apache-airflow-providers-presto-5.1.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.503250 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.534941 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.540718 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8316 2023-07-26 06:59:50.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.547217 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/gcs_to_presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:57.571464 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5841 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:57.000000 apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-presto-5.1.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-29 12:08:57.576640 apache-airflow-providers-presto-5.1.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-07-29 12:08:56.000000 apache-airflow-providers-presto-5.1.2rc1/setup.py
```

### Comparing `apache-airflow-providers-presto-5.1.1rc1/LICENSE` & `apache-airflow-providers-presto-5.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in` & `apache-airflow-providers-presto-5.1.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.1.1"
+__version__ = "5.1.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-presto:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-presto",
         "name": "Presto",
         "description": "`Presto <https://prestodb.github.io/>`__\n",
         "suspended": False,
         "versions": [
+            "5.1.2",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.2.2",
             "4.2.1",
             "4.2.0",
             "4.1.0",
```

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/hooks/presto.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import json
 import os
-from typing import Any, Callable, Iterable, Mapping
+from typing import Any, Iterable, Mapping, TypeVar
 
 import prestodb
 from prestodb.exceptions import DatabaseError
 from prestodb.transaction import IsolationLevel
 
 from airflow import AirflowException
 from airflow.configuration import conf
 from airflow.models import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.utils.operator_helpers import AIRFLOW_VAR_NAME_FORMAT_MAPPING, DEFAULT_FORMAT_PREFIX
 
+T = TypeVar("T")
+
 
 def generate_presto_client_info() -> str:
     """Return json string with dag_id, task_id, execution_date and try_number."""
     context_var = {
         format_map["default"].replace(DEFAULT_FORMAT_PREFIX, ""): os.environ.get(
             format_map["env_var_format"], ""
         )
@@ -132,24 +134,26 @@
         db = self.get_connection(self.presto_conn_id)  # type: ignore[attr-defined]
         isolation_level = db.extra_dejson.get("isolation_level", "AUTOCOMMIT").upper()
         return getattr(IsolationLevel, isolation_level, IsolationLevel.AUTOCOMMIT)
 
     def get_records(
         self,
         sql: str | list[str] = "",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
     ) -> Any:
         if not isinstance(sql, str):
             raise ValueError(f"The sql in Presto Hook must be a string and is {sql}!")
         try:
             return super().get_records(self.strip_sql_string(sql), parameters)
         except DatabaseError as e:
             raise PrestoException(e)
 
-    def get_first(self, sql: str | list[str] = "", parameters: Iterable | Mapping | None = None) -> Any:
+    def get_first(
+        self, sql: str | list[str] = "", parameters: Iterable | Mapping[str, Any] | None = None
+    ) -> Any:
         if not isinstance(sql, str):
             raise ValueError(f"The sql in Presto Hook must be a string and is {sql}!")
         try:
             return super().get_first(self.strip_sql_string(sql), parameters)
         except DatabaseError as e:
             raise PrestoException(e)
 
@@ -166,32 +170,14 @@
         if data:
             df = pandas.DataFrame(data, **kwargs)
             df.columns = [c[0] for c in column_descriptions]
         else:
             df = pandas.DataFrame(**kwargs)
         return df
 
-    def run(
-        self,
-        sql: str | Iterable[str],
-        autocommit: bool = False,
-        parameters: Iterable | Mapping | None = None,
-        handler: Callable | None = None,
-        split_statements: bool = False,
-        return_last: bool = True,
-    ) -> Any | list[Any] | None:
-        return super().run(
-            sql=sql,
-            autocommit=autocommit,
-            parameters=parameters,
-            handler=handler,
-            split_statements=split_statements,
-            return_last=return_last,
-        )
-
     def insert_rows(
         self,
         table: str,
         rows: Iterable[tuple],
         target_fields: Iterable[str] | None = None,
         commit_every: int = 0,
         replace: bool = False,
@@ -216,15 +202,14 @@
             commit_every = 0
 
         super().insert_rows(table, rows, target_fields, commit_every)
 
     @staticmethod
     def _serialize_cell(cell: Any, conn: Connection | None = None) -> Any:
         """
-        Presto will adapt all arguments to the execute() method internally,
-        hence we return cell without any conversion.
+        Presto will adapt all execute() args internally, hence we return cell without any conversion.
 
         :param cell: The cell to insert into the table
         :param conn: The database connection
         :return: The cell
         """
         return cell
```

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py` & `apache-airflow-providers-presto-5.1.2rc1/airflow/providers/presto/transfers/gcs_to_presto.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt` & `apache-airflow-providers-presto-5.1.2rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1rc1/pyproject.toml` & `apache-airflow-providers-presto-5.1.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-presto-5.1.1rc1/setup.cfg` & `apache-airflow-providers-presto-5.1.2rc1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-presto-5.1.1rc1/setup.py` & `apache-airflow-providers-presto-5.1.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-presto package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.1"
+version = "5.1.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-presto setup."""
     setup(
         version=version,
         extras_require={
```

