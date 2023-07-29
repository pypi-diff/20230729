# Comparing `tmp/mypy-boto3-dynamodb-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.15.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.28.15.post1.tar", last modified: Sat Jul 29 09:19:05 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.15.post2.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.28.15.post1.tar` & `mypy-boto3-dynamodb-1.28.15.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:19:05.903730 mypy-boto3-dynamodb-1.28.15.post1/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    25984 2023-07-29 09:19:05.903730 mypy-boto3-dynamodb-1.28.15.post1/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    24487 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:19:05.903730 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1858 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__init__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1856 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__init__.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      923 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__main__.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    53762 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/client.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    53695 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/client.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    12941 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/literals.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    12939 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/literals.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     8290 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/paginator.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     8283 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/paginator.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/py.typed
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    26844 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/service_resource.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    26817 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/service_resource.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)   122126 2023-07-29 09:16:19.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/type_defs.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)   121987 2023-07-29 09:16:18.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/type_defs.pyi
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       67 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/version.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2258 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/waiter.py
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2256 2023-07-29 09:16:16.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/waiter.pyi
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-29 09:19:05.903730 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)    25984 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      841 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       52 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       20 2023-07-29 09:19:05.000000 mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-29 09:19:05.903730 mypy-boto3-dynamodb-1.28.15.post1/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2009 2023-07-29 09:16:15.000000 mypy-boto3-dynamodb-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24487 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.361115 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53762 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53695 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26844 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-07-29 09:42:58.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   122126 2023-07-29 09:43:03.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121987 2023-07-29 09:43:02.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-29 09:42:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:02:59.000000 mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:59.365115 mypy-boto3-dynamodb-1.28.15.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:42:57.000000 mypy-boto3-dynamodb-1.28.15.post2/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/LICENSE` & `mypy-boto3-dynamodb-1.28.15.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/PKG-INFO` & `mypy-boto3-dynamodb-1.28.15.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.15.post1
+Version: 1.28.15.post2
 Summary: Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/README.md` & `mypy-boto3-dynamodb-1.28.15.post2/README.md`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        "Type annotations for boto3.DynamoDB 1.28.15\nVersion:         1.28.15.post2\nBuilder"
         " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.15.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.28.15.post1
+Version: 1.28.15.post2
 Summary: Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
```

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.15.post2/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.28.15.post1/setup.py` & `mypy-boto3-dynamodb-1.28.15.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.28.15.post1",
+    version="1.28.15.post2",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.DynamoDB 1.28.15 service generated with mypy-boto3-builder"
```

