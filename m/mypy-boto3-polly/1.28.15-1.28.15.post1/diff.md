# Comparing `tmp/mypy-boto3-polly-1.28.15.tar.gz` & `tmp/mypy-boto3-polly-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-polly-1.28.15.tar", last modified: Fri Jul 28 20:43:29 2023, max compression
+gzip compressed data, was "mypy-boto3-polly-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:54 2023, max compression
```

## Comparing `mypy-boto3-polly-1.28.15.tar` & `mypy-boto3-polly-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.325667 mypy-boto3-polly-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-28 20:43:29.325667 mypy-boto3-polly-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.317667 mypy-boto3-polly-1.28.15/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-28 20:33:36.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-28 20:33:36.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-28 20:33:36.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:29.325667 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:29.000000 mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:29.325667 mypy-boto3-polly-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:33:33.000000 mypy-boto3-polly-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.641343 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:54.000000 mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:54.653343 mypy-boto3-polly-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:53:28.000000 mypy-boto3-polly-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-polly-1.28.15/LICENSE` & `mypy-boto3-polly-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/PKG-INFO` & `mypy-boto3-polly-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.15
-Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-polly-1.28.15/README.md` & `mypy-boto3-polly-1.28.15.post1/README.md`

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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/__main__.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Polly 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Polly 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.28.15
-Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
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
 [mypy-boto3-polly docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-polly-1.28.15/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.28.15.post1/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.28.15/setup.py` & `mypy-boto3-polly-1.28.15.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.Polly 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

