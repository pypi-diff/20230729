# Comparing `tmp/quickstart-vdk-0.2.948436673.dev12518.tar.gz` & `tmp/quickstart-vdk-0.2.949261637.dev12538.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.948436673.dev12518.tar", last modified: Fri Jul 28 09:18:28 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.949261637.dev12538.tar", last modified: Sat Jul 29 04:26:12 2023, max compression
```

## Comparing `quickstart-vdk-0.2.948436673.dev12518.tar` & `quickstart-vdk-0.2.949261637.dev12538.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:18:28.840718 quickstart-vdk-0.2.948436673.dev12518/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-28 09:18:28.840718 quickstart-vdk-0.2.948436673.dev12518/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-28 09:18:07.000000 quickstart-vdk-0.2.948436673.dev12518/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:18:28.840718 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-28 09:18:28.000000 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-28 09:18:28.000000 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:18:28.000000 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-28 09:18:28.000000 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-28 09:18:28.000000 quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:18:28.844718 quickstart-vdk-0.2.948436673.dev12518/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-28 09:18:17.000000 quickstart-vdk-0.2.948436673.dev12518/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:18:28.840718 quickstart-vdk-0.2.948436673.dev12518/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-28 09:18:07.000000 quickstart-vdk-0.2.948436673.dev12518/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:26:12.515416 quickstart-vdk-0.2.949261637.dev12538/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-29 04:26:12.515416 quickstart-vdk-0.2.949261637.dev12538/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-29 04:23:24.000000 quickstart-vdk-0.2.949261637.dev12538/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:26:12.515416 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-29 04:26:12.000000 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-29 04:26:12.000000 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 04:26:12.000000 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-29 04:26:12.000000 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-29 04:26:12.000000 quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 04:26:12.515416 quickstart-vdk-0.2.949261637.dev12538/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-29 04:26:00.000000 quickstart-vdk-0.2.949261637.dev12538/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 04:26:12.515416 quickstart-vdk-0.2.949261637.dev12538/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-29 04:23:24.000000 quickstart-vdk-0.2.949261637.dev12538/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.948436673.dev12518/PKG-INFO` & `quickstart-vdk-0.2.949261637.dev12538/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.948436673.dev12518
+Version: 0.2.949261637.dev12538
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.948436673.dev12518/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.949261637.dev12538/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.948436673.dev12518
+Version: 0.2.949261637.dev12538
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.948436673.dev12518/setup.py` & `quickstart-vdk-0.2.949261637.dev12538/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.948436673.dev12518"
+__version__ = "0.2.949261637.dev12538"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

