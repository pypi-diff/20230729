# Comparing `tmp/mypy-boto3-devicefarm-1.28.15.tar.gz` & `tmp/mypy-boto3-devicefarm-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devicefarm-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
+gzip compressed data, was "mypy-boto3-devicefarm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:55 2023, max compression
```

## Comparing `mypy-boto3-devicefarm-1.28.15.tar` & `mypy-boto3-devicefarm-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.720957 mypy-boto3-devicefarm-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24826 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23327 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57697 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57593 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22346 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22324 2023-07-28 20:22:47.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74057 2023-07-28 20:22:50.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73966 2023-07-28 20:22:49.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.716957 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24826 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:37.000000 mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.720957 mypy-boto3-devicefarm-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:22:46.000000 mypy-boto3-devicefarm-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23327 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.789101 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58062 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57958 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22418 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-07-29 09:42:15.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    74125 2023-07-29 09:42:17.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74034 2023-07-29 09:42:16.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:55.793101 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:55.000000 mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:55.797101 mypy-boto3-devicefarm-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:42:13.000000 mypy-boto3-devicefarm-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-devicefarm-1.28.15/LICENSE` & `mypy-boto3-devicefarm-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/PKG-INFO` & `mypy-boto3-devicefarm-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.15
-Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devicefarm-1.28.15/README.md` & `mypy-boto3-devicefarm-1.28.15.post1/README.md`

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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__init__.pyi` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/__main__.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DeviceFarm 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.DeviceFarm 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm\nOther"
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

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
@@ -114,23 +115,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
+    TestGridVpcConfigOutputTypeDef,
     TestGridVpcConfigTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
+    VpcConfigOutputTypeDef,
     VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -249,15 +252,19 @@
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_network_profile)
         """
 
     def create_project(
-        self, *, name: str, defaultJobTimeoutMinutes: int = ..., vpcConfig: VpcConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        defaultJobTimeoutMinutes: int = ...,
+        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_project)
         """
@@ -282,15 +289,19 @@
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_remote_access_session)
         """
 
     def create_test_grid_project(
-        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        description: str = ...,
+        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_test_grid_project)
         """
@@ -615,15 +626,19 @@
         Gets information about device pools.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_device_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_device_pools)
         """
 
     def list_devices(
-        self, *, arn: str = ..., nextToken: str = ..., filters: Sequence[DeviceFilterTypeDef] = ...
+        self,
+        *,
+        arn: str = ...,
+        nextToken: str = ...,
+        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_devices)
         """
