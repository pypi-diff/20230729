# Comparing `tmp/calfcv-0.0.2.tar.gz` & `tmp/calfcv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calfcv-0.0.2.tar", last modified: Sat Jul 29 01:56:40 2023, max compression
+gzip compressed data, was "calfcv-0.0.3.tar", last modified: Sat Jul 29 01:59:55 2023, max compression
```

## Comparing `calfcv-0.0.2.tar` & `calfcv-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:56:40.426446 calfcv-0.0.2/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.2/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.2/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:56:40.426446 calfcv-0.0.2/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1601 2023-07-29 01:03:54.000000 calfcv-0.0.2/README.rst
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:56:40.426446 calfcv-0.0.2/calfcv/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.2/calfcv/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-25 13:03:05.000000 calfcv-0.0.2/calfcv/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8413 2023-07-28 22:24:41.000000 calfcv-0.0.2/calfcv/calfcv.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:56:40.426446 calfcv-0.0.2/calfcv/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.2/calfcv/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.2/calfcv/tests/test_calfcv.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.2/calfcv/tests/test_common.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:56:40.426446 calfcv-0.0.2/calfcv.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:56:40.000000 calfcv-0.0.2/calfcv.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 01:56:40.000000 calfcv-0.0.2/calfcv.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 01:56:40.000000 calfcv-0.0.2/calfcv.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.2/calfcv.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 01:56:40.000000 calfcv-0.0.2/calfcv.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 01:56:40.000000 calfcv-0.0.2/calfcv.egg-info/top_level.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.2/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 01:56:40.430446 calfcv-0.0.2/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1775 2023-07-29 01:23:31.000000 calfcv-0.0.2/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1495 2023-07-29 01:55:36.000000 calfcv-0.0.3/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-24 23:20:23.000000 calfcv-0.0.3/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:59:55.887296 calfcv-0.0.3/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1601 2023-07-29 01:03:54.000000 calfcv-0.0.3/README.rst
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       98 2023-07-28 23:01:34.000000 calfcv-0.0.3/calfcv/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-07-29 01:59:39.000000 calfcv-0.0.3/calfcv/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8413 2023-07-28 22:24:41.000000 calfcv-0.0.3/calfcv/calfcv.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-24 23:20:23.000000 calfcv-0.0.3/calfcv/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1563 2023-07-28 13:25:35.000000 calfcv-0.0.3/calfcv/tests/test_calfcv.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      257 2023-07-28 12:52:06.000000 calfcv-0.0.3/calfcv/tests/test_common.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-07-29 01:59:55.887296 calfcv-0.0.3/calfcv.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2229 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      380 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-07-28 23:40:52.000000 calfcv-0.0.3/calfcv.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        7 2023-07-29 01:59:55.000000 calfcv-0.0.3/calfcv.egg-info/top_level.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       24 2023-07-24 23:20:23.000000 calfcv-0.0.3/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-07-29 01:59:55.887296 calfcv-0.0.3/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1775 2023-07-29 01:59:39.000000 calfcv-0.0.3/setup.py
```

### Comparing `calfcv-0.0.2/LICENSE` & `calfcv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.2/PKG-INFO` & `calfcv-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.2
+Version: 0.0.3
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calfcv-0.0.2/README.rst` & `calfcv-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.2/calfcv/calfcv.py` & `calfcv-0.0.3/calfcv/calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.2/calfcv/tests/test_calfcv.py` & `calfcv-0.0.3/calfcv/tests/test_calfcv.py`

 * *Files identical despite different names*

### Comparing `calfcv-0.0.2/calfcv.egg-info/PKG-INFO` & `calfcv-0.0.3/calfcv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calfcv
-Version: 0.0.2
+Version: 0.0.3
 Summary: Coarse approximation linear function with cross validation
 Home-page: 
 Download-URL: https://github.com/scikit-learn-contrib/project-template
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
```

### Comparing `calfcv-0.0.2/setup.py` & `calfcv-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 with codecs.open('README.rst', encoding='utf-8-sig') as f:
     LONG_DESCRIPTION = f.read()
 MAINTAINER = 'Carlson Research, LLC'
 MAINTAINER_EMAIL = 'hrolfrc@gmail.com'
 URL = ''
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/scikit-learn-contrib/project-template'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
                'Topic :: Scientific/Engineering',
                'Operating System :: OS Independent',
```

