# Comparing `tmp/pyanthem-1.1.8.tar.gz` & `tmp/pyanthem-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyanthem-1.1.8.tar", last modified: Fri Jun 17 16:02:48 2022, max compression
+gzip compressed data, was "pyanthem-1.1.9.tar", last modified: Fri Jun 17 16:19:41 2022, max compression
```

## Comparing `pyanthem-1.1.8.tar` & `pyanthem-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:02:48.000000 pyanthem-1.1.8/
--rw-r--r--   0 nicthib    (501) staff       (20)     1073 2022-06-17 15:48:49.000000 pyanthem-1.1.8/LICENSE
--rw-r--r--   0 nicthib    (501) staff       (20)       29 2022-06-17 15:48:49.000000 pyanthem-1.1.8/MANIFEST.in
--rw-r--r--   0 nicthib    (501) staff       (20)     9630 2022-06-17 16:02:48.000000 pyanthem-1.1.8/PKG-INFO
--rw-r--r--   0 nicthib    (501) staff       (20)     9162 2022-06-17 15:48:49.000000 pyanthem-1.1.8/README.rst
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:02:48.000000 pyanthem-1.1.8/pyanthem/
--rw-r--r--   0 nicthib    (501) staff       (20)       68 2022-06-17 15:48:49.000000 pyanthem-1.1.8/pyanthem/__init__.py
--rw-r--r--   0 nicthib    (501) staff       (20)      767 2022-06-17 15:48:49.000000 pyanthem-1.1.8/pyanthem/decompmp4.py
--rw-r--r--   0 nicthib    (501) staff       (20)     1527 2022-06-17 15:48:49.000000 pyanthem-1.1.8/pyanthem/obsolete.py
--rw-r--r--   0 nicthib    (501) staff       (20)    35039 2022-06-17 15:56:00.000000 pyanthem-1.1.8/pyanthem/pyanthem.py
--rw-r--r--   0 nicthib    (501) staff       (20)     1521 2022-06-17 15:48:49.000000 pyanthem-1.1.8/pyanthem/pyanthem_vars.py
-drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:02:48.000000 pyanthem-1.1.8/pyanthem.egg-info/
--rw-r--r--   0 nicthib    (501) staff       (20)     9630 2022-06-17 16:02:47.000000 pyanthem-1.1.8/pyanthem.egg-info/PKG-INFO
--rw-r--r--   0 nicthib    (501) staff       (20)      309 2022-06-17 16:02:48.000000 pyanthem-1.1.8/pyanthem.egg-info/SOURCES.txt
--rw-r--r--   0 nicthib    (501) staff       (20)        1 2022-06-17 16:02:47.000000 pyanthem-1.1.8/pyanthem.egg-info/dependency_links.txt
--rw-r--r--   0 nicthib    (501) staff       (20)      106 2022-06-17 16:02:47.000000 pyanthem-1.1.8/pyanthem.egg-info/requires.txt
--rw-r--r--   0 nicthib    (501) staff       (20)        9 2022-06-17 16:02:47.000000 pyanthem-1.1.8/pyanthem.egg-info/top_level.txt
--rw-r--r--   0 nicthib    (501) staff       (20)       38 2022-06-17 16:02:48.000000 pyanthem-1.1.8/setup.cfg
--rw-r--r--   0 nicthib    (501) staff       (20)      913 2022-06-17 16:02:34.000000 pyanthem-1.1.8/setup.py
+drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.050736 pyanthem-1.1.9/
+-rw-r--r--   0 nicthib    (501) staff       (20)     1073 2022-06-17 15:48:49.000000 pyanthem-1.1.9/LICENSE
+-rw-r--r--   0 nicthib    (501) staff       (20)       29 2022-06-17 15:48:49.000000 pyanthem-1.1.9/MANIFEST.in
+-rw-r--r--   0 nicthib    (501) staff       (20)     9676 2022-06-17 16:19:41.050545 pyanthem-1.1.9/PKG-INFO
+-rw-r--r--   0 nicthib    (501) staff       (20)     9162 2022-06-17 15:48:49.000000 pyanthem-1.1.9/README.rst
+drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.049584 pyanthem-1.1.9/pyanthem/
+-rw-r--r--   0 nicthib    (501) staff       (20)       68 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/__init__.py
+-rw-r--r--   0 nicthib    (501) staff       (20)      767 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/decompmp4.py
+-rw-r--r--   0 nicthib    (501) staff       (20)     1527 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/obsolete.py
+-rw-r--r--   0 nicthib    (501) staff       (20)    35039 2022-06-17 15:56:00.000000 pyanthem-1.1.9/pyanthem/pyanthem.py
+-rw-r--r--   0 nicthib    (501) staff       (20)     1521 2022-06-17 15:48:49.000000 pyanthem-1.1.9/pyanthem/pyanthem_vars.py
+drwxr-xr-x   0 nicthib    (501) staff       (20)        0 2022-06-17 16:19:41.050345 pyanthem-1.1.9/pyanthem.egg-info/
+-rw-r--r--   0 nicthib    (501) staff       (20)     9676 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/PKG-INFO
+-rw-r--r--   0 nicthib    (501) staff       (20)      309 2022-06-17 16:19:41.000000 pyanthem-1.1.9/pyanthem.egg-info/SOURCES.txt
+-rw-r--r--   0 nicthib    (501) staff       (20)        1 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/dependency_links.txt
+-rw-r--r--   0 nicthib    (501) staff       (20)       93 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/requires.txt
+-rw-r--r--   0 nicthib    (501) staff       (20)        9 2022-06-17 16:19:40.000000 pyanthem-1.1.9/pyanthem.egg-info/top_level.txt
+-rw-r--r--   0 nicthib    (501) staff       (20)       38 2022-06-17 16:19:41.050781 pyanthem-1.1.9/setup.cfg
+-rw-r--r--   0 nicthib    (501) staff       (20)      909 2022-06-17 16:19:33.000000 pyanthem-1.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyanthem-1.1.8/LICENSE` & `pyanthem-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/PKG-INFO` & `pyanthem-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pyanthem
-Version: 1.1.8
+Version: 1.1.9
 Summary: pyanthem - an audiovisualization tool to make your data more interesting
 Home-page: https://github.com/nicthib/pyanthem
 Author: Nic Thibodeaux
 Author-email: dnt2111@columbia.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.7,!= 3.8.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ********************************************************************
 pyanthem: Transforming your datasets into a colorful, audible format
 ********************************************************************
 
