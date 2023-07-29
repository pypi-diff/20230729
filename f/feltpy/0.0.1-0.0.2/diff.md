# Comparing `tmp/feltpy-0.0.1.tar.gz` & `tmp/feltpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feltpy-0.0.1.tar", last modified: Sat Jul 29 14:08:01 2023, max compression
+gzip compressed data, was "feltpy-0.0.2.tar", last modified: Sat Jul 29 14:16:17 2023, max compression
```

## Comparing `feltpy-0.0.1.tar` & `feltpy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 14:08:01.246549 feltpy-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-07-28 22:54:39.000000 feltpy-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     3489 2023-07-29 14:08:01.245539 feltpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2951 2023-07-29 13:55:35.000000 feltpy-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 14:08:01.217771 feltpy-0.0.1/feltpy/
--rw-rw-rw-   0        0        0        0 2023-07-28 22:44:47.000000 feltpy-0.0.1/feltpy/__init__.py
--rw-rw-rw-   0        0        0    22810 2023-07-28 22:41:18.000000 feltpy-0.0.1/feltpy/feltpy.py
-drwxrwxrwx   0        0        0        0 2023-07-29 14:08:01.244034 feltpy-0.0.1/feltpy.egg-info/
--rw-rw-rw-   0        0        0     3489 2023-07-29 14:08:01.000000 feltpy-0.0.1/feltpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-29 14:08:01.000000 feltpy-0.0.1/feltpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 14:08:01.000000 feltpy-0.0.1/feltpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-29 14:08:01.000000 feltpy-0.0.1/feltpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 14:08:01.000000 feltpy-0.0.1/feltpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2023-07-29 14:05:49.000000 feltpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 14:08:01.247558 feltpy-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.324557 feltpy-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-28 22:54:39.000000 feltpy-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     3524 2023-07-29 14:16:17.322558 feltpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2986 2023-07-29 14:15:34.000000 feltpy-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.298367 feltpy-0.0.2/feltpy/
+-rw-rw-rw-   0        0        0        0 2023-07-28 22:44:47.000000 feltpy-0.0.2/feltpy/__init__.py
+-rw-rw-rw-   0        0        0    22810 2023-07-28 22:41:18.000000 feltpy-0.0.2/feltpy/feltpy.py
+drwxrwxrwx   0        0        0        0 2023-07-29 14:16:17.321664 feltpy-0.0.2/feltpy.egg-info/
+-rw-rw-rw-   0        0        0     3524 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-29 14:16:17.000000 feltpy-0.0.2/feltpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      668 2023-07-29 14:14:45.000000 feltpy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 14:16:17.324557 feltpy-0.0.2/setup.cfg
```

### Comparing `feltpy-0.0.1/LICENSE.md` & `feltpy-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feltpy-0.0.1/PKG-INFO` & `feltpy-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for interacting with the API of Felt.com
 Author-email: David Moss <davidmoss1221@gmail.com>
 Project-URL: Homepage, https://github.com/moss-xyz/feltpy
 Project-URL: Bug Tracker, https://github.com/moss-xyz/feltpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
 This package only requires a few packages, most of which come with a default installation of Python, namely:
-- requests
 - re
 - os
+- [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
 
 ### Set-Up
 
 All functions in this package are only set up, currently, to work with Felt's __Personal Access Tokens__, which must be acquired ahead of time. More information on doing so can be found on [Felt's API documentation](https://feltmaps.notion.site/Felt-Public-API-reference-c01e0e6b0d954a678c608131b894e8e1#065791134e0c4d82b156d97db3f663a5).
```

### Comparing `feltpy-0.0.1/README.md` & `feltpy-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
 This package only requires a few packages, most of which come with a default installation of Python, namely:
-- requests
 - re
 - os
+- [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
 
 ### Set-Up
 
 All functions in this package are only set up, currently, to work with Felt's __Personal Access Tokens__, which must be acquired ahead of time. More information on doing so can be found on [Felt's API documentation](https://feltmaps.notion.site/Felt-Public-API-reference-c01e0e6b0d954a678c608131b894e8e1#065791134e0c4d82b156d97db3f663a5).
```

### Comparing `feltpy-0.0.1/feltpy/feltpy.py` & `feltpy-0.0.2/feltpy/feltpy.py`

 * *Files identical despite different names*

### Comparing `feltpy-0.0.1/feltpy.egg-info/PKG-INFO` & `feltpy-0.0.2/feltpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feltpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for interacting with the API of Felt.com
 Author-email: David Moss <davidmoss1221@gmail.com>
 Project-URL: Homepage, https://github.com/moss-xyz/feltpy
 Project-URL: Bug Tracker, https://github.com/moss-xyz/feltpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
 
 This package is available in PyPI, and can be installed like so:
 ```bash
 pip install feltpy
 ```
 
 This package only requires a few packages, most of which come with a default installation of Python, namely:
-- requests
 - re
 - os
+- [requests](https://github.com/psf/requests)
 - [geopandas](https://github.com/geopandas/geopandas)
 
 I've only tested this on Python 3.10, but it will presumably work with older version of Python 3!
 
 ### Set-Up
 
 All functions in this package are only set up, currently, to work with Felt's __Personal Access Tokens__, which must be acquired ahead of time. More information on doing so can be found on [Felt's API documentation](https://feltmaps.notion.site/Felt-Public-API-reference-c01e0e6b0d954a678c608131b894e8e1#065791134e0c4d82b156d97db3f663a5).
```

### Comparing `feltpy-0.0.1/pyproject.toml` & `feltpy-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feltpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="David Moss", email="davidmoss1221@gmail.com" },
 ]
 description = "A package for interacting with the API of Felt.com"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests",
-    "re",
-    "os",
     "geopandas"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/moss-xyz/feltpy"
 "Bug Tracker" = "https://github.com/moss-xyz/feltpy/issues"
```

