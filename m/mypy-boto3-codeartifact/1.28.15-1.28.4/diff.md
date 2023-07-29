# Comparing `tmp/mypy-boto3-codeartifact-1.28.15.tar.gz` & `tmp/mypy-boto3-codeartifact-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeartifact-1.28.15.tar", last modified: Fri Jul 28 20:42:28 2023, max compression
+gzip compressed data, was "mypy-boto3-codeartifact-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-codeartifact-1.28.15.tar` & `mypy-boto3-codeartifact-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.532824 mypy-boto3-codeartifact-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-28 20:42:28.532824 mypy-boto3-codeartifact-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.532824 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-28 20:21:13.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-07-28 20:21:13.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-28 20:21:13.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-28 20:21:13.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-07-28 20:21:13.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46848 2023-07-28 20:21:15.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46769 2023-07-28 20:21:14.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:28.532824 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:28.000000 mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:28.532824 mypy-boto3-codeartifact-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:21:12.000000 mypy-boto3-codeartifact-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34383 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34332 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46438 2023-07-18 01:00:27.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46363 2023-07-18 01:00:26.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 01:01:41.000000 mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-codeartifact-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-18 01:00:25.000000 mypy-boto3-codeartifact-1.28.4/setup.py
```

### Comparing `mypy-boto3-codeartifact-1.28.15/LICENSE` & `mypy-boto3-codeartifact-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeArtifact 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,14 +394,16 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -413,15 +415,14 @@
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -437,14 +438,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.15/README.md` & `mypy-boto3-codeartifact-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,14 +362,16 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -381,15 +383,14 @@
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -405,14 +406,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__init__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__init__.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/__main__.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeArtifact 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.CodeArtifact 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/client.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/client.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/literals.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -272,28 +271,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/literals.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -270,28 +269,26 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/paginator.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/paginator.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/type_defs.py` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -96,15 +98,14 @@
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
@@ -120,14 +121,15 @@
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -141,34 +143,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -233,24 +224,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -266,15 +255,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -306,15 +294,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -584,28 +571,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -754,15 +739,14 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -841,15 +825,14 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
 )
 
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -941,15 +924,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -961,14 +943,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
+    {
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+    },
+)
+
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
@@ -1056,23 +1054,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1232,22 +1228,14 @@
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1375,15 +1363,14 @@
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
@@ -1548,20 +1535,27 @@
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1596,15 +1590,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1616,60 +1609,44 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact/type_defs.pyi` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     "PackageDependencyTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "ListRepositoriesInDomainRequestRequestTypeDef",
     "RepositorySummaryTypeDef",
     "ListRepositoriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "PackageOriginRestrictionsOutputTypeDef",
     "PackageOriginRestrictionsTypeDef",
     "PublishPackageVersionRequestRequestTypeDef",
     "PutDomainPermissionsPolicyRequestRequestTypeDef",
     "PutRepositoryPermissionsPolicyRequestRequestTypeDef",
     "RepositoryExternalConnectionInfoTypeDef",
     "UpstreamRepositoryInfoTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -95,15 +97,14 @@
     "ListPackageVersionAssetsResultTypeDef",
     "PublishPackageVersionResultTypeDef",
     "CopyPackageVersionsResultTypeDef",
     "DeletePackageVersionsResultTypeDef",
     "DisposePackageVersionsResultTypeDef",
     "UpdatePackageVersionsStatusResultTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainResultTypeDef",
     "DeleteDomainResultTypeDef",
     "DescribeDomainResultTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "UpdateRepositoryRequestRequestTypeDef",
     "DeleteDomainPermissionsPolicyResultTypeDef",
@@ -119,14 +120,15 @@
     "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef",
     "ListRepositoriesRequestListRepositoriesPaginateTypeDef",
     "ListPackageVersionDependenciesResultTypeDef",
     "ListRepositoriesInDomainResultTypeDef",
     "ListRepositoriesResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "PackageOriginConfigurationTypeDef",
     "PutPackageOriginConfigurationRequestRequestTypeDef",
     "RepositoryDescriptionTypeDef",
     "PackageVersionDescriptionTypeDef",
     "PackageVersionSummaryTypeDef",
     "PackageDescriptionTypeDef",
     "PackageSummaryTypeDef",
@@ -140,32 +142,23 @@
     "DescribePackageVersionResultTypeDef",
     "ListPackageVersionsResultTypeDef",
     "DescribePackageResultTypeDef",
     "DeletePackageResultTypeDef",
     "ListPackagesResultTypeDef",
 )
 
