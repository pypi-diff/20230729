# Comparing `tmp/mypy-boto3-cloudfront-1.28.15.tar.gz` & `tmp/mypy-boto3-cloudfront-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.28.15.tar", last modified: Fri Jul 28 19:47:31 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
```

## Comparing `mypy-boto3-cloudfront-1.28.15.tar` & `mypy-boto3-cloudfront-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31719 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79465 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79345 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-28 19:47:01.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   172458 2023-07-28 19:46:59.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-28 19:46:57.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 19:47:31.000000 mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:47:31.672180 mypy-boto3-cloudfront-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 19:46:56.000000 mypy-boto3-cloudfront-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.625051 mypy-boto3-cloudfront-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 10:02:41.621050 mypy-boto3-cloudfront-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31719 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.617051 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81323 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81203 2023-07-29 09:40:01.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   172819 2023-07-29 09:40:07.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172458 2023-07-29 09:40:04.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-29 09:40:02.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:41.621050 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33224 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:02:41.000000 mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:41.625051 mypy-boto3-cloudfront-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-29 09:40:00.000000 mypy-boto3-cloudfront-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.28.15/LICENSE` & `mypy-boto3-cloudfront-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/PKG-INFO` & `mypy-boto3-cloudfront-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.28.15/README.md` & `mypy-boto3-cloudfront-1.28.15.post1/README.md`

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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudFront 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
+    CachePolicyConfigOutputTypeDef,
     CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
@@ -51,19 +53,22 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileConfigTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
@@ -86,15 +91,17 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
+    KeyGroupConfigOutputTypeDef,
     KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
@@ -113,21 +120,25 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
@@ -371,15 +382,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
 
     def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
+        self, *, CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -391,26 +402,32 @@
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
 
     def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
+        self,
+        *,
+        ContinuousDeploymentPolicyConfig: Union[
+            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+        ]
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
 
     def create_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef
+        self,
+        *,
+        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -422,25 +439,33 @@
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
 
     def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
+        self,
+        *,
+        FieldLevelEncryptionConfig: Union[
+            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+        ]
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
 
     def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
+        self,
+        *,
+        FieldLevelEncryptionProfileConfig: Union[
+            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+        ]
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
@@ -456,25 +481,28 @@
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
 
     def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
+        self,
+        *,
+        DistributionId: str,
+        InvalidationBatch: Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
 
     def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
+        self, *, KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -497,15 +525,19 @@
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
 
     def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
+        self,
+        *,
+        OriginRequestPolicyConfig: Union[
+            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+        ]
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -536,25 +568,33 @@
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
 
     def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
+        self,
+        *,
+        ResponseHeadersPolicyConfig: Union[
+            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+        ]
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
 
     def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
+        self,
+        *,
+        StreamingDistributionConfig: Union[
+            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+        ]
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1241,15 +1281,17 @@
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
 
-    def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
+    def tag_resource(
+        self, *, Resource: str, Tags: Union[TagsTypeDef, TagsOutputTypeDef]
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
 
@@ -1275,15 +1317,19 @@
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
 
     def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1301,27 +1347,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
 
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
+        ContinuousDeploymentPolicyConfig: Union[
+            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
 
     def update_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1336,29 +1388,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
 
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
+        FieldLevelEncryptionConfig: Union[
+            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
 
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
+        FieldLevelEncryptionProfileConfig: Union[
+            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1377,15 +1433,19 @@
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
 
     def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1403,15 +1463,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
 
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
+        OriginRequestPolicyConfig: Union[
+            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1443,29 +1505,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
 
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
+        ResponseHeadersPolicyConfig: Union[
+            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
 
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
+        StreamingDistributionConfig: Union[
+            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 from .paginator import (
     ListCloudFrontOriginAccessIdentitiesPaginator,
     ListDistributionsPaginator,
     ListInvalidationsPaginator,
     ListStreamingDistributionsPaginator,
 )
 from .type_defs import (
+    CachePolicyConfigOutputTypeDef,
     CachePolicyConfigTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
     CopyDistributionResultTypeDef,
     CreateCachePolicyResultTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
@@ -51,19 +53,22 @@
     CreateOriginRequestPolicyResultTypeDef,
     CreatePublicKeyResultTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     DescribeFunctionResultTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionConfigTypeDef,
     DistributionConfigWithTagsTypeDef,
     EmptyResponseMetadataTypeDef,
     EndPointTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileConfigTypeDef,
     FunctionConfigTypeDef,
     GetCachePolicyConfigResultTypeDef,
     GetCachePolicyResultTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
@@ -86,15 +91,17 @@
     GetPublicKeyConfigResultTypeDef,
     GetPublicKeyResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
     GetStreamingDistributionResultTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
+    KeyGroupConfigOutputTypeDef,
     KeyGroupConfigTypeDef,
     ListCachePoliciesResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
@@ -113,21 +120,25 @@
     ListPublicKeysResultTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
     ListStreamingDistributionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlConfigTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     OriginRequestPolicyConfigTypeDef,
     PublicKeyConfigTypeDef,
     PublishFunctionResultTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagKeysTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
     TestFunctionResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateContinuousDeploymentPolicyResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
@@ -362,15 +373,15 @@
         Creates a staging distribution using the configuration of the provided primary
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.copy_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#copy_distribution)
         """
     def create_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef
+        self, *, CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef]
     ) -> CreateCachePolicyResultTypeDef:
         """
         Creates a cache policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cache_policy)
         """
@@ -380,25 +391,31 @@
         """
         Creates a new origin access identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_cloud_front_origin_access_identity)
         """
     def create_continuous_deployment_policy(
-        self, *, ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef
+        self,
+        *,
+        ContinuousDeploymentPolicyConfig: Union[
+            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+        ]
     ) -> CreateContinuousDeploymentPolicyResultTypeDef:
         """
         Creates a continuous deployment policy that distributes traffic for a custom
         domain name to two different CloudFront distributions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_continuous_deployment_policy)
         """
     def create_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef
+        self,
+        *,
+        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef]
     ) -> CreateDistributionResultTypeDef:
         """
         Creates a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution)
         """
@@ -408,24 +425,32 @@
         """
         Create a new distribution with tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_distribution_with_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_distribution_with_tags)
         """
     def create_field_level_encryption_config(
-        self, *, FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef
+        self,
+        *,
+        FieldLevelEncryptionConfig: Union[
+            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+        ]
     ) -> CreateFieldLevelEncryptionConfigResultTypeDef:
         """
         Create a new field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_config)
         """
     def create_field_level_encryption_profile(
-        self, *, FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef
+        self,
+        *,
+        FieldLevelEncryptionProfileConfig: Union[
+            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+        ]
     ) -> CreateFieldLevelEncryptionProfileResultTypeDef:
         """
         Create a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_field_level_encryption_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_field_level_encryption_profile)
         """
@@ -439,24 +464,27 @@
         """
         Creates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_function)
         """
     def create_invalidation(
-        self, *, DistributionId: str, InvalidationBatch: InvalidationBatchTypeDef
+        self,
+        *,
+        DistributionId: str,
+        InvalidationBatch: Union[InvalidationBatchTypeDef, InvalidationBatchOutputTypeDef]
     ) -> CreateInvalidationResultTypeDef:
         """
         Create a new invalidation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_invalidation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_invalidation)
         """
     def create_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef
+        self, *, KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef]
     ) -> CreateKeyGroupResultTypeDef:
         """
         Creates a key group that you can use with [CloudFront signed URLs and signed
         cookies](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/PrivateContent.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_key_group)
@@ -476,15 +504,19 @@
         """
         Creates a new origin access control in CloudFront.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_access_control)
         """
     def create_origin_request_policy(
-        self, *, OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef
+        self,
+        *,
+        OriginRequestPolicyConfig: Union[
+            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+        ]
     ) -> CreateOriginRequestPolicyResultTypeDef:
         """
         Creates an origin request policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_origin_request_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_origin_request_policy)
         """
@@ -512,24 +544,32 @@
         """
         Creates a real-time log configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_realtime_log_config)
         """
     def create_response_headers_policy(
-        self, *, ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef
+        self,
+        *,
+        ResponseHeadersPolicyConfig: Union[
+            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+        ]
     ) -> CreateResponseHeadersPolicyResultTypeDef:
         """
         Creates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_response_headers_policy)
         """
     def create_streaming_distribution(
-        self, *, StreamingDistributionConfig: StreamingDistributionConfigTypeDef
+        self,
+        *,
+        StreamingDistributionConfig: Union[
+            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+        ]
     ) -> CreateStreamingDistributionResultTypeDef:
         """
         This API is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.create_streaming_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#create_streaming_distribution)
         """
@@ -1145,15 +1185,17 @@
         """
         Publishes a CloudFront function by copying the function code from the
         `DEVELOPMENT` stage to `LIVE`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.publish_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#publish_function)
         """
-    def tag_resource(self, *, Resource: str, Tags: TagsTypeDef) -> EmptyResponseMetadataTypeDef:
+    def tag_resource(
+        self, *, Resource: str, Tags: Union[TagsTypeDef, TagsOutputTypeDef]
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Add tags to a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#tag_resource)
         """
     def test_function(
@@ -1176,15 +1218,19 @@
         """
         Remove tags from a CloudFront resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#untag_resource)
         """
     def update_cache_policy(
-        self, *, CachePolicyConfig: CachePolicyConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        CachePolicyConfig: Union[CachePolicyConfigTypeDef, CachePolicyConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateCachePolicyResultTypeDef:
         """
         Updates a cache policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cache_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cache_policy)
         """
@@ -1200,26 +1246,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_cloud_front_origin_access_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_cloud_front_origin_access_identity)
         """
     def update_continuous_deployment_policy(
         self,
         *,
-        ContinuousDeploymentPolicyConfig: ContinuousDeploymentPolicyConfigTypeDef,
+        ContinuousDeploymentPolicyConfig: Union[
+            ContinuousDeploymentPolicyConfigTypeDef, ContinuousDeploymentPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateContinuousDeploymentPolicyResultTypeDef:
         """
         Updates a continuous deployment policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_continuous_deployment_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_continuous_deployment_policy)
         """
     def update_distribution(
-        self, *, DistributionConfig: DistributionConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        DistributionConfig: Union[DistributionConfigTypeDef, DistributionConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates the configuration for a CloudFront distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution)
         """
@@ -1232,28 +1284,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_distribution_with_staging_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_distribution_with_staging_config)
         """
     def update_field_level_encryption_config(
         self,
         *,
-        FieldLevelEncryptionConfig: FieldLevelEncryptionConfigTypeDef,
+        FieldLevelEncryptionConfig: Union[
+            FieldLevelEncryptionConfigTypeDef, FieldLevelEncryptionConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionConfigResultTypeDef:
         """
         Update a field-level encryption configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_field_level_encryption_config)
         """
     def update_field_level_encryption_profile(
         self,
         *,
-        FieldLevelEncryptionProfileConfig: FieldLevelEncryptionProfileConfigTypeDef,
+        FieldLevelEncryptionProfileConfig: Union[
+            FieldLevelEncryptionProfileConfigTypeDef, FieldLevelEncryptionProfileConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateFieldLevelEncryptionProfileResultTypeDef:
         """
         Update a field-level encryption profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_field_level_encryption_profile)
@@ -1270,15 +1326,19 @@
         """
         Updates a CloudFront function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_function)
         """
     def update_key_group(
-        self, *, KeyGroupConfig: KeyGroupConfigTypeDef, Id: str, IfMatch: str = ...
+        self,
+        *,
+        KeyGroupConfig: Union[KeyGroupConfigTypeDef, KeyGroupConfigOutputTypeDef],
+        Id: str,
+        IfMatch: str = ...
     ) -> UpdateKeyGroupResultTypeDef:
         """
         Updates a key group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_key_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_key_group)
         """
@@ -1294,15 +1354,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_access_control)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_origin_access_control)
         """
     def update_origin_request_policy(
         self,
         *,
-        OriginRequestPolicyConfig: OriginRequestPolicyConfigTypeDef,
+        OriginRequestPolicyConfig: Union[
+            OriginRequestPolicyConfigTypeDef, OriginRequestPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateOriginRequestPolicyResultTypeDef:
         """
         Updates an origin request policy configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_origin_request_policy)
@@ -1331,28 +1393,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_realtime_log_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_realtime_log_config)
         """
     def update_response_headers_policy(
         self,
         *,
-        ResponseHeadersPolicyConfig: ResponseHeadersPolicyConfigTypeDef,
+        ResponseHeadersPolicyConfig: Union[
+            ResponseHeadersPolicyConfigTypeDef, ResponseHeadersPolicyConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateResponseHeadersPolicyResultTypeDef:
         """
         Updates a response headers policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_response_headers_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/client/#update_response_headers_policy)
         """
     def update_streaming_distribution(
         self,
         *,
-        StreamingDistributionConfig: StreamingDistributionConfigTypeDef,
+        StreamingDistributionConfig: Union[
+            StreamingDistributionConfigTypeDef, StreamingDistributionConfigOutputTypeDef
+        ],
         Id: str,
         IfMatch: str = ...
     ) -> UpdateStreamingDistributionResultTypeDef:
         """
         Update a streaming distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront.Client.update_streaming_distribution)
```

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudfront-1.28.15/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.28.15.post1/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.15/setup.py` & `mypy-boto3-cloudfront-1.28.15.post1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudFront 1.28.15 service generated with mypy-boto3-builder"
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

