# Comparing `tmp/apache-airflow-providers-apache-beam-5.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-beam-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-beam-5.1.1rc1.tar", last modified: Tue Jun 20 11:41:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-beam-5.2.0rc1.tar", last modified: Sat Jul 29 12:07:50 2023, max compression
```

## Comparing `apache-airflow-providers-apache-beam-5.1.1rc1.tar` & `apache-airflow-providers-apache-beam-5.2.0rc1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.706713 apache-airflow-providers-apache-beam-5.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15861 2023-06-20 11:41:06.707716 apache-airflow-providers-apache-beam-5.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14295 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.634552 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.635650 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.636649 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.668032 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.673565 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14197 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.679189 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32492 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.704020 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15861 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-beam-5.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1880 2023-06-20 11:41:06.709699 apache-airflow-providers-apache-beam-5.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.966138 apache-airflow-providers-apache-beam-5.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:07:49.000000 apache-airflow-providers-apache-beam-5.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-29 12:07:50.966668 apache-airflow-providers-apache-beam-5.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-07-29 12:07:49.000000 apache-airflow-providers-apache-beam-5.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.885683 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.886846 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.888069 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.921121 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-07-29 12:07:49.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.926755 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21721 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/hooks/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.932838 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35757 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/operators/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.939042 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5107 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/triggers/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:50.963847 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5459 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:50.000000 apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-beam-5.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-07-29 12:07:50.968566 apache-airflow-providers-apache-beam-5.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-07-29 12:07:49.000000 apache-airflow-providers-apache-beam-5.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/LICENSE` & `apache-airflow-providers-apache-beam-5.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-beam-5.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/__init__.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.1.1"
+__version__ = "5.2.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-apache-beam:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/get_provider_info.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-beam",
         "name": "Apache Beam",
         "description": "`Apache Beam <https://beam.apache.org/>`__.\n",
         "suspended": False,
         "versions": [
+            "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
@@ -65,9 +66,15 @@
         ],
         "hooks": [
             {
                 "integration-name": "Apache Beam",
                 "python-modules": ["airflow.providers.apache.beam.hooks.beam"],
             }
         ],
+        "triggers": [
+            {
+                "integration-name": "Apache Beam",
+                "python-modules": ["airflow.providers.apache.beam.triggers.beam"],
+            }
+        ],
         "additional-extras": [{"name": "google", "dependencies": ["apache-beam[gcp]"]}],
     }
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/__init__.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/__init__.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/beam.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/airflow/providers/apache/beam/operators/beam.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,31 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Apache Beam operators."""
 from __future__ import annotations
 
+import asyncio
+import contextlib
 import copy
 import os
 import stat
 import tempfile
 from abc import ABC, ABCMeta, abstractmethod
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import ExitStack
 from functools import partial
-from typing import TYPE_CHECKING, Callable, Sequence
+from typing import IO, TYPE_CHECKING, Any, Callable, Sequence
 
 from airflow import AirflowException
+from airflow.configuration import conf
 from airflow.models import BaseOperator
 from airflow.providers.apache.beam.hooks.beam import BeamHook, BeamRunnerType
+from airflow.providers.apache.beam.triggers.beam import BeamPipelineTrigger
 from airflow.providers.google.cloud.hooks.dataflow import (
     DataflowHook,
     process_line_and_extract_dataflow_job_id_callback,
 )
 from airflow.providers.google.cloud.hooks.gcs import GCSHook, _parse_gcs_url
 from airflow.providers.google.cloud.links.dataflow import DataflowJobLink
 from airflow.providers.google.cloud.operators.dataflow import CheckJobRunning, DataflowConfiguration
@@ -43,15 +47,16 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class BeamDataflowMixin(metaclass=ABCMeta):
     """
