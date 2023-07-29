# Comparing `tmp/newline-0.0.6.tar.gz` & `tmp/newline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newline-0.0.6.tar", last modified: Sat Jul 29 05:21:14 2023, max compression
+gzip compressed data, was "newline-0.0.7.tar", last modified: Sat Jul 29 05:22:53 2023, max compression
```

## Comparing `newline-0.0.6.tar` & `newline-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:21:14.910070 newline-0.0.6/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:21:14.910070 newline-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:21:14.900071 newline-0.0.6/newline/
--rw-rw-rw-   0        0        0      273 2023-07-29 05:20:49.000000 newline-0.0.6/newline/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-29 05:05:28.000000 newline-0.0.6/newline/newline1.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:21:14.909087 newline-0.0.6/newline.egg-info/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:21:14.000000 newline-0.0.6/newline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-07-29 05:21:14.000000 newline-0.0.6/newline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:21:14.000000 newline-0.0.6/newline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 05:21:14.000000 newline-0.0.6/newline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:21:14.911077 newline-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-07-29 05:21:05.000000 newline-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:22:53.642359 newline-0.0.7/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:22:53.641360 newline-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:22:53.634358 newline-0.0.7/newline/
+-rw-rw-rw-   0        0        0        0 2023-07-29 05:22:38.000000 newline-0.0.7/newline/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-07-29 05:05:28.000000 newline-0.0.7/newline/newline1.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:22:53.641360 newline-0.0.7/newline.egg-info/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:22:53.000000 newline-0.0.7/newline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-07-29 05:22:53.000000 newline-0.0.7/newline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:22:53.000000 newline-0.0.7/newline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 05:22:53.000000 newline-0.0.7/newline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:22:53.642359 newline-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-07-29 05:22:47.000000 newline-0.0.7/setup.py
```

### Comparing `newline-0.0.6/newline/newline1.py` & `newline-0.0.7/newline/newline1.py`

 * *Files identical despite different names*

### Comparing `newline-0.0.6/setup.py` & `newline-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 
 setuptools.setup(
     name="newline",
-    version="0.0.6",
+    version="0.0.7",
     author="Ayush Sharma",
     author_email="ayushsharma14@gmail.com",
     description="A small package to make it easy to store data in CSV format using python",
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-sharma-py/NewLine.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

