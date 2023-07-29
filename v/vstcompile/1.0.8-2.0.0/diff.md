# Comparing `tmp/vstcompile-1.0.8.tar.gz` & `tmp/vstcompile-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vstcompile-1.0.8.tar", last modified: Wed Jun 20 09:43:36 2018, max compression
+gzip compressed data, was "vstcompile-2.0.0.tar", last modified: Sat Jul 29 04:59:02 2023, max compression
```

## Comparing `vstcompile-1.0.8.tar` & `vstcompile-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-20 09:43:36.000000 vstcompile-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/
--rw-r--r--   0 root         (0) root         (0)       11 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      326 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      196 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2699 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1175 2018-06-20 09:43:31.000000 vstcompile-1.0.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      829 2018-06-20 09:43:36.000000 vstcompile-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-06-20 09:43:36.000000 vstcompile-1.0.8/vstcompile/
--rw-rw-rw-   0 root         (0) root         (0)     1884 2018-06-20 09:43:31.000000 vstcompile-1.0.8/vstcompile/release.py
--rw-rw-rw-   0 root         (0) root         (0)     2925 2018-06-20 09:43:31.000000 vstcompile-1.0.8/vstcompile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2018-06-20 09:43:31.000000 vstcompile-1.0.8/requirements-release.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2018-06-20 09:43:31.000000 vstcompile-1.0.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)    11333 2018-06-20 09:43:31.000000 vstcompile-1.0.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      131 2018-06-20 09:43:31.000000 vstcompile-1.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      803 2018-06-20 09:43:31.000000 vstcompile-1.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2018-06-20 09:43:31.000000 vstcompile-1.0.8/requirements-doc.txt
--rw-r--r--   0 root         (0) root         (0)     2699 2018-06-20 09:43:36.000000 vstcompile-1.0.8/PKG-INFO
+drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/
+-rw-rw-r--   0 grey      (1000) grey      (1000)    11344 2023-07-29 03:48:47.000000 vstcompile-2.0.0/LICENSE
+-rwxrwxr-x   0 grey      (1000) grey      (1000)       33 2023-07-29 04:06:42.000000 vstcompile-2.0.0/MANIFEST.in
+-rw-rw-r--   0 grey      (1000) grey      (1000)      585 2023-07-29 03:48:47.000000 vstcompile-2.0.0/NOTICE
+-rw-rw-r--   0 grey      (1000) grey      (1000)     2815 2023-07-29 04:59:02.992552 vstcompile-2.0.0/PKG-INFO
+-rw-rw-r--   0 grey      (1000) grey      (1000)     1472 2023-07-29 04:58:15.000000 vstcompile-2.0.0/README.rst
+-rw-rw-r--   0 grey      (1000) grey      (1000)     1698 2023-07-29 04:58:36.000000 vstcompile-2.0.0/pyproject.toml
+-rw-rw-r--   0 grey      (1000) grey      (1000)       38 2023-07-29 04:59:02.992552 vstcompile-2.0.0/setup.cfg
+-rw-rw-r--   0 grey      (1000) grey      (1000)      200 2023-07-29 04:07:16.000000 vstcompile-2.0.0/setup.py
+drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/vstcompile/
+-rw-rw-r--   0 grey      (1000) grey      (1000)    11758 2023-07-29 04:18:29.000000 vstcompile-2.0.0/vstcompile/__init__.py
+-rw-rw-r--   0 grey      (1000) grey      (1000)     1590 2023-07-29 04:54:34.000000 vstcompile-2.0.0/vstcompile/github.py
+-rw-rw-r--   0 grey      (1000) grey      (1000)      742 2023-07-29 04:16:26.000000 vstcompile-2.0.0/vstcompile/utils.py
+drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-07-29 04:59:02.992552 vstcompile-2.0.0/vstcompile.egg-info/
+-rw-rw-r--   0 grey      (1000) grey      (1000)     2815 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/PKG-INFO
+-rw-rw-r--   0 grey      (1000) grey      (1000)      327 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/SOURCES.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/dependency_links.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/not-zip-safe
+-rw-rw-r--   0 grey      (1000) grey      (1000)       58 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/requires.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)       11 2023-07-29 04:59:02.000000 vstcompile-2.0.0/vstcompile.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vstcompile-1.0.8/vstcompile.egg-info/PKG-INFO` & `vstcompile-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 Metadata-Version: 2.1
 Name: vstcompile
-Version: 1.0.8
+Version: 2.0.0
 Summary: VST util for easy compile
-Home-page: https://github.com/vstconsulting
-Author: VST Consulting
-Author-email: sergey.k@vstconsulting.net
-License: Apache Software License
+Author-email: VST Consulting <sergey.k@vstconsulting.net>
+License: Apache License 2.0
+Project-URL: Home, https://github.com/vstconsulting/vstcompile
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstcompile/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstcompile
 Project-URL: Releases, https://pypi.org/project/vstcompile/#history
-Description: VST Compile utility
-        ===================
-        
-        Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
-        
-        Quick start
-        -----------
-        
-        1. Install package via `pip install vstcompile`
-        
-        2. Create `requirements.txt` and `setup.py` in your project:
-           .. sourcecode:: python
-        
-              import os
-              
-              # allow setup.py to be run from any path
-              
-              os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-        
-              from vstcompile import load_requirements, make_setup, find_packages
-        
-              ext_list = [
-                ... some extentions import paths with `*.py, *.c or *.pyx` extentions ...
-              ]
-              
-              make_setup(
-                packages=find_packages(exclude=['tests']+ext_list),
-                
-                ext_modules_list=ext_list,
-                
-                include_package_data=True,
-                
-                install_requires=load_requirements('requirements.txt')
-              )
-        
-        3. Run `python setup.py compile` to compile and pack dist-package.
-        
-        
-        Requirements
-        ------------
-        
-        If you want to use Sphinx in projects, you should install package:
-        
-           .. sourcecode:: bash
-        
-              pip install vstcompile[doc]
-        
-        
-        LICENCE
-        -------
-        
-        Apache Software License
-        
-Keywords: cythonize,compile,util
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Provides-Extra: compile
-Provides-Extra: doc
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: cython
 Provides-Extra: release
