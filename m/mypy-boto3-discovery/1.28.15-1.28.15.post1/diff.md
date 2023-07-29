# Comparing `tmp/mypy-boto3-discovery-1.28.15.tar.gz` & `tmp/mypy-boto3-discovery-1.28.15.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-discovery-1.28.15.tar", last modified: Fri Jul 28 20:42:38 2023, max compression
+gzip compressed data, was "mypy-boto3-discovery-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:57 2023, max compression
```

## Comparing `mypy-boto3-discovery-1.28.15.tar` & `mypy-boto3-discovery-1.28.15.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.100962 mypy-boto3-discovery-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-28 20:42:38.096962 mypy-boto3-discovery-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.088962 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-07-28 20:23:01.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.096962 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:38.100962 mypy-boto3-discovery-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.853109 mypy-boto3-discovery-1.28.15.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-07-29 10:02:57.845109 mypy-boto3-discovery-1.28.15.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.837109 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-07-29 09:42:29.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-07-29 09:42:28.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:57.845109 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17092 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-29 10:02:57.000000 mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:57.853109 mypy-boto3-discovery-1.28.15.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-29 09:42:27.000000 mypy-boto3-discovery-1.28.15.post1/setup.py
```

### Comparing `mypy-boto3-discovery-1.28.15/LICENSE` & `mypy-boto3-discovery-1.28.15.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/PKG-INFO` & `mypy-boto3-discovery-1.28.15.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.15
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.28.15/README.md` & `mypy-boto3-discovery-1.28.15.post1/README.md`

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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.py` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.pyi` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.py` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.pyi` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.py` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.pyi` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.py` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.pyi` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.py` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.pyi` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/PKG-INFO` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.15
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.15.post1
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/SOURCES.txt` & `mypy-boto3-discovery-1.28.15.post1/mypy_boto3_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.15/setup.py` & `mypy-boto3-discovery-1.28.15.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-discovery",
-    version="1.28.15",
+    version="1.28.15.post1",
     packages=["mypy_boto3_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

