# Comparing `tmp/lighthouse_python_plus-1.1.0.tar.gz` & `tmp/lighthouse_python_plus-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighthouse_python_plus-1.1.0.tar", last modified: Sat Jul 29 07:26:14 2023, max compression
+gzip compressed data, was "lighthouse_python_plus-1.2.0.tar", last modified: Sat Jul 29 13:26:40 2023, max compression
```

## Comparing `lighthouse_python_plus-1.1.0.tar` & `lighthouse_python_plus-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 07:26:14.536842 lighthouse_python_plus-1.1.0/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1069 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/LICENSE
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2032 2023-07-29 07:26:14.536842 lighthouse_python_plus-1.1.0/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1642 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 07:26:14.532842 lighthouse_python_plus-1.1.0/lighthouse/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       92 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/lighthouse/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      988 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/lighthouse/batch.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2940 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/lighthouse/report.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     3430 2023-07-29 07:12:03.000000 lighthouse_python_plus-1.1.0/lighthouse/runner.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 07:26:14.536842 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     2032 2023-07-29 07:26:14.000000 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      340 2023-07-29 07:26:14.000000 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-29 07:26:14.000000 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       11 2023-07-29 07:26:14.000000 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/requires.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       11 2023-07-29 07:26:14.000000 lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-29 07:26:14.536842 lighthouse_python_plus-1.1.0/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      736 2023-07-29 07:22:45.000000 lighthouse_python_plus-1.1.0/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 13:26:40.514106 lighthouse_python_plus-1.2.0/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1087 2023-07-29 13:12:54.000000 lighthouse_python_plus-1.2.0/LICENSE
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2087 2023-07-29 13:26:40.514106 lighthouse_python_plus-1.2.0/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1697 2023-07-29 13:20:07.000000 lighthouse_python_plus-1.2.0/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 13:26:40.510106 lighthouse_python_plus-1.2.0/lighthouse/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       74 2023-07-29 12:59:37.000000 lighthouse_python_plus-1.2.0/lighthouse/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     3521 2023-07-29 13:03:51.000000 lighthouse_python_plus-1.2.0/lighthouse/report.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)    12695 2023-07-29 13:04:13.000000 lighthouse_python_plus-1.2.0/lighthouse/runner.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-29 13:26:40.514106 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2087 2023-07-29 13:26:40.000000 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      320 2023-07-29 13:26:40.000000 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-29 13:26:40.000000 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       11 2023-07-29 13:26:40.000000 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/requires.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       11 2023-07-29 13:26:40.000000 lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-29 13:26:40.514106 lighthouse_python_plus-1.2.0/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      736 2023-07-29 13:21:37.000000 lighthouse_python_plus-1.2.0/setup.py
```

### Comparing `lighthouse_python_plus-1.1.0/LICENSE` & `lighthouse_python_plus-1.2.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Adam Cupiał
+Copyright (c) 2023 Adam Cupiał & alireza sharifi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lighthouse_python_plus-1.1.0/PKG-INFO` & `lighthouse_python_plus-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: lighthouse_python_plus
-Version: 1.1.0
-Summary: Lighthouse runner is a Python package that wraps the Lighthouse tool for easy integration into Python projects.
-Author: alireza sharifi
-Author-email: sharifialireza276@gmail.com
-Project-URL: Github, https://github.com/sh-alireza/lighthouse-python-plus
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Lighthouse runner for python
 
 ## About This Repository
 This repository is based on the original work of [Adam Cupiał](https://github.com/adamcupial) and was forked from his [lighthouse-python](https://github.com/adamcupial/lighthouse-python) repository. While the original repository had not been updated in five years, I found it to be a valuable resource and decided to update it (I have made some changes, fixed some bugs) and turn it into a package for PyPI. I want to acknowledge the original author for creating the foundation of this project and making it available to the community.
 
 
 ## Description
@@ -28,17 +18,21 @@
 ```
 
 ## Usage
 
 ```python
 from lighthouse import LighthouseRunner
 
-report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False).report
+TIMINGS = [
+    'speed-index'
+]
+
+report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False, timings=TIMINGS).report
 assert report.score['performance'] > 0.5
