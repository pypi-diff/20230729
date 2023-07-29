# Comparing `tmp/mypy-boto3-mq-1.28.15.tar.gz` & `tmp/mypy-boto3-mq-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mq-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
+gzip compressed data, was "mypy-boto3-mq-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:44 2023, max compression
```

## Comparing `mypy-boto3-mq-1.28.15.tar` & `mypy-boto3-mq-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.097554 mypy-boto3-mq-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-28 20:43:21.093554 mypy-boto3-mq-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.089554 mypy-boto3-mq-1.28.15/mypy_boto3_mq/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-07-28 20:32:12.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.093554 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.101554 mypy-boto3-mq-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.469301 mypy-boto3-mq-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-29 10:03:44.465301 mypy-boto3-mq-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.461301 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-07-29 09:51:50.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-07-29 09:51:50.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:44.465301 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-29 10:03:44.000000 mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:44.469301 mypy-boto3-mq-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-29 09:51:49.000000 mypy-boto3-mq-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-mq-1.28.15/LICENSE` & `mypy-boto3-mq-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/PKG-INFO` & `mypy-boto3-mq-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.15
-Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mq-1.28.15/README.md` & `mypy-boto3-mq-1.28.15.post1/README.md`

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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.py` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.pyi` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.py` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.pyi` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.py` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.pyi` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.py` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.pyi` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.py` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.pyi` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/PKG-INFO` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.15
-Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/SOURCES.txt` & `mypy-boto3-mq-1.28.15.post1/mypy_boto3_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.15/setup.py` & `mypy-boto3-mq-1.28.15.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mq",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