-    Helper class to store common, Dataflow specific logic for both
+    Helper class to store common, Dataflow specific logic for both.
+
     :class:`~airflow.providers.apache.beam.operators.beam.BeamRunPythonPipelineOperator`,
     :class:`~airflow.providers.apache.beam.operators.beam.BeamRunJavaPipelineOperator` and
     :class:`~airflow.providers.apache.beam.operators.beam.BeamRunGoPipelineOperator`.
     """
 
     dataflow_hook: DataflowHook | None
     dataflow_config: DataflowConfiguration
@@ -139,15 +144,15 @@
           If the value is ``['A', 'B']`` and the key is ``key`` then the ``--key=A --key=B`` options
           will be left
         * Other value types will be replaced with the Python textual representation.
 
         When defining labels (labels option), you can also provide a dictionary.
     :param gcp_conn_id: Optional.
         The connection ID to use connecting to Google Cloud Storage if python file is on GCS.
-    :param dataflow_config: Dataflow configuration, used when runner type is set to DataflowRunner,
+    :param dataflow_config: Dataflow's configuration, used when runner type is set to DataflowRunner,
         (optional) defaults to None.
     """
 
     def __init__(
         self,
         *,
         runner: str = "DirectRunner",
@@ -162,15 +167,15 @@
         self.default_pipeline_options = default_pipeline_options or {}
         self.pipeline_options = pipeline_options or {}
         self.gcp_conn_id = gcp_conn_id
         if isinstance(dataflow_config, dict):
             self.dataflow_config = DataflowConfiguration(**dataflow_config)
         else:
             self.dataflow_config = dataflow_config or DataflowConfiguration()
-        self.beam_hook: BeamHook | None = None
+        self.beam_hook: BeamHook
         self.dataflow_hook: DataflowHook | None = None
         self.dataflow_job_id: str | None = None
 
         if self.dataflow_config and self.runner.lower() != BeamRunnerType.DataflowRunner.lower():
             self.log.warning(
                 "dataflow_config is defined but runner is different than DataflowRunner (%s)", self.runner
             )
@@ -201,19 +206,21 @@
             return is_dataflow, dataflow_job_name, snake_case_pipeline_options, process_line_callback
 
         return is_dataflow, dataflow_job_name, pipeline_options, process_line_callback
 
 
 class BeamRunPythonPipelineOperator(BeamBasePipelineOperator):
     """
-    Launching Apache Beam pipelines written in Python. Note that both
-    ``default_pipeline_options`` and ``pipeline_options`` will be merged to specify pipeline
-    execution parameter, and ``default_pipeline_options`` is expected to save
-    high-level options, for instances, project and zone information, which
-    apply to all beam operators in the DAG.
+    Launch Apache Beam pipelines written in Python.
+
+    Note that both ``default_pipeline_options`` and ``pipeline_options``
+    will be merged to specify pipeline execution parameter, and
+    ``default_pipeline_options`` is expected to save high-level options,
+    for instances, project and zone information, which apply to all beam
+    operators in the DAG.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:BeamRunPythonPipelineOperator`
 
     .. seealso::
         For more detail on Apache Beam have a look at the reference:
@@ -230,16 +237,16 @@
         If a value is passed to this parameter, a new virtual environment has been created with
         additional packages installed.
 
         You could also install the apache_beam package if it is not installed on your system or you want
         to use a different version.
     :param py_system_site_packages: Whether to include system_site_packages in your virtualenv.
         See virtualenv documentation for more information.
-
         This option is only relevant if the ``py_requirements`` parameter is not None.
+    :param deferrable: Run operator in the deferrable mode: checks for the state using asynchronous calls.
     """
 
     template_fields: Sequence[str] = (
         "py_file",
         "runner",
         "pipeline_options",
         "default_pipeline_options",
@@ -257,14 +264,15 @@
         pipeline_options: dict | None = None,
         py_interpreter: str = "python3",
         py_options: list[str] | None = None,
         py_requirements: list[str] | None = None,
         py_system_site_packages: bool = False,
         gcp_conn_id: str = "google_cloud_default",
         dataflow_config: DataflowConfiguration | dict | None = None,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(
             runner=runner,
             default_pipeline_options=default_pipeline_options,
             pipeline_options=pipeline_options,
             gcp_conn_id=gcp_conn_id,
@@ -276,71 +284,135 @@
         self.py_options = py_options or []
         self.py_interpreter = py_interpreter
         self.py_requirements = py_requirements
         self.py_system_site_packages = py_system_site_packages
         self.pipeline_options.setdefault("labels", {}).update(
             {"airflow-version": "v" + version.replace(".", "-").replace("+", "-")}
         )
+        self.deferrable = deferrable
 
     def execute(self, context: Context):
         """Execute the Apache Beam Pipeline."""
         (
-            is_dataflow,
-            dataflow_job_name,
-            snake_case_pipeline_options,
-            process_line_callback,
+            self.is_dataflow,
+            self.dataflow_job_name,
+            self.snake_case_pipeline_options,
+            self.process_line_callback,
         ) = self._init_pipeline_options(format_pipeline_options=True, job_name_variable_key="job_name")
-
         if not self.beam_hook:
             raise AirflowException("Beam hook is not defined.")
+        # Check deferrable parameter passed to the operator
+        # to determine type of run - asynchronous or synchronous
+        if self.deferrable:
+            asyncio.run(self.execute_async(context))
+        else:
+            return self.execute_sync(context)
 
+    def execute_sync(self, context: Context):
         with ExitStack() as exit_stack:
             if self.py_file.lower().startswith("gs://"):
                 gcs_hook = GCSHook(gcp_conn_id=self.gcp_conn_id)
                 tmp_gcs_file = exit_stack.enter_context(gcs_hook.provide_file(object_url=self.py_file))
                 self.py_file = tmp_gcs_file.name
 
-            if is_dataflow and self.dataflow_hook:
+            if self.is_dataflow and self.dataflow_hook:
                 with self.dataflow_hook.provide_authorized_gcloud():
                     self.beam_hook.start_python_pipeline(
-                        variables=snake_case_pipeline_options,
+                        variables=self.snake_case_pipeline_options,
                         py_file=self.py_file,
                         py_options=self.py_options,
                         py_interpreter=self.py_interpreter,
                         py_requirements=self.py_requirements,
                         py_system_site_packages=self.py_system_site_packages,
-                        process_line_callback=process_line_callback,
+                        process_line_callback=self.process_line_callback,
                     )
                 DataflowJobLink.persist(
                     self,
                     context,
                     self.dataflow_config.project_id,
                     self.dataflow_config.location,
                     self.dataflow_job_id,
                 )
-                if dataflow_job_name and self.dataflow_config.location:
-                    self.dataflow_hook.wait_for_done(
-                        job_name=dataflow_job_name,
-                        location=self.dataflow_config.location,
-                        job_id=self.dataflow_job_id,
-                        multiple_jobs=False,
-                        project_id=self.dataflow_config.project_id,
-                    )
                 return {"dataflow_job_id": self.dataflow_job_id}
             else:
                 self.beam_hook.start_python_pipeline(
-                    variables=snake_case_pipeline_options,
+                    variables=self.snake_case_pipeline_options,
                     py_file=self.py_file,
                     py_options=self.py_options,
                     py_interpreter=self.py_interpreter,
                     py_requirements=self.py_requirements,
                     py_system_site_packages=self.py_system_site_packages,
-                    process_line_callback=process_line_callback,
+                    process_line_callback=self.process_line_callback,
                 )
 
+    async def execute_async(self, context: Context):
+        # Creating a new event loop to manage I/O operations asynchronously
+        loop = asyncio.get_event_loop()
+        if self.py_file.lower().startswith("gs://"):
+            gcs_hook = GCSHook(gcp_conn_id=self.gcp_conn_id)
+            # Running synchronous `enter_context()` method in a separate
+            # thread using the default executor `None`. The `run_in_executor()` function returns the
+            # file object, which is created using gcs function `provide_file()`, asynchronously.
+            # This means we can perform asynchronous operations with this file.
+            create_tmp_file_call = gcs_hook.provide_file(object_url=self.py_file)
+            tmp_gcs_file: IO[str] = await loop.run_in_executor(
+                None, contextlib.ExitStack().enter_context, create_tmp_file_call
+            )
+            self.py_file = tmp_gcs_file.name
+
+        if self.is_dataflow and self.dataflow_hook:
+            DataflowJobLink.persist(
+                self,
+                context,
+                self.dataflow_config.project_id,
+                self.dataflow_config.location,
+                self.dataflow_job_id,
+            )
+            with self.dataflow_hook.provide_authorized_gcloud():
+                self.defer(
+                    trigger=BeamPipelineTrigger(
+                        variables=self.snake_case_pipeline_options,
+                        py_file=self.py_file,
+                        py_options=self.py_options,
+                        py_interpreter=self.py_interpreter,
+                        py_requirements=self.py_requirements,
+                        py_system_site_packages=self.py_system_site_packages,
+                        runner=self.runner,
+                    ),
+                    method_name="execute_complete",
+                )
+        else:
+            self.defer(
+                trigger=BeamPipelineTrigger(
+                    variables=self.snake_case_pipeline_options,
+                    py_file=self.py_file,
+                    py_options=self.py_options,
+                    py_interpreter=self.py_interpreter,
+                    py_requirements=self.py_requirements,
+                    py_system_site_packages=self.py_system_site_packages,
+                    runner=self.runner,
+                ),
+                method_name="execute_complete",
+            )
+
+    def execute_complete(self, context: Context, event: dict[str, Any]):
+        """
+        Callback for when the trigger fires - returns immediately.
+        Relies on trigger to throw an exception, otherwise it assumes execution was
+        successful.
+        """
+        if event["status"] == "error":
+            raise AirflowException(event["message"])
+        self.log.info(
+            "%s completed with response %s ",
+            self.task_id,
+            event["message"],
+        )
+        return {"dataflow_job_id": self.dataflow_job_id}
+
     def on_kill(self) -> None:
         if self.dataflow_hook and self.dataflow_job_id:
             self.log.info("Dataflow job with id: `%s` was requested to be cancelled.", self.dataflow_job_id)
             self.dataflow_hook.cancel_job(
                 job_id=self.dataflow_job_id,
                 project_id=self.dataflow_config.project_id,
             )
@@ -494,19 +566,21 @@
                 job_id=self.dataflow_job_id,
                 project_id=self.dataflow_config.project_id,
             )
 
 
 class BeamRunGoPipelineOperator(BeamBasePipelineOperator):
     """
-    Launching Apache Beam pipelines written in Go. Note that both
-    ``default_pipeline_options`` and ``pipeline_options`` will be merged to specify pipeline
-    execution parameter, and ``default_pipeline_options`` is expected to save
-    high-level options, for instances, project and zone information, which
-    apply to all beam operators in the DAG.
+    Launch Apache Beam pipelines written in Go.
+
+    Note that both ``default_pipeline_options`` and ``pipeline_options``
+    will be merged to specify pipeline execution parameter, and
+    ``default_pipeline_options`` is expected to save high-level options,
+    for instances, project and zone information, which apply to all beam
+    operators in the DAG.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:BeamRunGoPipelineOperator`
 
     .. seealso::
         For more detail on Apache Beam have a look at the reference:
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-beam-5.2.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 setup.py
 airflow/providers/apache/beam/__init__.py
 airflow/providers/apache/beam/get_provider_info.py
 airflow/providers/apache/beam/hooks/__init__.py
 airflow/providers/apache/beam/hooks/beam.py
 airflow/providers/apache/beam/operators/__init__.py
 airflow/providers/apache/beam/operators/beam.py
+airflow/providers/apache/beam/triggers/__init__.py
+airflow/providers/apache/beam/triggers/beam.py
 apache_airflow_providers_apache_beam.egg-info/PKG-INFO
 apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
 apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
 apache_airflow_providers_apache_beam.egg-info/entry_points.txt
 apache_airflow_providers_apache_beam.egg-info/not-zip-safe
 apache_airflow_providers_apache_beam.egg-info/requires.txt
 apache_airflow_providers_apache_beam.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-beam-5.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-beam-5.2.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.2.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.2.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1rc1/setup.py` & `apache-airflow-providers-apache-beam-5.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-beam package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.1.1"
+version = "5.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-beam setup."""
     setup(
         version=version,
         extras_require={"google": ["apache-airflow-providers-google", "apache-beam[gcp]"]},
```

