# Comparing `tmp/BloxPy-0.1.1.tar.gz` & `tmp/BloxPy-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BloxPy-0.1.1.tar", last modified: Fri Jul 28 21:12:17 2023, max compression
+gzip compressed data, was "BloxPy-0.1.11.tar", last modified: Fri Jul 28 21:58:16 2023, max compression
```

## Comparing `BloxPy-0.1.1.tar` & `BloxPy-0.1.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 21:12:17.266790 BloxPy-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-28 21:12:17.249549 BloxPy-0.1.1/BloxPy/
--rw-rw-rw-   0        0        0      343 2023-07-28 20:19:36.000000 BloxPy-0.1.1/BloxPy/Users.py
--rw-rw-rw-   0        0        0       26 2023-07-28 21:01:51.000000 BloxPy-0.1.1/BloxPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 21:12:17.265556 BloxPy-0.1.1/BloxPy.egg-info/
--rw-rw-rw-   0        0        0     2919 2023-07-28 21:12:17.000000 BloxPy-0.1.1/BloxPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-28 21:12:17.000000 BloxPy-0.1.1/BloxPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 21:12:17.000000 BloxPy-0.1.1/BloxPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-28 21:12:17.000000 BloxPy-0.1.1/BloxPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 21:12:17.000000 BloxPy-0.1.1/BloxPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2919 2023-07-28 21:12:17.266790 BloxPy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-07-28 20:35:14.000000 BloxPy-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 21:12:17.267791 BloxPy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1738 2023-07-28 21:11:31.000000 BloxPy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.323167 BloxPy-0.1.11/
+drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.315171 BloxPy-0.1.11/BloxPy/
+-rw-rw-rw-   0        0        0        0 2023-07-28 21:18:45.000000 BloxPy-0.1.11/BloxPy/__init__.py
+-rw-rw-rw-   0        0        0      343 2023-07-28 20:19:36.000000 BloxPy-0.1.11/BloxPy/users.py
+drwxrwxrwx   0        0        0        0 2023-07-28 21:58:16.321168 BloxPy-0.1.11/BloxPy.egg-info/
+-rw-rw-rw-   0        0        0     2921 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 21:58:16.000000 BloxPy-0.1.11/BloxPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2921 2023-07-28 21:58:16.323167 BloxPy-0.1.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-07-28 20:35:14.000000 BloxPy-0.1.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-28 21:58:16.323167 BloxPy-0.1.11/setup.cfg
+-rw-rw-rw-   0        0        0     1740 2023-07-28 21:58:04.000000 BloxPy-0.1.11/setup.py
```

### Comparing `BloxPy-0.1.1/BloxPy.egg-info/PKG-INFO` & `BloxPy-0.1.11/BloxPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.1
+Version: 0.1.11
 Summary: BloxPy: Your All-in-One Python Library for Roblox Development
 Home-page: https://github.com/yourusername/bloxpy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `BloxPy-0.1.1/PKG-INFO` & `BloxPy-0.1.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.1
+Version: 0.1.11
 Summary: BloxPy: Your All-in-One Python Library for Roblox Development
 Home-page: https://github.com/yourusername/bloxpy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `BloxPy-0.1.1/README.md` & `BloxPy-0.1.11/README.md`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.1/setup.py` & `BloxPy-0.1.11/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = 'BloxPy'
-VERSION = '0.1.1'
+VERSION = '0.1.11'
 DESCRIPTION = 'BloxPy: Your All-in-One Python Library for Roblox Development'
 LONG_DESCRIPTION = 'BloxPy is the ultimate Python library for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.'
 AUTHOR = 'Developer X'
 EMAIL = 'developer.x.business@gmail.com'
 URL = 'https://github.com/yourusername/bloxpy'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.6'
@@ -27,15 +27,15 @@
     author_email=EMAIL,
     url=URL,
     license=LICENSE,
     python_requires=PYTHON_REQUIRES,
     packages=find_packages(exclude=['tests']), 
     install_requires=REQUIRES,
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

