# Comparing `tmp/flake8_private_name_import-0.1.5.tar.gz` & `tmp/flake8_private_name_import-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_private_name_import-0.1.5.tar", last modified: Thu Jul 27 21:19:20 2023, max compression
+gzip compressed data, was "dist/flake8_private_name_import-1.0.0.tar", last modified: Sat Jul 29 20:17:38 2023, max compression
```

## Comparing `flake8_private_name_import-0.1.5.tar` & `flake8_private_name_import-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      647 2023-07-27 21:08:22.000000 flake8_private_name_import-0.1.5/README.md
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/SOURCES.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/dependency_links.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       62 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/entry_points.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/not-zip-safe
--rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/requires.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.egg-info/top_level.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)     4235 2023-07-27 21:19:10.000000 flake8_private_name_import-0.1.5/flake8_private_name_import.py
--rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-27 21:19:20.000000 flake8_private_name_import-0.1.5/setup.cfg
--rw-rw-r--   0 rows      (1000) rows      (1000)     1778 2023-07-27 21:19:10.000000 flake8_private_name_import-0.1.5/setup.py
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     7031 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)     4518 2023-07-29 20:16:00.000000 flake8_private_name_import-1.0.0/README.md
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     7031 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       62 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/entry_points.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/not-zip-safe
+-rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/requires.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.egg-info/top_level.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)     9308 2023-07-29 20:09:38.000000 flake8_private_name_import-1.0.0/flake8_private_name_import.py
+-rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-29 20:17:38.000000 flake8_private_name_import-1.0.0/setup.cfg
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1749 2023-07-29 20:09:38.000000 flake8_private_name_import-1.0.0/setup.py
```

### Comparing `flake8_private_name_import-0.1.5/setup.py` & `flake8_private_name_import-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='flake8_private_name_import',
-    version='0.1.5',
+    version='1.0.0',
     description="flake8 plugin that reports imports of private names",
-    long_description="flake8 plugin that reports imports of private names",
+    long_description=open('README.md').read(),
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: Flake8',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
```