@@ -210,7 +212,9 @@
 
 Support
 =======
 
 - Twitter: `@nicthibs`_
 
 .. _`@nicthibs`: http://twitter.com/nicthibs
+
+
```

### Comparing `pyanthem-1.1.8/README.rst` & `pyanthem-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/pyanthem/decompmp4.py` & `pyanthem-1.1.9/pyanthem/decompmp4.py`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/pyanthem/obsolete.py` & `pyanthem-1.1.9/pyanthem/obsolete.py`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/pyanthem/pyanthem.py` & `pyanthem-1.1.9/pyanthem/pyanthem.py`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/pyanthem/pyanthem_vars.py` & `pyanthem-1.1.9/pyanthem/pyanthem_vars.py`

 * *Files identical despite different names*

### Comparing `pyanthem-1.1.8/pyanthem.egg-info/PKG-INFO` & `pyanthem-1.1.9/pyanthem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pyanthem
-Version: 1.1.8
+Version: 1.1.9
 Summary: pyanthem - an audiovisualization tool to make your data more interesting
 Home-page: https://github.com/nicthib/pyanthem
 Author: Nic Thibodeaux
 Author-email: dnt2111@columbia.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.7,!= 3.8.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ********************************************************************
 pyanthem: Transforming your datasets into a colorful, audible format
 ********************************************************************
 
@@ -210,7 +212,9 @@
 
 Support
 =======
 
 - Twitter: `@nicthibs`_
 
 .. _`@nicthibs`: http://twitter.com/nicthibs
+
+
```

### Comparing `pyanthem-1.1.8/setup.py` & `pyanthem-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # conda remove --name pyanthem --all
 import setuptools
 with open('README.rst', 'r') as fh:
 	long_description = fh.read()
 setuptools.setup(
 	name='pyanthem',
-	version='1.1.8',
+	version='1.1.9',
 	author='Nic Thibodeaux',
 	author_email='dnt2111@columbia.edu',
 	description='pyanthem - an audiovisualization tool to make your data more interesting',
 	long_description=long_description,
 	long_description_content_type='text/x-rst',
 	url='https://github.com/nicthib/pyanthem',
 	packages=setuptools.find_packages(),
 	setup_requires=[
 		'numpy',
 		'scipy'],
 	install_requires=[
 		'midiutil',
 		'matplotlib',
-		'pygame==2.0.0.dev10',
+		'pygame',
 		'sklearn',
 		'requests',
 		'googledrivedownloader',
 		'pillow',
 		'mido',
 		'ttkthemes',
 		'h5py'
 	  ],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python :: 3',
 		'License :: OSI Approved :: MIT License',
 		'Operating System :: OS Independent',
 	],
-	python_requires='>=3.7',
+	python_requires='>=3.7,!= 3.8.*',
 )
```

