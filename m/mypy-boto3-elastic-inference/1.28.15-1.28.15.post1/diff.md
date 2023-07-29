# Comparing `tmp/mypy-boto3-elastic-inference-1.28.15.tar.gz` & `tmp/mypy-boto3-elastic-inference-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastic-inference-1.28.15.tar", last modified: Fri Jul 28 20:42:44 2023, max compression
+gzip compressed data, was "mypy-boto3-elastic-inference-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-elastic-inference-1.28.15.tar` & `mypy-boto3-elastic-inference-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.757129 mypy-boto3-elastic-inference-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-07-29 10:03:02.757129 mypy-boto3-elastic-inference-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.757129 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:33.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.757129 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-29 10:03:02.000000 mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.757129 mypy-boto3-elastic-inference-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-29 09:44:32.000000 mypy-boto3-elastic-inference-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-elastic-inference-1.28.15/LICENSE` & `mypy-boto3-elastic-inference-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.15/README.md` & `mypy-boto3-elastic-inference-1.28.15.post1/README.md`

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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.pyi` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__main__.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticInference 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.ElasticInference 1.28.15\nVersion:        "
+        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.pyi` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.pyi` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.pyi` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.py` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.pyi` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.15
-Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/SOURCES.txt` & `mypy-boto3-elastic-inference-1.28.15.post1/mypy_boto3_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.15/setup.py` & `mypy-boto3-elastic-inference-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastic-inference",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ElasticInference 1.28.15 service generated with"
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

