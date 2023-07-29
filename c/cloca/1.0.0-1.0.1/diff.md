# Comparing `tmp/cloca-1.0.0.tar.gz` & `tmp/cloca-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloca-1.0.0.tar", last modified: Sat Jul 29 00:27:08 2023, max compression
+gzip compressed data, was "cloca-1.0.1.tar", last modified: Sat Jul 29 00:30:19 2023, max compression
```

## Comparing `cloca-1.0.0.tar` & `cloca-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:27:08.355287 cloca-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 00:26:56.000000 cloca-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-29 00:27:08.355287 cloca-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-29 00:26:56.000000 cloca-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:27:08.355287 cloca-1.0.0/cloca/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 00:26:56.000000 cloca-1.0.0/cloca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-29 00:26:56.000000 cloca-1.0.0/cloca/cloca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:27:08.355287 cloca-1.0.0/cloca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-29 00:27:08.000000 cloca-1.0.0/cloca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 00:27:08.000000 cloca-1.0.0/cloca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:27:08.000000 cloca-1.0.0/cloca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:27:08.000000 cloca-1.0.0/cloca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:27:08.355287 cloca-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 00:26:56.000000 cloca-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 00:30:08.000000 cloca-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-29 00:30:19.823624 cloca-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-29 00:30:08.000000 cloca-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/cloca/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 00:30:08.000000 cloca-1.0.1/cloca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-29 00:30:08.000000 cloca-1.0.1/cloca/cloca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/cloca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:30:19.823624 cloca-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 00:30:08.000000 cloca-1.0.1/setup.py
```

### Comparing `cloca-1.0.0/LICENSE` & `cloca-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloca-1.0.0/PKG-INFO` & `cloca-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.0.0
+Version: 1.0.1
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,11 +109,7 @@
 If you encounter any problems or have questions, please feel free to open an issue [here](https://github.com/ahmad-siavashi/cloca/issues).
 
 ### Acknowledgments
 
 This project was inspired by the need for a simple global clock for Python projects.
 
 
----
-
-Thank you for using cloca! We hope this library simplifies time management in your Python projects. If you have any feedback or suggestions, please let us know. Happy coding!
-
```

### Comparing `cloca-1.0.0/README.md` & `cloca-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,12 +89,7 @@
 ### Issues
 
 If you encounter any problems or have questions, please feel free to open an issue [here](https://github.com/ahmad-siavashi/cloca/issues).
 
 ### Acknowledgments
 
 This project was inspired by the need for a simple global clock for Python projects.
-
-
----
-
-Thank you for using cloca! We hope this library simplifies time management in your Python projects. If you have any feedback or suggestions, please let us know. Happy coding!
```

### Comparing `cloca-1.0.0/cloca/cloca.py` & `cloca-1.0.1/cloca/cloca.py`

 * *Files identical despite different names*

### Comparing `cloca-1.0.0/cloca.egg-info/PKG-INFO` & `cloca-1.0.1/cloca.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.0.0
+Version: 1.0.1
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -109,11 +109,7 @@
 If you encounter any problems or have questions, please feel free to open an issue [here](https://github.com/ahmad-siavashi/cloca/issues).
 
 ### Acknowledgments
 
 This project was inspired by the need for a simple global clock for Python projects.
 
 
----
-
-Thank you for using cloca! We hope this library simplifies time management in your Python projects. If you have any feedback or suggestions, please let us know. Happy coding!
-
```

### Comparing `cloca-1.0.0/setup.py` & `cloca-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cloca',
-    version='1.0.0',
+    version='1.0.1',
     description='Global Clock Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

