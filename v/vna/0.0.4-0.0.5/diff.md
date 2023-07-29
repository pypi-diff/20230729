# Comparing `tmp/vna-0.0.4.tar.gz` & `tmp/vna-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vna-0.0.4.tar", last modified: Sat Jul 29 15:03:12 2023, max compression
+gzip compressed data, was "vna-0.0.5.tar", last modified: Sat Jul 29 17:31:59 2023, max compression
```

## Comparing `vna-0.0.4.tar` & `vna-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 15:03:12.153809 vna-0.0.4/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      699 2023-07-29 15:03:12.153809 vna-0.0.4/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-07-20 13:52:50.000000 vna-0.0.4/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-07-29 15:03:12.153809 vna-0.0.4/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      822 2023-07-29 15:03:09.000000 vna-0.0.4/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 15:03:12.153809 vna-0.0.4/vna/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-07-20 13:40:23.000000 vna-0.0.4/vna/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    69909 2023-07-29 15:02:49.000000 vna-0.0.4/vna/vna.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 15:03:12.153809 vna-0.0.4/vna.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      699 2023-07-29 15:03:12.000000 vna-0.0.4/vna.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      153 2023-07-29 15:03:12.000000 vna-0.0.4/vna.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-07-29 15:03:12.000000 vna-0.0.4/vna.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        4 2023-07-29 15:03:12.000000 vna-0.0.4/vna.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 17:31:59.829466 vna-0.0.5/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      699 2023-07-29 17:31:59.829466 vna-0.0.5/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-07-20 13:52:50.000000 vna-0.0.5/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-07-29 17:31:59.829466 vna-0.0.5/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      822 2023-07-29 17:31:45.000000 vna-0.0.5/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 17:31:59.829466 vna-0.0.5/vna/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        0 2023-07-20 13:40:23.000000 vna-0.0.5/vna/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    69905 2023-07-29 17:31:54.000000 vna-0.0.5/vna/vna.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-07-29 17:31:59.829466 vna-0.0.5/vna.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      699 2023-07-29 17:31:59.000000 vna-0.0.5/vna.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      153 2023-07-29 17:31:59.000000 vna-0.0.5/vna.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-07-29 17:31:59.000000 vna-0.0.5/vna.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        4 2023-07-29 17:31:59.000000 vna-0.0.5/vna.egg-info/top_level.txt
```

### Comparing `vna-0.0.4/PKG-INFO` & `vna-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vna
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instrument control library for the PicoVNA 106 and PicoVNA 108. Please note that additional libraries are required, not installed by this package. See the Python Programming Manual for details.
 Home-page: http://picotech.com
 Author: AAI Robotics Ltd
 Author-email: help@aairobotics.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vna-0.0.4/setup.py` & `vna-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import distutils.sysconfig
 
 setup(
     name='vna',
-    version='0.0.4',
+    version='0.0.5',
     description='Instrument control library for the PicoVNA 106 and PicoVNA 108. Please note that additional libraries are required, not installed by this package. See the Python Programming Manual for details.',
     url='http://picotech.com',
     author='AAI Robotics Ltd',
     author_email='help@aairobotics.com',
     license='MIT',
     packages=["vna"],
     include_package_data=True,
```

### Comparing `vna-0.0.4/vna/vna.py` & `vna-0.0.5/vna/vna.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from sys import version_info as _swig_python_version_info
 # Import the low-level C/C++ module
 #if __package__ or "." in __name__:
 #    from . import _vna_python
 #else:
 #    import _vna_python
-    import _vna_python
+import _vna_python
 
 try:
     import builtins as __builtin__
 except ImportError:
     import __builtin__
 
 def _swig_repr(self):
```

### Comparing `vna-0.0.4/vna.egg-info/PKG-INFO` & `vna-0.0.5/vna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vna
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instrument control library for the PicoVNA 106 and PicoVNA 108. Please note that additional libraries are required, not installed by this package. See the Python Programming Manual for details.
 Home-page: http://picotech.com
 Author: AAI Robotics Ltd
 Author-email: help@aairobotics.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

