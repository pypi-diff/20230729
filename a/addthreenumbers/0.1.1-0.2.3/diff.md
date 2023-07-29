# Comparing `tmp/addthreenumbers-0.1.1.tar.gz` & `tmp/addthreenumbers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addthreenumbers-0.1.1.tar", last modified: Sat Jul 29 11:42:34 2023, max compression
+gzip compressed data, was "addthreenumbers-0.2.3.tar", last modified: Sat Jul 29 11:51:24 2023, max compression
```

## Comparing `addthreenumbers-0.1.1.tar` & `addthreenumbers-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.769565 addthreenumbers-0.1.1/
--rw-rw-rw-   0        0        0      508 2023-07-29 11:42:34.768564 addthreenumbers-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.754562 addthreenumbers-0.1.1/addthreenumbers/
--rw-rw-rw-   0        0        0       87 2023-07-29 08:09:26.000000 addthreenumbers-0.1.1/addthreenumbers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:42:34.766565 addthreenumbers-0.1.1/addthreenumbers.egg-info/
--rw-rw-rw-   0        0        0      508 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-29 11:42:34.000000 addthreenumbers-0.1.1/addthreenumbers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:42:34.769565 addthreenumbers-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-07-29 08:09:16.000000 addthreenumbers-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:24.054778 addthreenumbers-0.2.3/
+-rw-rw-rw-   0        0        0      508 2023-07-29 11:51:24.053779 addthreenumbers-0.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:24.042776 addthreenumbers-0.2.3/addthreenumbers/
+-rw-rw-rw-   0        0        0      133 2023-07-29 11:45:58.000000 addthreenumbers-0.2.3/addthreenumbers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 11:51:24.051777 addthreenumbers-0.2.3/addthreenumbers.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-07-29 11:51:23.000000 addthreenumbers-0.2.3/addthreenumbers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-29 11:51:23.000000 addthreenumbers-0.2.3/addthreenumbers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 11:51:23.000000 addthreenumbers-0.2.3/addthreenumbers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-29 11:51:23.000000 addthreenumbers-0.2.3/addthreenumbers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 11:51:24.055778 addthreenumbers-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      628 2023-07-29 11:50:13.000000 addthreenumbers-0.2.3/setup.py
```

### Comparing `addthreenumbers-0.1.1/setup.py` & `addthreenumbers-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='addthreenumbers',
-    version='0.1.1',
+    version='0.2.3',
     description='A simple library to add three numbers',
     author='Your Name',
     author_email='your@email.com',
     packages=find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
```

