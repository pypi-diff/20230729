# Comparing `tmp/MAZAlib-0.0.1.tar.gz` & `tmp/MAZAlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAZAlib-0.0.1.tar", last modified: Sat Jul 29 12:30:33 2023, max compression
+gzip compressed data, was "MAZAlib-0.0.2.tar", last modified: Sat Jul 29 13:17:47 2023, max compression
```

## Comparing `MAZAlib-0.0.1.tar` & `MAZAlib-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 12:30:33.878756 MAZAlib-0.0.1/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.1/LICENSE.txt
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 12:30:33.878756 MAZAlib-0.0.1/MAZAlib.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2566 2023-07-29 12:30:33.000000 MAZAlib-0.0.1/MAZAlib.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      215 2023-07-29 12:30:33.000000 MAZAlib-0.0.1/MAZAlib.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 12:30:33.000000 MAZAlib-0.0.1/MAZAlib.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       14 2023-07-29 12:30:33.000000 MAZAlib-0.0.1/MAZAlib.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2566 2023-07-29 12:30:33.878756 MAZAlib-0.0.1/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1920 2023-07-29 11:28:49.000000 MAZAlib-0.0.1/README.md
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 12:30:33.878756 MAZAlib-0.0.1/maza_cwrapper/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2023-07-29 12:00:38.000000 MAZAlib-0.0.1/maza_cwrapper/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       57 2023-07-29 12:03:21.000000 MAZAlib-0.0.1/maza_cwrapper/my_dist.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 12:30:33.878756 MAZAlib-0.0.1/setup.cfg
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      819 2023-07-29 12:30:26.000000 MAZAlib-0.0.1/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.2/LICENSE.txt
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/MAZAlib.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2566 2023-07-29 13:17:47.000000 MAZAlib-0.0.2/MAZAlib.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      188 2023-07-29 13:17:47.000000 MAZAlib-0.0.2/MAZAlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 13:17:47.000000 MAZAlib-0.0.2/MAZAlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        8 2023-07-29 13:17:47.000000 MAZAlib-0.0.2/MAZAlib.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2566 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1920 2023-07-29 12:39:10.000000 MAZAlib-0.0.2/README.md
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/mydist/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/mydist/src/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      150 2023-07-29 12:47:45.000000 MAZAlib-0.0.2/mydist/src/mydist.cpp
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 13:17:47.247346 MAZAlib-0.0.2/setup.cfg
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1148 2023-07-29 13:17:44.000000 MAZAlib-0.0.2/setup.py
```

### Comparing `MAZAlib-0.0.1/LICENSE.txt` & `MAZAlib-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.1/MAZAlib.egg-info/PKG-INFO` & `MAZAlib-0.0.2/MAZAlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: TBA
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.txt
 
 # MAZAlib
 
-Version 0.0.1 silent
+Version 0.0.2 silent
 
 Cross-platform 2d/3d image segmentation C++ library
 
 Compliles with: MSVC 14.0 and later, GCC 9.2. Other GCC: not tested yet.
 Compatible with C++14, C++11 - not tested
 
 Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
```

### Comparing `MAZAlib-0.0.1/PKG-INFO` & `MAZAlib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: TBA
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 License-File: LICENSE.txt
 
 # MAZAlib
 
-Version 0.0.1 silent
+Version 0.0.2 silent
 
 Cross-platform 2d/3d image segmentation C++ library
 
 Compliles with: MSVC 14.0 and later, GCC 9.2. Other GCC: not tested yet.
 Compatible with C++14, C++11 - not tested
 
 Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
```

### Comparing `MAZAlib-0.0.1/README.md` & `MAZAlib-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MAZAlib
 
-Version 0.0.1 silent
+Version 0.0.2 silent
 
 Cross-platform 2d/3d image segmentation C++ library
 
 Compliles with: MSVC 14.0 and later, GCC 9.2. Other GCC: not tested yet.
 Compatible with C++14, C++11 - not tested
 
 Authors: Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
```

### Comparing `MAZAlib-0.0.1/setup.py` & `MAZAlib-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import setuptools
-
+import glob
 
 libName="MAZAlib"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=libName,
-    version="0.0.1",
+    version="0.0.2",
     description='TBA',
     long_description=long_description,
     author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina',
     author_email='mathieu.gravey@unil.ch',
     license='GPLv3',
     packages=setuptools.find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Programming Language :: C++',
         'Programming Language :: Python :: 3 :: Only',
         'Operating System :: OS Independent'
-    ]
+    ],
+    ext_modules=[setuptools.Extension(libName, sources=['./maza_cwrapper/pythonInterface.cpp']+glob.glob('./mydist/src/*.cpp'),
+			language="c++", 
+			extra_compile_args=["-std=c++17",'-O3', '-w'],
+			extra_link_args=["-std=c++17"],
+			include_dirs=['./mydist/include'],
+			libraries = [],
+			library_dirs = []
+			)]
 )
```

