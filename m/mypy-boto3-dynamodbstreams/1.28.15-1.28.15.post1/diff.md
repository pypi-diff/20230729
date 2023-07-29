# Comparing `tmp/mypy-boto3-dynamodbstreams-1.28.15.tar.gz` & `tmp/mypy-boto3-dynamodbstreams-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodbstreams-1.28.15.tar", last modified: Fri Jul 28 20:42:41 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodbstreams-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
```

## Comparing `mypy-boto3-dynamodbstreams-1.28.15.tar` & `mypy-boto3-dynamodbstreams-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.053003 mypy-boto3-dynamodbstreams-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:41.053003 mypy-boto3-dynamodbstreams-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.373115 mypy-boto3-dynamodbstreams-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-29 10:02:59.353115 mypy-boto3-dynamodbstreams-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.349115 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.349115 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 10:02:59.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:59.373115 mypy-boto3-dynamodbstreams-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-29 09:43:04.000000 mypy-boto3-dynamodbstreams-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/LICENSE` & `mypy-boto3-dynamodbstreams-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.28.15
-Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/README.md` & `mypy-boto3-dynamodbstreams-1.28.15.post1/README.md`

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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__main__.py` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDBStreams 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.DynamoDBStreams 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.py` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.pyi` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.py` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.pyi` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.py` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.pyi` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.28.15
-Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt` & `mypy-boto3-dynamodbstreams-1.28.15.post1/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.15/setup.py` & `mypy-boto3-dynamodbstreams-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodbstreams",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with"
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

