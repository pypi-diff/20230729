# Comparing `tmp/spiralpy-0.1.1.tar.gz` & `tmp/spiralpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiralpy-0.1.1.tar", last modified: Tue Jul 25 19:20:59 2023, max compression
+gzip compressed data, was "spiralpy-1.0.1.tar", last modified: Sat Jul 29 03:53:26 2023, max compression
```

## Comparing `spiralpy-0.1.1.tar` & `spiralpy-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,42 @@
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:20:59.296515 spiralpy-0.1.1/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5694 2023-07-25 18:30:42.000000 spiralpy-0.1.1/Contributing.md
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1541 2023-07-20 19:02:18.000000 spiralpy-0.1.1/LICENSE
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       88 2023-07-25 17:49:05.000000 spiralpy-0.1.1/MANIFEST.in
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-25 19:20:59.295527 spiralpy-0.1.1/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6004 2023-07-25 17:25:12.000000 spiralpy-0.1.1/README.md
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-25 19:20:59.296529 spiralpy-0.1.1/setup.cfg
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1556 2023-07-25 19:18:03.000000 spiralpy-0.1.1/setup.py
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:20:59.286536 spiralpy-0.1.1/spiralpy/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3859 2023-07-20 19:02:14.000000 spiralpy-0.1.1/spiralpy/CMakeLists.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3339 2023-07-25 18:40:20.000000 spiralpy-0.1.1/spiralpy/__init__.py
-drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-25 19:20:59.293540 spiralpy-0.1.1/spiralpy.egg-info/
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-25 19:20:59.000000 spiralpy-0.1.1/spiralpy.egg-info/PKG-INFO
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)      227 2023-07-25 19:20:59.000000 spiralpy-0.1.1/spiralpy.egg-info/SOURCES.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-25 19:20:59.000000 spiralpy-0.1.1/spiralpy.egg-info/dependency_links.txt
--rw-r--r--   0 pbroderick (16220) pbroderick (28128)        9 2023-07-25 19:20:59.000000 spiralpy-0.1.1/spiralpy.egg-info/top_level.txt
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.010266 spiralpy-1.0.1/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5694 2023-07-25 18:30:42.000000 spiralpy-1.0.1/Contributing.md
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1541 2023-07-20 19:02:18.000000 spiralpy-1.0.1/LICENSE
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       88 2023-07-25 17:49:05.000000 spiralpy-1.0.1/MANIFEST.in
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-29 03:53:26.010263 spiralpy-1.0.1/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6803 2023-07-28 23:28:09.000000 spiralpy-1.0.1/README.md
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:25.974268 spiralpy-1.0.1/examples/
+-rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)    10941 2023-07-25 20:31:37.000000 spiralpy-1.0.1/examples/foo.sh
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      659 2023-07-27 19:11:23.000000 spiralpy-1.0.1/examples/print-metadata.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4409 2023-07-28 22:16:43.000000 spiralpy-1.0.1/examples/run-batchdft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1935 2023-07-28 22:17:23.000000 spiralpy-1.0.1/examples/run-batchmddft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1542 2023-07-28 22:18:10.000000 spiralpy-1.0.1/examples/run-dft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      542 2023-07-28 22:19:07.000000 spiralpy-1.0.1/examples/run-hockney130.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      534 2023-07-28 22:19:26.000000 spiralpy-1.0.1/examples/run-hockney8.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2158 2023-07-28 22:19:50.000000 spiralpy-1.0.1/examples/run-mddft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2592 2023-07-28 22:20:09.000000 spiralpy-1.0.1/examples/run-mdprdft.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1610 2023-07-28 19:30:46.000000 spiralpy-1.0.1/examples/run-mdrconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1448 2023-07-28 22:20:37.000000 spiralpy-1.0.1/examples/run-mdrfsconv.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1650 2023-07-28 03:30:38.000000 spiralpy-1.0.1/examples/run-stepphase.py
+-rwxr-xr-x   0 pbroderick (16220) pbroderick (28128)     6483 2023-07-28 22:12:20.000000 spiralpy-1.0.1/examples/test-many.sh
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)       38 2023-07-29 03:53:26.011263 spiralpy-1.0.1/setup.cfg
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     1952 2023-07-29 03:53:15.000000 spiralpy-1.0.1/setup.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.000266 spiralpy-1.0.1/spiralpy/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3859 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/CMakeLists.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4692 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/__init__.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5382 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/batchmddftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2400 2023-07-27 18:29:55.000000 spiralpy-1.0.1/spiralpy/constants.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6092 2023-07-27 18:00:26.000000 spiralpy-1.0.1/spiralpy/dftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/hockneysolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     4687 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/mddftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6537 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/mdprdftsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6229 2023-07-28 19:29:46.000000 spiralpy-1.0.1/spiralpy/mdrconvsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     6597 2023-07-28 04:13:51.000000 spiralpy-1.0.1/spiralpy/mdrfsconvsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     3139 2023-07-27 18:57:42.000000 spiralpy-1.0.1/spiralpy/metadata.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     2955 2023-07-27 17:46:05.000000 spiralpy-1.0.1/spiralpy/spiral.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)    14114 2023-07-28 03:44:11.000000 spiralpy-1.0.1/spiralpy/spsolver.py
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)     5079 2023-07-28 04:18:23.000000 spiralpy-1.0.1/spiralpy/stepphasesolver.py
+drwxr-xr-x   0 pbroderick (16220) pbroderick (28128)        0 2023-07-29 03:53:26.008262 spiralpy-1.0.1/spiralpy.egg-info/
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      710 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/PKG-INFO
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)      886 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/SOURCES.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        1 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/dependency_links.txt
+-rw-r--r--   0 pbroderick (16220) pbroderick (28128)        9 2023-07-29 03:53:25.000000 spiralpy-1.0.1/spiralpy.egg-info/top_level.txt
```

### Comparing `spiralpy-0.1.1/Contributing.md` & `spiralpy-1.0.1/Contributing.md`

 * *Files identical despite different names*

### Comparing `spiralpy-0.1.1/LICENSE` & `spiralpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spiralpy-0.1.1/PKG-INFO` & `spiralpy-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralpy
-Version: 0.1.1
+Version: 1.0.1
 Summary: A Python front end to specify high-level numerical computations
 Home-page: https://github.com/spiral-software/python-package-spiralpy
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-2-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-spiralpy
 Platform: UNKNOWN
