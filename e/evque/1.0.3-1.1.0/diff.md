# Comparing `tmp/evque-1.0.3.tar.gz` & `tmp/evque-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evque-1.0.3.tar", last modified: Fri Jul 28 13:32:41 2023, max compression
+gzip compressed data, was "evque-1.1.0.tar", last modified: Fri Jul 28 23:54:12 2023, max compression
```

## Comparing `evque-1.0.3.tar` & `evque-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:32:41.772433 evque-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-28 13:32:31.000000 evque-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-28 13:32:41.772433 evque-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-28 13:32:31.000000 evque-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:32:41.772433 evque-1.0.3/evque/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-28 13:32:31.000000 evque-1.0.3/evque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-28 13:32:31.000000 evque-1.0.3/evque/evque.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:32:41.772433 evque-1.0.3/evque.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-28 13:32:41.000000 evque-1.0.3/evque.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 13:32:41.000000 evque-1.0.3/evque.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:32:41.000000 evque-1.0.3/evque.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 13:32:41.000000 evque-1.0.3/evque.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:32:41.772433 evque-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 13:32:31.000000 evque-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:54:12.885188 evque-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-28 23:54:02.000000 evque-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-28 23:54:12.885188 evque-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-28 23:54:02.000000 evque-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:54:12.881188 evque-1.1.0/evque/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-28 23:54:02.000000 evque-1.1.0/evque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-28 23:54:02.000000 evque-1.1.0/evque/evque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:54:12.885188 evque-1.1.0/evque.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-28 23:54:12.000000 evque-1.1.0/evque.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-28 23:54:12.000000 evque-1.1.0/evque.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:54:12.000000 evque-1.1.0/evque.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 23:54:12.000000 evque-1.1.0/evque.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:54:12.885188 evque-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 23:54:02.000000 evque-1.1.0/setup.py
```

### Comparing `evque-1.0.3/LICENSE.txt` & `evque-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evque-1.0.3/setup.py` & `evque-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='evque',
-    version='1.0.3',
+    version='1.1.0',
     description='A simple event queue library with support for topics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Ahmad Siavashi',
     author_email='siavashi@aut.ac.ir',
     packages=find_packages(),
     install_requires=[],
```

