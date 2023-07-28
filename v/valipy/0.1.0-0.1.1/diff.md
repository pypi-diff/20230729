# Comparing `tmp/valipy-0.1.0.tar.gz` & `tmp/valipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valipy-0.1.0.tar", last modified: Thu Jul 27 10:03:17 2023, max compression
+gzip compressed data, was "valipy-0.1.1.tar", last modified: Fri Jul 28 22:42:01 2023, max compression
```

## Comparing `valipy-0.1.0.tar` & `valipy-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-27 10:03:17.642275 valipy-0.1.0/
--rw-r--r--   0 josevonchong   (501) staff       (20)      677 2023-07-27 10:03:17.642339 valipy-0.1.0/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-27 10:03:17.642532 valipy-0.1.0/setup.cfg
--rw-r--r--   0 josevonchong   (501) staff       (20)     1252 2023-07-27 10:00:25.000000 valipy-0.1.0/setup.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-27 10:03:17.640761 valipy-0.1.0/test/
--rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.1.0/test/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)      346 2023-07-27 09:30:05.000000 valipy-0.1.0/test/test.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-27 10:03:17.641529 valipy-0.1.0/valipy/
--rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.1.0/valipy/__init__.py
--rw-r--r--   0 josevonchong   (501) staff       (20)     8724 2023-07-27 08:58:53.000000 valipy-0.1.0/valipy/exceptions.py
--rw-r--r--   0 josevonchong   (501) staff       (20)    10869 2023-07-27 09:54:23.000000 valipy-0.1.0/valipy/myFunctions.py
-drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-27 10:03:17.642120 valipy-0.1.0/valipy.egg-info/
--rw-r--r--   0 josevonchong   (501) staff       (20)      677 2023-07-27 10:03:17.000000 valipy-0.1.0/valipy.egg-info/PKG-INFO
--rw-r--r--   0 josevonchong   (501) staff       (20)      230 2023-07-27 10:03:17.000000 valipy-0.1.0/valipy.egg-info/SOURCES.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-27 10:03:17.000000 valipy-0.1.0/valipy.egg-info/dependency_links.txt
--rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-27 10:03:17.000000 valipy-0.1.0/valipy.egg-info/top_level.txt
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-28 22:42:01.740434 valipy-0.1.1/
+-rw-r--r--   0 josevonchong   (501) staff       (20)      626 2023-07-28 22:42:01.740517 valipy-0.1.1/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)       79 2023-07-28 22:42:01.740803 valipy-0.1.1/setup.cfg
+-rw-r--r--   0 josevonchong   (501) staff       (20)     1165 2023-07-28 22:41:56.000000 valipy-0.1.1/setup.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-28 22:42:01.737066 valipy-0.1.1/test/
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-27 09:20:29.000000 valipy-0.1.1/test/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)        0 2023-07-28 22:40:16.000000 valipy-0.1.1/test/misc.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)      348 2023-07-28 22:39:44.000000 valipy-0.1.1/test/test.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-28 22:42:01.738272 valipy-0.1.1/valipy/
+-rw-r--r--   0 josevonchong   (501) staff       (20)       58 2023-07-27 09:21:33.000000 valipy-0.1.1/valipy/__init__.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)     8724 2023-07-27 08:58:53.000000 valipy-0.1.1/valipy/exceptions.py
+-rw-r--r--   0 josevonchong   (501) staff       (20)    10869 2023-07-27 10:12:21.000000 valipy-0.1.1/valipy/myFunctions.py
+drwxr-xr-x   0 josevonchong   (501) staff       (20)        0 2023-07-28 22:42:01.740281 valipy-0.1.1/valipy.egg-info/
+-rw-r--r--   0 josevonchong   (501) staff       (20)      626 2023-07-28 22:42:01.000000 valipy-0.1.1/valipy.egg-info/PKG-INFO
+-rw-r--r--   0 josevonchong   (501) staff       (20)      243 2023-07-28 22:42:01.000000 valipy-0.1.1/valipy.egg-info/SOURCES.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)        1 2023-07-28 22:42:01.000000 valipy-0.1.1/valipy.egg-info/dependency_links.txt
+-rw-r--r--   0 josevonchong   (501) staff       (20)       12 2023-07-28 22:42:01.000000 valipy-0.1.1/valipy.egg-info/top_level.txt
```

### Comparing `valipy-0.1.0/PKG-INFO` & `valipy-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `valipy-0.1.0/setup.py` & `valipy-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import find_packages, setup
 setup(
     name='valipy',
     packages=find_packages(),
-    version='0.1.0',
+    version='0.1.1',
     description='A chainable, fluent Python library for validating data',
     author='Joaquin Jose Von Chong',
     license='MIT',
     author_email = 'jjvonchong@outlook.com',      # Type in your E-Mail
     url = 'https://github.com/pimepan/valipy',   # Provide either the link to your github or to your website
     download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
     keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
+    readme='README.md',
     install_requires=[],
     classifiers=[
         'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',      # Define that your audience are developers
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',   # Again, pick a license
-        'Programming Language :: Python :: 3.10',      #Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `valipy-0.1.0/valipy/exceptions.py` & `valipy-0.1.1/valipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.1.0/valipy/myFunctions.py` & `valipy-0.1.1/valipy/myFunctions.py`

 * *Files identical despite different names*

### Comparing `valipy-0.1.0/valipy.egg-info/PKG-INFO` & `valipy-0.1.1/valipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: valipy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A chainable, fluent Python library for validating data
 Home-page: https://github.com/pimepan/valipy
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Joaquin Jose Von Chong
 Author-email: jjvonchong@outlook.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