-_RequiredAssetSummaryTypeDef = TypedDict(
-    "_RequiredAssetSummaryTypeDef",
+AssetSummaryTypeDef = TypedDict(
+    "AssetSummaryTypeDef",
     {
         "name": str,
-    },
-)
-_OptionalAssetSummaryTypeDef = TypedDict(
-    "_OptionalAssetSummaryTypeDef",
-    {
         "size": int,
         "hashes": Dict[HashAlgorithmType, str],
     },
-    total=False,
 )
 
-class AssetSummaryTypeDef(_RequiredAssetSummaryTypeDef, _OptionalAssetSummaryTypeDef):
-    pass
-
 _RequiredAssociateExternalConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateExternalConnectionRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
         "externalConnection": str,
     },
@@ -226,24 +219,22 @@
 
 PackageVersionErrorTypeDef = TypedDict(
     "PackageVersionErrorTypeDef",
     {
         "errorCode": PackageVersionErrorCodeType,
         "errorMessage": str,
     },
-    total=False,
 )
 
 SuccessfulPackageVersionInfoTypeDef = TypedDict(
     "SuccessfulPackageVersionInfoTypeDef",
     {
         "revision": str,
         "status": PackageVersionStatusType,
     },
-    total=False,
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
@@ -259,15 +250,14 @@
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
         "repositoryCount": int,
         "assetSizeBytes": int,
         "s3BucketArn": str,
     },
-    total=False,
 )
 
 UpstreamRepositoryTypeDef = TypedDict(
     "UpstreamRepositoryTypeDef",
     {
         "repositoryName": str,
     },
@@ -297,15 +287,14 @@
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "resourceArn": str,
         "revision": str,
         "document": str,
     },
-    total=False,
 )
 
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -553,28 +542,26 @@
 
 DomainEntryPointTypeDef = TypedDict(
     "DomainEntryPointTypeDef",
     {
         "repositoryName": str,
         "externalConnectionName": str,
     },
-    total=False,
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "name": str,
         "owner": str,
         "arn": str,
         "status": DomainStatusType,
         "createdTime": datetime,
         "encryptionKey": str,
     },
-    total=False,
 )
 
 _RequiredGetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizationTokenRequestRequestTypeDef",
     {
         "domain": str,
     },
@@ -711,15 +698,14 @@
 
 LicenseInfoTypeDef = TypedDict(
     "LicenseInfoTypeDef",
     {
         "name": str,
         "url": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -794,15 +780,14 @@
     "PackageDependencyTypeDef",
     {
         "namespace": str,
         "package": str,
         "dependencyType": str,
         "versionRequirement": str,
     },
-    total=False,
 )
 
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -888,15 +873,14 @@
         "administratorAccount": str,
         "domainName": str,
         "domainOwner": str,
         "arn": str,
         "description": str,
         "createdTime": datetime,
     },
