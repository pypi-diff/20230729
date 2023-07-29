# Comparing `tmp/mypy-boto3-appflow-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-appflow-1.28.15.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appflow-1.28.15.post1.tar", last modified: Fri Jul 28 23:40:22 2023, max compression
+gzip compressed data, was "mypy-boto3-appflow-1.28.15.post2.tar", last modified: Sat Jul 29 10:02:30 2023, max compression
```

## Comparing `mypy-boto3-appflow-1.28.15.post1.tar` & `mypy-boto3-appflow-1.28.15.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20715 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19222 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      373 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      372 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      919 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20024 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    19992 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18437 2023-07-28 23:35:35.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    18435 2023-07-28 23:35:35.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:35:34.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    86173 2023-07-28 23:39:46.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    86041 2023-07-28 23:35:37.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       67 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/version.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    20715 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      615 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       19 2023-07-28 23:40:21.000000 mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-28 23:40:21.987957 mypy-boto3-appflow-1.28.15.post1/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-07-28 23:39:43.000000 mypy-boto3-appflow-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.937007 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-07-29 09:38:09.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18435 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86173 2023-07-29 09:38:12.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86041 2023-07-29 09:38:11.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:02:30.000000 mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:30.945007 mypy-boto3-appflow-1.28.15.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:38:08.000000 mypy-boto3-appflow-1.28.15.post2/setup.py
```

### Comparing `mypy-boto3-appflow-1.28.15.post1/LICENSE` & `mypy-boto3-appflow-1.28.15.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/PKG-INFO` & `mypy-boto3-appflow-1.28.15.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.15.post2
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15.post1/README.md` & `mypy-boto3-appflow-1.28.15.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/__main__.py` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.15.0\nDocs:           "
+        "Type annotations for boto3.Appflow 1.28.15\nVersion:         1.28.15.post2\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.py` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/client.pyi` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.py` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/literals.pyi` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.py` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow/type_defs.pyi` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/PKG-INFO` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appflow
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.15.0
+Version: 1.28.15.post2
+Summary: Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appflow docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-appflow-1.28.15.post1/mypy_boto3_appflow.egg-info/SOURCES.txt` & `mypy-boto3-appflow-1.28.15.post2/mypy_boto3_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appflow-1.28.15.post1/setup.py` & `mypy-boto3-appflow-1.28.15.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appflow",
-    version="1.28.15.post1",
+    version="1.28.15.post2",
     packages=["mypy_boto3_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Appflow 1.28.15 service generated with mypy-boto3-builder"
-        " 7.15.0"
+        " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

