# Comparing `tmp/addthreenumbers-0.1.0.tar.gz` & `tmp/addthreenumbers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addthreenumbers-0.1.0.tar", last modified: Sat Jul 29 08:08:38 2023, max compression
+gzip compressed data, was "addthreenumbers-0.1.1.tar", last modified: Sat Jul 29 11:42:34 2023, max compression
```

## Comparing `addthreenumbers-0.1.0.tar` & `addthreenumbers-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 08:08:38.954270 addthreenumbers-0.1.0/
--rw-rw-rw-   0        0        0      508 2023-07-29 08:08:38.953264 addthreenumbers-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 08:08:38.922620 addthreenumbers-0.1.0/addthreenumbers/
--rw-rw-rw-   0        0        0       39 2023-07-29 08:03:08.000000 addthreenumbers-0.1.0/addthreenumbers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 08:08:38.951085 addthreenumbers-0.1.0/addthreenumbers.egg-info/
--rw-rw-rw-   0        0        0      508 2023-07-29 08:08:38.000000 addthreenumbers-0.1.0/addthreenumbers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-29 08:08:38.000000 addthreenumbers-0.1.0/addthreenumbers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 08:08:38.000000 addthreenumbers-0.1.0/addthreenumbers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-29 08:08:38.000000 addthreenumbers-0.1.0/addthreenumbers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 08:08:38.954270 addthreenumbers-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-07-29 08:03:48.000000 addthreenumbers-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.769565 addthreenumbers-0.1.1/
+-rw-rw-rw-   0        0        0      508 2023-07-29 11:42:34.768564 addthreenumbers-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.754562 addthreenumbers-0.1.1/addthreenumbers/
+-rw-rw-rw-   0        0        0       87 2023-07-29 08:09:26.000000 addthreenumbers-0.1.1/addthreenumbers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.766565 addthreenumbers-0.1.1/addthreenumbers.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:42:34.769565 addthreenumbers-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-07-29 08:09:16.000000 addthreenumbers-0.1.1/setup.py
```

### Comparing `addthreenumbers-0.1.0/setup.py` & `addthreenumbers-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='addthreenumbers',
-    version='0.1.0',
+    version='0.1.1',
     description='A simple library to add three numbers',
     author='Your Name',
     author_email='your@email.com',
     packages=find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