+License-File: LICENSE
+License-File: NOTICE
+
+VST Compile utility
+===================
+
+Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
+
+Quick start
+-----------
+
+1. Install package via `pip install vstcompile`
+
+2. Create `requirements.txt` and `setup.py` in your project:
+
+   .. sourcecode:: python
+
+      import os
+      from vstcompile import load_requirements, make_setup, find_packages
+
+
+      # allow setup.py to be run from any path
+      os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
+
+      ext_list = [
+        ... some extentions import paths with `*.py, *.c or *.pyx` extentions ...
+      ]
+      
+      make_setup(
+        packages=find_packages(exclude=['tests']+ext_list),
+        ext_modules_list=ext_list,
+        include_package_data=True,
+        install_requires=load_requirements('requirements.txt')
+      )
+
+3. Run `python setup.py compile` to compile and pack dist-package.
+
+4. Add requirement to `pyproject.toml` and enjoy!
+
+Requirements
+------------
+
+If you want to use Sphinx in projects, you should install package with sphinx packages.
+
+If you want to use github release, install it with extra `release` and use command `githubrelease`:
+
+   .. sourcecode:: bash
+
+      pip install vstcompile[release]
+      python setup.py githubrelease
+
+
+License
+-------
+
+VST Compile is licensed under the terms of the Apache License 2.0.
+See the file "LICENSE" for more information.
+
+Copyright 2018-2023 VST Consulting
```

### Comparing `vstcompile-1.0.8/LICENSE` & `vstcompile-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018 vst
+   Copyright 2018 VST Consulting
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vstcompile-1.0.8/PKG-INFO` & `vstcompile-2.0.0/vstcompile.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 Metadata-Version: 2.1
 Name: vstcompile
-Version: 1.0.8
+Version: 2.0.0
 Summary: VST util for easy compile
-Home-page: https://github.com/vstconsulting
-Author: VST Consulting
-Author-email: sergey.k@vstconsulting.net
-License: Apache Software License
+Author-email: VST Consulting <sergey.k@vstconsulting.net>
+License: Apache License 2.0
+Project-URL: Home, https://github.com/vstconsulting/vstcompile
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstcompile/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstcompile
 Project-URL: Releases, https://pypi.org/project/vstcompile/#history
-Description: VST Compile utility
-        ===================
-        
-        Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
-        
-        Quick start
-        -----------
-        
-        1. Install package via `pip install vstcompile`
-        
-        2. Create `requirements.txt` and `setup.py` in your project:
-           .. sourcecode:: python
-        
-              import os
-              
-              # allow setup.py to be run from any path
-              
-              os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-        
-              from vstcompile import load_requirements, make_setup, find_packages
-        
-              ext_list = [
-                ... some extentions import paths with `*.py, *.c or *.pyx` extentions ...
-              ]
-              
-              make_setup(
-                packages=find_packages(exclude=['tests']+ext_list),
-                
-                ext_modules_list=ext_list,
-                
-                include_package_data=True,
-                
-                install_requires=load_requirements('requirements.txt')
-              )
-        
-        3. Run `python setup.py compile` to compile and pack dist-package.
-        
-        
-        Requirements
-        ------------
-        
-        If you want to use Sphinx in projects, you should install package:
-        
-           .. sourcecode:: bash
-        
-              pip install vstcompile[doc]
-        
-        
-        LICENCE
-        -------
-        
-        Apache Software License
-        
-Keywords: cythonize,compile,util
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Provides-Extra: compile
-Provides-Extra: doc
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: cython
 Provides-Extra: release
+License-File: LICENSE
+License-File: NOTICE
+
+VST Compile utility
+===================
+
+Lib for quick formatting `setup.py` in projects. Moved from `vstutils` projects for easyer integration.
+
+Quick start
+-----------
+
+1. Install package via `pip install vstcompile`
+
+2. Create `requirements.txt` and `setup.py` in your project:
+
+   .. sourcecode:: python
+
+      import os
+      from vstcompile import load_requirements, make_setup, find_packages
+
+
+      # allow setup.py to be run from any path
+      os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
+
+      ext_list = [
+        ... some extentions import paths with `*.py, *.c or *.pyx` extentions ...
+      ]
+      
+      make_setup(
+        packages=find_packages(exclude=['tests']+ext_list),
+        ext_modules_list=ext_list,
+        include_package_data=True,
+        install_requires=load_requirements('requirements.txt')
+      )
+
+3. Run `python setup.py compile` to compile and pack dist-package.
+
+4. Add requirement to `pyproject.toml` and enjoy!
+
+Requirements
+------------
+
+If you want to use Sphinx in projects, you should install package with sphinx packages.
+
+If you want to use github release, install it with extra `release` and use command `githubrelease`:
+
+   .. sourcecode:: bash
+
+      pip install vstcompile[release]
+      python setup.py githubrelease
+
+
+License
+-------
+
+VST Compile is licensed under the terms of the Apache License 2.0.
+See the file "LICENSE" for more information.
+
+Copyright 2018-2023 VST Consulting
```

