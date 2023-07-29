# Comparing `tmp/cloca-1.0.1.tar.gz` & `tmp/cloca-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloca-1.0.1.tar", last modified: Sat Jul 29 00:30:19 2023, max compression
+gzip compressed data, was "cloca-1.1.0.tar", last modified: Sat Jul 29 15:32:06 2023, max compression
```

## Comparing `cloca-1.0.1.tar` & `cloca-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 00:30:08.000000 cloca-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-29 00:30:19.823624 cloca-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-29 00:30:08.000000 cloca-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/cloca/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 00:30:08.000000 cloca-1.0.1/cloca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-29 00:30:08.000000 cloca-1.0.1/cloca/cloca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:30:19.823624 cloca-1.0.1/cloca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 00:30:19.000000 cloca-1.0.1/cloca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:30:19.823624 cloca-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 00:30:08.000000 cloca-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-29 15:31:55.000000 cloca-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:32:06.071926 cloca-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-29 15:31:55.000000 cloca-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/cloca/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-29 15:31:55.000000 cloca-1.1.0/cloca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-29 15:31:55.000000 cloca-1.1.0/cloca/cloca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:32:06.071926 cloca-1.1.0/cloca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-29 15:32:06.000000 cloca-1.1.0/cloca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 15:32:06.071926 cloca-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-29 15:31:55.000000 cloca-1.1.0/setup.py
```

### Comparing `cloca-1.0.1/LICENSE` & `cloca-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloca-1.0.1/PKG-INFO` & `cloca-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.0.1
+Version: 1.1.0
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,15 @@
 
 cloca is a simple Python library that provides a global clock with functionalities to increment time, read the current time, and reset the clock. It is designed to be used across multiple modules, ensuring they all share the same state.
 
 ### Features
 
 - Global clock with manual time incrementation.
 - Read the current time from anywhere in your Python project.
+- Obtain future time after a specified delay.
 - Reset the clock to zero as needed.
 
 ### Installation
 
 You can install cloca using pip:
 
 ```
```

### Comparing `cloca-1.0.1/README.md` & `cloca-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 cloca is a simple Python library that provides a global clock with functionalities to increment time, read the current time, and reset the clock. It is designed to be used across multiple modules, ensuring they all share the same state.
 
 ### Features
 
 - Global clock with manual time incrementation.
 - Read the current time from anywhere in your Python project.
+- Obtain future time after a specified delay.
 - Reset the clock to zero as needed.
 
 ### Installation
 
 You can install cloca using pip:
 
 ```
```

### Comparing `cloca-1.0.1/cloca/cloca.py` & `cloca-1.1.0/cloca/cloca.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 class Cloca:
     """
     A global clock class that allows time incrementation, retrieval, and reset.
 
     Attributes
     ----------
-    current_time : int
+    _current_time : int
         The current time value.
 
     Methods
     -------
     increase(increment)
         Increase the current time by the specified increment.
 
     now()
         Get the current time value.
 
+    delayed(delay)
+        Get the current time value plus the specified delay.
+
     reset()
         Reset the current time to 0.
 
     """
     _instance = None
 
     def __new__(cls):
@@ -29,41 +32,57 @@
         -------
         Cloca
             A singleton instance of Clocca.
 
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
-            cls._instance.current_time = 0
+            cls._instance._current_time = 0
         return cls._instance
 
+    def delayed(self, delay):
+        """
+        Get the current time value plus the specified delay.
+
+        Parameters
+        ----------
+        delay : int
+            The delay to be added to the current time.
+
+        Returns
+        -------
+        int
+            The current time value plus the specified delay.
+
+        """
+        return self.now() + delay
+
     def increase(self, increment=1):
         """
         Increase the current time by the specified increment.
 
         Parameters
         ----------
         increment : int, optional
             The value by which to increase the current time. Default is 1.
 
         """
-        self.current_time += increment
+        self._current_time += increment
 
     def now(self):
         """
         Get the current time value.
 
         Returns
         -------
         int
             The current time value.
 
         """
-        return self.current_time
+        return self._current_time
 
     def reset(self):
         """
         Reset the current time to 0.
 
         """
-        self.current_time = 0
-
+        self._current_time = 0
```

### Comparing `cloca-1.0.1/cloca.egg-info/PKG-INFO` & `cloca-1.1.0/cloca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloca
-Version: 1.0.1
+Version: 1.1.0
 Summary: Global Clock Python Library
 Home-page: UNKNOWN
 Author: Ahmad Siavashi
 Author-email: siavashi@aut.ac.ir
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,15 @@
 
 cloca is a simple Python library that provides a global clock with functionalities to increment time, read the current time, and reset the clock. It is designed to be used across multiple modules, ensuring they all share the same state.
 
 ### Features
 
 - Global clock with manual time incrementation.
 - Read the current time from anywhere in your Python project.
+- Obtain future time after a specified delay.
 - Reset the clock to zero as needed.
 
 ### Installation
 
 You can install cloca using pip:
 
 ```
```

### Comparing `cloca-1.0.1/setup.py` & `cloca-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cloca',
-    version='1.0.1',
+    version='1.1.0',
     description='Global Clock Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