-    total=False,
 )
 
 ListRepositoriesRequestRequestTypeDef = TypedDict(
     "ListRepositoriesRequestRequestTypeDef",
     {
         "repositoryPrefix": str,
         "maxResults": int,
@@ -908,14 +892,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+PackageOriginRestrictionsOutputTypeDef = TypedDict(
+    "PackageOriginRestrictionsOutputTypeDef",
+    {
+        "publish": AllowPublishType,
+        "upstream": AllowUpstreamType,
+    },
+)
+
 PackageOriginRestrictionsTypeDef = TypedDict(
     "PackageOriginRestrictionsTypeDef",
     {
         "publish": AllowPublishType,
         "upstream": AllowUpstreamType,
     },
 )
@@ -997,23 +997,21 @@
 RepositoryExternalConnectionInfoTypeDef = TypedDict(
     "RepositoryExternalConnectionInfoTypeDef",
     {
         "externalConnectionName": str,
         "packageFormat": PackageFormatType,
         "status": Literal["Available"],
     },
-    total=False,
 )
 
 UpstreamRepositoryInfoTypeDef = TypedDict(
     "UpstreamRepositoryInfoTypeDef",
     {
         "repositoryName": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
@@ -1169,22 +1167,14 @@
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1308,15 +1298,14 @@
 
 PackageVersionOriginTypeDef = TypedDict(
     "PackageVersionOriginTypeDef",
     {
         "domainEntryPoint": DomainEntryPointTypeDef,
         "originType": PackageVersionOriginTypeType,
     },
-    total=False,
 )
 
 ListDomainsResultTypeDef = TypedDict(
     "ListDomainsResultTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
@@ -1473,20 +1462,27 @@
     {
         "repositories": List[RepositorySummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PackageOriginConfigurationTypeDef = TypedDict(
     "PackageOriginConfigurationTypeDef",
     {
-        "restrictions": PackageOriginRestrictionsTypeDef,
+        "restrictions": PackageOriginRestrictionsOutputTypeDef,
     },
-    total=False,
 )
 
 _RequiredPutPackageOriginConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutPackageOriginConfigurationRequestRequestTypeDef",
     {
         "domain": str,
         "repository": str,
@@ -1519,15 +1515,14 @@
         "domainOwner": str,
         "arn": str,
         "description": str,
         "upstreams": List[UpstreamRepositoryInfoTypeDef],
         "externalConnections": List[RepositoryExternalConnectionInfoTypeDef],
         "createdTime": datetime,
     },
-    total=False,
 )
 
 PackageVersionDescriptionTypeDef = TypedDict(
     "PackageVersionDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
@@ -1539,58 +1534,44 @@
         "sourceCodeRepository": str,
         "publishedTime": datetime,
         "licenses": List[LicenseInfoTypeDef],
         "revision": str,
         "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-_RequiredPackageVersionSummaryTypeDef = TypedDict(
-    "_RequiredPackageVersionSummaryTypeDef",
+PackageVersionSummaryTypeDef = TypedDict(
+    "PackageVersionSummaryTypeDef",
     {
         "version": str,
-        "status": PackageVersionStatusType,
-    },
-)
-_OptionalPackageVersionSummaryTypeDef = TypedDict(
-    "_OptionalPackageVersionSummaryTypeDef",
-    {
         "revision": str,
+        "status": PackageVersionStatusType,
         "origin": PackageVersionOriginTypeDef,
     },
-    total=False,
 )
 
-class PackageVersionSummaryTypeDef(
-    _RequiredPackageVersionSummaryTypeDef, _OptionalPackageVersionSummaryTypeDef
-):
-    pass
-
 PackageDescriptionTypeDef = TypedDict(
     "PackageDescriptionTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "name": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PackageSummaryTypeDef = TypedDict(
     "PackageSummaryTypeDef",
     {
         "format": PackageFormatType,
         "namespace": str,
         "package": str,
         "originConfiguration": PackageOriginConfigurationTypeDef,
     },
-    total=False,
 )
 
 PutPackageOriginConfigurationResultTypeDef = TypedDict(
     "PutPackageOriginConfigurationResultTypeDef",
     {
         "originConfiguration": PackageOriginConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/PKG-INFO` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeartifact
-Version: 1.28.15
-Summary: Type annotations for boto3.CodeArtifact 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.4
+Summary: Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeartifact"></a>
 
 # mypy-boto3-codeartifact
 
 [![PyPI - mypy-boto3-codeartifact](https://img.shields.io/pypi/v/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeartifact.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeartifact)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeartifact)](https://pepy.tech/project/mypy-boto3-codeartifact)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeartifact?color=blue)](https://pypistats.org/packages/mypy-boto3-codeartifact)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeArtifact 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
+[boto3.CodeArtifact 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeartifact docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeartifact/).
 
 See how it helps to find and fix potential bugs:
 
@@ -394,14 +394,16 @@
     PackageDependencyTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     ListPackagesRequestRequestTypeDef,
     ListRepositoriesInDomainRequestRequestTypeDef,
     RepositorySummaryTypeDef,
     ListRepositoriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    PackageOriginRestrictionsOutputTypeDef,
     PackageOriginRestrictionsTypeDef,
     PublishPackageVersionRequestRequestTypeDef,
     PutDomainPermissionsPolicyRequestRequestTypeDef,
     PutRepositoryPermissionsPolicyRequestRequestTypeDef,
     RepositoryExternalConnectionInfoTypeDef,
     UpstreamRepositoryInfoTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -413,15 +415,14 @@
     ListPackageVersionAssetsResultTypeDef,
     PublishPackageVersionResultTypeDef,
     CopyPackageVersionsResultTypeDef,
     DeletePackageVersionsResultTypeDef,
     DisposePackageVersionsResultTypeDef,
     UpdatePackageVersionsStatusResultTypeDef,
     CreateDomainRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainResultTypeDef,
     DeleteDomainResultTypeDef,
     DescribeDomainResultTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     UpdateRepositoryRequestRequestTypeDef,
     DeleteDomainPermissionsPolicyResultTypeDef,
@@ -437,14 +438,15 @@
     ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackagesRequestListPackagesPaginateTypeDef,
     ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef,
     ListRepositoriesRequestListRepositoriesPaginateTypeDef,
     ListPackageVersionDependenciesResultTypeDef,
     ListRepositoriesInDomainResultTypeDef,
     ListRepositoriesResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     PackageOriginConfigurationTypeDef,
     PutPackageOriginConfigurationRequestRequestTypeDef,
     RepositoryDescriptionTypeDef,
     PackageVersionDescriptionTypeDef,
     PackageVersionSummaryTypeDef,
     PackageDescriptionTypeDef,
     PackageSummaryTypeDef,
```

### Comparing `mypy-boto3-codeartifact-1.28.15/mypy_boto3_codeartifact.egg-info/SOURCES.txt` & `mypy-boto3-codeartifact-1.28.4/mypy_boto3_codeartifact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeartifact-1.28.15/setup.py` & `mypy-boto3-codeartifact-1.28.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeartifact",
-    version="1.28.15",
+    version="1.28.4",
     packages=["mypy_boto3_codeartifact"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeArtifact 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        "Type annotations for boto3.CodeArtifact 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

