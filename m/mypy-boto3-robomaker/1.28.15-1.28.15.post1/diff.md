# Comparing `tmp/mypy-boto3-robomaker-1.28.15.tar.gz` & `tmp/mypy-boto3-robomaker-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-robomaker-1.28.15.tar", last modified: Fri Jul 28 20:43:35 2023, max compression
+gzip compressed data, was "mypy-boto3-robomaker-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
```

## Comparing `mypy-boto3-robomaker-1.28.15.tar` & `mypy-boto3-robomaker-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42233 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42158 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-28 20:37:03.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68764 2023-07-28 20:37:05.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68697 2023-07-28 20:37:04.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22084 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:34.000000 mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:35.113746 mypy-boto3-robomaker-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:37:02.000000 mypy-boto3-robomaker-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20589 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42816 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42741 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-29 09:57:08.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69081 2023-07-29 09:57:10.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69014 2023-07-29 09:57:09.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:04:01.000000 mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.381365 mypy-boto3-robomaker-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-29 09:57:07.000000 mypy-boto3-robomaker-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-robomaker-1.28.15/LICENSE` & `mypy-boto3-robomaker-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/PKG-INFO` & `mypy-boto3-robomaker-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.15
-Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,22 +409,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
+    DataSourceConfigOutputTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.15/README.md` & `mypy-boto3-robomaker-1.28.15.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,22 +377,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
+    DataSourceConfigOutputTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__init__.pyi` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/__main__.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RoboMaker 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.RoboMaker 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.15.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_robomaker.client import RoboMakerClient
 
     session = Session()
     client: RoboMakerClient = session.client("robomaker")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ArchitectureType, FailureBehaviorType
 from .paginator import (
     ListDeploymentJobsPaginator,
     ListFleetsPaginator,
@@ -44,15 +44,17 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
     DataSourceConfigTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
@@ -78,26 +80,30 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
+    RobotApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     RobotSoftwareSuiteTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     SimulationApplicationConfigTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobRequestTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
+    VPCConfigOutputTypeDef,
     VPCConfigTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -220,15 +226,17 @@
         """
 
     def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
+        deploymentApplicationConfigs: Sequence[
+            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
+        ],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -329,19 +337,23 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
+        robotApplications: Sequence[
+            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
+        ] = ...,
+        simulationApplications: Sequence[
+            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
+        ] = ...,
+        dataSources: Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigTypeDef = ...,
+        vpcConfig: Union[VPCConfigTypeDef, VPCConfigOutputTypeDef] = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#create_simulation_job)
@@ -710,15 +722,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#restart_simulation_job)
         """
 
     def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
+        createSimulationJobRequests: Sequence[
+            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
+        ],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/client.pyi` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_robomaker.client import RoboMakerClient
 
     session = Session()
     client: RoboMakerClient = session.client("robomaker")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ArchitectureType, FailureBehaviorType
 from .paginator import (
     ListDeploymentJobsPaginator,
     ListFleetsPaginator,
@@ -44,15 +44,17 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
     DataSourceConfigTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
@@ -78,26 +80,30 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
+    RobotApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     RobotSoftwareSuiteTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     SimulationApplicationConfigTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobRequestTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
+    VPCConfigOutputTypeDef,
     VPCConfigTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -206,15 +212,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#close)
         """
     def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
+        deploymentApplicationConfigs: Sequence[
+            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
+        ],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -308,19 +316,23 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
+        robotApplications: Sequence[
+            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
+        ] = ...,
+        simulationApplications: Sequence[
+            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
+        ] = ...,
+        dataSources: Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigTypeDef = ...,
+        vpcConfig: Union[VPCConfigTypeDef, VPCConfigOutputTypeDef] = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#create_simulation_job)
@@ -652,15 +664,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/client/#restart_simulation_job)
         """
     def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
+        createSimulationJobRequests: Sequence[
+            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
+        ],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/literals.pyi` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/paginator.pyi` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.py` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
     data: BatchDeleteWorldsRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -66,22 +66,22 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
+    "DataSourceConfigOutputTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
@@ -458,14 +458,38 @@
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDataSourceConfigTypeDef = TypedDict(
     "_RequiredDataSourceConfigTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": Sequence[str],
     },
@@ -545,38 +569,14 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
-
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -2048,15 +2048,17 @@
 )
 
 _RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": Sequence[
+            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentJobRequestRequestTypeDef",
     {
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Mapping[str, str],
@@ -2427,17 +2429,21 @@
 _OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "robotApplications": Sequence[
+            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
+        ],
+        "simulationApplications": Sequence[
+            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
+        ],
+        "dataSources": Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]],
         "tags": Mapping[str, str],
         "vpcConfig": VPCConfigTypeDef,
         "compute": ComputeTypeDef,
     },
     total=False,
 )
 
@@ -2499,15 +2505,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
+        "createSimulationJobRequests": Sequence[
+            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
+        ],
     },
 )
 _OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker/type_defs.pyi` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
     data: BatchDeleteWorldsRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -65,22 +65,22 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
+    "DataSourceConfigOutputTypeDef",
     "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "DataSourceConfigOutputTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
     "DeploymentLaunchConfigOutputTypeDef",
@@ -449,14 +449,36 @@
 
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
 _RequiredDataSourceConfigTypeDef = TypedDict(
     "_RequiredDataSourceConfigTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": Sequence[str],
     },
@@ -532,36 +554,14 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -1999,15 +1999,17 @@
 )
 
 _RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": Sequence[
+            Union[DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef]
+        ],
     },
 )
 _OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentJobRequestRequestTypeDef",
     {
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Mapping[str, str],
@@ -2366,17 +2368,21 @@
 _OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "robotApplications": Sequence[
+            Union[RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef]
+        ],
+        "simulationApplications": Sequence[
+            Union[SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef]
+        ],
+        "dataSources": Sequence[Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]],
         "tags": Mapping[str, str],
         "vpcConfig": VPCConfigTypeDef,
         "compute": ComputeTypeDef,
     },
     total=False,
 )
 
@@ -2434,15 +2440,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
+        "createSimulationJobRequests": Sequence[
+            Union[SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef]
+        ],
     },
 )
 _OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
     "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/PKG-INFO` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-robomaker
-Version: 1.28.15
-Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-robomaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_robomaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -409,22 +409,22 @@
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
+    DataSourceConfigOutputTypeDef,
     DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    DataSourceConfigOutputTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
     DeploymentLaunchConfigOutputTypeDef,
```

### Comparing `mypy-boto3-robomaker-1.28.15/mypy_boto3_robomaker.egg-info/SOURCES.txt` & `mypy-boto3-robomaker-1.28.15.post1/mypy_boto3_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-robomaker-1.28.15/setup.py` & `mypy-boto3-robomaker-1.28.15.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-robomaker",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.RoboMaker 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