```

### Comparing `spiralpy-0.1.1/README.md` & `spiralpy-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 internal documentation of the installed package.  For example:
 
 ```python console
 >>> import spiralpy
 >>> help(spiralpy)
 ```
 
-See the `examples` directory for a quick introduction.
+See the `examples` (discussed further below) directory for a quick introduction.
 
 *DISTRIBUTION STATEMENT A.  Approved for public release.  Distribution is unlimited.*
 
 ## Prerequisites
 
 - **Python3** (3.7 or higher)
     - **NumPy**
@@ -75,51 +75,78 @@
 ## Installing and Configuring SpiralPy
 
 The easiest method to install **SpiralPy** is to use Python's package manager **pip**, e.g.,
 ```shell
 pip install spiralpy
 ```
 
-If you want to develop, contribute to, or possibly modify **SpiralPy** it may be better to clone or
-fork the **SpiralPy** repository, see
+When you install **spiralpy** the modules are installed in your ```site-packages``` location.  You
+can determine this location (and your base location) by running this python command:
+```shell
+python -m site --user-site --user-base
+##   Sample output -- On Unix/Linux/MacOS
+##   ~/.local:~/.local/lib/python3.9/site-packages
+##   Windows
+##   C:\Users\<user>\AppData\Roaming\Python;C:\Users\<user>\AppData\Roaming\Python\Python38\site-packages
+```
+
+Base location is always output first, the two locations are separated by a ':' (Unix/Linux/MacOS)
+or a ';' (Windows).
+
+The examples and other miscellaneous files will be installed at ```share/spiralpy``` under your
+base location.  The ```.libs``` folder (see below) is also located here.
+
+If you want to develop, contribute to, or possibly modify **SpiralPy** it may be better to clone
+or fork the **SpiralPy** repository, see
 [**Contributing**](https://github.com/spiral-software/python-package-spiralpy/blob/main/Contributing.md).
 Clone **python-package-spiralpy** to a location on your computer renaming it to **spiralpy**.  For
 example:
 ```shell
 cd ~/work/python-packages
 git clone https://github.com/spiral-software/python-package-spiralpy spiralpy
 ```
 
-If you clone or fork the **SpiralPy** repository (vs installing the package) you need to add the directory that contains it to the environment variable **PYTHONPATH**.  (In the above example that would be ```~/work/python-packages/spiralpy```.)  This allows Python to locate the **spiralpy** module.
-
-By default, **SpiralPy** puts generated files into a temporary directory under the current working directory, then deletes that temporary directory after a successful build.  If there is an error during the build, the temporary directory will remain.  There are two environment variables that can modify this default behavior:
+If you clone or fork the **SpiralPy** repository (vs installing the package) you need to add the
+directory that contains it to the environment variable **PYTHONPATH**.  (In the above example that
+would be ```~/work/python-packages/spiralpy```).  This allows Python to locate the **spiralpy**
+module.
+
+By default, **SpiralPy** puts generated files into a temporary directory under the current working
+directory, then deletes that temporary directory after a successful build.  If there is an error
+during the build, the temporary directory will remain.  There are two environment variables that
+can modify this default behavior: 
 
-+ **SW_WORKDIR** specifies the path to the parent directory of the temporary build directories.  If that specified directory does not exist, **SpiralPy** uses the current directory.
-
-+ **SW_KEEPTEMP** if defined (any value) tells **SpiralPy** to preserve temporary build directories.
++ **SP_WORKDIR** specifies the path to the parent directory of the temporary build directories.
+If that specified directory does not exist, **SpiralPy** uses the current directory.
 
++ **SP_KEEPTEMP** if defined (any value) tells **SpiralPy** to preserve temporary build
+directories.
 
 ## Exernal Libraries
 
-**Spiralpy** can access libraries built by [**FFTX**](https://github.com/spiral-software/fftx), which have metadata that describes their contents.  **SpiralPy** looks in its ```.libs``` directory for any libraries containing compatible metadata.  It also looks for libraries in directories specified by the **SW_LIBRARY_PATH** environment variable, with the list of directories having the same format as used for the **PATH** variable.
+**SpiralPy** can access libraries built by [**FFTX**](https://github.com/spiral-software/fftx), which have metadata that describes their contents.  **SpiralPy** looks in its ```.libs``` directory for any libraries containing compatible metadata.  It also looks for libraries in directories specified by the **SP_LIBRARY_PATH** environment variable, with the list of directories having the same format as used for the **PATH** variable.
 
 
 ## Try an Example
 
 Open a terminal window in the ```examples``` directory and run this example:
 
 ```shell
-~/work/python-packages/spiralpy/examples$ python run-mddft.py 32
+cd ~/work/python-packages/spiralpy/examples
+python run-mddft.py 32
 ```
-The first time you run it, you will see output from the CMake/SPIRAL/C build before the comparison results,
-similar to this:
 
+The first time you run it, you will see output from the CMake/SPIRAL/C build before the comparison
+results, similar to this:
 ```shell
 Generating CUDA
 Compiling and linking
-Diff between Python/C transforms = 1.206500728403121e-12
+Python/C transforms are equivalent, diff = 1.206500728403121e-12
 ```
 
-After that it will run much faster using the generated library, which is placed in the ```spiralpy/.libs``` directory.
-
-Some of the examples require additional arguments, and some options you can change.  Read through the examples for better understanding.  If you want to see the generated source files, set the **SW_KEEPTEMP** environment variable and look in the temporary directories.
+After that it will run much faster using the generated library, which is placed in the
+<br>
+```<base-location>/share/spiralpy/.libs``` directory.
 
+Some of the examples require additional arguments, and some options you can change.  Read through
+the examples for better understanding.  If you want to see the generated source files, set the
+**SP_KEEPTEMP** environment variable and look in the temporary directories.
```

### Comparing `spiralpy-0.1.1/spiralpy/CMakeLists.txt` & `spiralpy-1.0.1/spiralpy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `spiralpy-0.1.1/spiralpy.egg-info/PKG-INFO` & `spiralpy-1.0.1/spiralpy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiralpy
-Version: 0.1.1
+Version: 1.0.1
 Summary: A Python front end to specify high-level numerical computations
 Home-page: https://github.com/spiral-software/python-package-spiralpy
 Author: SpiralGen Inc.
 Author-email: Patrick.Broderick@spiralgen.com
 License: BSD-2-Clause
 Project-URL: Source Code, https://github.com/spiral-software/python-package-spiralpy
 Platform: UNKNOWN
```

