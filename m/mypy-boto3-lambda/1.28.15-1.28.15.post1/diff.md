# Comparing `tmp/mypy-boto3-lambda-1.28.15.tar.gz` & `tmp/mypy-boto3-lambda-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:30 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.28.15.tar` & `mypy-boto3-lambda-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.513381 mypy-boto3-lambda-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59706 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59616 2023-07-28 20:29:34.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79959 2023-07-28 20:29:38.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79852 2023-07-28 20:29:37.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.513381 mypy-boto3-lambda-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.485231 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60385 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60295 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79959 2023-07-29 09:49:15.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79852 2023-07-29 09:49:14.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-29 09:49:11.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25007 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-29 10:03:30.000000 mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:30.493232 mypy-boto3-lambda-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 09:49:10.000000 mypy-boto3-lambda-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-lambda-1.28.15/LICENSE` & `mypy-boto3-lambda-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/PKG-INFO` & `mypy-boto3-lambda-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.15
-Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lambda-1.28.15/README.md` & `mypy-boto3-lambda-1.28.15.post1/README.md`

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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Lambda 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,30 +45,34 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
+    AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
+    AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
+    CorsOutputTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
@@ -76,14 +80,15 @@
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
+    ImageConfigOutputTypeDef,
     ImageConfigTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
@@ -98,14 +103,15 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
+    SelfManagedEventSourceOutputTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
@@ -257,28 +263,30 @@
     def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
+        RoutingConfig: Union[
+            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+        ] = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
 
     def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: AllowedPublishersTypeDef,
+        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef],
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -288,28 +296,30 @@
     def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaTypeDef = ...,
+        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
         StartingPositionTimestamp: Union[datetime, str] = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
+        SelfManagedEventSource: Union[
+            SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
+        ] = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -336,15 +346,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigTypeDef = ...,
+        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -355,15 +365,15 @@
 
     def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: CorsTypeDef = ...,
+        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -993,15 +1003,17 @@
     def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
+        RoutingConfig: Union[
+            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+        ] = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -1010,15 +1022,15 @@
         """
 
     def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: AllowedPublishersTypeDef = ...,
+        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef] = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -1027,15 +1039,15 @@
     def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaTypeDef = ...,
+        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -1086,15 +1098,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigTypeDef = ...,
+        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1120,15 +1132,15 @@
 
     def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: CorsTypeDef = ...,
+        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,34 @@
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
     AliasConfigurationResponseTypeDef,
+    AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
+    AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
     ConcurrencyResponseTypeDef,
+    CorsOutputTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
     EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
     FunctionConfigurationResponseTypeDef,
     FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
@@ -76,14 +80,15 @@
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigResponseTypeDef,
+    ImageConfigOutputTypeDef,
     ImageConfigTypeDef,
     InvocationResponseTypeDef,
     InvokeAsyncResponseTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     LayerVersionContentInputTypeDef,
     ListAliasesResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
@@ -98,14 +103,15 @@
     ListTagsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     PutFunctionCodeSigningConfigResponseTypeDef,
     PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigResponseTypeDef,
     ScalingConfigTypeDef,
+    SelfManagedEventSourceOutputTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
     SnapStartTypeDef,
     SourceAccessConfigurationTypeDef,
     TracingConfigTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
@@ -248,27 +254,29 @@
     def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
+        RoutingConfig: Union[
+            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+        ] = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
     def create_code_signing_config(
         self,
         *,
-        AllowedPublishers: AllowedPublishersTypeDef,
+        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef],
         Description: str = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
@@ -277,28 +285,30 @@
     def create_event_source_mapping(
         self,
         *,
         FunctionName: str,
         EventSourceArn: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaTypeDef = ...,
+        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         ParallelizationFactor: int = ...,
         StartingPosition: EventSourcePositionType = ...,
         StartingPositionTimestamp: Union[datetime, str] = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         TumblingWindowInSeconds: int = ...,
         Topics: Sequence[str] = ...,
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
-        SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
+        SelfManagedEventSource: Union[
+            SelfManagedEventSourceTypeDef, SelfManagedEventSourceOutputTypeDef
+        ] = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
@@ -324,15 +334,15 @@
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         Environment: EnvironmentTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigTypeDef = ...,
+        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
@@ -342,15 +352,15 @@
         """
     def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
-        Cors: CorsTypeDef = ...,
+        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         InvokeMode: InvokeModeType = ...
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function_url_config)
@@ -926,15 +936,17 @@
     def update_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
+        RoutingConfig: Union[
+            AliasRoutingConfigurationTypeDef, AliasRoutingConfigurationOutputTypeDef
+        ] = ...,
         RevisionId: str = ...
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
@@ -942,15 +954,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_alias)
         """
     def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
-        AllowedPublishers: AllowedPublishersTypeDef = ...,
+        AllowedPublishers: Union[AllowedPublishersTypeDef, AllowedPublishersOutputTypeDef] = ...,
         CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_code_signing_config)
@@ -958,15 +970,15 @@
     def update_event_source_mapping(
         self,
         *,
         UUID: str,
         FunctionName: str = ...,
         Enabled: bool = ...,
         BatchSize: int = ...,
-        FilterCriteria: FilterCriteriaTypeDef = ...,
+        FilterCriteria: Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef] = ...,
         MaximumBatchingWindowInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...,
         MaximumRecordAgeInSeconds: int = ...,
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
@@ -1015,15 +1027,15 @@
         Runtime: RuntimeType = ...,
         DeadLetterConfig: DeadLetterConfigTypeDef = ...,
         KMSKeyArn: str = ...,
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
-        ImageConfig: ImageConfigTypeDef = ...,
+        ImageConfig: Union[ImageConfigTypeDef, ImageConfigOutputTypeDef] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
@@ -1047,15 +1059,15 @@
         """
     def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
-        Cors: CorsTypeDef = ...,
+        Cors: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         InvokeMode: InvokeModeType = ...
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_url_config)
```

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.15
-Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.28.15.post1/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.15/setup.py` & `mypy-boto3-lambda-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

