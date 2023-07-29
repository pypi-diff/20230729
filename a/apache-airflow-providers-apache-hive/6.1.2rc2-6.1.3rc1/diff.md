# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.2rc2.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.2rc2.tar", last modified: Thu Jul  6 04:50:11 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.3rc1.tar", last modified: Sat Jul 29 12:07:58 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.2rc2.tar` & `apache-airflow-providers-apache-hive-6.1.3rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.873354 apache-airflow-providers-apache-hive-6.1.2rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.2rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6929 2023-07-06 04:50:11.873895 apache-airflow-providers-apache-hive-6.1.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5149 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.742202 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.743421 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.744650 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.787671 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-06 04:42:33.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.793479 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42460 2023-07-04 13:46:32.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.800195 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.808843 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.814578 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.827768 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.847924 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6719 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:11.871107 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6929 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:11.000000 apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-apache-hive-6.1.2rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2154 2023-07-06 04:50:11.875786 apache-airflow-providers-apache-hive-6.1.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-07-06 04:50:10.000000 apache-airflow-providers-apache-hive-6.1.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.291641 apache-airflow-providers-apache-hive-6.1.3rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.3rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:07:57.000000 apache-airflow-providers-apache-hive-6.1.3rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-07-29 12:07:58.292192 apache-airflow-providers-apache-hive-6.1.3rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-07-29 12:07:57.000000 apache-airflow-providers-apache-hive-6.1.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.148770 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.150220 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.151961 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.198244 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6613 2023-07-29 12:07:57.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.206608 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42466 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.212882 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.223032 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.228901 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.241873 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.265506 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5280 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5664 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6719 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11748 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:58.289048 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6929 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-hive-6.1.3rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-07-29 12:07:58.294077 apache-airflow-providers-apache-hive-6.1.3rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-29 12:07:56.000000 apache-airflow-providers-apache-hive-6.1.3rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/LICENSE` & `apache-airflow-providers-apache-hive-6.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.2rc2
+Version: 6.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,28 +72,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.2rc2``
+Release: ``6.1.3rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -138,8 +138,8 @@
 `apache-airflow-providers-mysql <https://airflow.apache.org/docs/apache-airflow-providers-mysql>`_                      ``mysql``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_                    ``presto``
 `apache-airflow-providers-samba <https://airflow.apache.org/docs/apache-airflow-providers-samba>`_                      ``samba``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_                  ``vertica``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/README.rst` & `apache-airflow-providers-apache-hive-6.1.3rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.2rc2``
+Release: ``6.1.3rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -98,8 +98,8 @@
 `apache-airflow-providers-mysql <https://airflow.apache.org/docs/apache-airflow-providers-mysql>`_                      ``mysql``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_                    ``presto``
 `apache-airflow-providers-samba <https://airflow.apache.org/docs/apache-airflow-providers-samba>`_                      ``samba``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_                  ``vertica``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.1.2"
+__version__ = "6.1.3"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-apache-hive:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hive",
         "name": "Apache Hive",
         "description": "`Apache Hive <https://hive.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.3",
             "6.1.2",
             "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.1.3",
             "5.1.2",
             "5.1.1",
@@ -148,8 +149,29 @@
                 "hook-class-name": "airflow.providers.apache.hive.hooks.hive.HiveMetastoreHook",
                 "connection-type": "hive_metastore",
             },
         ],
         "plugins": [
             {"name": "hive", "plugin-class": "airflow.providers.apache.hive.plugins.hive.HivePlugin"}
         ],
+        "config": {
+            "hive": {
+                "description": None,
+                "options": {
+                    "default_hive_mapred_queue": {
+                        "description": "Default mapreduce queue for HiveOperator tasks\n",
+                        "version_added": None,
+                        "type": "string",
+                        "example": None,
+                        "default": "",
+                    },
+                    "mapred_job_name_template": {
+                        "description": "Template for mapred_job_name in HiveOperator, supports the following named parameters\nhostname, dag_id, task_id, execution_date\n",
+                        "version_added": None,
+                        "type": "string",
+                        "example": None,
+                        "default": None,
+                    },
+                },
+            }
+        },
     }
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/hooks/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
                 "O": "STRING",  # object
                 "S": "STRING",  # (byte-)string
                 "U": "STRING",  # Unicode
                 "V": "STRING",  # void
             }
 
             order_type = OrderedDict()
-            for col, dtype in df.dtypes.iteritems():
+            for col, dtype in df.dtypes.items():
                 order_type[col] = dtype_kind_hive_type[dtype.kind]
             return order_type
 
         if pandas_kwargs is None:
             pandas_kwargs = {}
 
         with TemporaryDirectory(prefix="airflow_hiveop_") as tmp_dir:
@@ -1010,15 +1010,15 @@
             # need to clean up the file first
             os.remove(csv_filepath)
             raise ValueError(message)
 
         self.log.info("Done. Loaded a total of %s rows.", i)
 
     def get_records(
-        self, sql: str | list[str], parameters: Iterable | Mapping | None = None, **kwargs
+        self, sql: str | list[str], parameters: Iterable | Mapping[str, Any] | None = None, **kwargs
     ) -> Any:
         """
         Get a set of records from a Hive query; optionally pass a 'schema' kwarg to specify target schema.
 
         :param sql: hql to be executed.
         :param parameters: optional configuration passed to get_results
         :return: result of hive execution
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.2rc2
+Version: 6.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -72,28 +72,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.2rc2``
+Release: ``6.1.3rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -138,8 +138,8 @@
 `apache-airflow-providers-mysql <https://airflow.apache.org/docs/apache-airflow-providers-mysql>`_                      ``mysql``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_                    ``presto``
 `apache-airflow-providers-samba <https://airflow.apache.org/docs/apache-airflow-providers-samba>`_                      ``samba``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_                  ``vertica``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.3rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.3rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.3rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.2/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.3/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -60,10 +60,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.2rc2/setup.py` & `apache-airflow-providers-apache-hive-6.1.3rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-hive package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.2"
+version = "6.1.3"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-hive setup."""
     setup(
         version=version,
         extras_require={
```

