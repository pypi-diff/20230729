# Comparing `tmp/newline-0.0.8.tar.gz` & `tmp/newline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newline-0.0.8.tar", last modified: Sat Jul 29 05:26:14 2023, max compression
+gzip compressed data, was "newline-0.0.9.tar", last modified: Sat Jul 29 05:44:49 2023, max compression
```

## Comparing `newline-0.0.8.tar` & `newline-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:26:14.470800 newline-0.0.8/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:26:14.469346 newline-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:26:14.460344 newline-0.0.8/newline/
--rw-rw-rw-   0        0        0        0 2023-07-29 05:22:38.000000 newline-0.0.8/newline/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-29 05:26:04.000000 newline-0.0.8/newline/newline.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:26:14.469346 newline-0.0.8/newline.egg-info/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:26:14.000000 newline-0.0.8/newline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-07-29 05:26:14.000000 newline-0.0.8/newline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:26:14.000000 newline-0.0.8/newline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 05:26:14.000000 newline-0.0.8/newline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:26:14.470800 newline-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-07-29 05:26:10.000000 newline-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.579052 newline-0.0.9/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:44:49.578046 newline-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.568595 newline-0.0.9/newline/
+-rw-rw-rw-   0        0        0     2823 2023-07-29 05:44:30.000000 newline-0.0.9/newline/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-07-29 05:26:04.000000 newline-0.0.9/newline/newline1.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.578046 newline-0.0.9/newline.egg-info/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:44:49.579052 newline-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-07-29 05:44:44.000000 newline-0.0.9/setup.py
```

### Comparing `newline-0.0.8/newline/newline.py` & `newline-0.0.9/newline/__init__.py`

 * *Files identical despite different names*

### Comparing `newline-0.0.8/setup.py` & `newline-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 
 setuptools.setup(
     name="newline",
-    version="0.0.8",
+    version="0.0.9",
     author="Ayush Sharma",
     author_email="ayushsharma14@gmail.com",
     description="A small package to make it easy to store data in CSV format using python",
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-sharma-py/NewLine.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

