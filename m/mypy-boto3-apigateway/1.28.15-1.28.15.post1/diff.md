# Comparing `tmp/mypy-boto3-apigateway-1.28.15.tar.gz` & `tmp/mypy-boto3-apigateway-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigateway-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-apigateway-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
```

## Comparing `mypy-boto3-apigateway-1.28.15.tar` & `mypy-boto3-apigateway-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.664609 mypy-boto3-apigateway-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24660 2023-07-28 20:42:12.664609 mypy-boto3-apigateway-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23161 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.656609 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82381 2023-07-28 20:19:01.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    82236 2023-07-28 20:19:01.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-28 20:19:02.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-28 20:19:02.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-28 20:19:01.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-07-28 20:19:01.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93286 2023-07-28 20:19:05.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93137 2023-07-28 20:19:03.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.664609 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24660 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:12.000000 mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.664609 mypy-boto3-apigateway-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:19:00.000000 mypy-boto3-apigateway-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.760993 mypy-boto3-apigateway-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-29 10:02:27.756993 mypy-boto3-apigateway-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23161 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.748993 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82677 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82532 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19976 2023-07-29 09:37:52.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    93316 2023-07-29 09:37:56.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93167 2023-07-29 09:37:54.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.756993 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:27.000000 mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.760993 mypy-boto3-apigateway-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:37:51.000000 mypy-boto3-apigateway-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-apigateway-1.28.15/LICENSE` & `mypy-boto3-apigateway-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/PKG-INFO` & `mypy-boto3-apigateway-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.28.15
-Summary: Type annotations for boto3.APIGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.APIGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apigateway-1.28.15/README.md` & `mypy-boto3-apigateway-1.28.15.post1/README.md`

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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__init__.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__init__.pyi` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/__main__.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.APIGateway 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.APIGateway 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway\nOther"
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

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/client.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,19 +53,21 @@
     GetVpcLinksPaginator,
 )
 from .type_defs import (
     AccountTypeDef,
     ApiKeyIdsTypeDef,
     ApiKeyResponseTypeDef,
     ApiKeysTypeDef,
+    ApiStageOutputTypeDef,
     ApiStageTypeDef,
     AuthorizerResponseTypeDef,
     AuthorizersTypeDef,
     BasePathMappingResponseTypeDef,
     BasePathMappingsTypeDef,
+    CanarySettingsOutputTypeDef,
     CanarySettingsTypeDef,
     ClientCertificateResponseTypeDef,
     ClientCertificatesTypeDef,
     DeploymentCanarySettingsTypeDef,
     DeploymentResponseTypeDef,
     DeploymentsTypeDef,
     DocumentationPartIdsTypeDef,
@@ -73,14 +75,15 @@
     DocumentationPartResponseTypeDef,
     DocumentationPartsTypeDef,
     DocumentationVersionResponseTypeDef,
     DocumentationVersionsTypeDef,
     DomainNameResponseTypeDef,
     DomainNamesTypeDef,
     EmptyResponseMetadataTypeDef,
+    EndpointConfigurationOutputTypeDef,
     EndpointConfigurationTypeDef,
     ExportResponseTypeDef,
     GatewayResponseResponseTypeDef,
     GatewayResponsesTypeDef,
     IntegrationExtraResponseTypeDef,
     IntegrationResponseResponseTypeDef,
     MethodExtraResponseTypeDef,
@@ -282,15 +285,17 @@
         certificateName: str = ...,
         certificateBody: str = ...,
         certificatePrivateKey: str = ...,
         certificateChain: str = ...,
         certificateArn: str = ...,
         regionalCertificateName: str = ...,
         regionalCertificateArn: str = ...,
-        endpointConfiguration: EndpointConfigurationTypeDef = ...,
+        endpointConfiguration: Union[
+            EndpointConfigurationTypeDef, EndpointConfigurationOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         securityPolicy: SecurityPolicyType = ...,
         mutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         ownershipVerificationCertificateArn: str = ...
     ) -> DomainNameResponseTypeDef:
         """
         Creates a new domain name.
@@ -346,15 +351,17 @@
         name: str,
         description: str = ...,
         version: str = ...,
         cloneFrom: str = ...,
         binaryMediaTypes: Sequence[str] = ...,
         minimumCompressionSize: int = ...,
         apiKeySource: ApiKeySourceTypeType = ...,
-        endpointConfiguration: EndpointConfigurationTypeDef = ...,
+        endpointConfiguration: Union[
+            EndpointConfigurationTypeDef, EndpointConfigurationOutputTypeDef
+        ] = ...,
         policy: str = ...,
         tags: Mapping[str, str] = ...,
         disableExecuteApiEndpoint: bool = ...
     ) -> RestApiResponseTypeDef:
         """
         Creates a new RestApi resource.
 
@@ -369,15 +376,15 @@
         stageName: str,
         deploymentId: str,
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         documentationVersion: str = ...,
-        canarySettings: CanarySettingsTypeDef = ...,
+        canarySettings: Union[CanarySettingsTypeDef, CanarySettingsOutputTypeDef] = ...,
         tracingEnabled: bool = ...,
         tags: Mapping[str, str] = ...
     ) -> StageResponseTypeDef:
         """
         Creates a new Stage resource that references a pre-existing Deployment for the
         API.
 
@@ -386,15 +393,15 @@
         """
 
     def create_usage_plan(
         self,
         *,
         name: str,
         description: str = ...,
-        apiStages: Sequence[ApiStageTypeDef] = ...,
+        apiStages: Sequence[Union[ApiStageTypeDef, ApiStageOutputTypeDef]] = ...,
         throttle: ThrottleSettingsTypeDef = ...,
         quota: QuotaSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> UsagePlanResponseTypeDef:
         """
         Creates a usage plan with the throttle and quota limits, as well as the
         associated API stages, specified in the payload.
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/client.pyi` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,19 +53,21 @@
     GetVpcLinksPaginator,
 )
 from .type_defs import (
     AccountTypeDef,
     ApiKeyIdsTypeDef,
     ApiKeyResponseTypeDef,
     ApiKeysTypeDef,
+    ApiStageOutputTypeDef,
     ApiStageTypeDef,
     AuthorizerResponseTypeDef,
     AuthorizersTypeDef,
     BasePathMappingResponseTypeDef,
     BasePathMappingsTypeDef,
+    CanarySettingsOutputTypeDef,
     CanarySettingsTypeDef,
     ClientCertificateResponseTypeDef,
     ClientCertificatesTypeDef,
     DeploymentCanarySettingsTypeDef,
     DeploymentResponseTypeDef,
     DeploymentsTypeDef,
     DocumentationPartIdsTypeDef,
@@ -73,14 +75,15 @@
     DocumentationPartResponseTypeDef,
     DocumentationPartsTypeDef,
     DocumentationVersionResponseTypeDef,
     DocumentationVersionsTypeDef,
     DomainNameResponseTypeDef,
     DomainNamesTypeDef,
     EmptyResponseMetadataTypeDef,
+    EndpointConfigurationOutputTypeDef,
     EndpointConfigurationTypeDef,
     ExportResponseTypeDef,
     GatewayResponseResponseTypeDef,
     GatewayResponsesTypeDef,
     IntegrationExtraResponseTypeDef,
     IntegrationResponseResponseTypeDef,
     MethodExtraResponseTypeDef,
@@ -269,15 +272,17 @@
         certificateName: str = ...,
         certificateBody: str = ...,
         certificatePrivateKey: str = ...,
         certificateChain: str = ...,
         certificateArn: str = ...,
         regionalCertificateName: str = ...,
         regionalCertificateArn: str = ...,
-        endpointConfiguration: EndpointConfigurationTypeDef = ...,
+        endpointConfiguration: Union[
+            EndpointConfigurationTypeDef, EndpointConfigurationOutputTypeDef
+        ] = ...,
         tags: Mapping[str, str] = ...,
         securityPolicy: SecurityPolicyType = ...,
         mutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         ownershipVerificationCertificateArn: str = ...
     ) -> DomainNameResponseTypeDef:
         """
         Creates a new domain name.
@@ -329,15 +334,17 @@
         name: str,
         description: str = ...,
         version: str = ...,
         cloneFrom: str = ...,
         binaryMediaTypes: Sequence[str] = ...,
         minimumCompressionSize: int = ...,
         apiKeySource: ApiKeySourceTypeType = ...,
-        endpointConfiguration: EndpointConfigurationTypeDef = ...,
+        endpointConfiguration: Union[
+            EndpointConfigurationTypeDef, EndpointConfigurationOutputTypeDef
+        ] = ...,
         policy: str = ...,
         tags: Mapping[str, str] = ...,
         disableExecuteApiEndpoint: bool = ...
     ) -> RestApiResponseTypeDef:
         """
         Creates a new RestApi resource.
 
@@ -351,15 +358,15 @@
         stageName: str,
         deploymentId: str,
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         documentationVersion: str = ...,
-        canarySettings: CanarySettingsTypeDef = ...,
+        canarySettings: Union[CanarySettingsTypeDef, CanarySettingsOutputTypeDef] = ...,
         tracingEnabled: bool = ...,
         tags: Mapping[str, str] = ...
     ) -> StageResponseTypeDef:
         """
         Creates a new Stage resource that references a pre-existing Deployment for the
         API.
 