-print(report.audits['performance'].failed)
+print(report.audits(0.5)['performance'].failed)
 ```
 
 report has 3 properties:
 
 - score: returns dict where keys are categories and values are scores (0 to 1)
 - timings: returns dict where keys are timings and values are timedelta objects
 - audits: dict where keys are categories and values are objects with passed and failed lists attached
```

### Comparing `lighthouse_python_plus-1.1.0/README.md` & `lighthouse_python_plus-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: lighthouse_python_plus
+Version: 1.2.0
+Summary: Lighthouse runner is a Python package that wraps the Lighthouse tool for easy integration into Python projects.
+Author: alireza sharifi
+Author-email: sharifialireza276@gmail.com
+Project-URL: Github, https://github.com/sh-alireza/lighthouse-python-plus
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Lighthouse runner for python
 
 ## About This Repository
 This repository is based on the original work of [Adam Cupiał](https://github.com/adamcupial) and was forked from his [lighthouse-python](https://github.com/adamcupial/lighthouse-python) repository. While the original repository had not been updated in five years, I found it to be a valuable resource and decided to update it (I have made some changes, fixed some bugs) and turn it into a package for PyPI. I want to acknowledge the original author for creating the foundation of this project and making it available to the community.
 
 
 ## Description
@@ -18,17 +28,21 @@
 ```
 
 ## Usage
 
 ```python
 from lighthouse import LighthouseRunner
 
-report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False).report
+TIMINGS = [
+    'speed-index'
+]
+
+report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False, timings=TIMINGS).report
 assert report.score['performance'] > 0.5
-print(report.audits['performance'].failed)
+print(report.audits(0.5)['performance'].failed)
 ```
 
 report has 3 properties:
 
 - score: returns dict where keys are categories and values are scores (0 to 1)
 - timings: returns dict where keys are timings and values are timedelta objects
 - audits: dict where keys are categories and values are objects with passed and failed lists attached
```

### Comparing `lighthouse_python_plus-1.1.0/lighthouse_python_plus.egg-info/PKG-INFO` & `lighthouse_python_plus-1.2.0/lighthouse_python_plus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighthouse-python-plus
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lighthouse runner is a Python package that wraps the Lighthouse tool for easy integration into Python projects.
 Author: alireza sharifi
 Author-email: sharifialireza276@gmail.com
 Project-URL: Github, https://github.com/sh-alireza/lighthouse-python-plus
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -28,17 +28,21 @@
 ```
 
 ## Usage
 
 ```python
 from lighthouse import LighthouseRunner
 
-report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False).report
+TIMINGS = [
+    'speed-index'
+]
+
+report = LighthouseRunner('https://github.com/adamcupial', form_factor='desktop', quiet=False, timings=TIMINGS).report
 assert report.score['performance'] > 0.5
-print(report.audits['performance'].failed)
+print(report.audits(0.5)['performance'].failed)
 ```
 
 report has 3 properties:
 
 - score: returns dict where keys are categories and values are scores (0 to 1)
 - timings: returns dict where keys are timings and values are timedelta objects
 - audits: dict where keys are categories and values are objects with passed and failed lists attached
```

### Comparing `lighthouse_python_plus-1.1.0/setup.py` & `lighthouse_python_plus-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 project_urls = {
   'Github': 'https://github.com/sh-alireza/lighthouse-python-plus',
 }
 
 setup(
     name='lighthouse_python_plus',
-    version='1.1.0',
+    version='1.2.0',
     description='Lighthouse runner is a Python package that wraps the Lighthouse tool for easy integration into Python projects.',
     author='alireza sharifi',
     author_email='sharifialireza276@gmail.com',
     project_urls=project_urls,
     packages=find_packages(),
     install_requires=[
         'tqdm>=4.30',
```

