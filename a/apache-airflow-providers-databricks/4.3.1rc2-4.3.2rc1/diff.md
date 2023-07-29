# Comparing `tmp/apache-airflow-providers-databricks-4.3.1rc2.tar.gz` & `tmp/apache-airflow-providers-databricks-4.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-databricks-4.3.1rc2.tar", last modified: Thu Jul  6 04:50:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-databricks-4.3.2rc1.tar", last modified: Sat Jul 29 12:08:19 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.3.1rc2.tar` & `apache-airflow-providers-databricks-4.3.2rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:35.029129 apache-airflow-providers-databricks-4.3.1rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.1rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5810 2023-07-06 04:50:35.029888 apache-airflow-providers-databricks-4.3.1rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4129 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.896378 apache-airflow-providers-databricks-4.3.1rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.897567 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.943174 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-05 18:49:44.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.957520 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16773 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26696 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.971570 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33530 2023-07-05 07:19:39.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13181 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    17010 2023-06-29 14:43:21.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.983172 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9827 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.990705 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:34.999085 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:35.026528 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5810 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:34.000000 apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-databricks-4.3.1rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-06 04:50:35.032113 apache-airflow-providers-databricks-4.3.1rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-07-06 04:50:33.000000 apache-airflow-providers-databricks-4.3.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.117853 apache-airflow-providers-databricks-4.3.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:17.000000 apache-airflow-providers-databricks-4.3.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-29 12:08:19.118378 apache-airflow-providers-databricks-4.3.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-07-29 12:08:17.000000 apache-airflow-providers-databricks-4.3.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.002577 apache-airflow-providers-databricks-4.3.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.004010 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.046338 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-07-29 12:01:19.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-07-29 12:08:17.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.058464 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16773 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26696 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)    10030 2023-07-26 06:59:50.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.070450 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33338 2023-07-26 06:59:50.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13181 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    17010 2023-06-29 14:43:21.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.079270 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9827 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.084848 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.090419 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-29 05:49:30.000000 apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:19.115640 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:18.000000 apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-databricks-4.3.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-29 12:08:19.120221 apache-airflow-providers-databricks-4.3.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-29 12:08:17.000000 apache-airflow-providers-databricks-4.3.2rc1/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/LICENSE` & `apache-airflow-providers-databricks-4.3.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/MANIFEST.in` & `apache-airflow-providers-databricks-4.3.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/PKG-INFO` & `apache-airflow-providers-databricks-4.3.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.1rc2
+Version: 4.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc2``
+Release: ``4.3.2rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -125,8 +125,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/README.rst` & `apache-airflow-providers-databricks-4.3.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc2``
+Release: ``4.3.2rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -90,8 +90,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.1"
+__version__ = "4.3.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-databricks:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.4.0",
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from contextlib import closing
 from copy import copy
-from typing import Any, Callable, Iterable, Mapping
+from typing import Any, Callable, Iterable, Mapping, TypeVar, overload
 
 from databricks import sql  # type: ignore[attr-defined]
 from databricks.sql.client import Connection  # type: ignore[attr-defined]
 
 from airflow.exceptions import AirflowException
 from airflow.providers.common.sql.hooks.sql import DbApiHook, return_single_query_results
 from airflow.providers.databricks.hooks.databricks_base import BaseDatabricksHook
 
 LIST_SQL_ENDPOINTS_ENDPOINT = ("GET", "api/2.0/sql/endpoints")
 
 
+T = TypeVar("T")
+
+
 class DatabricksSqlHook(BaseDatabricksHook, DbApiHook):
     """Hook to interact with Databricks SQL.
 
     :param databricks_conn_id: Reference to the
         :ref:`Databricks connection <howto/connection:databricks>`.
     :param http_path: Optional string specifying HTTP path of Databricks SQL Endpoint or cluster.
         If not specified, it should be either specified in the Databricks connection's extra parameters,
@@ -134,23 +137,47 @@
                 http_headers=self.http_headers,
                 _user_agent_entry=self.user_agent_value,
                 **self._get_extra_config(),
                 **self.additional_params,
             )
         return self._sql_conn
 
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
         split_statements: bool = True,
         return_last: bool = True,
-    ) -> Any | list[Any] | None:
+    ) -> T | list[T] | None:
         """Runs a command or a list of commands.
 
         Pass a list of SQL statements to the SQL parameter to get them to
         execute sequentially.
 
         :param sql: the sql statement to be executed (str) or a list of
             sql statements to execute
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,14 +667,18 @@
             del self.json["job_name"]
         self.run_id = hook.run_now(self.json)
         if self.deferrable:
             _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
         else:
             _handle_databricks_operator_execution(self, hook, self.log, context)
 
+    def execute_complete(self, context: Context, event: dict[str, Any] | None = None) -> None:
+        if event:
+            _handle_deferrable_databricks_operator_completion(event, self.log)
+
     def on_kill(self):
         if self.run_id:
             self._hook.cancel_run(self.run_id)
             self.log.info(
                 "Task: %s with run_id: %s was requested to be cancelled.", self.task_id, self.run_id
             )
         else:
@@ -689,15 +693,7 @@
             "`DatabricksRunNowDeferrableOperator` has been deprecated. "
             "Please use `airflow.providers.databricks.operators.DatabricksRunNowOperator` with "
             "`deferrable=True` instead.",
             AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         super().__init__(deferrable=True, *args, **kwargs)
-
-    def execute(self, context):
-        hook = self._get_hook(caller="DatabricksRunNowDeferrableOperator")
-        self.run_id = hook.run_now(self.json)
-        _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
-
-    def execute_complete(self, context: dict | None, event: dict):
-        _handle_deferrable_databricks_operator_completion(event, self.log)
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.3.2rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.1rc2
+Version: 4.3.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.1rc2``
+Release: ``4.3.2rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -125,8 +125,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.3.2rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/pyproject.toml` & `apache-airflow-providers-databricks-4.3.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/setup.cfg` & `apache-airflow-providers-databricks-4.3.2rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.1/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -57,10 +57,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.databricks
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-databricks-4.3.1rc2/setup.py` & `apache-airflow-providers-databricks-4.3.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-databricks package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.1"
+version = "4.3.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-databricks setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

