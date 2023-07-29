# Comparing `tmp/mypy-boto3-acm-1.28.15.tar.gz` & `tmp/mypy-boto3-acm-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:24 2023, max compression
```

## Comparing `mypy-boto3-acm-1.28.15.tar` & `mypy-boto3-acm-1.28.15.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-acm-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-28 20:18:40.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.632608 mypy-boto3-acm-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:23.980978 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-29 09:37:30.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:23.000000 mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:24.000978 mypy-boto3-acm-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:37:29.000000 mypy-boto3-acm-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-acm-1.28.15/LICENSE` & `mypy-boto3-acm-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/PKG-INFO` & `mypy-boto3-acm-1.28.15.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.15
-Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.28.15/README.md` & `mypy-boto3-acm-1.28.15.post1/README.md`

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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__main__.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACM 1.28.15\nVersion:         1.28.15\nBuilder version:"
-        " 7.16.1\nDocs:           "
+        "Type annotations for boto3.ACM 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.py` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.pyi` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.15
-Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy-boto3-acm-1.28.15.post1/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.15/setup.py` & `mypy-boto3-acm-1.28.15.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

