# Comparing `tmp/kot-0.20.1.tar.gz` & `tmp/kot-0.20.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.20.1.tar", last modified: Thu Jul 27 00:15:02 2023, max compression
+gzip compressed data, was "kot-0.20.2.tar", last modified: Sat Jul 29 12:01:22 2023, max compression
```

## Comparing `kot-0.20.1.tar` & `kot-0.20.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:15:01.999169 kot-0.20.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 00:14:49.000000 kot-0.20.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 00:15:01.999169 kot-0.20.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 00:14:49.000000 kot-0.20.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:15:02.003169 kot-0.20.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-27 00:14:49.000000 kot-0.20.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:15:01.999169 kot-0.20.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:15:01.999169 kot-0.20.1/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 00:14:49.000000 kot-0.20.1/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-27 00:14:49.000000 kot-0.20.1/src/kot/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-07-27 00:14:49.000000 kot-0.20.1/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:15:01.999169 kot-0.20.1/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 00:15:01.000000 kot-0.20.1/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:01:22.726626 kot-0.20.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-29 12:01:10.000000 kot-0.20.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-29 12:01:22.726626 kot-0.20.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-29 12:01:10.000000 kot-0.20.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:01:22.726626 kot-0.20.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-29 12:01:10.000000 kot-0.20.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:01:22.722626 kot-0.20.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:01:22.726626 kot-0.20.2/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 12:01:10.000000 kot-0.20.2/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-29 12:01:10.000000 kot-0.20.2/src/kot/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-07-29 12:01:10.000000 kot-0.20.2/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:01:22.726626 kot-0.20.2/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-29 12:01:22.000000 kot-0.20.2/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.20.1/LICENSE` & `kot-0.20.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.20.1/PKG-INFO` & `kot-0.20.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.20.1
+Version: 0.20.2
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

### Comparing `kot-0.20.1/README.md` & `kot-0.20.2/README.md`

 * *Files identical despite different names*

### Comparing `kot-0.20.1/setup.py` & `kot-0.20.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.20.1',
+version='0.20.2',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `kot-0.20.1/src/kot/gui.py` & `kot-0.20.2/src/kot/gui.py`

 * *Files identical despite different names*

### Comparing `kot-0.20.1/src/kot/kot.py` & `kot-0.20.2/src/kot/kot.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,20 +630,21 @@
 
             with contextlib.suppress(TypeError):
                 maybe_file = self.get(key)
                 if os.path.exists(maybe_file):
                     os.remove(maybe_file)
 
             the_get = self.get(key, no_cache=True, raw_dict=True, get_shotcut=True)
-            if the_get["short_cut"]:
-                with contextlib.suppress(TypeError):
+            with contextlib.suppress(TypeError):
                     maybe_file = self.get(key, custom_key_location=the_get["value"])
                     if os.path.exists(maybe_file):
-                        os.remove(maybe_file)
-                os.remove(the_get["value"])             
+                        os.remove(maybe_file)   
+            with contextlib.suppress(TypeError):
+                if the_get["short_cut"]:
+                    os.remove(the_get["value"])             
 
             if os.path.exists(key_location_compress_indicator):
                 os.remove(
                     os.path.join(self.location,
                                  key_location_compress_indicator))
             if os.path.exists(os.path.join(self.location, key_location)):
                 os.remove(os.path.join(self.location, key_location))
@@ -663,22 +664,23 @@
         return True
 
     def dict(self, encryption_key: str = "", no_data: bool = False):
         encryption_key = force_encrypt if force_encrypt != False else encryption_key
         result = {}
         for key in os.listdir(self.location):
             if not "." in key:
-                the_key = self.get_key(key)
-                if not the_key is None:
-                    if the_key != False:
-                        result_of_key = (self.get(
-                            the_key, encryption_key=encryption_key)
-                                         if not no_data else True)
-                        if not result_of_key is None:
-                            result[the_key] = result_of_key
+                with contextlib.suppress(Exception):
+                    the_key = self.get_key(key)
+                    if not the_key is None:
+                        if the_key != False:
+                            result_of_key = (self.get(
+                                the_key, encryption_key=encryption_key)
+                                            if not no_data else True)
+                            if not result_of_key is None:
+                                result[the_key] = result_of_key
         return result
 
     def size_all(self) -> int:
         # Calculate self.location size
         total_size = 0
 
         for dirpath, dirnames, filenames in os.walk(self.location):
```

### Comparing `kot-0.20.1/src/kot.egg-info/PKG-INFO` & `kot-0.20.2/src/kot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.20.1
+Version: 0.20.2
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT database
```

