# Comparing `tmp/aws-cdk.aws-neptune-alpha-2.89.0a0.tar.gz` & `tmp/aws-cdk.aws-neptune-alpha-2.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/aws-neptune-alpha/dist/python/aws-cdk.aws-neptune-alpha-2.89.0a0.tar", last modified: Fri Jul 28 22:05:35 2023, max compression
+gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-neptune/dist/python/aws-cdk.aws-neptune-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:06 2022, max compression
```

## Comparing `aws-cdk.aws-neptune-alpha-2.89.0a0.tar` & `aws-cdk.aws-neptune-alpha-2.9.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8781 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7780 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1870 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/
--rw-r--r--   0 root         (0) root         (0)   189030 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71724 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.89.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:24.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk/aws_neptune_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8781 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:05:35.000000 aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5750 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4782 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1795 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/
+-rw-r--r--   0 root         (0) root         (0)   111643 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      405 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55214 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk/aws_neptune_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5750 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      530 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.aws-neptune-alpha-2.89.0a0/LICENSE` & `aws-cdk.aws-neptune-alpha-2.9.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.aws-neptune-alpha-2.89.0a0/setup.py` & `aws-cdk.aws-neptune-alpha-2.9.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-neptune-alpha",
-    "version": "2.89.0.a0",
+    "version": "2.9.0.a0",
     "description": "The CDK Construct Library for AWS::Neptune",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,43 +22,41 @@
     },
     "packages": [
         "aws_cdk.aws_neptune_alpha",
         "aws_cdk.aws_neptune_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_neptune_alpha._jsii": [
-            "aws-neptune-alpha@2.89.0-alpha.0.jsii.tgz"
+            "aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_neptune_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.7",
+    "python_requires": ">=3.6",
     "install_requires": [
-        "aws-cdk-lib==2.89.0",
+        "aws-cdk-lib>=2.9.0, <3.0.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.85.0, <2.0.0",
-        "publication>=0.0.3",
-        "typeguard~=2.13.3"
+        "jsii>=1.52.1, <2.0.0",
+        "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 2"
+        "Framework :: AWS CDK :: 1"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

### Comparing `aws-cdk.aws-neptune-alpha-2.89.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-neptune-alpha-2.9.0a0/src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_neptune_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/requires.txt
 src/aws_cdk.aws_neptune_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_neptune_alpha/__init__.py
 src/aws_cdk/aws_neptune_alpha/py.typed
 src/aws_cdk/aws_neptune_alpha/_jsii/__init__.py
-src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.89.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_neptune_alpha/_jsii/aws-neptune-alpha@2.9.0-alpha.0.jsii.tgz
```

