# Comparing `tmp/live_example_python_test-0.0.1.tar.gz` & `tmp/live_example_python_test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "live_example_python_test-0.0.1.tar", last modified: Fri Jul 28 23:43:11 2023, max compression
+gzip compressed data, was "live_example_python_test-0.0.2.tar", last modified: Fri Jul 28 23:54:36 2023, max compression
```

## Comparing `live_example_python_test-0.0.1.tar` & `live_example_python_test-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:43:11.882496 live_example_python_test-0.0.1/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      580 2023-07-28 23:43:11.881500 live_example_python_test-0.0.1/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       10 2023-07-28 23:17:23.000000 live_example_python_test-0.0.1/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:43:11.857773 live_example_python_test-0.0.1/live_example_python_test/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       37 2023-07-28 23:30:34.000000 live_example_python_test-0.0.1/live_example_python_test/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      134 2023-07-28 23:34:44.000000 live_example_python_test-0.0.1/live_example_python_test/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      313 2023-07-28 23:31:51.000000 live_example_python_test-0.0.1/live_example_python_test/decorators.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:43:11.880503 live_example_python_test-0.0.1/live_example_python_test.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      580 2023-07-28 23:43:11.000000 live_example_python_test-0.0.1/live_example_python_test.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      323 2023-07-28 23:43:11.000000 live_example_python_test-0.0.1/live_example_python_test.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-07-28 23:43:11.000000 live_example_python_test-0.0.1/live_example_python_test.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       25 2023-07-28 23:43:11.000000 live_example_python_test-0.0.1/live_example_python_test.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-07-28 23:43:11.883495 live_example_python_test-0.0.1/setup.cfg
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1077 2023-07-28 23:42:17.000000 live_example_python_test-0.0.1/setup.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:54:36.869960 live_example_python_test-0.0.2/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      635 2023-07-28 23:54:36.868962 live_example_python_test-0.0.2/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       49 2023-07-28 23:51:59.000000 live_example_python_test-0.0.2/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:54:36.852992 live_example_python_test-0.0.2/live_example_python_test/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       37 2023-07-28 23:30:34.000000 live_example_python_test-0.0.2/live_example_python_test/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      134 2023-07-28 23:34:44.000000 live_example_python_test-0.0.2/live_example_python_test/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      343 2023-07-28 23:51:44.000000 live_example_python_test-0.0.2/live_example_python_test/decorators.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-07-28 23:54:36.867965 live_example_python_test-0.0.2/live_example_python_test.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      635 2023-07-28 23:54:36.000000 live_example_python_test-0.0.2/live_example_python_test.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      323 2023-07-28 23:54:36.000000 live_example_python_test-0.0.2/live_example_python_test.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-07-28 23:54:36.000000 live_example_python_test-0.0.2/live_example_python_test.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       25 2023-07-28 23:54:36.000000 live_example_python_test-0.0.2/live_example_python_test.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-07-28 23:54:36.870957 live_example_python_test-0.0.2/setup.cfg
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1077 2023-07-28 23:52:48.000000 live_example_python_test-0.0.2/setup.py
```

### Comparing `live_example_python_test-0.0.1/PKG-INFO` & `live_example_python_test-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: live_example_python_test
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple packages test
 Home-page: https://github.com/eduardogpg/live-example-python-packages
 Author: Eduardo Ismael García Pérez
 Author-email: eduardo78d@gmail.com
 License: MIT
 Description: ### README
+        
+        New feature to users args and params.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `live_example_python_test-0.0.1/live_example_python_test.egg-info/PKG-INFO` & `live_example_python_test-0.0.2/live_example_python_test.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: live-example-python-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple packages test
 Home-page: https://github.com/eduardogpg/live-example-python-packages
 Author: Eduardo Ismael García Pérez
 Author-email: eduardo78d@gmail.com
 License: MIT
 Description: ### README
+        
+        New feature to users args and params.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `live_example_python_test-0.0.1/setup.py` & `live_example_python_test-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path # > 3.6
 from setuptools import setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Simple packages test'
 PACKAGE_NAME = 'live_example_python_test'
 AUTHOR = 'Eduardo Ismael García Pérez'
 EMAIL = 'eduardo78d@gmail.com'
 GITHUB_URL = 'https://github.com/eduardogpg/live-example-python-packages'
 
 setup(
```

