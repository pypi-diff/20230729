# Comparing `tmp/aws-cdk.app-staging-synthesizer-alpha-2.88.0a0.tar.gz` & `tmp/aws-cdk.app-staging-synthesizer-alpha-2.89.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src3082485108/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer", last modified: Thu Jul 20 12:41:26 2023, max compression
+gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/app-staging-synthesizer-alpha/dist/python/aws-cdk.app-staging-synthesizer", last modified: Fri Jul 28 22:05:33 2023, max compression
```

## Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0.tar` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15939 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14919 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1949 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
--rw-r--r--   0 root         (0) root         (0)   181008 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82388 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.88.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:41:19.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15939 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-20 12:41:26.000000 aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15939 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14919 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/
+-rw-r--r--   0 root         (0) root         (0)   186500 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82762 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.89.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:24.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15939 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:05:33.000000 aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/LICENSE` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/PKG-INFO` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-staging-synthesizer-alpha
-Version: 2.88.0a0
+Version: 2.89.0a0
 Summary: Cdk synthesizer for with app-scoped staging stack
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/README.md` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/setup.py` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.app-staging-synthesizer-alpha",
-    "version": "2.88.0.a0",
+    "version": "2.89.0.a0",
     "description": "Cdk synthesizer for with app-scoped staging stack",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.app_staging_synthesizer_alpha",
         "aws_cdk.app_staging_synthesizer_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.app_staging_synthesizer_alpha._jsii": [
-            "app-staging-synthesizer-alpha@2.88.0-alpha.0.jsii.tgz"
+            "app-staging-synthesizer-alpha@2.89.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.app_staging_synthesizer_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.88.0",
+        "aws-cdk-lib==2.89.0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk/app_staging_synthesizer_alpha/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -468,39 +468,42 @@
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional["BootstrapRole"] = None,
         image_asset_publishing_role: typing.Optional["BootstrapRole"] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     ) -> "AppStagingSynthesizer":
         '''(experimental) Use the Default Staging Resources, creating a single stack per environment this app is deployed in.
 
         :param bootstrap_qualifier: (experimental) Qualifier to disambiguate multiple bootstrapped environments in the same account. This qualifier is only used to reference bootstrapped resources. It will not be used in the creation of app-specific staging resources: ``appId`` is used for that instead. Default: - Value of context key '@aws-cdk/core:bootstrapQualifier' if set, otherwise ``DEFAULT_QUALIFIER``
         :param deployment_identities: (experimental) What roles to use to deploy applications. These are the roles that have permissions to interact with CloudFormation on your behalf. By default these are the standard bootstrapped CDK roles, but you can customize them or turn them off and use the CLI credentials to deploy. Default: - The standard bootstrapped CDK roles
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
 
         :stability: experimental
         '''
         options = DefaultResourcesOptions(
             bootstrap_qualifier=bootstrap_qualifier,
             deployment_identities=deployment_identities,
             app_id=app_id,
             auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
+            staging_stack_name_prefix=staging_stack_name_prefix,
         )
 
         return typing.cast("AppStagingSynthesizer", jsii.sinvoke(cls, "defaultResources", [options]))
 
     @jsii.member(jsii_name="addDockerImageAsset")
     def add_docker_image_asset(
         self,
@@ -1213,37 +1216,40 @@
         "app_id": "appId",
         "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
+        "staging_stack_name_prefix": "stagingStackNamePrefix",
     },
 )
 class DefaultStagingStackOptions:
     def __init__(
         self,
         *,
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) User configurable options to the DefaultStagingStack.
 
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             default_staging_stack = DefaultStagingStack.factory(app_id="my-app-id")
@@ -1253,14 +1259,15 @@
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
             check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