@@ -977,30 +992,30 @@
 
     def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_project)
         """
 
     def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigTypeDef = ...
+        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/client.pyi` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     CreateProjectResultTypeDef,
     CreateRemoteAccessSessionConfigurationTypeDef,
     CreateRemoteAccessSessionResultTypeDef,
     CreateTestGridProjectResultTypeDef,
     CreateTestGridUrlResultTypeDef,
     CreateUploadResultTypeDef,
     CreateVPCEConfigurationResultTypeDef,
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     DeviceSelectionConfigurationTypeDef,
     ExecutionConfigurationTypeDef,
     GetAccountSettingsResultTypeDef,
     GetDeviceInstanceResultTypeDef,
     GetDevicePoolCompatibilityResultTypeDef,
     GetDevicePoolResultTypeDef,
@@ -114,23 +115,25 @@
     ScheduleRunConfigurationTypeDef,
     ScheduleRunResultTypeDef,
     ScheduleRunTestTypeDef,
     StopJobResultTypeDef,
     StopRemoteAccessSessionResultTypeDef,
     StopRunResultTypeDef,
     TagTypeDef,
+    TestGridVpcConfigOutputTypeDef,
     TestGridVpcConfigTypeDef,
     UpdateDeviceInstanceResultTypeDef,
     UpdateDevicePoolResultTypeDef,
     UpdateInstanceProfileResultTypeDef,
     UpdateNetworkProfileResultTypeDef,
     UpdateProjectResultTypeDef,
     UpdateTestGridProjectResultTypeDef,
     UpdateUploadResultTypeDef,
     UpdateVPCEConfigurationResultTypeDef,
+    VpcConfigOutputTypeDef,
     VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -239,15 +242,19 @@
         """
         Creates a network profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_network_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_network_profile)
         """
     def create_project(
-        self, *, name: str, defaultJobTimeoutMinutes: int = ..., vpcConfig: VpcConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        defaultJobTimeoutMinutes: int = ...,
+        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
     ) -> CreateProjectResultTypeDef:
         """
         Creates a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_project)
         """
@@ -270,15 +277,19 @@
         """
         Specifies and starts a remote access session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_remote_access_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_remote_access_session)
         """
     def create_test_grid_project(
-        self, *, name: str, description: str = ..., vpcConfig: TestGridVpcConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        description: str = ...,
+        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
     ) -> CreateTestGridProjectResultTypeDef:
         """
         Creates a Selenium testing project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.create_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#create_test_grid_project)
         """
@@ -567,15 +578,19 @@
         """
         Gets information about device pools.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_device_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_device_pools)
         """
     def list_devices(
-        self, *, arn: str = ..., nextToken: str = ..., filters: Sequence[DeviceFilterTypeDef] = ...
+        self,
+        *,
+        arn: str = ...,
+        nextToken: str = ...,
+        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...
     ) -> ListDevicesResultTypeDef:
         """
         Gets information about unique device types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#list_devices)
         """
@@ -896,29 +911,29 @@
         """
     def update_project(
         self,
         *,
         arn: str,
         name: str = ...,
         defaultJobTimeoutMinutes: int = ...,
-        vpcConfig: VpcConfigTypeDef = ...
+        vpcConfig: Union[VpcConfigTypeDef, VpcConfigOutputTypeDef] = ...
     ) -> UpdateProjectResultTypeDef:
         """
         Modifies the specified project name, given the project ARN and a new name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_project)
         """
     def update_test_grid_project(
         self,
         *,
         projectArn: str,
         name: str = ...,
         description: str = ...,
-        vpcConfig: TestGridVpcConfigTypeDef = ...
+        vpcConfig: Union[TestGridVpcConfigTypeDef, TestGridVpcConfigOutputTypeDef] = ...
     ) -> UpdateTestGridProjectResultTypeDef:
         """
         Change details of a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Client.update_test_grid_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/client/#update_test_grid_project)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/literals.pyi` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,25 +53,26 @@
     list_suites_paginator: ListSuitesPaginator = client.get_paginator("list_suites")
     list_tests_paginator: ListTestsPaginator = client.get_paginator("list_tests")
     list_unique_problems_paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")
     list_uploads_paginator: ListUploadsPaginator = client.get_paginator("list_uploads")
     list_vpce_configurations_paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
@@ -200,15 +201,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[DeviceFilterTypeDef] = ...,
+        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/paginator.pyi` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,25 +53,26 @@
     list_suites_paginator: ListSuitesPaginator = client.get_paginator("list_suites")
     list_tests_paginator: ListTestsPaginator = client.get_paginator("list_tests")
     list_unique_problems_paginator: ListUniqueProblemsPaginator = client.get_paginator("list_unique_problems")
     list_uploads_paginator: ListUploadsPaginator = client.get_paginator("list_uploads")
     list_vpce_configurations_paginator: ListVPCEConfigurationsPaginator = client.get_paginator("list_vpce_configurations")
     ```
 """
-from typing import Generic, Iterator, Sequence, TypeVar
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArtifactCategoryType,
     DevicePoolTypeType,
     NetworkProfileTypeType,
     UploadTypeType,
 )
 from .type_defs import (
+    DeviceFilterOutputTypeDef,
     DeviceFilterTypeDef,
     GetOfferingStatusResultTypeDef,
     ListArtifactsResultTypeDef,
     ListDeviceInstancesResultTypeDef,
     ListDevicePoolsResultTypeDef,
     ListDevicesResultTypeDef,
     ListInstanceProfilesResultTypeDef,
@@ -193,15 +194,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         arn: str = ...,
-        filters: Sequence[DeviceFilterTypeDef] = ...,
+        filters: Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#DeviceFarm.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.py` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1922,15 +1922,15 @@
 )
 
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
     },
     total=False,
 )
 
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
@@ -2029,15 +2029,15 @@
     pass
 
 
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm/type_defs.pyi` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1857,15 +1857,15 @@
 )
 
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "arn": str,
         "nextToken": str,
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
     },
     total=False,
 )
 
 SuiteTypeDef = TypedDict(
     "SuiteTypeDef",
     {
@@ -1960,15 +1960,15 @@
 ):
     pass
 
 ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
     "ListDevicesRequestListDevicesPaginateTypeDef",
     {
         "arn": str,
-        "filters": Sequence[DeviceFilterTypeDef],
+        "filters": Sequence[Union[DeviceFilterTypeDef, DeviceFilterOutputTypeDef]],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef = TypedDict(
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/PKG-INFO` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devicefarm
-Version: 1.28.15
-Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/
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
 [mypy-boto3-devicefarm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devicefarm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devicefarm-1.28.15/mypy_boto3_devicefarm.egg-info/SOURCES.txt` & `mypy-boto3-devicefarm-1.28.15.post1/mypy_boto3_devicefarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devicefarm-1.28.15/setup.py` & `mypy-boto3-devicefarm-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-devicefarm",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_devicefarm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DeviceFarm 1.28.15 service generated with mypy-boto3-builder"
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

