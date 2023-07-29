# Comparing `tmp/ptrack-0.1.1.tar.gz` & `tmp/ptrack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrack-0.1.1.tar", last modified: Sat Jul 29 10:18:39 2023, max compression
+gzip compressed data, was "ptrack-0.1.2.tar", last modified: Sat Jul 29 11:14:03 2023, max compression
```

## Comparing `ptrack-0.1.1.tar` & `ptrack-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.1/LICENSE
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 10:18:39.059416 ptrack-0.1.1/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      356 2023-07-29 04:54:02.000000 ptrack-0.1.1/README.md
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/ptrack/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      625 2023-07-29 04:54:02.000000 ptrack-0.1.1/ptrack/__init__.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     4415 2023-07-29 10:16:43.000000 ptrack-0.1.1/ptrack/main.py
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)     2784 2023-07-29 10:16:14.000000 ptrack-0.1.1/ptrack/methods.py
-drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 10:18:39.059416 ptrack-0.1.1/ptrack.egg-info/
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/PKG-INFO
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      260 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/SOURCES.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/dependency_links.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       90 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/entry_points.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       26 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/requires.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-07-29 10:18:39.000000 ptrack-0.1.1/ptrack.egg-info/top_level.txt
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-07-29 10:18:39.059416 ptrack-0.1.1/setup.cfg
--rw-r--r--   0 nvx1      (1000) nvx1      (1000)      564 2023-07-29 10:18:10.000000 ptrack-0.1.1/setup.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:14:03.284509 ptrack-0.1.2/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     1191 2023-07-29 04:54:02.000000 ptrack-0.1.2/LICENSE
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 11:14:03.284509 ptrack-0.1.2/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      356 2023-07-29 04:54:02.000000 ptrack-0.1.2/README.md
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:14:03.284509 ptrack-0.1.2/ptrack/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      731 2023-07-29 11:13:04.000000 ptrack-0.1.2/ptrack/__init__.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     5295 2023-07-29 11:11:33.000000 ptrack-0.1.2/ptrack/main.py
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)     3045 2023-07-29 11:09:47.000000 ptrack-0.1.2/ptrack/methods.py
+drwxr-xr-x   0 nvx1      (1000) nvx1      (1000)        0 2023-07-29 11:14:03.284509 ptrack-0.1.2/ptrack.egg-info/
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      226 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/PKG-INFO
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      260 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/SOURCES.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        1 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/dependency_links.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       90 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/entry_points.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       26 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/requires.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)        7 2023-07-29 11:14:03.000000 ptrack-0.1.2/ptrack.egg-info/top_level.txt
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)       38 2023-07-29 11:14:03.284509 ptrack-0.1.2/setup.cfg
+-rw-r--r--   0 nvx1      (1000) nvx1      (1000)      564 2023-07-29 11:13:11.000000 ptrack-0.1.2/setup.py
```

### Comparing `ptrack-0.1.1/LICENSE` & `ptrack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptrack-0.1.1/ptrack/__init__.py` & `ptrack-0.1.2/ptrack/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 import argcomplete
+version = '0.1.2'
 
 parser = argparse.ArgumentParser(description='A simple CLI utility for asthetically tracking progress when copying or moving files.')
 parser.add_argument('-v', '--verbose', action='store_true', help='verbose output')
 parser.add_argument('-c', '--copy', action='store_true', help='copy files (You can use `ptc` instead of `ptrack -c`)')
 parser.add_argument('-m', '--move', action='store_true', help='move files (You can use `ptm` instead of `ptrack -m`)')
+parser.add_argument('-V', '--version', action='version', version='%(prog)s ' + version)
 
 argcomplete.autocomplete(parser)
 args, unknown = parser.parse_known_args()
 
 verbose = args.verbose
 copy = args.copy
 move = args.move
```

### Comparing `ptrack-0.1.1/ptrack/methods.py` & `ptrack-0.1.2/ptrack/methods.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 import os
 from rich.progress import Progress, BarColumn, TextColumn, TimeRemainingColumn, FileSizeColumn
 
 
