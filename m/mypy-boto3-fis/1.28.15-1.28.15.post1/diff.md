# Comparing `tmp/mypy-boto3-fis-1.28.15.tar.gz` & `tmp/mypy-boto3-fis-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fis-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
+gzip compressed data, was "mypy-boto3-fis-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:09 2023, max compression
```

## Comparing `mypy-boto3-fis-1.28.15.tar` & `mypy-boto3-fis-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.689122 mypy-boto3-fis-1.28.15/mypy_boto3_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.277154 mypy-boto3-fis-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-07-29 10:03:09.265154 mypy-boto3-fis-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.265154 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-29 09:45:29.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:09.265154 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:03:09.000000 mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:09.277154 mypy-boto3-fis-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:45:28.000000 mypy-boto3-fis-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-fis-1.28.15/LICENSE` & `mypy-boto3-fis-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/PKG-INFO` & `mypy-boto3-fis-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.28.15
-Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fis-1.28.15/README.md` & `mypy-boto3-fis-1.28.15.post1/README.md`

 * *Files 1% similar despite different names*

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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.py` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.pyi` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.py` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.pyi` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.py` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.pyi` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/PKG-INFO` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.28.15
-Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/SOURCES.txt` & `mypy-boto3-fis-1.28.15.post1/mypy_boto3_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.15/setup.py` & `mypy-boto3-fis-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fis",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

