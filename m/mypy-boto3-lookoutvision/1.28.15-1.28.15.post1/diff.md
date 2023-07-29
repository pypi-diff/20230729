# Comparing `tmp/mypy-boto3-lookoutvision-1.28.15.tar.gz` & `tmp/mypy-boto3-lookoutvision-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutvision-1.28.15.tar", last modified: Fri Jul 28 20:43:11 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutvision-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:34 2023, max compression
```

## Comparing `mypy-boto3-lookoutvision-1.28.15.tar` & `mypy-boto3-lookoutvision-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.873427 mypy-boto3-lookoutvision-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-07-28 20:43:11.869427 mypy-boto3-lookoutvision-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.845427 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-28 20:30:37.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:11.869427 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:11.000000 mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:11.873427 mypy-boto3-lookoutvision-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:30:36.000000 mypy-boto3-lookoutvision-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.569256 mypy-boto3-lookoutvision-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-07-29 10:03:34.565256 mypy-boto3-lookoutvision-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.557256 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19116 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27131 2023-07-29 09:50:15.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:34.565256 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16316 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 10:03:34.000000 mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:34.569256 mypy-boto3-lookoutvision-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-29 09:50:14.000000 mypy-boto3-lookoutvision-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/LICENSE` & `mypy-boto3-lookoutvision-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.15
-Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/README.md` & `mypy-boto3-lookoutvision-1.28.15.post1/README.md`

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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__init__.pyi` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/__main__.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutforVision 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.LookoutforVision 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
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

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModelPackagingConfigurationOutputTypeDef,
     ModelPackagingConfigurationTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
@@ -329,15 +330,17 @@
         """
 
     def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: ModelPackagingConfigurationTypeDef,
+        Configuration: Union[
+            ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
+        ],
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/client.pyi` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     DescribeProjectResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ListModelsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModelPackagingConfigurationOutputTypeDef,
     ModelPackagingConfigurationTypeDef,
     OutputConfigTypeDef,
     StartModelPackagingJobResponseTypeDef,
     StartModelResponseTypeDef,
     StopModelResponseTypeDef,
     TagTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
@@ -304,15 +305,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/client/#start_model)
         """
     def start_model_packaging_job(
         self,
         *,
         ProjectName: str,
         ModelVersion: str,
-        Configuration: ModelPackagingConfigurationTypeDef,
+        Configuration: Union[
+            ModelPackagingConfigurationTypeDef, ModelPackagingConfigurationOutputTypeDef
+        ],
         JobName: str = ...,
         Description: str = ...,
         ClientToken: str = ...
     ) -> StartModelPackagingJobResponseTypeDef:
         """
         Starts an Amazon Lookout for Vision model packaging job.
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/literals.pyi` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/paginator.pyi` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.py` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision/type_defs.pyi` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.15
-Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.LookoutforVision 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-lookoutvision-1.28.15/mypy_boto3_lookoutvision.egg-info/SOURCES.txt` & `mypy-boto3-lookoutvision-1.28.15.post1/mypy_boto3_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.15/setup.py` & `mypy-boto3-lookoutvision-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutvision",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.LookoutforVision 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

