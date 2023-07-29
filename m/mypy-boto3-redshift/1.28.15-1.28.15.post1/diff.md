# Comparing `tmp/mypy-boto3-redshift-1.28.15.tar.gz` & `tmp/mypy-boto3-redshift-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:58 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.28.15.tar` & `mypy-boto3-redshift-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35427 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.449723 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115226 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   115059 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134047 2023-07-28 20:36:39.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   133928 2023-07-28 20:36:37.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.529356 mypy-boto3-redshift-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36924 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35427 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115226 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115059 2023-07-29 09:56:38.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-29 09:56:40.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134047 2023-07-29 09:56:47.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133928 2023-07-29 09:56:41.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-29 09:56:39.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:58.521356 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36924 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 10:03:58.000000 mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:58.529356 mypy-boto3-redshift-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-29 09:56:37.000000 mypy-boto3-redshift-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-redshift-1.28.15/LICENSE` & `mypy-boto3-redshift-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/PKG-INFO` & `mypy-boto3-redshift-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.15
-Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.28.15/README.md` & `mypy-boto3-redshift-1.28.15.post1/README.md`

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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.Redshift 1.28.15\nVersion:         1.28.15.post1\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.15
-Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.28.15.post1/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.15/setup.py` & `mypy-boto3-redshift-1.28.15.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder"
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

