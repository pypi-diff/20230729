# Comparing `tmp/apache-airflow-providers-snowflake-4.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.3.1rc1.tar", last modified: Wed Jul 12 19:13:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.4.0rc1.tar", last modified: Sat Jul 29 12:09:08 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.3.1rc1.tar` & `apache-airflow-providers-snowflake-4.4.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.488646 apache-airflow-providers-snowflake-4.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5873 2023-07-12 19:13:35.489212 apache-airflow-providers-snowflake-4.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4174 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.381882 apache-airflow-providers-snowflake-4.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.383080 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.419481 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-12 19:08:31.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4970 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.428181 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18283 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.437071 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.448706 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5083 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.454531 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.462898 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.486050 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5873 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-12 19:13:35.491041 apache-airflow-providers-snowflake-4.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.761202 apache-airflow-providers-snowflake-4.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.761764 apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.655883 apache-airflow-providers-snowflake-4.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.657068 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.694162 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 12:01:19.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4991 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.703082 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.708868 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24878 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.720597 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.726145 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.734576 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.758540 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-29 12:09:08.763589 apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/LICENSE` & `apache-airflow-providers-snowflake-4.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/MANIFEST.in` & `apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.1rc1
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: common.sql
+Provides-Extra: openlineage
 Provides-Extra: slack
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -68,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.1rc1``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -118,16 +119,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-snowflake[common.sql]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/README.rst` & `apache-airflow-providers-snowflake-4.4.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.1rc1``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -82,16 +82,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-snowflake[common.sql]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.1"
+__version__ = "4.4.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-snowflake:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.4.0",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.5",
             "4.0.4",
             "4.0.3",
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,27 +18,33 @@
 from __future__ import annotations
 
 import os
 from contextlib import closing, contextmanager
 from functools import wraps
 from io import StringIO
 from pathlib import Path
-from typing import Any, Callable, Iterable, Mapping
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Mapping, TypeVar, overload
+from urllib.parse import urlparse
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from snowflake import connector
 from snowflake.connector import DictCursor, SnowflakeConnection, util_text
 from snowflake.sqlalchemy import URL
 from sqlalchemy import create_engine
 
 from airflow import AirflowException
 from airflow.providers.common.sql.hooks.sql import DbApiHook, return_single_query_results
 from airflow.utils.strings import to_boolean
 
+T = TypeVar("T")
+if TYPE_CHECKING:
+    from airflow.providers.openlineage.extractors import OperatorLineage
+    from airflow.providers.openlineage.sqlparser import DatabaseInfo
+
 
 def _try_to_boolean(value: Any):
     if isinstance(value, (str, type(None))):
         return to_boolean(value)
     return value
 
 
@@ -317,24 +323,50 @@
     def set_autocommit(self, conn, autocommit: Any) -> None:
         conn.autocommit(autocommit)
         conn.autocommit_mode = autocommit
 
     def get_autocommit(self, conn):
         return getattr(conn, "autocommit_mode", False)
 
+    @overload
+    def run(
+        self,
+        sql: str | Iterable[str],
+        autocommit: bool = ...,
+        parameters: Iterable | Mapping[str, Any] | None = ...,
+        handler: None = ...,
+        split_statements: bool = ...,
+        return_last: bool = ...,
+        return_dictionaries: bool = ...,
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
+        return_dictionaries: bool = ...,
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
         return_dictionaries: bool = False,
-    ) -> Any | list[Any] | None:
+    ) -> T | list[T] | None:
         """Runs a command or a list of commands.
 
         Pass a list of SQL statements to the SQL parameter to get them to
         execute sequentially. The variable ``execution_info`` is returned so
         that it can be used in the Operators to modify the behavior depending on
         the result of the query (i.e fail the operator if the copy has processed
         0 files).
@@ -416,7 +448,72 @@
                 cursor = conn.cursor(DictCursor)
             else:
                 cursor = conn.cursor()
             yield cursor
         finally:
             if cursor is not None:
                 cursor.close()
+
+    def get_openlineage_database_info(self, connection) -> DatabaseInfo:
+        from airflow.providers.openlineage.sqlparser import DatabaseInfo
+
+        database = self.database or self._get_field(connection.extra_dejson, "database")
+
+        return DatabaseInfo(
+            scheme=self.get_openlineage_database_dialect(connection),
+            authority=self._get_openlineage_authority(connection),
+            information_schema_columns=[
+                "table_schema",
+                "table_name",
+                "column_name",
+                "ordinal_position",
+                "data_type",
+            ],
+            database=database,
+            is_information_schema_cross_db=True,
+            is_uppercase_names=True,
+        )
+
+    def get_openlineage_database_dialect(self, _) -> str:
+        return "snowflake"
+
+    def get_openlineage_default_schema(self) -> str | None:
+        """
+        Attempts to get current schema.
+
+        Usually ``SELECT CURRENT_SCHEMA();`` should work.
+        However, apparently you may set ``database`` without ``schema``
+        and get results from ``SELECT CURRENT_SCHEMAS();`` but not
+        from ``SELECT CURRENT_SCHEMA();``.
+        It still may return nothing if no database is set in connection.
+        """
+        schema = self._get_conn_params()["schema"]
+        if not schema:
+            current_schemas = self.get_first("SELECT PARSE_JSON(CURRENT_SCHEMAS())[0]::string;")[0]
+            if current_schemas:
+                _, schema = current_schemas.split(".")
+        return schema
+
+    def _get_openlineage_authority(self, _) -> str:
+        from openlineage.common.provider.snowflake import fix_snowflake_sqlalchemy_uri
+
+        uri = fix_snowflake_sqlalchemy_uri(self.get_uri())
+        return urlparse(uri).hostname
+
+    def get_openlineage_database_specific_lineage(self, _) -> OperatorLineage | None:
+        from openlineage.client.facet import ExternalQueryRunFacet
+
+        from airflow.providers.openlineage.extractors import OperatorLineage
+        from airflow.providers.openlineage.sqlparser import SQLParser
+
+        connection = self.get_connection(getattr(self, self.conn_name_attr))
+        namespace = SQLParser.create_namespace(self.get_database_info(connection))
+
+        if self.query_ids:
+            return OperatorLineage(
+                run_facets={
+                    "externalQuery": ExternalQueryRunFacet(
+                        externalQueryId=self.query_ids[0], source=namespace
+                    )
+                }
+            )
+        return None
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     from airflow.utils.context import Context
 
 
 class SnowflakeOperator(SQLExecuteQueryOperator):
     """
     Executes SQL code in a Snowflake database.
 
