# Comparing `tmp/newline-0.0.9.tar.gz` & `tmp/newline-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newline-0.0.9.tar", last modified: Sat Jul 29 05:44:49 2023, max compression
+gzip compressed data, was "newline-0.1.0.tar", last modified: Sat Jul 29 05:47:20 2023, max compression
```

## Comparing `newline-0.0.9.tar` & `newline-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.579052 newline-0.0.9/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:44:49.578046 newline-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.568595 newline-0.0.9/newline/
--rw-rw-rw-   0        0        0     2823 2023-07-29 05:44:30.000000 newline-0.0.9/newline/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-29 05:26:04.000000 newline-0.0.9/newline/newline1.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:44:49.578046 newline-0.0.9/newline.egg-info/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 05:44:49.000000 newline-0.0.9/newline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:44:49.579052 newline-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-07-29 05:44:44.000000 newline-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:47:20.555647 newline-0.1.0/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:47:20.555647 newline-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:47:20.540639 newline-0.1.0/newline/
+-rw-rw-rw-   0        0        0     2823 2023-07-29 05:46:45.000000 newline-0.1.0/newline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:47:20.554644 newline-0.1.0/newline.egg-info/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:47:20.000000 newline-0.1.0/newline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-07-29 05:47:20.000000 newline-0.1.0/newline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:47:20.000000 newline-0.1.0/newline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 05:47:20.000000 newline-0.1.0/newline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:47:20.555647 newline-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-07-29 05:47:11.000000 newline-0.1.0/setup.py
```

### Comparing `newline-0.0.9/newline/__init__.py` & `newline-0.1.0/newline/__init__.py`

 * *Files identical despite different names*

### Comparing `newline-0.0.9/setup.py` & `newline-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 
 setuptools.setup(
     name="newline",
-    version="0.0.9",
+    version="0.1.0",
     author="Ayush Sharma",
     author_email="ayushsharma14@gmail.com",
     description="A small package to make it easy to store data in CSV format using python",
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-sharma-py/NewLine.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

