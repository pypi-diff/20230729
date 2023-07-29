# Comparing `tmp/apache-airflow-providers-postgres-5.5.2rc2.tar.gz` & `tmp/apache-airflow-providers-postgres-5.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-postgres-5.5.2rc2.tar", last modified: Thu Jul  6 04:51:20 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.6.0rc1.tar", last modified: Sat Jul 29 12:08:55 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.5.2rc2.tar` & `apache-airflow-providers-postgres-5.6.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.382146 apache-airflow-providers-postgres-5.5.2rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.382738 apache-airflow-providers-postgres-5.5.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4113 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.304592 apache-airflow-providers-postgres-5.5.2rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.305843 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.340819 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 04:42:33.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.347351 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13342 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.353272 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3467 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.379739 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2012 2023-07-06 04:51:20.384790 apache-airflow-providers-postgres-5.5.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.714646 apache-airflow-providers-postgres-5.6.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.6.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-29 12:08:55.715213 apache-airflow-providers-postgres-5.6.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4256 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.643536 apache-airflow-providers-postgres-5.6.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.644825 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.676948 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-29 12:01:19.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.682658 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15392 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.688432 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-07-16 17:25:26.000000 apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:55.712231 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      249 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:55.000000 apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-postgres-5.6.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-29 12:08:55.717130 apache-airflow-providers-postgres-5.6.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-07-29 12:08:54.000000 apache-airflow-providers-postgres-5.6.0rc1/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/LICENSE` & `apache-airflow-providers-postgres-5.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in` & `apache-airflow-providers-postgres-5.6.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/PKG-INFO` & `apache-airflow-providers-postgres-5.6.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.2rc2
+Version: 5.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
+Provides-Extra: openlineage
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
@@ -68,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2rc2``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -117,16 +118,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-postgres[amazon]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_          ``amazon``
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_            ``amazon``
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/README.rst` & `apache-airflow-providers-postgres-5.6.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2rc2``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,16 +81,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-postgres[amazon]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_          ``amazon``
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_            ``amazon``
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.5.2"
+__version__ = "5.6.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-postgres:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-postgres",
         "name": "PostgreSQL",
         "description": "`PostgreSQL <https://www.postgresql.org/>`__\n",
         "suspended": False,
         "versions": [
+            "5.6.0",
             "5.5.2",
             "5.5.1",
             "5.5.0",
             "5.4.0",
             "5.3.1",
             "5.3.0",
             "5.2.2",
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/hooks/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,29 @@
 # under the License.
 from __future__ import annotations
 
 import os
 import warnings
 from contextlib import closing
 from copy import deepcopy
-from typing import Any, Iterable, Union
+from typing import TYPE_CHECKING, Any, Iterable, Union
 
 import psycopg2
 import psycopg2.extensions
 import psycopg2.extras
 from psycopg2.extensions import connection
 from psycopg2.extras import DictCursor, NamedTupleCursor, RealDictCursor
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models.connection import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
+if TYPE_CHECKING:
+    from airflow.providers.openlineage.sqlparser import DatabaseInfo
+
 CursorType = Union[DictCursor, RealDictCursor, NamedTupleCursor]
 
 
 class PostgresHook(DbApiHook):
     """Interact with Postgres.
 
     You can specify ssl parameters in the extra field of your connection
@@ -313,7 +316,50 @@
             if replace_target:
                 replace_target_str = ", ".join(f"{col} = excluded.{col}" for col in replace_target)
                 sql += f"{on_conflict_str} DO UPDATE SET {replace_target_str}"
             else:
                 sql += f"{on_conflict_str} DO NOTHING"
 
         return sql
+
+    def get_openlineage_database_info(self, connection) -> DatabaseInfo:
+        """Returns Postgres/Redshift specific information for OpenLineage."""
+        from airflow.providers.openlineage.sqlparser import DatabaseInfo
+
+        is_redshift = connection.extra_dejson.get("redshift", False)
+
+        if is_redshift:
+            authority = self._get_openlineage_redshift_authority_part(connection)
+        else:
+            authority = DbApiHook.get_openlineage_authority_part(connection, default_port=5432)
+
+        return DatabaseInfo(
+            scheme="postgres" if not is_redshift else "redshift",
+            authority=authority,
+            database=self.database or connection.schema,
+        )
+
+    def _get_openlineage_redshift_authority_part(self, connection) -> str:
+        try:
+            from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
+        except ImportError:
+            from airflow.exceptions import AirflowException
+
+            raise AirflowException(
+                "apache-airflow-providers-amazon not installed, run: "
+                "pip install 'apache-airflow-providers-postgres[amazon]'."
+            )
+        aws_conn_id = connection.extra_dejson.get("aws_conn_id", "aws_default")
+
+        port = connection.port or 5439
+        cluster_identifier = connection.extra_dejson.get("cluster-identifier", connection.host.split(".")[0])
+        region_name = AwsBaseHook(aws_conn_id=aws_conn_id).region_name
+
+        return f"{cluster_identifier}.{region_name}:{port}"
+
+    def get_openlineage_database_dialect(self, connection) -> str:
+        """Returns postgres/redshift dialect."""
+        return "redshift" if connection.extra_dejson.get("redshift", False) else "postgres"
+
+    def get_openlineage_default_schema(self) -> str | None:
+        """Returns current schema. This is usually changed with ``SEARCH_PATH`` parameter."""
+        return self.get_first("SELECT CURRENT_SCHEMA;")[0]
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.6.0rc1/airflow/providers/postgres/operators/postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class PostgresOperator(SQLExecuteQueryOperator):
     """
     Executes sql code in a specific Postgres database.
 
+    This class is deprecated.
+
+    Please use :class:`airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
+
     :param sql: the SQL code to be executed as a single string, or
         a list of str (sql statements), or a reference to a template file.
         Template references are recognized by str ending in '.sql'
     :param postgres_conn_id: The :ref:`postgres conn id <howto/connection:postgres>`
         reference to a specific postgres database.
     :param autocommit: if True, each command is automatically committed.
         (default value: False)
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.2rc2
+Version: 5.6.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
+Provides-Extra: openlineage
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
@@ -68,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.2rc2``
+Release: ``5.6.0rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -117,16 +118,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-postgres[amazon]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_          ``amazon``
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-amazon <https://airflow.apache.org/docs/apache-airflow-providers-amazon>`_            ``amazon``
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.6.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml` & `apache-airflow-providers-postgres-5.6.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/setup.cfg` & `apache-airflow-providers-postgres-5.6.0rc1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.6.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.5.2rc2/setup.py` & `apache-airflow-providers-postgres-5.6.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,24 +22,25 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-postgres package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.5.2"
+version = "5.6.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-postgres setup."""
     setup(
         version=version,
         extras_require={
             "amazon": ["apache-airflow-providers-amazon>=2.6.0"],
             "common.sql": ["apache-airflow-providers-common-sql"],
+            "openlineage": ["apache-airflow-providers-openlineage"],
         },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.postgres",
                 "airflow.providers.postgres.*",
                 "airflow.providers.postgres_vendor",
                 "airflow.providers.postgres_vendor.*",
```

