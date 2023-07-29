# Comparing `tmp/mypy-boto3-apigatewayv2-1.28.15.tar.gz` & `tmp/mypy-boto3-apigatewayv2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewayv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
```

## Comparing `mypy-boto3-apigatewayv2-1.28.15.tar` & `mypy-boto3-apigatewayv2-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.256654 mypy-boto3-apigatewayv2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-28 20:42:16.252654 mypy-boto3-apigatewayv2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.248654 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51603 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-28 20:19:08.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76314 2023-07-28 20:19:11.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76203 2023-07-28 20:19:10.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.252654 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:16.000000 mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.256654 mypy-boto3-apigatewayv2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:19:07.000000 mypy-boto3-apigatewayv2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.780993 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52061 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51972 2023-07-29 09:37:58.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-29 09:37:59.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76448 2023-07-29 09:38:02.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-07-29 09:38:00.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 10:02:27.000000 mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.800994 mypy-boto3-apigatewayv2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-29 09:37:57.000000 mypy-boto3-apigatewayv2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/LICENSE` & `mypy-boto3-apigatewayv2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.15
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,17 +377,17 @@
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
-    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/README.md` & `mypy-boto3-apigatewayv2-1.28.15.post1/README.md`

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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,17 +345,17 @@
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
-    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__init__.pyi` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/__main__.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayV2 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ApiGatewayV2 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 
     session = Session()
     client: ApiGatewayV2Client = session.client("apigatewayv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthorizationTypeType,
     AuthorizerTypeType,
     ConnectionTypeType,
@@ -38,27 +38,29 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
+    CorsOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     DomainNameConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
@@ -81,14 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
+    JWTConfigurationOutputTypeDef,
     JWTConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
@@ -166,15 +169,15 @@
 
     def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -207,15 +210,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_authorizer)
         """
@@ -230,15 +233,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_deployment)
         """
 
     def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -836,15 +841,15 @@
         """
 
     def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -883,15 +888,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...,
+        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_authorizer)
@@ -907,15 +912,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_deployment)
         """
 
     def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_domain_name)
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/client.pyi` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mypy_boto3_apigatewayv2.client import ApiGatewayV2Client
 
     session = Session()
     client: ApiGatewayV2Client = session.client("apigatewayv2")
     ```
 """
 import sys
-from typing import Any, Dict, Mapping, Sequence, Type, overload
+from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AuthorizationTypeType,
     AuthorizerTypeType,
     ConnectionTypeType,
@@ -38,27 +38,29 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
+    CorsOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     DomainNameConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
@@ -81,14 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
+    JWTConfigurationOutputTypeDef,
     JWTConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
@@ -159,15 +162,15 @@
         """
     def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -198,15 +201,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_authorizer)
         """
@@ -219,15 +222,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#create_deployment)
         """
     def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -768,15 +773,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#untag_resource)
         """
     def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: Union[CorsTypeDef, CorsOutputTypeDef] = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -813,15 +818,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...,
+        JwtConfiguration: Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef] = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_authorizer)
@@ -835,15 +840,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_deployment)
         """
     def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/client/#update_domain_name)
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/literals.pyi` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/paginator.pyi` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -336,57 +336,57 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": datetime,
+        "CertificateUploadDate": Union[datetime, str],
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
+    {
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
+    },
+    total=False,
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -1886,15 +1886,17 @@
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
@@ -1909,15 +1911,17 @@
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
     },
     total=False,
 )
 
 
 class UpdateDomainNameRequestRequestTypeDef(
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2/type_defs.pyi` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     "CorsOutputTypeDef",
     "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
-    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
@@ -329,57 +329,57 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
-DomainNameConfigurationOutputTypeDef = TypedDict(
-    "DomainNameConfigurationOutputTypeDef",
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": datetime,
+        "CertificateUploadDate": Union[datetime, str],
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
+    {
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
+    },
+    total=False,
+)
+
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -1819,15 +1819,17 @@
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateDomainNameRequestRequestTypeDef(
@@ -1840,15 +1842,17 @@
     {
         "DomainName": str,
     },
 )
 _OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDomainNameRequestRequestTypeDef",
     {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": Sequence[
+            Union[DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef]
+        ],
         "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
     },
     total=False,
 )
 
 class UpdateDomainNameRequestRequestTypeDef(
     _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/PKG-INFO` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewayv2
-Version: 1.28.15
-Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/
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
 [mypy-boto3-apigatewayv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,17 +377,17 @@
     CorsOutputTypeDef,
     JWTConfigurationOutputTypeDef,
     CorsTypeDef,
     CreateApiMappingRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
-    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
```

### Comparing `mypy-boto3-apigatewayv2-1.28.15/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt` & `mypy-boto3-apigatewayv2-1.28.15.post1/mypy_boto3_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewayv2-1.28.15/setup.py` & `mypy-boto3-apigatewayv2-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewayv2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ApiGatewayV2 1.28.15 service generated with mypy-boto3-builder"
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

