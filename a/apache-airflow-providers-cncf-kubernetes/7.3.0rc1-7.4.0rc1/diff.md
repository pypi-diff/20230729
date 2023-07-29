# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar", last modified: Wed Jul 12 19:13:20 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar", last modified: Sat Jul 29 12:08:13 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1.tar`

### file list

```diff
@@ -1,52 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.421423 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-12 19:13:20.422013 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2963 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.285314 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.286510 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.287650 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.338150 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-12 19:08:31.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.343829 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.349520 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4504 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.355146 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23125 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.370152 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    40898 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-06-28 06:26:40.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.375749 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.384149 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.395876 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0 root         (0) root         (0)    28931 2023-07-09 14:40:47.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:20.418731 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4637 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1893 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:20.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-12 19:13:20.423922 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-12 19:13:19.000000 apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.233596 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-29 12:08:13.234305 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.028423 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.029770 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.031174 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.115362 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-29 12:01:19.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.121187 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.127824 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.143163 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30257 2023-07-29 09:53:35.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0 root         (0) root         (0)    21132 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-07-29 06:50:08.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.149392 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23140 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.152575 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.169619 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    41271 2023-07-29 09:53:35.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)    23849 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0 root         (0) root         (0)    12129 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.172463 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.178255 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.186594 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-16 17:25:26.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    11511 2023-07-12 12:42:21.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.202681 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5176 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    28943 2023-07-26 06:59:50.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:30.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:13.230124 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4637 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:12.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-29 12:08:13.236467 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-29 12:08:11.000000 apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.3.0rc1
+Version: 7.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.3.0rc1``
+Release: ``7.4.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.3.0rc1``
+Release: ``7.4.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -71,8 +71,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.3.0"
+__version__ = "7.4.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-cncf-kubernetes:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from kubernetes.client.models import V1Pod
 from kubernetes.config import ConfigException
 from kubernetes_asyncio import client as async_client, config as async_config
 from urllib3.exceptions import HTTPError
 
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.hooks.base import BaseHook
-from airflow.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
 from airflow.models import Connection
+from airflow.providers.cncf.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
 from airflow.providers.cncf.kubernetes.utils.pod_manager import PodOperatorHookProtocol
 from airflow.utils import yaml
 
 LOADING_KUBE_CONFIG_FILE_RESOURCE = "Loading Kubernetes configuration file kube_config from {}..."
 
 
 def _load_body_to_dict(body: str) -> dict:
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+"""This module is deprecated. Please use :mod:`airflow.providers.cncf.kubernetes.operators.pod` instead."""
 from __future__ import annotations
 
 import warnings
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.cncf.kubernetes.operators.pod import *  # noqa
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
-from airflow.kubernetes import pod_generator
-from airflow.kubernetes.pod_generator import PodGenerator
-from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
+from airflow.providers.cncf.kubernetes import pod_generator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
     convert_configmap,
     convert_env_vars,
     convert_image_pull_secrets,
     convert_pod_runtime_info_env,
     convert_port,
     convert_toleration,
     convert_volume,
     convert_volume_mount,
 )
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook
+from airflow.providers.cncf.kubernetes.pod_generator import PodGenerator
+from airflow.providers.cncf.kubernetes.secret import Secret
 from airflow.providers.cncf.kubernetes.triggers.pod import KubernetesPodTrigger
 from airflow.providers.cncf.kubernetes.utils import xcom_sidecar  # type: ignore[attr-defined]
 from airflow.providers.cncf.kubernetes.utils.pod_manager import (
     OnFinishAction,
     PodLaunchFailedException,
     PodManager,
     PodOperatorHookProtocol,
@@ -234,14 +234,16 @@
     :param on_finish_action: What to do when the pod reaches its final state, or the execution is interrupted.
         If "delete_pod", the pod will be deleted regardless it's state; if "delete_succeeded_pod",
         only succeeded pod will be deleted. You can set to "keep_pod" to keep the pod.
     :param is_delete_operator_pod: What to do when the pod reaches its final
         state, or the execution is interrupted. If True (default), delete the
         pod; if False, leave the pod.
         Deprecated - use `on_finish_action` instead.
+    :param termination_message_policy: The termination message policy of the base container.
+        Default value is "File"
     """
 
     # This field can be overloaded at the instance level via base_container_name
     BASE_CONTAINER_NAME = "base"
 
     POD_CHECKED_KEY = "already_checked"
     POST_TERMINATION_TIMEOUT = 120
@@ -313,14 +315,15 @@
         skip_on_exit_code: int | Container[int] | None = None,
         base_container_name: str | None = None,
         deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: float = 2,
         log_pod_spec_on_failure: bool = True,
         on_finish_action: str = "delete_pod",
         is_delete_operator_pod: None | bool = None,
+        termination_message_policy: str = "File",
         **kwargs,
     ) -> None:
         # TODO: remove in provider 6.0.0 release. This is a mitigate step to advise users to switch to the
         # container_resources parameter.
         if isinstance(kwargs.get("resources"), k8s.V1ResourceRequirements):
             raise AirflowException(
                 "Specifying resources for the launched pod with 'resources' is deprecated. "
@@ -411,14 +414,15 @@
             self.on_finish_action = (
                 OnFinishAction.DELETE_POD if is_delete_operator_pod else OnFinishAction.KEEP_POD
             )
             self.is_delete_operator_pod = is_delete_operator_pod
         else:
             self.on_finish_action = OnFinishAction(on_finish_action)
             self.is_delete_operator_pod = self.on_finish_action == OnFinishAction.DELETE_POD
+        self.termination_message_policy = termination_message_policy
 
         self._config_dict: dict | None = None  # TODO: remove it when removing convert_config_file_to_dict
 
     @cached_property
     def _incluster_namespace(self):
         from pathlib import Path
 
@@ -834,14 +838,15 @@
                         image_pull_policy=self.image_pull_policy,
                         resources=self.container_resources,
                         volume_mounts=self.volume_mounts,
                         args=self.arguments,
                         env=self.env_vars,
                         env_from=self.env_from,
                         security_context=self.container_security_context,
+                        termination_message_policy=self.termination_message_policy,
                     )
                 ],
                 image_pull_secrets=self.image_pull_secrets,
                 service_account_name=self.service_account_name,
                 host_network=self.hostnetwork,
                 hostname=self.hostname,
                 subdomain=self.subdomain,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Sequence
 
+from kubernetes.client import ApiException
 from kubernetes.watch import Watch
 
 from airflow import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook, _load_body_to_dict
 
 if TYPE_CHECKING:
+    from kubernetes.client.models import CoreV1EventList
+
     from airflow.utils.context import Context
 
 
 class SparkKubernetesOperator(BaseOperator):
     """
     Creates sparkApplication object in kubernetes cluster.
 
@@ -81,28 +84,47 @@
         self.hook = KubernetesHook(
             conn_id=self.kubernetes_conn_id,
             in_cluster=self.in_cluster,
             config_file=self.config_file,
             cluster_context=self.cluster_context,
         )
 
+    def _get_namespace_event_stream(self, namespace, query_kwargs=None):
+        try:
+            return Watch().stream(
+                self.hook.core_v1_client.list_namespaced_event,
+                namespace=namespace,
+                watch=True,
+                **(query_kwargs or {}),
+            )
+        except ApiException as e:
+            if e.status == 410:  # Resource version is too old
+                events: CoreV1EventList = self.hook.core_v1_client.list_namespaced_event(
+                    namespace=namespace, watch=False
+                )
+                resource_version = events.metadata.resource_version
+                query_kwargs["resource_version"] = resource_version
+                return self._get_namespace_event_stream(namespace, query_kwargs)
+            else:
+                raise
+
     def execute(self, context: Context):
         body = _load_body_to_dict(self.application_file)
         name = body["metadata"]["name"]
         namespace = self.namespace or self.hook.get_namespace()
 
         response = None
         is_job_created = False
         if self.watch:
             try:
-                namespace_event_stream = Watch().stream(
-                    self.hook.core_v1_client.list_namespaced_event,
+                namespace_event_stream = self._get_namespace_event_stream(
                     namespace=namespace,
-                    watch=True,
-                    field_selector=f"involvedObject.kind=SparkApplication,involvedObject.name={name}",
+                    query_kwargs={
+                        "field_selector": f"involvedObject.kind=SparkApplication,involvedObject.name={name}"
+                    },
                 )
 
                 response = self.hook.create_custom_object(
                     group=self.api_group,
                     version=self.api_version,
                     plural=self.plural,
                     body=body,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+"""This module is deprecated. Please use :mod:`airflow.providers.cncf.kubernetes.triggers.pod` instead."""
 from __future__ import annotations
 
 import warnings
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.cncf.kubernetes.triggers.pod import *  # noqa
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from pendulum import DateTime
 from pendulum.parsing.exceptions import ParserError
 from tenacity import before_log
 from urllib3.exceptions import HTTPError as BaseHTTPError
 from urllib3.response import HTTPResponse
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
-from airflow.kubernetes.pod_generator import PodDefaults
+from airflow.providers.cncf.kubernetes.pod_generator import PodDefaults
 from airflow.typing_compat import Literal, Protocol
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.timezone import utcnow
 
 if TYPE_CHECKING:
     from kubernetes.client.models.core_v1_event_list import CoreV1EventList
 
@@ -85,15 +85,15 @@
     Subclasses of KubernetesPodOperator, such as GKEStartPodOperator, may use
     hooks that don't extend KubernetesHook.  We use this protocol to document the
     methods used by KPO and ensure that these methods exist on such other hooks.
     """
 
     @property
     def core_v1_client(self) -> client.CoreV1Api:
-        """Get authenticated CoreV1Api object."""
+        """Get authenticated client object."""
 
     @property
     def is_in_cluster(self) -> bool:
         """Expose whether the hook is configured with ``load_incluster_config`` or not."""
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
         """Read pod object from kubernetes API."""
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.3.0rc1
+Version: 7.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.3.0rc1``
+Release: ``7.4.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,8 +105,8 @@
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,51 @@
 NOTICE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/cncf/kubernetes/__init__.py
 airflow/providers/cncf/kubernetes/get_provider_info.py
+airflow/providers/cncf/kubernetes/k8s_model.py
+airflow/providers/cncf/kubernetes/kube_client.py
+airflow/providers/cncf/kubernetes/kube_config.py
+airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+airflow/providers/cncf/kubernetes/pod_generator.py
+airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
 airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
 airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+airflow/providers/cncf/kubernetes/secret.py
+airflow/providers/cncf/kubernetes/template_rendering.py
 airflow/providers/cncf/kubernetes/backcompat/__init__.py
 airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
 airflow/providers/cncf/kubernetes/decorators/__init__.py
 airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+airflow/providers/cncf/kubernetes/executors/__init__.py
+airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
 airflow/providers/cncf/kubernetes/hooks/__init__.py
 airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
 airflow/providers/cncf/kubernetes/operators/__init__.py
 airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
 airflow/providers/cncf/kubernetes/operators/pod.py
 airflow/providers/cncf/kubernetes/operators/resource.py
 airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
 airflow/providers/cncf/kubernetes/sensors/__init__.py
 airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
 airflow/providers/cncf/kubernetes/triggers/__init__.py
 airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
 airflow/providers/cncf/kubernetes/triggers/pod.py
 airflow/providers/cncf/kubernetes/utils/__init__.py
 airflow/providers/cncf/kubernetes/utils/delete_from.py
+airflow/providers/cncf/kubernetes/utils/k8s_hashlib_wrapper.py
 airflow/providers/cncf/kubernetes/utils/pod_manager.py
 airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
 apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
 apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.3.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.4.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.3.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.4.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.3.0"
+version = "7.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

