# Comparing `tmp/mypy-boto3-kinesisanalyticsv2-1.28.15.tar.gz` & `tmp/mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:28 2023, max compression
```

## Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15.tar` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-28 20:29:19.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-28 20:29:21.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69775 2023-07-28 20:29:23.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-07-28 20:29:22.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:43:05.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.753343 mypy-boto3-kinesisanalyticsv2-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 20:29:18.000000 mypy-boto3-kinesisanalyticsv2-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19766 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.729225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27513 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-29 09:48:57.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-29 09:48:57.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69775 2023-07-29 09:48:58.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69672 2023-07-29 09:48:58.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-29 10:03:28.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:28.741225 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-29 09:48:56.000000 mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/LICENSE` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.15
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/README.md` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/README.md`

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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__init__.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/__main__.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.KinesisAnalyticsV2 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/client.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/literals.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/paginator.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2/type_defs.pyi` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesisanalyticsv2
-Version: 1.28.15
-Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/
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
 [mypy-boto3-kinesisanalyticsv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/mypy_boto3_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesisanalyticsv2-1.28.15/setup.py` & `mypy-boto3-kinesisanalyticsv2-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesisanalyticsv2",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.KinesisAnalyticsV2 1.28.15 service generated with"
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

