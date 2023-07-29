# Comparing `tmp/mypy-boto3-databrew-1.28.15.tar.gz` & `tmp/mypy-boto3-databrew-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-databrew-1.28.15.tar", last modified: Fri Jul 28 20:42:35 2023, max compression
+gzip compressed data, was "mypy-boto3-databrew-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:54 2023, max compression
```

## Comparing `mypy-boto3-databrew-1.28.15.tar` & `mypy-boto3-databrew-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.032918 mypy-boto3-databrew-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-28 20:42:35.028918 mypy-boto3-databrew-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.016918 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-28 20:22:29.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-28 20:22:29.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59540 2023-07-28 20:22:32.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59430 2023-07-28 20:22:31.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.028918 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:35.032918 mypy-boto3-databrew-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.817097 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34421 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34362 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-29 09:41:56.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-29 09:41:56.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59707 2023-07-29 09:41:59.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59597 2023-07-29 09:41:58.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:02:54.000000 mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:54.829097 mypy-boto3-databrew-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-29 09:41:55.000000 mypy-boto3-databrew-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-databrew-1.28.15/LICENSE` & `mypy-boto3-databrew-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/PKG-INFO` & `mypy-boto3-databrew-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.15
-Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-databrew-1.28.15/README.md` & `mypy-boto3-databrew-1.28.15.post1/README.md`

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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.pyi` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__main__.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlueDataBrew 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.GlueDataBrew 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_databrew.client import GlueDataBrewClient
 
     session = Session()
     client: GlueDataBrewClient = session.client("databrew")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionModeType, InputFormatType, LogSubscriptionType
 from .paginator import (
     ListDatasetsPaginator,
     ListJobRunsPaginator,
@@ -49,32 +49,37 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
+    PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
+    ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
+    RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
@@ -161,16 +166,16 @@
 
     def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...,
+        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
+        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_dataset)
@@ -184,15 +189,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: ProfileConfigurationTypeDef = ...,
+        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -218,15 +223,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_project)
         """
 
     def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[RecipeStepTypeDef],
+        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -240,15 +245,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[OutputTypeDef] = ...,
+        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -262,15 +267,15 @@
         """
 
     def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[RuleTypeDef],
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -519,15 +524,15 @@
         """
 
     def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: RecipeStepTypeDef = ...,
+        RecipeStep: Union[RecipeStepTypeDef, RecipeStepOutputTypeDef] = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -582,31 +587,31 @@
 
     def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...
+        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
+        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_dataset)
         """
 
     def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: ProfileConfigurationTypeDef = ...,
+        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -626,15 +631,19 @@
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_project)
         """
 
     def update_recipe(
-        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepTypeDef] = ...
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe)
         """
@@ -645,28 +654,32 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[OutputTypeDef] = ...,
+        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe_job)
         """
 
     def update_ruleset(
-        self, *, Name: str, Rules: Sequence[RuleTypeDef], Description: str = ...
+        self,
+        *,
+        Name: str,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_ruleset)
         """
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.pyi` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_databrew.client import GlueDataBrewClient
 
     session = Session()
     client: GlueDataBrewClient = session.client("databrew")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EncryptionModeType, InputFormatType, LogSubscriptionType
 from .paginator import (
     ListDatasetsPaginator,
     ListJobRunsPaginator,
@@ -49,32 +49,37 @@
     DescribeDatasetResponseTypeDef,
     DescribeJobResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     DescribeRulesetResponseTypeDef,
     DescribeScheduleResponseTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
     InputTypeDef,
     JobSampleTypeDef,
     ListDatasetsResponseTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListRecipesResponseTypeDef,
     ListRecipeVersionsResponseTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
+    PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
+    ProfileConfigurationOutputTypeDef,
     ProfileConfigurationTypeDef,
     PublishRecipeResponseTypeDef,
     RecipeReferenceTypeDef,
+    RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     S3LocationTypeDef,
     SampleTypeDef,
     SendProjectSessionActionResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartProjectSessionResponseTypeDef,
     StopJobRunResponseTypeDef,
@@ -153,16 +158,16 @@
         """
     def create_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...,
+        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
+        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_dataset)
@@ -175,15 +180,15 @@
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Configuration: ProfileConfigurationTypeDef = ...,
+        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
         JobSample: JobSampleTypeDef = ...
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
@@ -207,15 +212,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_project)
         """
     def create_recipe(
         self,
         *,
         Name: str,
-        Steps: Sequence[RecipeStepTypeDef],
+        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
@@ -228,15 +233,15 @@
         RoleArn: str,
         DatasetName: str = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[OutputTypeDef] = ...,
+        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...
     ) -> CreateRecipeJobResponseTypeDef:
@@ -249,15 +254,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#create_recipe_job)
         """
     def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
-        Rules: Sequence[RuleTypeDef],
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a dataset.
 
@@ -480,15 +485,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#publish_recipe)
         """
     def send_project_session_action(
         self,
         *,
         Name: str,
         Preview: bool = ...,
-        RecipeStep: RecipeStepTypeDef = ...,
+        RecipeStep: Union[RecipeStepTypeDef, RecipeStepOutputTypeDef] = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
         ViewFrame: ViewFrameTypeDef = ...
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
@@ -537,30 +542,30 @@
         """
     def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
-        FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...
+        FormatOptions: Union[FormatOptionsTypeDef, FormatOptionsOutputTypeDef] = ...,
+        PathOptions: Union[PathOptionsTypeDef, PathOptionsOutputTypeDef] = ...
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_dataset)
         """
     def update_profile_job(
         self,
         *,
         Name: str,
         OutputLocation: S3LocationTypeDef,
         RoleArn: str,
-        Configuration: ProfileConfigurationTypeDef = ...,
+        Configuration: Union[ProfileConfigurationTypeDef, ProfileConfigurationOutputTypeDef] = ...,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
@@ -578,15 +583,19 @@
         """
         Modifies the definition of an existing DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_project)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_project)
         """
     def update_recipe(
-        self, *, Name: str, Description: str = ..., Steps: Sequence[RecipeStepTypeDef] = ...
+        self,
+        *,
+        Name: str,
+        Description: str = ...,
+        Steps: Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]] = ...
     ) -> UpdateRecipeResponseTypeDef:
         """
         Modifies the definition of the `LATEST_WORKING` version of a DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe)
         """
@@ -596,27 +605,31 @@
         Name: str,
         RoleArn: str,
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
-        Outputs: Sequence[OutputTypeDef] = ...,
+        Outputs: Sequence[Union[OutputTypeDef, OutputTypeDef]] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         Timeout: int = ...
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_recipe_job)
         """
     def update_ruleset(
-        self, *, Name: str, Rules: Sequence[RuleTypeDef], Description: str = ...
+        self,
+        *,
+        Name: str,
+        Rules: Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
+        Description: str = ...
     ) -> UpdateRulesetResponseTypeDef:
         """
         Updates specified ruleset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_ruleset)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/client/#update_ruleset)
         """
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.pyi` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.pyi` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.py` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
     data: AllowedStatisticsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AnalyticsModeType,
     CompressionFormatType,
     EncryptionModeType,
     InputFormatType,
     JobRunStateType,
