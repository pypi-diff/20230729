# Comparing `tmp/apache-airflow-providers-celery-3.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-celery-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-celery-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:39 2023, max compression
+gzip compressed data, was "apache-airflow-providers-celery-3.3.0rc1.tar", last modified: Sat Jul 29 12:08:10 2023, max compression
```

## Comparing `apache-airflow-providers-celery-3.2.1rc1.tar` & `apache-airflow-providers-celery-3.3.0rc1.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.607708 apache-airflow-providers-celery-3.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9653 2023-06-20 11:41:39.609077 apache-airflow-providers-celery-3.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8125 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.531177 apache-airflow-providers-celery-3.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.532943 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.570323 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.576244 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/celery_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.604153 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9653 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-celery-3.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1862 2023-06-20 11:41:39.611375 apache-airflow-providers-celery-3.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.464499 apache-airflow-providers-celery-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.465122 apache-airflow-providers-celery-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.376279 apache-airflow-providers-celery-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.377486 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.414891 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.430149 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-12 12:42:21.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18336 2023-07-29 09:53:35.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor.py
+-rw-r--r--   0 root         (0) root         (0)    13011 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_executor_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-29 06:50:08.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/celery_kubernetes_executor.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-26 06:59:50.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/executors/default_celery.py
+-rw-r--r--   0 root         (0) root         (0)    16209 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.437531 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-06-29 05:49:30.000000 apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:10.461789 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:10.000000 apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-celery-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-07-29 12:08:10.466958 apache-airflow-providers-celery-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-07-29 12:08:09.000000 apache-airflow-providers-celery-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-celery-3.2.1rc1/LICENSE` & `apache-airflow-providers-celery-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1rc1/MANIFEST.in` & `apache-airflow-providers-celery-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/__init__.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.1"
+__version__ = "3.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-celery:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/__init__.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/celery_queue.py` & `apache-airflow-providers-celery-3.3.0rc1/airflow/providers/celery/sensors/celery_queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,33 +25,32 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class CeleryQueueSensor(BaseSensorOperator):
     """
-    Waits for a Celery queue to be empty. By default, in order to be considered
-    empty, the queue must not have any tasks in the ``reserved``, ``scheduled``
-    or ``active`` states.
+    Waits for a Celery queue to be empty.
+
+    By default, in order to be considered empty, the queue must not have
+    any tasks in the ``reserved``, ``scheduled`` or ``active`` states.
 
     :param celery_queue: The name of the Celery queue to wait for.
     :param target_task_id: Task id for checking
     """
 
     def __init__(self, *, celery_queue: str, target_task_id: str | None = None, **kwargs) -> None:
 
         super().__init__(**kwargs)
         self.celery_queue = celery_queue
         self.target_task_id = target_task_id
 
     def _check_task_id(self, context: Context) -> bool:
         """
-        Gets the returned Celery result from the Airflow task
-        ID provided to the sensor, and returns True if the
-        celery result has been finished execution.
+        Get the Celery result from the Airflow task ID and return True if the result has finished execution.
 
         :param context: Airflow's execution context
         :return: True if task has been executed, otherwise False
         """
         ti = context["ti"]
         celery_result = ti.xcom_pull(task_ids=self.target_task_id)
         return celery_result.ready()
```

### Comparing `apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt` & `apache-airflow-providers-celery-3.3.0rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 NOTICE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/celery/__init__.py
 airflow/providers/celery/get_provider_info.py
+airflow/providers/celery/executors/__init__.py
+airflow/providers/celery/executors/celery_executor.py
+airflow/providers/celery/executors/celery_executor_utils.py
+airflow/providers/celery/executors/celery_kubernetes_executor.py
+airflow/providers/celery/executors/default_celery.py
 airflow/providers/celery/sensors/__init__.py
 airflow/providers/celery/sensors/celery_queue.py
 apache_airflow_providers_celery.egg-info/PKG-INFO
 apache_airflow_providers_celery.egg-info/SOURCES.txt
 apache_airflow_providers_celery.egg-info/dependency_links.txt
 apache_airflow_providers_celery.egg-info/entry_points.txt
 apache_airflow_providers_celery.egg-info/not-zip-safe
```

### Comparing `apache-airflow-providers-celery-3.2.1rc1/pyproject.toml` & `apache-airflow-providers-celery-3.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-celery-3.2.1rc1/setup.cfg` & `apache-airflow-providers-celery-3.3.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-celery/3.3.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-celery-3.2.1rc1/setup.py` & `apache-airflow-providers-celery-3.3.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-celery package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-celery setup."""
     setup(
         version=version,
-        extras_require={},
+        extras_require={"cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]},
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.celery",
                 "airflow.providers.celery.*",
                 "airflow.providers.celery_vendor",
                 "airflow.providers.celery_vendor.*",
             ],
```
