# Comparing `tmp/mypy-boto3-cloudsearch-1.28.15.tar.gz` & `tmp/mypy-boto3-cloudsearch-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearch-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearch-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:43 2023, max compression
```

## Comparing `mypy-boto3-cloudsearch-1.28.15.tar` & `mypy-boto3-cloudsearch-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.564783 mypy-boto3-cloudsearch-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15318 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-28 20:21:02.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25454 2023-07-28 20:21:02.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.556783 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15318 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:25.000000 mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.564783 mypy-boto3-cloudsearch-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:21:01.000000 mypy-boto3-cloudsearch-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:43.709059 mypy-boto3-cloudsearch-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-29 10:02:43.709059 mypy-boto3-cloudsearch-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:43.705059 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25479 2023-07-29 09:40:13.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25454 2023-07-29 09:40:12.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:43.709059 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 10:02:43.000000 mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:43.709059 mypy-boto3-cloudsearch-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-29 09:40:11.000000 mypy-boto3-cloudsearch-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-cloudsearch-1.28.15/LICENSE` & `mypy-boto3-cloudsearch-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/PKG-INFO` & `mypy-boto3-cloudsearch-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearch-1.28.15/README.md` & `mypy-boto3-cloudsearch-1.28.15.post1/README.md`

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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/__main__.py` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearch 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.CloudSearch 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#CloudSearch\nOther"
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

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.py` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/client.pyi` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.py` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/literals.pyi` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.py` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch/type_defs.pyi` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/PKG-INFO` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearch
-Version: 1.28.15
-Summary: Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/
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
 [mypy-boto3-cloudsearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-cloudsearch-1.28.15/mypy_boto3_cloudsearch.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearch-1.28.15.post1/mypy_boto3_cloudsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearch-1.28.15/setup.py` & `mypy-boto3-cloudsearch-1.28.15.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearch",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_cloudsearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CloudSearch 1.28.15 service generated with mypy-boto3-builder"
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