@@ -1879,15 +1879,15 @@
     pass
 
 
 _RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecipeRequestRequestTypeDef",
     {
         "Name": str,
-        "Steps": Sequence[RecipeStepTypeDef],
+        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
     },
 )
 _OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRecipeRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Mapping[str, str],
@@ -1934,15 +1934,15 @@
         "Name": str,
     },
 )
 _OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRecipeRequestRequestTypeDef",
     {
         "Description": str,
-        "Steps": Sequence[RecipeStepTypeDef],
+        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
     },
     total=False,
 )
 
 
 class UpdateRecipeRequestRequestTypeDef(
     _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
@@ -1968,15 +1968,15 @@
 )
 
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "TargetArn": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 _OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRulesetRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Mapping[str, str],
@@ -1991,15 +1991,15 @@
     pass
 
 
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 _OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
         "Description": str,
     },
@@ -2068,15 +2068,15 @@
     {
         "DatasetName": str,
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[OutputTypeDef],
+        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "ProjectName": str,
         "RecipeReference": RecipeReferenceTypeDef,
         "Tags": Mapping[str, str],
         "Timeout": int,
     },
@@ -2167,15 +2167,15 @@
     "_OptionalUpdateRecipeJobRequestRequestTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[OutputTypeDef],
+        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "Timeout": int,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.pyi` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_databrew.type_defs import AllowedStatisticsOutputTypeDef
 
     data: AllowedStatisticsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AnalyticsModeType,
     CompressionFormatType,
     EncryptionModeType,
     InputFormatType,
     JobRunStateType,
@@ -1798,15 +1798,15 @@
 class RecipeTypeDef(_RequiredRecipeTypeDef, _OptionalRecipeTypeDef):
     pass
 
 _RequiredCreateRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRecipeRequestRequestTypeDef",
     {
         "Name": str,
-        "Steps": Sequence[RecipeStepTypeDef],
+        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
     },
 )
 _OptionalCreateRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRecipeRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Mapping[str, str],
@@ -1849,15 +1849,15 @@
         "Name": str,
     },
 )
 _OptionalUpdateRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRecipeRequestRequestTypeDef",
     {
         "Description": str,
-        "Steps": Sequence[RecipeStepTypeDef],
+        "Steps": Sequence[Union[RecipeStepTypeDef, RecipeStepOutputTypeDef]],
     },
     total=False,
 )
 
 class UpdateRecipeRequestRequestTypeDef(
     _RequiredUpdateRecipeRequestRequestTypeDef, _OptionalUpdateRecipeRequestRequestTypeDef
 ):
@@ -1881,15 +1881,15 @@
 )
 
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
         "TargetArn": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 _OptionalCreateRulesetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateRulesetRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Mapping[str, str],
@@ -1902,15 +1902,15 @@
 ):
     pass
 
 _RequiredUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRulesetRequestRequestTypeDef",
     {
         "Name": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[Union[RuleTypeDef, RuleOutputTypeDef]],
     },
 )
 _OptionalUpdateRulesetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateRulesetRequestRequestTypeDef",
     {
         "Description": str,
     },
@@ -1973,15 +1973,15 @@
     {
         "DatasetName": str,
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[OutputTypeDef],
+        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "ProjectName": str,
         "RecipeReference": RecipeReferenceTypeDef,
         "Tags": Mapping[str, str],
         "Timeout": int,
     },
@@ -2068,15 +2068,15 @@
     "_OptionalUpdateRecipeJobRequestRequestTypeDef",
     {
         "EncryptionKeyArn": str,
         "EncryptionMode": EncryptionModeType,
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
-        "Outputs": Sequence[OutputTypeDef],
+        "Outputs": Sequence[Union[OutputTypeDef, OutputTypeDef]],
         "DataCatalogOutputs": Sequence[DataCatalogOutputTypeDef],
         "DatabaseOutputs": Sequence[DatabaseOutputTypeDef],
         "Timeout": int,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/PKG-INFO` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.15
-Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/SOURCES.txt` & `mypy-boto3-databrew-1.28.15.post1/mypy_boto3_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.15/setup.py` & `mypy-boto3-databrew-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-databrew",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder"
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

