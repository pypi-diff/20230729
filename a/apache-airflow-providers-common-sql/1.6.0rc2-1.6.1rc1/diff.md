# Comparing `tmp/apache-airflow-providers-common-sql-1.6.0rc2.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-common-sql-1.6.0rc2.tar", last modified: Thu Jul  6 04:50:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-common-sql-1.6.1rc1.tar", last modified: Sat Jul 29 12:08:15 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.6.0rc2.tar` & `apache-airflow-providers-common-sql-1.6.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:33.010937 apache-airflow-providers-common-sql-1.6.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-06 04:50:33.011661 apache-airflow-providers-common-sql-1.6.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3861 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.923094 apache-airflow-providers-common-sql-1.6.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.924264 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.925494 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.964214 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 18:48:54.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.970182 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23801 2023-07-05 14:56:16.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.976491 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46900 2023-07-05 14:56:16.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:32.982791 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:33.008107 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:32.000000 apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-common-sql-1.6.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-06 04:50:33.013643 apache-airflow-providers-common-sql-1.6.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-06 04:50:31.000000 apache-airflow-providers-common-sql-1.6.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.344153 apache-airflow-providers-common-sql-1.6.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-29 12:08:15.344852 apache-airflow-providers-common-sql-1.6.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.254916 apache-airflow-providers-common-sql-1.6.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.256070 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.257141 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.292983 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-29 12:01:19.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.299054 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24869 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.306104 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46908 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.312673 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.341060 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-common-sql-1.6.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-29 12:08:15.347635 apache-airflow-providers-common-sql-1.6.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/LICENSE` & `apache-airflow-providers-common-sql-1.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/MANIFEST.in` & `apache-airflow-providers-common-sql-1.6.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.0rc2
+Version: 1.6.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
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
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc2``
+Release: ``1.6.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/README.rst` & `apache-airflow-providers-common-sql-1.6.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc2``
+Release: ``1.6.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -87,8 +87,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-common-sql:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-sql",
         "name": "Common SQL",
         "description": "`Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__\n",
         "suspended": False,
         "versions": [
+            "1.6.1",
             "1.6.0",
             "1.5.2",
             "1.5.1",
             "1.5.0",
             "1.4.0",
             "1.3.4",
             "1.3.3",
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,26 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from contextlib import closing
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, Protocol, Sequence, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Mapping,
+    Protocol,
+    Sequence,
+    TypeVar,
+    cast,
+    overload,
+)
 from urllib.parse import urlparse
 
 import sqlparse
 from packaging.version import Version
 from sqlalchemy import create_engine
 
 from airflow import AirflowException
@@ -30,14 +41,17 @@
 from airflow.version import version
 
 if TYPE_CHECKING:
     from airflow.providers.openlineage.extractors import OperatorLineage
     from airflow.providers.openlineage.sqlparser import DatabaseInfo
 
 
+T = TypeVar("T")
+
+
 def return_single_query_results(sql: str | Iterable[str], return_last: bool, split_statements: bool):
     """
     Determines when results of single query only should be returned.
 
     For compatibility reasons, the behaviour of the DBAPIHook is somewhat confusing.
     In some cases, when multiple queries are run, the return value will be an iterable (list) of results
     -- one for each query. However, in other cases, when single query is run, the return value will be just
@@ -180,15 +194,15 @@
         :param engine_kwargs: Kwargs used in :func:`~sqlalchemy.create_engine`.
         :return: the created engine.
         """
         if engine_kwargs is None:
             engine_kwargs = {}
         return create_engine(self.get_uri(), **engine_kwargs)
 
-    def get_pandas_df(self, sql, parameters=None, **kwargs):
+    def get_pandas_df(self, sql, parameters: Iterable | Mapping[str, Any] | None = None, **kwargs):
         """
         Executes the sql and returns a pandas dataframe.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         :param kwargs: (optional) passed into pandas.io.sql.read_sql method
@@ -200,15 +214,17 @@
                 "pandas library not installed, run: pip install "
                 "'apache-airflow-providers-common-sql[pandas]'."
             )
 
         with closing(self.get_conn()) as conn:
             return psql.read_sql(sql, con=conn, params=parameters, **kwargs)
 
-    def get_pandas_df_by_chunks(self, sql, parameters=None, *, chunksize, **kwargs):
+    def get_pandas_df_by_chunks(
+        self, sql, parameters: Iterable | Mapping[str, Any] | None = None, *, chunksize: int | None, **kwargs
+    ):
         """
         Executes the sql and returns a generator.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
         :param parameters: The parameters to render the SQL query with
         :param chunksize: number of rows to include in  each chunk