-def format_file_size(file_size):
-    if file_size >= 1024 ** 5:  # Petabyte
-        return f"{file_size / (1024 ** 5):.2f} PB"
-    elif file_size >= 1024 ** 4:  # Terabyte
-        return f"{file_size / (1024 ** 4):.2f} TB"
-    elif file_size >= 1024 ** 3:  # Gigabyte
-        return f"{file_size / (1024 ** 3):.2f} GB"
-    elif file_size >= 1024 ** 2:  # Megabyte
-        return f"{file_size / (1024 ** 2):.2f} MB"
-    elif file_size >= 1024:  # Kilobyte
-        return f"{file_size / 1024:.2f} kB"
-    elif file_size >= 8:  # Byte
-        return f"{file_size} bytes"
-    else:  # Bit
-        return f"{file_size * 8} bits"
-
-
 def getTotalSize(srcPaths):
     total_size = 0
     for path in srcPaths:
         if os.path.isfile(path):
             total_size += os.path.getsize(path)
         else:
             for r, d, files in os.walk(path):
                 for f in files:
                     fp = os.path.join(r, f)
                     total_size += os.path.getsize(fp)
     return total_size
 
 
+def format_file_size(file_size):
+    if file_size >= 1000 ** 4:  # Terabyte
+        return f"{round(file_size / (1000 ** 4))} TB"
+    elif file_size >= 1000 ** 3:  # Gigabyte
+        return f"{round(file_size / (1000 ** 3))} GB"
+    elif file_size >= 1000 ** 2:  # Megabyte
+        return f"{round(file_size / (1000 ** 2))} MB"
+    elif file_size >= 1000:  # Kilobyte
+        return f"{round(file_size / 1000)} kB"
+    else:  # Byte
+        return f"{file_size} bytes"
+
+
 def regular_copy(src, dst, console, task, progress):
-    with open(src, 'rb') as fsrc, open(dst, 'wb') as fdst:
-        while True:
-            buf = fsrc.read(1024*1024)
-            if not buf:
-                break
-            fdst.write(buf)
-            progress.update(task, advance=len(buf))
-            progress.refresh()
+    operation_cancelled = False
+    try:
+        with open(src, 'rb') as fsrc, open(dst, 'wb') as fdst:
+            while True:
+                buf = fsrc.read(1024*1024)
+                if operation_cancelled:
+                    return "c"
+                fdst.write(buf)
+                progress.update(task, advance=len(buf))
+                progress.refresh()
 
+    except KeyboardInterrupt:
+        operation_cancelled = True
+        progress.stop()
+        return "c"
 
-def verbose_copy(src, dst, console, current, total_files):
 
+def verbose_copy(src, dst, console, current, total_files):
+    operation_cancelled = False
     file_size = os.path.getsize(src)
 
     with Progress(
         BarColumn(bar_width=50),
         "[progress.percentage]{task.percentage:>3.0f}%",
         TimeRemainingColumn(),
         "[#ea2a6f][[/#ea2a6f]",
@@ -58,22 +61,27 @@
         "[#ea2a6f]][/#ea2a6f]",
         f"({current} of {total_files})",
         console=console,
         auto_refresh=False
     ) as progress:
         task = progress.add_task("", total=file_size, file_size=format_file_size(file_size))
 
-        with open(src, 'rb') as fsrc, open(dst, 'wb') as fdst:
-            while not progress.finished:
-                buf = fsrc.read(1024*1024)
-                if not buf:
-                    break
-                fdst.write(buf)
-                progress.update(task, advance=len(buf))
-                progress.refresh()
+        try:
+            with open(src, 'rb') as fsrc, open(dst, 'wb') as fdst:
+                while not progress.finished:
+                    buf = fsrc.read(1024*1024)
+                    if operation_cancelled:
+                        return "c"
+                    fdst.write(buf)
+                    progress.update(task, advance=len(buf))
+                    progress.refresh()
+        except KeyboardInterrupt:
+            operation_cancelled = True
+            progress.stop()
+            return "c"
 
 
 def hlp():
     print("""
 usage: ptrack [-h] [-v] [-c] [-m]
 
 A simple CLI utility for asthetically tracking progress when copying or moving files.
```

### Comparing `ptrack-0.1.1/setup.py` & `ptrack-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptrack',
-    version='0.1.1',
+    version='0.1.2',
     description='A simple CLI utility for asthetically tracking progress when copying or moving files.',
     author='Connor Etherington',
     author_email='connor@concise.cc',
     packages=find_packages(),
     install_requires=[
         'rich',
         'argparse',
```

