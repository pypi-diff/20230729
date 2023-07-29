# Comparing `tmp/mypy-boto3-servicecatalog-appregistry-1.28.15.tar.gz` & `tmp/mypy-boto3-servicecatalog-appregistry-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:11 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15.tar` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.273872 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-07-28 20:39:18.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21647 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-28 20:39:16.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.853402 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-07-29 10:04:11.853402 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.829402 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21647 2023-07-29 09:59:27.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:11.829402 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:11.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:11.853402 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-29 09:59:26.000000 mypy-boto3-servicecatalog-appregistry-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/LICENSE` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.15
-Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/README.md` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/README.md`

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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.15
-Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.15/setup.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog-appregistry",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

