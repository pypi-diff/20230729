# Comparing `tmp/apache-airflow-providers-apache-spark-4.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.1rc1.tar", last modified: Tue Jun 20 11:41:30 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.2rc1.tar", last modified: Sat Jul 29 12:08:04 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.1.1rc1.tar` & `apache-airflow-providers-apache-spark-4.1.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.186280 apache-airflow-providers-apache-spark-4.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.187336 apache-airflow-providers-apache-spark-4.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.094919 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.096025 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.097257 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.132264 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3516 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.147465 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11383 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28715 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.159330 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9973 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8414 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.183585 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1874 2023-06-20 11:41:30.189305 apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.723019 apache-airflow-providers-apache-spark-4.1.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-07-29 12:08:04.723680 apache-airflow-providers-apache-spark-4.1.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.634056 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.635118 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.636143 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.666849 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.681199 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7037 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28687 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.692959 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9935 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8370 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.720342 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-spark-4.1.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-07-29 12:08:04.725683 apache-airflow-providers-apache-spark-4.1.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE` & `apache-airflow-providers-apache-spark-4.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.1.1"
+__version__ = "4.1.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-apache-spark:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "4.1.2",
             "4.1.1",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
@@ -88,8 +89,11 @@
                 "connection-type": "spark_sql",
             },
             {
                 "hook-class-name": "airflow.providers.apache.spark.hooks.spark_submit.SparkSubmitHook",
                 "connection-type": "spark",
             },
         ],
+        "additional-extras": [
+            {"name": "cncf.kubernetes", "dependencies": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]}
+        ],
     }
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
 from airflow.exceptions import AirflowException
 from airflow.providers.apache.spark.hooks.spark_submit import SparkSubmitHook
 
 
 class SparkJDBCHook(SparkSubmitHook):
     """
-    This hook extends the SparkSubmitHook specifically for performing data
-    transfers to/from JDBC-based databases with Apache Spark.
+    Extends the SparkSubmitHook for performing data transfers to/from JDBC-based databases with Apache Spark.
 
     :param spark_app_name: Name of the job (default airflow-spark-jdbc)
     :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark>`
         as configured in Airflow administration
     :param spark_conf: Any additional Spark configuration properties
     :param spark_py_files: Additional python files used (.zip, .egg, or .py)
     :param spark_files: Additional files to upload to the container running the job
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 if TYPE_CHECKING:
     from airflow.models.connection import Connection
 
 
 class SparkSqlHook(BaseHook):
     """
-    This hook is a wrapper around the spark-sql binary. It requires that the
-    "spark-sql" binary is in the PATH.
+    This hook is a wrapper around the spark-sql binary; requires the "spark-sql" binary to be in the PATH.
 
     :param sql: The SQL query to execute
     :param conf: arbitrary Spark configuration property
     :param conn_id: connection_id string
     :param total_executor_cores: (Standalone & Mesos only) Total cores for all executors
         (Default: all the available cores on the worker)
     :param executor_cores: (Standalone & YARN only) Number of cores per
@@ -108,16 +107,15 @@
         self._sp: Any = None
 
     def get_conn(self) -> Any:
         pass
 
     def _prepare_command(self, cmd: str | list[str]) -> list[str]:
         """
-        Construct the spark-sql command to execute. Verbose output is enabled
-        as default.
+        Construct the spark-sql command to execute. Verbose output is enabled as default.
 
         :param cmd: command to append to the spark-sql command
         :return: full command to be executed
         """
         connection_cmd = ["spark-sql"]
         if self._conf:
             for conf_el in self._conf.split(","):
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,22 @@
 from airflow.configuration import conf as airflow_conf
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.security.kerberos import renew_from_kt
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 with contextlib.suppress(ImportError, NameError):
-    from airflow.kubernetes import kube_client
+    from airflow.providers.cncf.kubernetes import kube_client
 
 ALLOWED_SPARK_BINARIES = ["spark-submit", "spark2-submit", "spark3-submit"]
 
 
 class SparkSubmitHook(BaseHook, LoggingMixin):
     """
-    This hook is a wrapper around the spark-submit binary to kick off a spark-submit job.
-    It requires that the "spark-submit" binary is in the PATH.
+    Wrap the spark-submit binary to kick off a spark-submit job; requires "spark-submit" binary in the PATH.
 
     :param conf: Arbitrary Spark configuration properties
     :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark>` as configured
         in Airflow administration. When an invalid connection_id is supplied, it will default
         to yarn.
     :param files: Upload additional files to the executor running the job, separated by a
         comma. Files will be placed in the working directory of each executor.
@@ -516,14 +515,15 @@
 
         if valid_response and not driver_found:
             self._driver_status = "UNKNOWN"
 
     def _start_driver_status_tracking(self) -> None:
         """
         Polls the driver based on self._driver_id to get the status.
+
         Finish successfully when the status is FINISHED.
         Finish failed when the status is ERROR/UNKNOWN/KILLED/FAILED.
 
         Possible status:
 
         SUBMITTED
             Submitted but not yet scheduled on a worker
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SparkJDBCOperator(SparkSubmitOperator):
     """
-    This operator extends the SparkSubmitOperator specifically for performing data
-    transfers to/from JDBC-based databases with Apache Spark. As with the
-    SparkSubmitOperator, it assumes that the "spark-submit" binary is available on the
-    PATH.
+    Extend the SparkSubmitOperator to perform data transfers to/from JDBC-based databases with Apache Spark.
+
+     As with the SparkSubmitOperator, it assumes that the "spark-submit" binary is available on the PATH.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SparkJDBCOperator`
 
     :param spark_app_name: Name of the job (default airflow-spark-jdbc)
     :param spark_conn_id: The :ref:`spark connection id <howto/connection:spark>`
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SparkSubmitOperator(BaseOperator):
     """
-    This hook is a wrapper around the spark-submit binary to kick off a spark-submit job.
-    It requires that the "spark-submit" binary is in the PATH.
+    Wrap the spark-submit binary to kick off a spark-submit job; requires "spark-submit" binary in the PATH.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SparkSubmitOperator`
 
     :param application: The application that submitted as a job, either jar or py file. (templated)
     :param conf: Arbitrary Spark configuration properties (templated)
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.2rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1rc1/setup.py` & `apache-airflow-providers-apache-spark-4.1.2rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-spark package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.1"
+version = "4.1.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-spark setup."""
     setup(
         version=version,
-        extras_require={},
+        extras_require={"cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]},
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.apache.spark",
                 "airflow.providers.apache.spark.*",
                 "airflow.providers.apache.spark_vendor",
                 "airflow.providers.apache.spark_vendor.*",
             ],
```

