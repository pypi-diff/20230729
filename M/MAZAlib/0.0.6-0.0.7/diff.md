# Comparing `tmp/MAZAlib-0.0.6.tar.gz` & `tmp/MAZAlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAZAlib-0.0.6.tar", last modified: Sat Jul 29 13:52:24 2023, max compression
+gzip compressed data, was "MAZAlib-0.0.7.tar", last modified: Sat Jul 29 13:56:34 2023, max compression
```

## Comparing `MAZAlib-0.0.6.tar` & `MAZAlib-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:52:24.606207 MAZAlib-0.0.6/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.6/LICENSE.txt
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:52:24.606207 MAZAlib-0.0.6/MAZAlib.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 13:52:24.000000 MAZAlib-0.0.6/MAZAlib.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      200 2023-07-29 13:52:24.000000 MAZAlib-0.0.6/MAZAlib.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 13:52:24.000000 MAZAlib-0.0.6/MAZAlib.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        8 2023-07-29 13:52:24.000000 MAZAlib-0.0.6/MAZAlib.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 13:52:24.606207 MAZAlib-0.0.6/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1898 2023-07-29 13:42:12.000000 MAZAlib-0.0.6/README.md
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:52:24.606207 MAZAlib-0.0.6/maza_cwrapper/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1206 2023-07-29 13:11:12.000000 MAZAlib-0.0.6/maza_cwrapper/pythoninterface.cpp
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 13:52:24.606207 MAZAlib-0.0.6/setup.cfg
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1198 2023-07-29 13:52:10.000000 MAZAlib-0.0.6/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:56:34.830528 MAZAlib-0.0.7/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.7/LICENSE.txt
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:56:34.830528 MAZAlib-0.0.7/MAZAlib.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 13:56:34.000000 MAZAlib-0.0.7/MAZAlib.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      200 2023-07-29 13:56:34.000000 MAZAlib-0.0.7/MAZAlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 13:56:34.000000 MAZAlib-0.0.7/MAZAlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        8 2023-07-29 13:56:34.000000 MAZAlib-0.0.7/MAZAlib.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 13:56:34.830528 MAZAlib-0.0.7/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1898 2023-07-29 13:42:12.000000 MAZAlib-0.0.7/README.md
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:56:34.830528 MAZAlib-0.0.7/maza_cwrapper/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1206 2023-07-29 13:11:12.000000 MAZAlib-0.0.7/maza_cwrapper/pythoninterface.cpp
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 13:56:34.830528 MAZAlib-0.0.7/setup.cfg
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1203 2023-07-29 13:56:21.000000 MAZAlib-0.0.7/setup.py
```

### Comparing `MAZAlib-0.0.6/LICENSE.txt` & `MAZAlib-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.6/MAZAlib.egg-info/PKG-INFO` & `MAZAlib-0.0.7/MAZAlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: TODO
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MAZAlib-0.0.6/PKG-INFO` & `MAZAlib-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: TODO
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MAZAlib-0.0.6/README.md` & `MAZAlib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.6/maza_cwrapper/pythoninterface.cpp` & `MAZAlib-0.0.7/maza_cwrapper/pythoninterface.cpp`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.6/setup.py` & `MAZAlib-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 libName="MAZAlib"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=libName,
-    version="0.0.6",
+    version="0.0.7",
     description='TODO',
     long_description=long_description,
     author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina',
     author_email='mathieu.gravey@unil.ch',
     license='GPLv3',
     packages=setuptools.find_packages(),
     classifiers=[
@@ -20,15 +20,15 @@
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Programming Language :: C++',
         'Programming Language :: Python :: 3 :: Only',
         'Operating System :: OS Independent'
     ],
-    package_data={'mydist_lib': ['libmydist_lib.so']},
+    package_data={'': ['./mydist/build/libmydist_lib.so']},
     ext_modules=[setuptools.Extension(libName, sources=['./maza_cwrapper/pythoninterface.cpp'],
 			language="c++", 
 			extra_compile_args=["-std=c++17",'-O3', '-w'],
 			extra_link_args=["-std=c++17"],
 			# include_dirs=['./mydist/include'],
 			libraries = ["mydist_lib"],
 			library_dirs = ["./mydist//"]
```

