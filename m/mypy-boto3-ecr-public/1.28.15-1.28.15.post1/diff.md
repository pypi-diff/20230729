# Comparing `tmp/mypy-boto3-ecr-public-1.28.15.tar.gz` & `tmp/mypy-boto3-ecr-public-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-public-1.28.15.tar", last modified: Fri Jul 28 20:42:43 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-public-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:02 2023, max compression
```

## Comparing `mypy-boto3-ecr-public-1.28.15.tar` & `mypy-boto3-ecr-public-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-07-28 20:24:47.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:43.000000 mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.549038 mypy-boto3-ecr-public-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-28 20:24:46.000000 mypy-boto3-ecr-public-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.349127 mypy-boto3-ecr-public-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-29 10:03:02.345127 mypy-boto3-ecr-public-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14299 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.341127 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23708 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-07-29 09:44:16.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:02.345127 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15803 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 10:03:02.000000 mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:02.349127 mypy-boto3-ecr-public-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-29 09:44:15.000000 mypy-boto3-ecr-public-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-ecr-public-1.28.15/LICENSE` & `mypy-boto3-ecr-public-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/PKG-INFO` & `mypy-boto3-ecr-public-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.15
-Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-public-1.28.15/README.md` & `mypy-boto3-ecr-public-1.28.15.post1/README.md`

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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__init__.pyi` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/__main__.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECRPublic 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ECRPublic 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/client.pyi` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/literals.pyi` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/paginator.pyi` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.py` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public/type_defs.pyi` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/PKG-INFO` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr-public
-Version: 1.28.15
-Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/
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
 [mypy-boto3-ecr-public docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr_public/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ecr-public-1.28.15/mypy_boto3_ecr_public.egg-info/SOURCES.txt` & `mypy-boto3-ecr-public-1.28.15.post1/mypy_boto3_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-public-1.28.15/setup.py` & `mypy-boto3-ecr-public-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr-public",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ECRPublic 1.28.15 service generated with mypy-boto3-builder"
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