+    This class is deprecated.
+
+    Please use :class:`airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
+
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SnowflakeOperator`
 
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
     :param sql: the SQL code to be executed as a single string, or
@@ -193,15 +197,15 @@
     ui_color = "#ededed"
 
     def __init__(
         self,
         *,
         sql: str,
         snowflake_conn_id: str = "snowflake_default",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         autocommit: bool = True,
         do_xcom_push: bool = True,
         warehouse: str | None = None,
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
@@ -258,15 +262,15 @@
     def __init__(
         self,
         *,
         sql: str,
         pass_value: Any,
         tolerance: Any = None,
         snowflake_conn_id: str = "snowflake_default",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         autocommit: bool = True,
         do_xcom_push: bool = True,
         warehouse: str | None = None,
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
@@ -333,15 +337,15 @@
         self,
         *,
         table: str,
         metrics_thresholds: dict,
         date_filter_column: str = "ds",
         days_back: SupportsAbs[int] = -7,
         snowflake_conn_id: str = "snowflake_default",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         autocommit: bool = True,
         do_xcom_push: bool = True,
         warehouse: str | None = None,
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
-from typing import Iterable, Mapping, Sequence
+from typing import Any, Iterable, Mapping, Sequence
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.slack.transfers.sql_to_slack import SqlToSlackOperator
 
 
 class SnowflakeToSlackOperator(SqlToSlackOperator):
     """
@@ -64,15 +64,15 @@
         self,
         *,
         sql: str,
         slack_message: str,
         snowflake_conn_id: str = "snowflake_default",
         slack_conn_id: str = "slack_default",
         results_df_name: str = "results_df",
-        parameters: Iterable | Mapping | None = None,
+        parameters: Iterable | Mapping[str, Any] | None = None,
         warehouse: str | None = None,
         database: str | None = None,
         schema: str | None = None,
         role: str | None = None,
         slack_token: str | None = None,
         **kwargs,
     ) -> None:
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.1rc1
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: common.sql
+Provides-Extra: openlineage
 Provides-Extra: slack
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -68,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.1rc1``
+Release: ``4.4.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -118,16 +119,17 @@
 You can install such cross-provider dependencies when installing from PyPI. For example:
 
 .. code-block:: bash
 
     pip install apache-airflow-providers-snowflake[common.sql]
 
 
-============================================================================================================  ==============
-Dependent package                                                                                             Extra
-============================================================================================================  ==============
-`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
-`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
-============================================================================================================  ==============
+==============================================================================================================  ===============
+Dependent package                                                                                               Extra
+==============================================================================================================  ===============
+`apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
+`apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
+==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/pyproject.toml` & `apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/setup.cfg` & `apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-snowflake-4.3.1rc1/setup.py` & `apache-airflow-providers-snowflake-4.4.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-snowflake package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.1"
+version = "4.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-snowflake setup."""
     setup(
         version=version,
         extras_require={
             "common.sql": ["apache-airflow-providers-common-sql"],
+            "openlineage": ["apache-airflow-providers-openlineage"],
             "slack": ["apache-airflow-providers-slack"],
         },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.snowflake",
                 "airflow.providers.snowflake.*",
                 "airflow.providers.snowflake_vendor",
```

