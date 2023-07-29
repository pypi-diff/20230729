# Comparing `tmp/motipy-1.0.0.tar.gz` & `tmp/motipy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motipy-1.0.0.tar", last modified: Fri Jul 14 10:11:10 2023, max compression
+gzip compressed data, was "motipy-1.1.0.tar", last modified: Sat Jul 29 10:27:16 2023, max compression
```

## Comparing `motipy-1.0.0.tar` & `motipy-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 10:11:10.326848 motipy-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 motipy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1140 2023-07-14 10:11:10.326848 motipy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      391 2023-07-14 10:07:02.000000 motipy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 10:11:10.326848 motipy-1.0.0/motipy/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-14 09:50:29.000000 motipy-1.0.0/motipy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24879 2023-07-14 09:50:32.000000 motipy-1.0.0/motipy/motipy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-14 10:11:10.326848 motipy-1.0.0/motipy.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1140 2023-07-14 10:11:10.000000 motipy-1.0.0/motipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-07-14 10:11:10.000000 motipy-1.0.0/motipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-14 10:11:10.000000 motipy-1.0.0/motipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-14 10:11:10.000000 motipy-1.0.0/motipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 motipy-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-14 10:11:10.326848 motipy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      669 2023-07-14 10:06:37.000000 motipy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-29 10:27:16.162319 motipy-1.1.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1067 2023-07-10 06:41:18.000000 motipy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1140 2023-07-29 10:27:16.162319 motipy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      391 2023-07-14 10:07:02.000000 motipy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-29 10:27:16.162319 motipy-1.1.0/motipy/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-07-14 09:50:29.000000 motipy-1.1.0/motipy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24862 2023-07-29 10:14:03.000000 motipy-1.1.0/motipy/motipy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-29 10:27:16.162319 motipy-1.1.0/motipy.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1140 2023-07-29 10:27:15.000000 motipy-1.1.0/motipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      197 2023-07-29 10:27:16.000000 motipy-1.1.0/motipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-29 10:27:15.000000 motipy-1.1.0/motipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-29 10:27:15.000000 motipy-1.1.0/motipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-07-10 17:36:39.000000 motipy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-29 10:27:16.162319 motipy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      669 2023-07-29 10:20:39.000000 motipy-1.1.0/setup.py
```

### Comparing `motipy-1.0.0/LICENSE` & `motipy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motipy-1.0.0/PKG-INFO` & `motipy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motipy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Un package Python pour obtenir des messages de motivation.
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `motipy-1.0.0/motipy/motipy.py` & `motipy-1.1.0/motipy/motipy.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,10 +299,8 @@
     "« La motivation te sert de départ, l'habitude te fait continuer, mais c'est la persévérance qui te fait arriver au bout. » - Roy T. Bennett",
     "« Les rêves se réalisent si tu as le courage de les poursuivre. » - Walt Disney",
     "« Le succès est la somme de petits efforts répétés jour après jour. » - Robert Collier"
 ]
 
 
 def moty():
-    fact = random.choice(motivation)
-    return fact
-
+    return random.choice(motivation)
```

### Comparing `motipy-1.0.0/motipy.egg-info/PKG-INFO` & `motipy-1.1.0/motipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motipy
-Version: 1.0.0
+Version: 1.1.0
 Summary: Un package Python pour obtenir des messages de motivation.
 Author: Coding Team
 Author-email: codingteam@telegmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `motipy-1.0.0/pyproject.toml` & `motipy-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `motipy-1.0.0/setup.py` & `motipy-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from readme_renderer.markdown import render
 
 with open('README.md', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name="motipy",
-    version="1.0.0",
+    version="1.1.0",
     author="Coding Team",
     author_email="codingteam@telegmail.com",
     license='MIT',
     description='Un package Python pour obtenir des messages de motivation.',
     long_description=render(long_description),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["testing"]),
```

