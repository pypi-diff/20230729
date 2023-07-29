# Comparing `tmp/newline-0.0.1.tar.gz` & `tmp/newline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\newline-0.0.1.tar", last modified: Sun Sep 20 08:00:57 2020, max compression
+gzip compressed data, was "newline-0.0.2.tar", last modified: Sat Jul 29 04:49:18 2023, max compression
```

## Comparing `newline-0.0.1.tar` & `newline-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2020-09-20 08:00:57.000000 newline-0.0.1/
--rw-rw-rw-   0        0        0     1136 2020-09-20 08:00:57.000000 newline-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      532 2020-09-18 20:03:31.000000 newline-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2020-09-20 08:00:57.000000 newline-0.0.1/example_pkg/
--rw-rw-rw-   0        0        0        0 2020-09-19 07:04:59.000000 newline-0.0.1/example_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2020-09-20 08:00:57.000000 newline-0.0.1/newline.egg-info/
--rw-rw-rw-   0        0        0     1136 2020-09-20 08:00:53.000000 newline-0.0.1/newline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2020-09-20 08:00:54.000000 newline-0.0.1/newline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-20 08:00:53.000000 newline-0.0.1/newline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2020-09-20 08:00:53.000000 newline-0.0.1/newline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-09-20 08:00:57.000000 newline-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      718 2020-09-20 07:59:22.000000 newline-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:49:18.260192 newline-0.0.2/
+-rw-rw-rw-   0        0        0      471 2023-07-29 04:49:18.259193 newline-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 04:49:18.246188 newline-0.0.2/newline/
+-rw-rw-rw-   0        0        0      273 2023-07-29 04:39:53.000000 newline-0.0.2/newline/__init__.py
+-rw-rw-rw-   0        0        0     2827 2023-07-29 04:14:18.000000 newline-0.0.2/newline/newline.py
+drwxrwxrwx   0        0        0        0 2023-07-29 04:49:18.259193 newline-0.0.2/newline.egg-info/
+-rw-rw-rw-   0        0        0      471 2023-07-29 04:49:18.000000 newline-0.0.2/newline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-07-29 04:49:18.000000 newline-0.0.2/newline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 04:49:18.000000 newline-0.0.2/newline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-29 04:49:18.000000 newline-0.0.2/newline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 04:49:18.260192 newline-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-07-29 04:49:14.000000 newline-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `newline-0.0.1/setup.py` & `newline-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
+import os
 
 setuptools.setup(
     name="newline",
-    version="0.0.1",
+    version="0.0.2",
     author="Ayush Sharma",
     author_email="ayushsharma14@gmail.com",
     description="A small package to make it easy to store data in CSV format using python",
-    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-sharma-py/NewLine.git",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

