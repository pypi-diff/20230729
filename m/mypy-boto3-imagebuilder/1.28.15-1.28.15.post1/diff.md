# Comparing `tmp/mypy-boto3-imagebuilder-1.28.15.tar.gz` & `tmp/mypy-boto3-imagebuilder-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-imagebuilder-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
+gzip compressed data, was "mypy-boto3-imagebuilder-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:16 2023, max compression
```

## Comparing `mypy-boto3-imagebuilder-1.28.15.tar` & `mypy-boto3-imagebuilder-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.265213 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41846 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-28 20:27:38.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-28 20:27:38.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70382 2023-07-28 20:27:40.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70321 2023-07-28 20:27:39.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:56.000000 mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.269213 mypy-boto3-imagebuilder-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:27:36.000000 mypy-boto3-imagebuilder-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.549174 mypy-boto3-imagebuilder-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-29 10:03:16.545174 mypy-boto3-imagebuilder-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.537174 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42485 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42422 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-07-29 09:47:10.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-29 09:47:10.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    70589 2023-07-29 09:47:14.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70528 2023-07-29 09:47:11.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:16.545174 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:03:16.000000 mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:16.549174 mypy-boto3-imagebuilder-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:47:09.000000 mypy-boto3-imagebuilder-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/LICENSE` & `mypy-boto3-imagebuilder-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.15
-Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/README.md` & `mypy-boto3-imagebuilder-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/__main__.py` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.imagebuilder 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.imagebuilder 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.py` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_imagebuilder.client import imagebuilderClient
 
     session = Session()
     client: imagebuilderClient = session.client("imagebuilder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
@@ -33,14 +34,15 @@
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
@@ -49,19 +51,21 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
@@ -195,20 +199,24 @@
 
     def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationTypeDef = ...,
+        instanceConfiguration: Union[
+            InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+        ] = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -220,15 +228,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_container_recipe)
         """
 
     def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -243,15 +251,17 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image)
         """
@@ -267,29 +277,33 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image_pipeline)
         """
 
     def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -827,15 +841,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#untag_resource)
         """
 
     def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -852,15 +866,17 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/client.pyi` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     from mypy_boto3_imagebuilder.client import imagebuilderClient
 
     session = Session()
     client: imagebuilderClient = session.client("imagebuilder")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type
+from typing import Any, Dict, Mapping, Sequence, Type, Union
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
@@ -33,14 +34,15 @@
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
@@ -49,19 +51,21 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
@@ -186,20 +190,24 @@
         """
     def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationTypeDef = ...,
+        instanceConfiguration: Union[
+            InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+        ] = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -210,15 +218,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_container_recipe)
         """
     def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -232,15 +240,17 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image)
         """
@@ -255,28 +265,32 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#create_image_pipeline)
         """
     def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -766,15 +780,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#untag_resource)
         """
     def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -790,15 +804,17 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: Union[
+            ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+        ] = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.py` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/literals.pyi` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.py` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_imagebuilder.type_defs import SeverityCountsTypeDef
 
     data: SeverityCountsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -2036,15 +2036,17 @@
 )
 
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         "parentImage": str,
         "clientToken": str,
     },
 )
 _OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImageRecipeRequestRequestTypeDef",
     {
@@ -2448,15 +2450,17 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2528,15 +2532,15 @@
     pass
 
 
 _RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
     {
         "name": str,
-        "distributions": Sequence[DistributionTypeDef],
+        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         "clientToken": str,
     },
 )
 _OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
     {
         "description": str,
@@ -2553,15 +2557,15 @@
     pass
 
 
 _RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionTypeDef],
+        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         "clientToken": str,
     },
 )
 _OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
     {
         "description": str,
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder/type_defs.pyi` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_imagebuilder.type_defs import SeverityCountsTypeDef
 
     data: SeverityCountsTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -1999,15 +1999,17 @@
 )
 
 _RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImageRecipeRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         "parentImage": str,
         "clientToken": str,
     },
 )
 _OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateImageRecipeRequestRequestTypeDef",
     {
@@ -2395,15 +2397,17 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[
+            Union[ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef]
+        ],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2471,15 +2475,15 @@
 ):
     pass
 
 _RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
     {
         "name": str,
-        "distributions": Sequence[DistributionTypeDef],
+        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         "clientToken": str,
     },
 )
 _OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
     {
         "description": str,
@@ -2494,15 +2498,15 @@
 ):
     pass
 
 _RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionTypeDef],
+        "distributions": Sequence[Union[DistributionTypeDef, DistributionOutputTypeDef]],
         "clientToken": str,
     },
 )
 _OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
     {
         "description": str,
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/PKG-INFO` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.28.15
-Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
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
 [mypy-boto3-imagebuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-imagebuilder-1.28.15/mypy_boto3_imagebuilder.egg-info/SOURCES.txt` & `mypy-boto3-imagebuilder-1.28.15.post1/mypy_boto3_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.28.15/setup.py` & `mypy-boto3-imagebuilder-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-imagebuilder",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.imagebuilder 1.28.15 service generated with mypy-boto3-builder"
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

