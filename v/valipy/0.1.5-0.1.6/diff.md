# Comparing `tmp/valipy-0.1.5.tar.gz` & `tmp/valipy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valipy-0.1.5.tar", last modified: Sat Jul 29 06:45:17 2023, max compression
+gzip compressed data, was "valipy-0.1.6.tar", last modified: Sat Jul 29 06:46:25 2023, max compression
```

## Comparing `valipy-0.1.5.tar` & `valipy-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:45:17.950578 valipy-0.1.5/
--rw-r--r--   0 josevonchong   (501) staff       (20)      573 2023-07-29 06:45:17.950654 valipy-0.1.5/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-29 06:45:17.950893 valipy-0.1.5/setup.cfg
--rw-r--r--   0 josevonchong   (501) staff       (20)     1055 2023-07-29 06:45:12.000000 valipy-0.1.5/setup.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:45:17.948547 valipy-0.1.5/test/
--rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.1.5/test/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      168 2023-07-29 06:17:54.000000 valipy-0.1.5/test/misc.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.1.5/test/test.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:45:17.949638 valipy-0.1.5/valipy/
--rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.1.5/valipy/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)     7890 2023-07-29 05:13:30.000000 valipy-0.1.5/valipy/exceptions.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    11447 2023-07-29 05:40:37.000000 valipy-0.1.5/valipy/myFunctions.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:45:17.950426 valipy-0.1.5/valipy.egg-info/
--rw-r--r--   0 josevonchong   (501) staff       (20)      573 2023-07-29 06:45:17.000000 valipy-0.1.5/valipy.egg-info/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-29 06:45:17.000000 valipy-0.1.5/valipy.egg-info/SOURCES.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-29 06:45:17.000000 valipy-0.1.5/valipy.egg-info/dependency_links.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-29 06:45:17.000000 valipy-0.1.5/valipy.egg-info/top_level.txt
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:46:25.366071 valipy-0.1.6/
+-rw-r--r--   0 josevonchong   (501) staff       (20)      573 2023-07-29 06:46:25.366152 valipy-0.1.6/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-29 06:46:25.366493 valipy-0.1.6/setup.cfg
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1079 2023-07-29 06:46:20.000000 valipy-0.1.6/setup.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:46:25.364310 valipy-0.1.6/test/
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.1.6/test/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      168 2023-07-29 06:17:54.000000 valipy-0.1.6/test/misc.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.1.6/test/test.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:46:25.365096 valipy-0.1.6/valipy/
+-rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.1.6/valipy/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)     7890 2023-07-29 05:13:30.000000 valipy-0.1.6/valipy/exceptions.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    11447 2023-07-29 05:40:37.000000 valipy-0.1.6/valipy/myFunctions.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-29 06:46:25.365912 valipy-0.1.6/valipy.egg-info/
+-rw-r--r--   0 josevonchong   (501) staff       (20)      573 2023-07-29 06:46:25.000000 valipy-0.1.6/valipy.egg-info/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-29 06:46:25.000000 valipy-0.1.6/valipy.egg-info/SOURCES.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-29 06:46:25.000000 valipy-0.1.6/valipy.egg-info/dependency_links.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-29 06:46:25.000000 valipy-0.1.6/valipy.egg-info/top_level.txt
```

### Comparing `valipy-0.1.5/PKG-INFO` & `valipy-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: validation,data,schema,schema validation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `valipy-0.1.5/setup.py` & `valipy-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='valipy',
     packages=find_packages(),
-    version='0.1.5',
+    version='0.1.6',
     description='A chainable, fluent Python library for validating data',
     author='Joaquin Jose Von Chong',
     license='MIT',
+    readme='readme.md',
     author_email = 'jjvonchong@outlook.com',      # Type in your E-Mail
     url = 'https://github.com/pimepan/valipy',   # Provide either the link to your github or to your website
     keywords = ['validation', 'data', 'schema', 'schema validation'],   # Keywords that define your package best
     install_requires=[],
     classifiers=[
         'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',      # Define that your audience are developers
```

### Comparing `valipy-0.1.5/valipy/exceptions.py` & `valipy-0.1.6/valipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.1.5/valipy/myFunctions.py` & `valipy-0.1.6/valipy/myFunctions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.1.5/valipy.egg-info/PKG-INFO` & `valipy-0.1.6/valipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: validation,data,schema,schema validation
 Classifier: Development Status :: 4 - Beta
```

