# Comparing `tmp/ptrack-0.1.0.tar.gz` & `tmp/ptrack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrack-0.1.0.tar", last modified: Sat Jul 29 05:45:02 2023, max compression
+gzip compressed data, was "ptrack-0.1.1.tar", last modified: Sat Jul 29 10:18:39 2023, max compression
```

## Comparing `ptrack-0.1.0.tar` & `ptrack-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:45:02.374263 ptrack-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-29 05:45:02.374263 ptrack-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-29 04:54:02.000000 ptrack-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:45:02.374263 ptrack-0.1.0/ptrack/
--rw-r--r--   0 root         (0) root         (0)      625 2023-07-29 04:54:02.000000 ptrack-0.1.0/ptrack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4561 2023-07-29 04:54:02.000000 ptrack-0.1.0/ptrack/main.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-07-29 04:54:02.000000 ptrack-0.1.0/ptrack/methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 05:45:02.374263 ptrack-0.1.0/ptrack.egg-info/
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-29 05:45:02.000000 ptrack-0.1.0/ptrack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 05:45:02.374263 ptrack-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-29 04:54:02.000000 ptrack-0.1.0/setup.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.1/LICENSE
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 10:18:39.059416 ptrack-0.1.1/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      356 2023-07-29 04:54:02.000000 ptrack-0.1.1/README.md
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/ptrack/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      625 2023-07-29 04:54:02.000000 ptrack-0.1.1/ptrack/__init__.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     4415 2023-07-29 10:16:43.000000 ptrack-0.1.1/ptrack/main.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2784 2023-07-29 10:16:14.000000 ptrack-0.1.1/ptrack/methods.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/ptrack.egg-info/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      260 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/SOURCES.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/dependency_links.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       90 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/entry_points.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       26 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/requires.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/top_level.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-07-29 10:18:39.059416 ptrack-0.1.1/setup.cfg
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      564 2023-07-29 10:18:10.000000 ptrack-0.1.1/setup.py
```

### Comparing `ptrack-0.1.0/LICENSE` & `ptrack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.0/ptrack/__init__.py` & `ptrack-0.1.1/ptrack/__init__.py`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.0/ptrack/main.py` & `ptrack-0.1.1/ptrack/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 import ptrack
-from ptrack.methods import format_file_size, regular_copy, verbose_copy, hlp
+from ptrack.methods import format_file_size, regular_copy, verbose_copy, hlp, getTotalSize
 from rich.progress import Progress, BarColumn, TextColumn, TimeRemainingColumn, FileSizeColumn
 from rich.console import Console
 import shutil
 
 verbose = ptrack.verbose
 argCopy = ptrack.copy
 argMove = ptrack.move
@@ -35,15 +35,16 @@
         dst_dir = dst
         new_name = None
     else:
         dst_dir = os.path.dirname(dst)
         new_name = os.path.basename(dst)
 
     total_files = sum(len(files) for path in srcPaths for r, d, files in os.walk(path) if os.path.isdir(path)) + sum(1 for path in srcPaths if os.path.isfile(path))
-    total_size = sum(os.path.getsize(os.path.join(r, f)) for path in srcPaths for r, d, files in os.walk(path) for f in files) + sum(os.path.getsize(path) for path in srcPaths if os.path.isfile(path))
+    total_size = getTotalSize(srcPaths)
+
     current_file = 1
 
     if total_files > 1:
         console.print(f"\n[#ea2a6f]{process}:[/#ea2a6f] [bold cyan]{total_files} files[/bold cyan]\n")
     else:
         for src_path in srcPaths:
             if os.path.isfile(src_path):
```

### Comparing `ptrack-0.1.0/setup.py` & `ptrack-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptrack',
-    version='0.1.0',
+    version='0.1.1',
     description='A simple CLI utility for asthetically tracking progress when copying or moving files.',
     author='Connor Etherington',
     author_email='connor@concise.cc',
     packages=find_packages(),
     install_requires=[
         'rich',
         'argparse',
```

