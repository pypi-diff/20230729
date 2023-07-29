# Comparing `tmp/ptrack-0.1.3.tar.gz` & `tmp/ptrack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrack-0.1.3.tar", last modified: Sat Jul 29 11:51:42 2023, max compression
+gzip compressed data, was "ptrack-0.1.4.tar", last modified: Sat Jul 29 17:05:25 2023, max compression
```

## Comparing `ptrack-0.1.3.tar` & `ptrack-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:51:42.856099 ptrack-0.1.3/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.3/LICENSE
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 11:51:42.856099 ptrack-0.1.3/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      356 2023-07-29 04:54:02.000000 ptrack-0.1.3/README.md
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:51:42.856099 ptrack-0.1.3/ptrack/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      714 2023-07-29 11:51:24.000000 ptrack-0.1.3/ptrack/__init__.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     5295 2023-07-29 11:11:33.000000 ptrack-0.1.3/ptrack/main.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     3057 2023-07-29 11:22:37.000000 ptrack-0.1.3/ptrack/methods.py
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:51:42.856099 ptrack-0.1.3/ptrack.egg-info/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      260 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/SOURCES.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/dependency_links.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       90 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/entry_points.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       26 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/requires.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-07-29 11:51:42.000000 ptrack-0.1.3/ptrack.egg-info/top_level.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-07-29 11:51:42.856099 ptrack-0.1.3/setup.cfg
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      564 2023-07-29 11:51:37.000000 ptrack-0.1.3/setup.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 17:05:25.065183 ptrack-0.1.4/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.4/LICENSE
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 17:05:25.065183 ptrack-0.1.4/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      356 2023-07-29 04:54:02.000000 ptrack-0.1.4/README.md
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 17:05:25.065183 ptrack-0.1.4/ptrack/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      728 2023-07-29 17:03:57.000000 ptrack-0.1.4/ptrack/__init__.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     5295 2023-07-29 11:11:33.000000 ptrack-0.1.4/ptrack/main.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     3057 2023-07-29 11:22:37.000000 ptrack-0.1.4/ptrack/methods.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 17:05:25.065183 ptrack-0.1.4/ptrack.egg-info/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      260 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/SOURCES.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/dependency_links.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       90 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/entry_points.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       26 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/requires.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-07-29 17:05:25.000000 ptrack-0.1.4/ptrack.egg-info/top_level.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-07-29 17:05:25.065183 ptrack-0.1.4/setup.cfg
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      564 2023-07-29 17:05:20.000000 ptrack-0.1.4/setup.py
```

### Comparing `ptrack-0.1.3/LICENSE` & `ptrack-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.3/ptrack/__init__.py` & `ptrack-0.1.4/ptrack/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import argcomplete
-version="0.1.3"
+version="0.1.4"
 
 parser = argparse.ArgumentParser(description='A simple CLI utility for asthetically tracking progress when copying or moving files.')
 parser.add_argument('-v', '--verbose', action='store_true', help='verbose output')
 parser.add_argument('-c', '--copy', action='store_true', help='copy files (You can use `ptc` instead of `ptrack -c`)')
 parser.add_argument('-m', '--move', action='store_true', help='move files (You can use `ptm` instead of `ptrack -m`)')
-parser.add_argument('-V', '--version', action='version', version="0.1.3"
+parser.add_argument('-V', '--version', action='version', version='%(prog)s' + version)
 
 argcomplete.autocomplete(parser)
 args, unknown = parser.parse_known_args()
 
 verbose = args.verbose
 copy = args.copy
 move = args.move
```

### Comparing `ptrack-0.1.3/ptrack/main.py` & `ptrack-0.1.4/ptrack/main.py`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.3/ptrack/methods.py` & `ptrack-0.1.4/ptrack/methods.py`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.3/setup.py` & `ptrack-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptrack',
-    version="0.1.3",
+    version="0.1.4",
     description='A simple CLI utility for asthetically tracking progress when copying or moving files.',
     author='Connor Etherington',
     author_email='connor@concise.cc',
     packages=find_packages(),
     install_requires=[
         'rich',
         'argparse',
```

