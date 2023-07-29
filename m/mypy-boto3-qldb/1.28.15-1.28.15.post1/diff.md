# Comparing `tmp/mypy-boto3-qldb-1.28.15.tar.gz` & `tmp/mypy-boto3-qldb-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:55 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.28.15.tar` & `mypy-boto3-qldb-1.28.15.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.709686 mypy-boto3-qldb-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-28 20:43:30.701686 mypy-boto3-qldb-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.697685 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-28 20:33:48.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-28 20:33:48.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.701686 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.709686 mypy-boto3-qldb-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.761347 mypy-boto3-qldb-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-29 10:03:55.753347 mypy-boto3-qldb-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.737347 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-29 09:53:41.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:55.753347 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 10:03:55.000000 mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:55.761347 mypy-boto3-qldb-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-29 09:53:40.000000 mypy-boto3-qldb-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-qldb-1.28.15/LICENSE` & `mypy-boto3-qldb-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/PKG-INFO` & `mypy-boto3-qldb-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.15
-Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qldb-1.28.15/README.md` & `mypy-boto3-qldb-1.28.15.post1/README.md`

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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.QLDB 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.15
-Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.28.15.post1/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.15/setup.py` & `mypy-boto3-qldb-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

