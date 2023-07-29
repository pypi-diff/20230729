# Comparing `tmp/logg3r-1.0.tar.gz` & `tmp/logg3r-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logg3r-1.0.tar", last modified: Sat Oct 24 18:49:07 2020, max compression
+gzip compressed data, was "logg3r-2.0.tar", last modified: Sat Jul 29 03:24:27 2023, max compression
```

## Comparing `logg3r-1.0.tar` & `logg3r-2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxr-x   0 gage      (1000) gage      (1000)        0 2020-10-24 18:49:07.559049 logg3r-1.0/
--rw-rw-r--   0 gage      (1000) gage      (1000)     2402 2020-10-24 18:49:07.559049 logg3r-1.0/PKG-INFO
--rw-rw-r--   0 gage      (1000) gage      (1000)     1624 2020-10-24 18:40:51.000000 logg3r-1.0/README.md
-drwxrwxr-x   0 gage      (1000) gage      (1000)        0 2020-10-24 18:49:07.559049 logg3r-1.0/logg3r.egg-info/
--rw-rw-r--   0 gage      (1000) gage      (1000)     2402 2020-10-24 18:49:07.000000 logg3r-1.0/logg3r.egg-info/PKG-INFO
--rw-rw-r--   0 gage      (1000) gage      (1000)      148 2020-10-24 18:49:07.000000 logg3r-1.0/logg3r.egg-info/SOURCES.txt
--rw-rw-r--   0 gage      (1000) gage      (1000)        1 2020-10-24 18:49:07.000000 logg3r-1.0/logg3r.egg-info/dependency_links.txt
--rw-rw-r--   0 gage      (1000) gage      (1000)        1 2020-10-24 18:49:07.000000 logg3r-1.0/logg3r.egg-info/top_level.txt
--rw-rw-r--   0 gage      (1000) gage      (1000)     5972 2020-10-24 18:41:04.000000 logg3r-1.0/logg3r.py
--rw-rw-r--   0 gage      (1000) gage      (1000)       38 2020-10-24 18:49:07.559049 logg3r-1.0/setup.cfg
--rw-rw-r--   0 gage      (1000) gage      (1000)      647 2020-10-24 18:46:52.000000 logg3r-1.0/setup.py
+drwxr-xr-x   0 gage      (1000) gage      (1000)        0 2023-07-29 03:24:27.171122 logg3r-2.0/
+-rw-r--r--   0 gage      (1000) gage      (1000)     1065 2023-07-29 03:04:34.000000 logg3r-2.0/LICENSE
+-rw-r--r--   0 gage      (1000) gage      (1000)      160 2023-07-29 03:21:57.000000 logg3r-2.0/MANIFEST.in
+-rw-r--r--   0 gage      (1000) gage      (1000)     5664 2023-07-29 03:24:27.171122 logg3r-2.0/PKG-INFO
+-rw-r--r--   0 gage      (1000) gage      (1000)     4158 2023-07-29 03:20:01.000000 logg3r-2.0/README.md
+drwxr-xr-x   0 gage      (1000) gage      (1000)        0 2023-07-29 03:24:27.170122 logg3r-2.0/logg3r.egg-info/
+-rw-r--r--   0 gage      (1000) gage      (1000)     5664 2023-07-29 03:24:27.000000 logg3r-2.0/logg3r.egg-info/PKG-INFO
+-rw-r--r--   0 gage      (1000) gage      (1000)      168 2023-07-29 03:24:27.000000 logg3r-2.0/logg3r.egg-info/SOURCES.txt
+-rw-r--r--   0 gage      (1000) gage      (1000)        1 2023-07-29 03:24:27.000000 logg3r-2.0/logg3r.egg-info/dependency_links.txt
+-rw-r--r--   0 gage      (1000) gage      (1000)        1 2023-07-29 03:24:27.000000 logg3r-2.0/logg3r.egg-info/top_level.txt
+-rw-r--r--   0 gage      (1000) gage      (1000)     5987 2023-07-29 02:10:51.000000 logg3r-2.0/logg3r.py
+-rw-r--r--   0 gage      (1000) gage      (1000)       38 2023-07-29 03:24:27.171122 logg3r-2.0/setup.cfg
+-rw-r--r--   0 gage      (1000) gage      (1000)      624 2023-07-29 03:20:47.000000 logg3r-2.0/setup.py
```

### Comparing `logg3r-1.0/setup.py` & `logg3r-2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("./README.md","r")as f:
     long_description = f.read()
 
 setup(name='logg3r',
-        version=open("./version","r").read(),
+        version="2.0",
         description='Simple python log helper',
         author='Gage Helton',
         author_email='gagehelton@gmail.com',
         url='https://github.com/mghelton/logg3r',
         packages=['.'],
         classifiers=[
             "Programming Language :: Python :: 3",
```

