# Comparing `tmp/newline-0.0.3.tar.gz` & `tmp/newline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newline-0.0.3.tar", last modified: Sat Jul 29 05:09:20 2023, max compression
+gzip compressed data, was "newline-0.0.4.tar", last modified: Sat Jul 29 05:12:01 2023, max compression
```

## Comparing `newline-0.0.3.tar` & `newline-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 05:09:20.758403 newline-0.0.3/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:09:20.757403 newline-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 05:09:20.749405 newline-0.0.3/newline/
--rw-rw-rw-   0        0        0      273 2023-07-29 04:39:53.000000 newline-0.0.3/newline/__init__.py
--rw-rw-rw-   0        0        0     2823 2023-07-29 05:05:28.000000 newline-0.0.3/newline/main.py
-drwxrwxrwx   0        0        0        0 2023-07-29 05:09:20.757403 newline-0.0.3/newline.egg-info/
--rw-rw-rw-   0        0        0      471 2023-07-29 05:09:20.000000 newline-0.0.3/newline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-29 05:09:20.000000 newline-0.0.3/newline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 05:09:20.000000 newline-0.0.3/newline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 05:09:20.000000 newline-0.0.3/newline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 05:09:20.758403 newline-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-07-29 05:09:16.000000 newline-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:12:01.025274 newline-0.0.4/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:12:01.025274 newline-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 05:12:01.016272 newline-0.0.4/newline/
+-rw-rw-rw-   0        0        0      246 2023-07-29 05:11:02.000000 newline-0.0.4/newline/__init__.py
+-rw-rw-rw-   0        0        0     2823 2023-07-29 05:05:28.000000 newline-0.0.4/newline/main.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:12:01.024309 newline-0.0.4/newline.egg-info/
+-rw-rw-rw-   0        0        0      471 2023-07-29 05:12:00.000000 newline-0.0.4/newline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-29 05:12:00.000000 newline-0.0.4/newline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:12:00.000000 newline-0.0.4/newline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 05:12:00.000000 newline-0.0.4/newline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:12:01.025274 newline-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-07-29 05:11:53.000000 newline-0.0.4/setup.py
```

### Comparing `newline-0.0.3/newline/main.py` & `newline-0.0.4/newline/main.py`

 * *Files identical despite different names*

### Comparing `newline-0.0.3/setup.py` & `newline-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 
 setuptools.setup(
     name="newline",
-    version="0.0.3",
+    version="0.0.4",
     author="Ayush Sharma",
     author_email="ayushsharma14@gmail.com",
     description="A small package to make it easy to store data in CSV format using python",
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-sharma-py/NewLine.git",
     packages=setuptools.find_packages(),
     classifiers=[
```