+            check_type(argname="argument staging_stack_name_prefix", value=staging_stack_name_prefix, expected_type=type_hints["staging_stack_name_prefix"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "app_id": app_id,
         }
         if auto_delete_staging_assets is not None:
             self._values["auto_delete_staging_assets"] = auto_delete_staging_assets
         if deploy_time_file_asset_lifetime is not None:
             self._values["deploy_time_file_asset_lifetime"] = deploy_time_file_asset_lifetime
@@ -1268,14 +1275,16 @@
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
             self._values["image_asset_version_count"] = image_asset_version_count
         if staging_bucket_name is not None:
             self._values["staging_bucket_name"] = staging_bucket_name
+        if staging_stack_name_prefix is not None:
+            self._values["staging_stack_name_prefix"] = staging_stack_name_prefix
 
     @builtins.property
     def app_id(self) -> builtins.str:
         '''(experimental) A unique identifier for the application that the staging stack belongs to.
 
         This identifier will be used in the name of staging resources
         created for this application, and should be unique across CDK apps.
@@ -1368,14 +1377,29 @@
         :default: - a well-known name unique to this app/env.
 
         :stability: experimental
         '''
         result = self._values.get("staging_bucket_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def staging_stack_name_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Specify a custom prefix to be used as the staging stack name and construct ID.
+
+        The prefix will be appended before the appId, which
+        is required to be part of the stack name and construct ID to
+        ensure uniqueness.
+
+        :default: 'StagingStack'
+
+        :stability: experimental
+        '''
+        result = self._values.get("staging_stack_name_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1391,14 +1415,15 @@
         "app_id": "appId",
         "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
+        "staging_stack_name_prefix": "stagingStackNamePrefix",
         "analytics_reporting": "analyticsReporting",
         "cross_region_references": "crossRegionReferences",
         "description": "description",
         "env": "env",
         "permissions_boundary": "permissionsBoundary",
         "stack_name": "stackName",
         "suppress_template_indentation": "suppressTemplateIndentation",
@@ -1419,14 +1444,15 @@
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         suppress_template_indentation: typing.Optional[builtins.bool] = None,
@@ -1441,14 +1467,15 @@
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
@@ -1489,14 +1516,15 @@
                 ),
                 file_asset_publishing_role=bootstrap_role,
                 image_asset_publishing_role=bootstrap_role,
                 image_asset_version_count=123,
                 permissions_boundary=permissions_boundary,
                 stack_name="stackName",
                 staging_bucket_name="stagingBucketName",
+                staging_stack_name_prefix="stagingStackNamePrefix",
                 suppress_template_indentation=False,
                 synthesizer=stack_synthesizer,
                 tags={
                     "tags_key": "tags"
                 },
                 termination_protection=False
             )
@@ -1508,14 +1536,15 @@
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
             check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
+            check_type(argname="argument staging_stack_name_prefix", value=staging_stack_name_prefix, expected_type=type_hints["staging_stack_name_prefix"])
             check_type(argname="argument analytics_reporting", value=analytics_reporting, expected_type=type_hints["analytics_reporting"])
             check_type(argname="argument cross_region_references", value=cross_region_references, expected_type=type_hints["cross_region_references"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
             check_type(argname="argument stack_name", value=stack_name, expected_type=type_hints["stack_name"])
             check_type(argname="argument suppress_template_indentation", value=suppress_template_indentation, expected_type=type_hints["suppress_template_indentation"])
@@ -1536,14 +1565,16 @@
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
             self._values["image_asset_version_count"] = image_asset_version_count
         if staging_bucket_name is not None:
             self._values["staging_bucket_name"] = staging_bucket_name
+        if staging_stack_name_prefix is not None:
+            self._values["staging_stack_name_prefix"] = staging_stack_name_prefix
         if analytics_reporting is not None:
             self._values["analytics_reporting"] = analytics_reporting
         if cross_region_references is not None:
             self._values["cross_region_references"] = cross_region_references
         if description is not None:
             self._values["description"] = description
         if env is not None:
@@ -1659,14 +1690,29 @@
 
         :stability: experimental
         '''
         result = self._values.get("staging_bucket_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def staging_stack_name_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Specify a custom prefix to be used as the staging stack name and construct ID.
+
+        The prefix will be appended before the appId, which
+        is required to be part of the stack name and construct ID to
+        ensure uniqueness.
+
+        :default: 'StagingStack'
+
+        :stability: experimental
+        '''
+        result = self._values.get("staging_stack_name_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def analytics_reporting(self) -> typing.Optional[builtins.bool]:
         '''Include runtime versioning information in this Stack.
 
         :default:
 
         ``analyticsReporting`` setting of containing ``App``, or value of
         'aws:cdk:version-reporting' context key
@@ -2682,14 +2728,15 @@
         "app_id": "appId",
         "auto_delete_staging_assets": "autoDeleteStagingAssets",
         "deploy_time_file_asset_lifetime": "deployTimeFileAssetLifetime",
         "file_asset_publishing_role": "fileAssetPublishingRole",
         "image_asset_publishing_role": "imageAssetPublishingRole",
         "image_asset_version_count": "imageAssetVersionCount",
         "staging_bucket_name": "stagingBucketName",
+        "staging_stack_name_prefix": "stagingStackNamePrefix",
     },
 )
 class DefaultResourcesOptions(AppStagingSynthesizerOptions, DefaultStagingStackOptions):
     def __init__(
         self,
         *,
         bootstrap_qualifier: typing.Optional[builtins.str] = None,
@@ -2697,26 +2744,28 @@
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Properties for stackPerEnv static method.
 
         :param bootstrap_qualifier: (experimental) Qualifier to disambiguate multiple bootstrapped environments in the same account. This qualifier is only used to reference bootstrapped resources. It will not be used in the creation of app-specific staging resources: ``appId`` is used for that instead. Default: - Value of context key '@aws-cdk/core:bootstrapQualifier' if set, otherwise ``DEFAULT_QUALIFIER``
         :param deployment_identities: (experimental) What roles to use to deploy applications. These are the roles that have permissions to interact with CloudFormation on your behalf. By default these are the standard bootstrapped CDK roles, but you can customize them or turn them off and use the CLI credentials to deploy. Default: - The standard bootstrapped CDK roles
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
 
         :stability: experimental
         :exampleMetadata: infused
 
         Example::
 
             app = App(
@@ -2734,14 +2783,15 @@
             check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
             check_type(argname="argument auto_delete_staging_assets", value=auto_delete_staging_assets, expected_type=type_hints["auto_delete_staging_assets"])
             check_type(argname="argument deploy_time_file_asset_lifetime", value=deploy_time_file_asset_lifetime, expected_type=type_hints["deploy_time_file_asset_lifetime"])
             check_type(argname="argument file_asset_publishing_role", value=file_asset_publishing_role, expected_type=type_hints["file_asset_publishing_role"])
             check_type(argname="argument image_asset_publishing_role", value=image_asset_publishing_role, expected_type=type_hints["image_asset_publishing_role"])
             check_type(argname="argument image_asset_version_count", value=image_asset_version_count, expected_type=type_hints["image_asset_version_count"])
             check_type(argname="argument staging_bucket_name", value=staging_bucket_name, expected_type=type_hints["staging_bucket_name"])
+            check_type(argname="argument staging_stack_name_prefix", value=staging_stack_name_prefix, expected_type=type_hints["staging_stack_name_prefix"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "app_id": app_id,
         }
         if bootstrap_qualifier is not None:
             self._values["bootstrap_qualifier"] = bootstrap_qualifier
         if deployment_identities is not None:
             self._values["deployment_identities"] = deployment_identities
@@ -2753,14 +2803,16 @@
             self._values["file_asset_publishing_role"] = file_asset_publishing_role
         if image_asset_publishing_role is not None:
             self._values["image_asset_publishing_role"] = image_asset_publishing_role
         if image_asset_version_count is not None:
             self._values["image_asset_version_count"] = image_asset_version_count
         if staging_bucket_name is not None:
             self._values["staging_bucket_name"] = staging_bucket_name
+        if staging_stack_name_prefix is not None:
+            self._values["staging_stack_name_prefix"] = staging_stack_name_prefix
 
     @builtins.property
     def bootstrap_qualifier(self) -> typing.Optional[builtins.str]:
         '''(experimental) Qualifier to disambiguate multiple bootstrapped environments in the same account.
 
         This qualifier is only used to reference bootstrapped resources. It will not
         be used in the creation of app-specific staging resources: ``appId`` is used for that
@@ -2884,14 +2936,29 @@
         :default: - a well-known name unique to this app/env.
 
         :stability: experimental
         '''
         result = self._values.get("staging_bucket_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def staging_stack_name_prefix(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Specify a custom prefix to be used as the staging stack name and construct ID.
+
+        The prefix will be appended before the appId, which
+        is required to be part of the stack name and construct ID to
+        ensure uniqueness.
+
+        :default: 'StagingStack'
+
+        :stability: experimental
+        '''
+        result = self._values.get("staging_stack_name_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -2925,14 +2992,15 @@
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         suppress_template_indentation: typing.Optional[builtins.bool] = None,
@@ -2948,14 +3016,15 @@
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
         :param env: The AWS environment (account/region) where this stack will be deployed. Set the ``region``/``account`` fields of ``env`` to either a concrete value to select the indicated environment (recommended for production stacks), or to the values of environment variables ``CDK_DEFAULT_REGION``/``CDK_DEFAULT_ACCOUNT`` to let the target environment depend on the AWS credentials/configuration that the CDK CLI is executed under (recommended for development stacks). If the ``Stack`` is instantiated inside a ``Stage``, any undefined ``region``/``account`` fields from ``env`` will default to the same field on the encompassing ``Stage``, if configured there. If either ``region`` or ``account`` are not set nor inherited from ``Stage``, the Stack will be considered "*environment-agnostic*"". Environment-agnostic stacks can be deployed to any environment but may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups such as ``ec2.Vpc.fromLookup`` and will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environment of the containing ``Stage`` if available, otherwise create the stack will be environment-agnostic.
         :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
         :param stack_name: Name to deploy the stack with. Default: - Derived from construct path.
         :param suppress_template_indentation: Enable this flag to suppress indentation in generated CloudFormation templates. If not specified, the value of the ``@aws-cdk/core:suppressTemplateIndentation`` context key will be used. If that is not specified, then the default value ``false`` will be used. Default: - the value of ``@aws-cdk/core:suppressTemplateIndentation``, or ``false`` if that is not set.
@@ -2975,14 +3044,15 @@
             app_id=app_id,
             auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
+            staging_stack_name_prefix=staging_stack_name_prefix,
             analytics_reporting=analytics_reporting,
             cross_region_references=cross_region_references,
             description=description,
             env=env,
             permissions_boundary=permissions_boundary,
             stack_name=stack_name,
             suppress_template_indentation=suppress_template_indentation,
@@ -3001,35 +3071,38 @@
         app_id: builtins.str,
         auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
         deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
         image_asset_version_count: typing.Optional[jsii.Number] = None,
         staging_bucket_name: typing.Optional[builtins.str] = None,
+        staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     ) -> IStagingResourcesFactory:
         '''(experimental) Return a factory that will create DefaultStagingStacks.
 
         :param app_id: (experimental) A unique identifier for the application that the staging stack belongs to. This identifier will be used in the name of staging resources created for this application, and should be unique across CDK apps. The identifier should include lowercase characters and dashes ('-') only and have a maximum of 20 characters.
         :param auto_delete_staging_assets: (experimental) Auto deletes objects in the staging S3 bucket and images in the staging ECR repositories. Default: true
         :param deploy_time_file_asset_lifetime: (experimental) The lifetime for deploy time file assets. Assets that are only necessary at deployment time (for instance, CloudFormation templates and Lambda source code bundles) will be automatically deleted after this many days. Assets that may be read from the staging bucket during your application's run time will not be deleted. Set this to the length of time you wish to be able to roll back to previous versions of your application without having to do a new ``cdk synth`` and re-upload of assets. Default: - Duration.days(30)
         :param file_asset_publishing_role: (experimental) Pass in an existing role to be used as the file publishing role. Default: - a new role will be created
         :param image_asset_publishing_role: (experimental) Pass in an existing role to be used as the image publishing role. Default: - a new role will be created
         :param image_asset_version_count: (experimental) The maximum number of image versions to store in a repository. Previous versions of an image can be stored for rollback purposes. Once a repository has more than 3 image versions stored, the oldest version will be discarded. This allows for sensible garbage collection while maintaining a few previous versions for rollback scenarios. Default: - up to 3 versions stored
         :param staging_bucket_name: (experimental) Explicit name for the staging bucket. Default: - a well-known name unique to this app/env.
+        :param staging_stack_name_prefix: (experimental) Specify a custom prefix to be used as the staging stack name and construct ID. The prefix will be appended before the appId, which is required to be part of the stack name and construct ID to ensure uniqueness. Default: 'StagingStack'
 
         :stability: experimental
         '''
         options = DefaultStagingStackOptions(
             app_id=app_id,
             auto_delete_staging_assets=auto_delete_staging_assets,
             deploy_time_file_asset_lifetime=deploy_time_file_asset_lifetime,
             file_asset_publishing_role=file_asset_publishing_role,
             image_asset_publishing_role=image_asset_publishing_role,
             image_asset_version_count=image_asset_version_count,
             staging_bucket_name=staging_bucket_name,
+            staging_stack_name_prefix=staging_stack_name_prefix,
         )
 
         return typing.cast(IStagingResourcesFactory, jsii.sinvoke(cls, "factory", [options]))
 
     @jsii.member(jsii_name="addDockerImage")
     def add_docker_image(
         self,
@@ -3240,27 +3313,29 @@
     app_id: builtins.str,
     auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
+    staging_stack_name_prefix: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ac9f132bcac8375ac08c16bf3c9bb7407b641e71cfd23cea8b50befa3cf79bbf(
     *,
     app_id: builtins.str,
     auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
+    staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
     suppress_template_indentation: typing.Optional[builtins.bool] = None,
@@ -3333,14 +3408,15 @@
     app_id: builtins.str,
     auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
+    staging_stack_name_prefix: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ca741a4572a1f95a8d82e9d029388b8a2d72acacb69715277b6a785b4968e662(
     scope: _aws_cdk_ceddda9d.App,
     id: builtins.str,
@@ -3350,14 +3426,15 @@
     app_id: builtins.str,
     auto_delete_staging_assets: typing.Optional[builtins.bool] = None,
     deploy_time_file_asset_lifetime: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     file_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_publishing_role: typing.Optional[BootstrapRole] = None,
     image_asset_version_count: typing.Optional[jsii.Number] = None,
     staging_bucket_name: typing.Optional[builtins.str] = None,
+    staging_stack_name_prefix: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
     suppress_template_indentation: typing.Optional[builtins.bool] = None,
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.app-staging-synthesizer-alpha
-Version: 2.88.0a0
+Version: 2.89.0a0
 Summary: Cdk synthesizer for with app-scoped staging stack
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.app-staging-synthesizer-alpha-2.88.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt` & `aws-cdk.app-staging-synthesizer-alpha-2.89.0a0/src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/SOURCES.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/dependency_links.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/requires.txt
 src/aws_cdk.app_staging_synthesizer_alpha.egg-info/top_level.txt
 src/aws_cdk/app_staging_synthesizer_alpha/__init__.py
 src/aws_cdk/app_staging_synthesizer_alpha/py.typed
 src/aws_cdk/app_staging_synthesizer_alpha/_jsii/__init__.py
-src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.88.0-alpha.0.jsii.tgz
+src/aws_cdk/app_staging_synthesizer_alpha/_jsii/app-staging-synthesizer-alpha@2.89.0-alpha.0.jsii.tgz
```

