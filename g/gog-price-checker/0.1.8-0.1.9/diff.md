# Comparing `tmp/gog_price_checker-0.1.8.tar.gz` & `tmp/gog_price_checker-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gog_price_checker-0.1.8.tar", last modified: Fri Jul 28 16:22:59 2023, max compression
+gzip compressed data, was "gog_price_checker-0.1.9.tar", last modified: Fri Jul 28 16:58:59 2023, max compression
```

## Comparing `gog_price_checker-0.1.8.tar` & `gog_price_checker-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/gog_price_checker/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/gog_price_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/gog_price_checker/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/gog_price_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 16:22:59.000000 gog_price_checker-0.1.8/gog_price_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:22:59.321152 gog_price_checker-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 16:22:44.000000 gog_price_checker-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/gog_price_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/gog_price_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/gog_price_checker/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/gog_price_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 16:58:59.000000 gog_price_checker-0.1.9/gog_price_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:58:59.710582 gog_price_checker-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-28 16:58:49.000000 gog_price_checker-0.1.9/setup.py
```

### Comparing `gog_price_checker-0.1.8/PKG-INFO` & `gog_price_checker-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog_price_checker
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gog_price_checker-0.1.8/README.md` & `gog_price_checker-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.8/gog_price_checker/__main__.py` & `gog_price_checker-0.1.9/gog_price_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `gog_price_checker-0.1.8/gog_price_checker.egg-info/PKG-INFO` & `gog_price_checker-0.1.9/gog_price_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gog-price-checker
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool to check game prices from GOG API
 Home-page: https://github.com/iampopovich/gog_price_checker
 Author: Alex
 Author-email: iampopovich@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gog_price_checker-0.1.8/setup.py` & `gog_price_checker-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gog_price_checker",
-    version="0.1.8",
+    version="0.1.9",
     author="Alex",
     author_email="iampopovich@example.com",
     description="A tool to check game prices from GOG API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iampopovich/gog_price_checker",
     packages=["gog_price_checker"],
```

