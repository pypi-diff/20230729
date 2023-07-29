# Comparing `tmp/Boco-0.3.tar.gz` & `tmp/Boco-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Boco-0.3.tar", last modified: Sat Jul 29 12:09:15 2023, max compression
+gzip compressed data, was "Boco-0.3.1.tar", last modified: Sat Jul 29 12:13:54 2023, max compression
```

## Comparing `Boco-0.3.tar` & `Boco-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/Boco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-29 12:09:15.000000 Boco-0.3/Boco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-29 12:09:15.000000 Boco-0.3/Boco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:09:15.000000 Boco-0.3/Boco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 12:09:15.000000 Boco-0.3/Boco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-29 12:09:15.925158 Boco-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-29 12:09:06.000000 Boco-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/boco/
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-29 12:09:06.000000 Boco-0.3/boco/CorpusBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-29 12:09:06.000000 Boco-0.3/boco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/boco/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-29 12:09:06.000000 Boco-0.3/boco/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-29 12:09:06.000000 Boco-0.3/boco/filters/filter_by_pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 12:09:06.000000 Boco-0.3/boco/filters/filter_by_unique.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/boco/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-29 12:09:06.000000 Boco-0.3/boco/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-29 12:09:06.000000 Boco-0.3/boco/operations/counts_by_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-29 12:09:06.000000 Boco-0.3/boco/operations/counts_by_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-29 12:09:06.000000 Boco-0.3/boco/operations/search_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-29 12:09:06.000000 Boco-0.3/boco/operations/search_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:15.925158 Boco-0.3/boco/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:09:06.000000 Boco-0.3/boco/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-29 12:09:06.000000 Boco-0.3/boco/utils/_add_pos.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:09:15.925158 Boco-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-29 12:09:06.000000 Boco-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/Boco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-29 12:13:54.000000 Boco-0.3.1/Boco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-29 12:13:54.000000 Boco-0.3.1/Boco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:13:54.000000 Boco-0.3.1/Boco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-29 12:13:54.000000 Boco-0.3.1/Boco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-29 12:13:54.244846 Boco-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-29 12:13:40.000000 Boco-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/boco/
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/CorpusBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/boco/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/filters/filter_by_pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/filters/filter_by_unique.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/boco/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/operations/counts_by_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/operations/counts_by_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/operations/search_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/operations/search_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:54.244846 Boco-0.3.1/boco/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-29 12:13:40.000000 Boco-0.3.1/boco/utils/_add_pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:13:54.244846 Boco-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-29 12:13:40.000000 Boco-0.3.1/setup.py
```

### Comparing `Boco-0.3/Boco.egg-info/PKG-INFO` & `Boco-0.3.1/Boco.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Boco
-Version: 0.3
+Version: 0.3.1
 Summary: A corpus manager for Tibetan Language
-Home-page: https://github.com/lopenling/bocor
+Home-page: https://github.com/lopenling/boco
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 License: MIT
 Keywords: language corpus linguistics tibetan
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Boco-0.3/PKG-INFO` & `Boco-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Boco
-Version: 0.3
+Version: 0.3.1
 Summary: A corpus manager for Tibetan Language
-Home-page: https://github.com/lopenling/bocor
+Home-page: https://github.com/lopenling/boco
 Author: Mikko Kotila
 Author-email: mailme@mikkokotila.com
 License: MIT
 Keywords: language corpus linguistics tibetan
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Boco-0.3/README.md` & `Boco-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/CorpusBuilder.py` & `Boco-0.3.1/boco/CorpusBuilder.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/filters/filter_by_pos.py` & `Boco-0.3.1/boco/filters/filter_by_pos.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/operations/counts_by_segment.py` & `Boco-0.3.1/boco/operations/counts_by_segment.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/operations/counts_by_token.py` & `Boco-0.3.1/boco/operations/counts_by_token.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/operations/search_string.py` & `Boco-0.3.1/boco/operations/search_string.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/boco/operations/search_token.py` & `Boco-0.3.1/boco/operations/search_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
         # iterate through all the segments in the text
         for segment in corpus.data['texts'][text]['tokens']:
             if token in segment:
                 out.append([''.join(segment), text])
 
     if unique:
 
-        from bocor.filters.filter_by_unique import filter_by_unique
+        from boco.filters.filter_by_unique import filter_by_unique
         return filter_by_unique(out)
 
     return out
```

### Comparing `Boco-0.3/boco/utils/_add_pos.py` & `Boco-0.3.1/boco/utils/_add_pos.py`

 * *Files identical despite different names*

### Comparing `Boco-0.3/setup.py` & `Boco-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='Boco',
-    version='v0.3',
+    version='v0.3.1',
     description='A corpus manager for Tibetan Language',
     long_description='Boco corpus manager is used for building, maintaining, and using corpora. The motivation is to make it as straightforward as possible to manage multiple corpora per project, as well as perform cross-corpus operations between those corpora.',
-    url='https://github.com/lopenling/bocor',
+    url='https://github.com/lopenling/boco',
     author='Mikko Kotila',
     author_email='mailme@mikkokotila.com',
     license='MIT',
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