@@ -224,25 +240,25 @@
 
         with closing(self.get_conn()) as conn:
             yield from psql.read_sql(sql, con=conn, params=parameters, chunksize=chunksize, **kwargs)
 
     def get_records(
         self,
         sql: str | list[str],
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
     ) -> Any:
         """
         Executes the sql and returns a set of records.
 
         :param sql: the sql statement to be executed (str) or a list of sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         return self.run(sql=sql, parameters=parameters, handler=fetch_all_handler)
 
-    def get_first(self, sql: str | list[str], parameters: Iterable | Mapping | None = None) -> Any:
+    def get_first(self, sql: str | list[str], parameters: Iterable | Mapping[str, Any] | None = None) -> Any:
         """
         Executes the sql and returns the first resulting row.
 
         :param sql: the sql statement to be executed (str) or a list of sql statements to execute
         :param parameters: The parameters to render the SQL query with.
         """
         return self.run(sql=sql, parameters=parameters, handler=fetch_one_handler)
@@ -264,23 +280,47 @@
 
     @property
     def last_description(self) -> Sequence[Sequence] | None:
         if not self.descriptions:
             return None
         return self.descriptions[-1]
 
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
 
         Pass a list of SQL statements to the sql parameter to get them to
         execute sequentially.
 
         The method will return either single query results (typically list of rows) or list of those results
         where each element in the list are results of one of the queries (typically list of list of rows :D)
@@ -554,17 +594,23 @@
         This method is called only on completion of the task.
 
         :param task_instance: this may be used to retrieve additional information
             that is collected during runtime of the task
         """
 
     @staticmethod
-    def get_openlineage_authority_part(connection) -> str:
+    def get_openlineage_authority_part(connection, default_port: int | None = None) -> str:
         """
         This method serves as common method for several hooks to get authority part from Airflow Connection.
 
         The authority represents the hostname and port of the connection
         and conforms OpenLineage naming convention for a number of databases (e.g. MySQL, Postgres, Trino).
+
+        :param default_port: (optional) used if no port parsed from connection URI
         """
         parsed = urlparse(connection.get_uri())
-        authority = f"{parsed.hostname}:{parsed.port}"
+        port = parsed.port or default_port
+        if port:
+            authority = f"{parsed.hostname}:{port}"
+        else:
+            authority = parsed.hostname
         return authority
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,20 +326,20 @@
             database=self.database,
             sqlalchemy_engine=hook.get_sqlalchemy_engine(),
         )
 
         return operator_lineage
 
     def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage | None:
-        operator_lineage = self.get_openlineage_facets_on_start() or OperatorLineage()
-
         try:
             from airflow.providers.openlineage.extractors import OperatorLineage
         except ImportError:
-            return operator_lineage
+            return None
+
+        operator_lineage = self.get_openlineage_facets_on_start() or OperatorLineage()
 
         hook = self.get_db_hook()
         try:
             database_specific_lineage = hook.get_openlineage_database_specific_lineage(task_instance)
         except AttributeError:
             database_specific_lineage = None
 
@@ -758,15 +758,15 @@
 
     def __init__(
         self,
         *,
         sql: str,
         conn_id: str | None = None,
         database: str | None = None,
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(conn_id=conn_id, database=database, **kwargs)
         self.sql = sql
         self.parameters = parameters
 
     def execute(self, context: Context):
@@ -1125,15 +1125,15 @@
         self,
         *,
         sql: str,
         follow_task_ids_if_true: list[str],
         follow_task_ids_if_false: list[str],
         conn_id: str = "default_conn_id",
         database: str | None = None,
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(conn_id=conn_id, database=database, **kwargs)
         self.sql = sql
         self.parameters = parameters
         self.follow_task_ids_if_true = follow_task_ids_if_true
         self.follow_task_ids_if_false = follow_task_ids_if_false
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.0rc2
+Version: 1.6.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
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
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.0rc2``
+Release: ``1.6.1rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/pyproject.toml` & `apache-airflow-providers-common-sql-1.6.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/setup.cfg` & `apache-airflow-providers-common-sql-1.6.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.common.sql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.common.sql
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-common-sql-1.6.0rc2/setup.py` & `apache-airflow-providers-common-sql-1.6.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-common-sql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.6.0"
+version = "1.6.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-common-sql setup."""
     setup(
         version=version,
         extras_require={
```

