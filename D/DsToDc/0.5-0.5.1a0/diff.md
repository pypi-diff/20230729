# Comparing `tmp/DsToDc-0.5.tar.gz` & `tmp/DsToDc-0.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DsToDc-0.5.tar", last modified: Sat Jul 29 11:44:55 2023, max compression
+gzip compressed data, was "DsToDc-0.5.1a0.tar", last modified: Sat Jul 29 12:03:46 2023, max compression
```

## Comparing `DsToDc-0.5.tar` & `DsToDc-0.5.1a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:44:55.216045 DsToDc-0.5/
-drwxrwxrwx   0        0        0        0 2023-07-29 11:44:55.214047 DsToDc-0.5/DsToDc.egg-info/
--rw-rw-rw-   0        0        0      492 2023-07-29 11:44:55.000000 DsToDc-0.5/DsToDc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-07-29 11:44:55.000000 DsToDc-0.5/DsToDc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:44:55.000000 DsToDc-0.5/DsToDc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:44:55.000000 DsToDc-0.5/DsToDc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      492 2023-07-29 11:44:55.216045 DsToDc-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-29 11:44:55.216045 DsToDc-0.5/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-07-29 11:43:31.000000 DsToDc-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:03:46.321160 DsToDc-0.5.1a0/
+drwxrwxrwx   0        0        0        0 2023-07-29 12:03:46.320161 DsToDc-0.5.1a0/DsToDc.egg-info/
+-rw-rw-rw-   0        0        0      496 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:03:46.000000 DsToDc-0.5.1a0/DsToDc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      496 2023-07-29 12:03:46.321160 DsToDc-0.5.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-29 12:03:46.322162 DsToDc-0.5.1a0/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-07-29 12:03:43.000000 DsToDc-0.5.1a0/setup.py
```

### Comparing `DsToDc-0.5/setup.py` & `DsToDc-0.5.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5'
+VERSION = '0.5.1a'
 DESCRIPTION = 'A package to convert from Data collections to Data Containers'
 LONG_DESCRIPTION = 'A package that assists in converting unstructured data collections into data containers'
 
 setup(
     name="DsToDc",
     version=VERSION,
     description=DESCRIPTION,
```

