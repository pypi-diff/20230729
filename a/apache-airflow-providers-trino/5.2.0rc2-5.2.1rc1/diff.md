# Comparing `tmp/apache-airflow-providers-trino-5.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-trino-5.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-trino-5.2.0rc2.tar", last modified: Thu Jul  6 04:51:40 2023, max compression
+gzip compressed data, was "apache-airflow-providers-trino-5.2.1rc1.tar", last modified: Sat Jul 29 12:09:14 2023, max compression
```

## Comparing `apache-airflow-providers-trino-5.2.0rc2.tar` & `apache-airflow-providers-trino-5.2.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.318871 apache-airflow-providers-trino-5.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5821 2023-07-06 04:51:40.319536 apache-airflow-providers-trino-5.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4137 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.233436 apache-airflow-providers-trino-5.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.237418 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.273142 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-07-05 18:55:40.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3068 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.278826 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-06-25 14:35:06.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.284621 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.290307 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:40.315854 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5821 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:40.000000 apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-trino-5.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1999 2023-07-06 04:51:40.321552 apache-airflow-providers-trino-5.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1767 2023-07-06 04:51:39.000000 apache-airflow-providers-trino-5.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.456011 apache-airflow-providers-trino-5.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-29 12:09:14.456555 apache-airflow-providers-trino-5.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.378819 apache-airflow-providers-trino-5.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.380084 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.413526 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3089 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.419229 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9073 2023-07-26 06:59:50.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.424892 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-16 17:25:26.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.430414 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4999 2023-06-02 11:31:21.000000 apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:14.453338 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5821 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:14.000000 apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-trino-5.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-29 12:09:14.458548 apache-airflow-providers-trino-5.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-29 12:09:13.000000 apache-airflow-providers-trino-5.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/LICENSE` & `apache-airflow-providers-trino-5.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/MANIFEST.in` & `apache-airflow-providers-trino-5.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/PKG-INFO` & `apache-airflow-providers-trino-5.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.0rc2
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc2``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -126,8 +126,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_          ``google``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/README.rst` & `apache-airflow-providers-trino-5.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc2``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -90,8 +90,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_          ``google``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.2.0"
+__version__ = "5.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-trino:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/get_provider_info.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-trino",
         "name": "Trino",
         "description": "`Trino <https://trino.io/>`__\n",
         "suspended": False,
         "versions": [
+            "5.2.1",
             "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.3.2",
             "4.3.1",
             "4.3.0",
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/hooks/trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/hooks/trino.py`

 * *Files 4% similar despite different names*

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
 
 import trino
 from trino.exceptions import DatabaseError
 from trino.transaction import IsolationLevel
 
 from airflow import AirflowException
 from airflow.configuration import conf
 from airflow.models import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.utils.operator_helpers import AIRFLOW_VAR_NAME_FORMAT_MAPPING, DEFAULT_FORMAT_PREFIX
 
+T = TypeVar("T")
+
 
 def generate_trino_client_info() -> str:
     """Return json string with dag_id, task_id, execution_date and try_number."""
     context_var = {
         format_map["default"].replace(DEFAULT_FORMAT_PREFIX, ""): os.environ.get(
             format_map["env_var_format"], ""
         )
@@ -150,33 +152,35 @@
         db = self.get_connection(self.trino_conn_id)  # type: ignore[attr-defined]
         isolation_level = db.extra_dejson.get("isolation_level", "AUTOCOMMIT").upper()
         return getattr(IsolationLevel, isolation_level, IsolationLevel.AUTOCOMMIT)
 
     def get_records(
         self,
         sql: str | list[str] = "",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
     ) -> Any:
         if not isinstance(sql, str):
             raise ValueError(f"The sql in Trino Hook must be a string and is {sql}!")
         try:
             return super().get_records(self.strip_sql_string(sql), parameters)
         except DatabaseError as e:
             raise TrinoException(e)
 
-    def get_first(self, sql: str | list[str] = "", parameters: Iterable | Mapping | None = None) -> Any:
+    def get_first(
+        self, sql: str | list[str] = "", parameters: Iterable | Mapping[str, Any] | None = None
+    ) -> Any:
         if not isinstance(sql, str):
             raise ValueError(f"The sql in Trino Hook must be a string and is {sql}!")
         try:
             return super().get_first(self.strip_sql_string(sql), parameters)
         except DatabaseError as e:
             raise TrinoException(e)
 
     def get_pandas_df(
-        self, sql: str = "", parameters: Iterable | Mapping | None = None, **kwargs
+        self, sql: str = "", parameters: Iterable | Mapping[str, Any] | None = None, **kwargs
     ):  # type: ignore[override]
         import pandas
 
         cursor = self.get_cursor()
         try:
             cursor.execute(self.strip_sql_string(sql), parameters)
             data = cursor.fetchall()
@@ -186,32 +190,14 @@
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
@@ -236,15 +222,14 @@
             commit_every = 0
 
         super().insert_rows(table, rows, target_fields, commit_every, replace)
 
     @staticmethod
     def _serialize_cell(cell: Any, conn: Connection | None = None) -> Any:
         """
-        Trino will adapt all arguments to the execute() method internally,
-        hence we return cell without any conversion.
+        Trino will adapt all execute() args internally, hence we return cell without any conversion.
 
         :param cell: The cell to insert into the table
         :param conn: The database connection
         :return: The cell
         """
         return cell
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/operators/trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/operators/trino.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 from airflow.providers.trino.hooks.trino import TrinoHook
 
 
 class TrinoOperator(SQLExecuteQueryOperator):
     """
     Executes sql code using a specific Trino query Engine.
 
+    This class is deprecated.
+
+    Please use :class:`airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
+
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:TrinoOperator`
 
     :param sql: the SQL code to be executed as a single string, or
         a list of str (sql statements), or a reference to a template file.
     :param trino_conn_id: id of the connection config for the target Trino
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/__init__.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/airflow/providers/trino/transfers/gcs_to_trino.py` & `apache-airflow-providers-trino-5.2.1rc1/airflow/providers/trino/transfers/gcs_to_trino.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/PKG-INFO` & `apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-trino
-Version: 5.2.0rc2
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-trino package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-trino``
 
-Release: ``5.2.0rc2``
+Release: ``5.2.1rc1``
 
 
 `Trino <https://trino.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``trino`` provider. All classes for this provider package
 are in ``airflow.providers.trino`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -126,8 +126,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_          ``google``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/apache_airflow_providers_trino.egg-info/SOURCES.txt` & `apache-airflow-providers-trino-5.2.1rc1/apache_airflow_providers_trino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-trino-5.2.0rc2/pyproject.toml` & `apache-airflow-providers-trino-5.2.1rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
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
 
@@ -69,14 +70,16 @@
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
@@ -95,54 +98,28 @@
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

### Comparing `apache-airflow-providers-trino-5.2.0rc2/setup.cfg` & `apache-airflow-providers-trino-5.2.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-trino/5.2.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.trino.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.trino
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-trino-5.2.0rc2/setup.py` & `apache-airflow-providers-trino-5.2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-trino package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.2.0"
+version = "5.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-trino setup."""
     setup(
         version=version,
         extras_require={
```