@@ -367,15 +374,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/client/#create_stage)
         """
     def create_usage_plan(
         self,
         *,
         name: str,
         description: str = ...,
-        apiStages: Sequence[ApiStageTypeDef] = ...,
+        apiStages: Sequence[Union[ApiStageTypeDef, ApiStageOutputTypeDef]] = ...,
         throttle: ThrottleSettingsTypeDef = ...,
         quota: QuotaSettingsTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> UsagePlanResponseTypeDef:
         """
         Creates a usage plan with the throttle and quota limits, as well as the
         associated API stages, specified in the payload.
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/literals.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/literals.pyi` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/paginator.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/paginator.pyi` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/type_defs.py` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3541,15 +3541,15 @@
         "name": str,
     },
 )
 _OptionalCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_OptionalCreateUsagePlanRequestRequestTypeDef",
     {
         "description": str,
-        "apiStages": Sequence[ApiStageTypeDef],
+        "apiStages": Sequence[Union[ApiStageTypeDef, ApiStageOutputTypeDef]],
         "throttle": ThrottleSettingsTypeDef,
         "quota": QuotaSettingsTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway/type_defs.pyi` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -3394,15 +3394,15 @@
         "name": str,
     },
 )
 _OptionalCreateUsagePlanRequestRequestTypeDef = TypedDict(
     "_OptionalCreateUsagePlanRequestRequestTypeDef",
     {
         "description": str,
-        "apiStages": Sequence[ApiStageTypeDef],
+        "apiStages": Sequence[Union[ApiStageTypeDef, ApiStageOutputTypeDef]],
         "throttle": ThrottleSettingsTypeDef,
         "quota": QuotaSettingsTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/PKG-INFO` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigateway
-Version: 1.28.15
-Summary: Type annotations for boto3.APIGateway 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.APIGateway 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/
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
 [mypy-boto3-apigateway docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-apigateway-1.28.15/mypy_boto3_apigateway.egg-info/SOURCES.txt` & `mypy-boto3-apigateway-1.28.15.post1/mypy_boto3_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigateway-1.28.15/setup.py` & `mypy-boto3-apigateway-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigateway",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_apigateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.APIGateway 1.28.15 service generated with mypy-boto3-builder"
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

