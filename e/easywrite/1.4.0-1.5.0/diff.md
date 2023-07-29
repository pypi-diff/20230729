# Comparing `tmp/easywrite-1.4.0.tar.gz` & `tmp/easywrite-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easywrite-1.4.0.tar", last modified: Sat Jul 29 01:49:22 2023, max compression
+gzip compressed data, was "easywrite-1.5.0.tar", last modified: Sat Jul 29 02:09:17 2023, max compression
```

## Comparing `easywrite-1.4.0.tar` & `easywrite-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 01:49:22.260000 easywrite-1.4.0/
--rw-rw-rw-   0        0        0      430 2023-07-29 01:49:24.000000 easywrite-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-28 14:48:58.000000 easywrite-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 01:49:22.290000 easywrite-1.4.0/easywrite.egg-info/
--rw-rw-rw-   0        0        0      430 2023-07-29 01:49:24.000000 easywrite-1.4.0/easywrite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-29 01:49:24.000000 easywrite-1.4.0/easywrite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 01:49:24.000000 easywrite-1.4.0/easywrite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 01:49:24.000000 easywrite-1.4.0/easywrite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      598 2023-07-29 01:48:48.000000 easywrite-1.4.0/easywrite.py
--rw-rw-rw-   0        0        0       42 2023-07-29 01:49:24.000000 easywrite-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-29 01:49:10.000000 easywrite-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:09:17.560000 easywrite-1.5.0/
+-rw-rw-rw-   0        0        0      430 2023-07-29 02:09:18.000000 easywrite-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-28 14:48:58.000000 easywrite-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-29 02:09:17.600000 easywrite-1.5.0/easywrite.egg-info/
+-rw-rw-rw-   0        0        0      430 2023-07-29 02:09:18.000000 easywrite-1.5.0/easywrite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-29 02:09:18.000000 easywrite-1.5.0/easywrite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 02:09:18.000000 easywrite-1.5.0/easywrite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 02:09:18.000000 easywrite-1.5.0/easywrite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      480 2023-07-29 02:03:34.000000 easywrite-1.5.0/easywrite.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 02:09:18.000000 easywrite-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-29 02:08:54.000000 easywrite-1.5.0/setup.py
```

### Comparing `easywrite-1.4.0/setup.py` & `easywrite-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='easywrite',
-    version='1.4.0',
+    version='1.5.0',
     author='skxllhead',
     description='A Python module for easy text output with colors',
     long_description='Put a more detailed description of your module here',
     long_description_content_type='text/markdown',
     url='https://github.com/skxllhead/easywrite',
     py_modules=['easywrite'],
     classifiers=[
```

