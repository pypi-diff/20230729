# Comparing `tmp/feltpy-0.0.2.tar.gz` & `tmp/feltpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feltpy-0.0.2.tar", last modified: Sat Jul 29 14:16:17 2023, max compression
+gzip compressed data, was "feltpy-0.0.3.tar", last modified: Sat Jul 29 14:26:41 2023, max compression
```

## Comparing `feltpy-0.0.2.tar` & `feltpy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.324557 feltpy-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-07-28 22:54:39.000000 feltpy-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     3524 2023-07-29 14:16:17.322558 feltpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2986 2023-07-29 14:15:34.000000 feltpy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.298367 feltpy-0.0.2/feltpy/
--rw-rw-rw-   0        0        0        0 2023-07-28 22:44:47.000000 feltpy-0.0.2/feltpy/__init__.py
--rw-rw-rw-   0        0        0    22810 2023-07-28 22:41:18.000000 feltpy-0.0.2/feltpy/feltpy.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.321664 feltpy-0.0.2/feltpy.egg-info/
--rw-rw-rw-   0        0        0     3524 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      668 2023-07-29 14:14:45.000000 feltpy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 14:16:17.324557 feltpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 14:26:41.588192 feltpy-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-07-28 22:54:39.000000 feltpy-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     3598 2023-07-29 14:26:41.586173 feltpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3060 2023-07-29 14:25:45.000000 feltpy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 14:26:41.541852 feltpy-0.0.3/feltpy/
+-rw-rw-rw-   0        0        0      156 2023-07-29 14:24:47.000000 feltpy-0.0.3/feltpy/__init__.py
+-rw-rw-rw-   0        0        0    22810 2023-07-28 22:41:18.000000 feltpy-0.0.3/feltpy/feltpy.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:26:41.583653 feltpy-0.0.3/feltpy.egg-info/
+-rw-rw-rw-   0        0        0     3598 2023-07-29 14:26:41.000000 feltpy-0.0.3/feltpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-29 14:26:41.000000 feltpy-0.0.3/feltpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:26:41.000000 feltpy-0.0.3/feltpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 14:26:41.000000 feltpy-0.0.3/feltpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 14:26:41.000000 feltpy-0.0.3/feltpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      668 2023-07-29 14:26:21.000000 feltpy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:26:41.589195 feltpy-0.0.3/setup.cfg
```

### Comparing `feltpy-0.0.2/LICENSE.md` & `feltpy-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feltpy-0.0.2/PKG-INFO` & `feltpy-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for interacting with the API of Felt.com
 Author-email: David Moss <davidmoss1221@gmail.com>
 Project-URL: Homepage, https://github.com/moss-xyz/feltpy
 Project-URL: Bug Tracker, https://github.com/moss-xyz/feltpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,19 @@
 ### Installation
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
+Once installed, import the package with
+```python
+import feltpy
+```
+
 This package only requires a few packages, most of which come with a default installation of Python, namely:
 - re
 - os
 - [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
```

### Comparing `feltpy-0.0.2/README.md` & `feltpy-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 ### Installation
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
+Once installed, import the package with
+```python
+import feltpy
+```
+
 This package only requires a few packages, most of which come with a default installation of Python, namely:
 - re
 - os
 - [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
```

### Comparing `feltpy-0.0.2/feltpy/feltpy.py` & `feltpy-0.0.3/feltpy/feltpy.py`

 * *Files identical despite different names*

### Comparing `feltpy-0.0.2/feltpy.egg-info/PKG-INFO` & `feltpy-0.0.3/feltpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for interacting with the API of Felt.com
 Author-email: David Moss <davidmoss1221@gmail.com>
 Project-URL: Homepage, https://github.com/moss-xyz/feltpy
 Project-URL: Bug Tracker, https://github.com/moss-xyz/feltpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,19 @@
 ### Installation
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
+Once installed, import the package with
+```python
+import feltpy
+```
+
 This package only requires a few packages, most of which come with a default installation of Python, namely:
 - re
 - os
 - [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
```

### Comparing `feltpy-0.0.2/pyproject.toml` & `feltpy-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feltpy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="David Moss", email="davidmoss1221@gmail.com" },
 ]
 description = "A package for interacting with the API of Felt.com"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

