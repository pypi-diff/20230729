# Comparing `tmp/xctools_kamaalio-0.0.1.tar.gz` & `tmp/xctools_kamaalio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.0.1.tar", last modified: Fri Jul 28 20:09:55 2023, max compression
+gzip compressed data, was "xctools_kamaalio-0.0.2.tar", last modified: Sat Jul 29 08:47:21 2023, max compression
```

## Comparing `xctools_kamaalio-0.0.1.tar` & `xctools_kamaalio-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-28 20:09:55.073674 xctools_kamaalio-0.0.1/
--rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-28 18:57:31.000000 xctools_kamaalio-0.0.1/LICENSE
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-28 20:09:55.073554 xctools_kamaalio-0.0.1/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-28 19:49:50.000000 xctools_kamaalio-0.0.1/README.md
--rw-r--r--   0 kamaal     (503) staff       (20)      597 2023-07-28 20:02:32.000000 xctools_kamaalio-0.0.1/pyproject.toml
--rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-28 20:09:55.073761 xctools_kamaalio-0.0.1/setup.cfg
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-28 20:09:55.072344 xctools_kamaalio-0.0.1/src/
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-28 20:09:55.072839 xctools_kamaalio-0.0.1/src/xctools_kamaalio/
--rw-r--r--   0 kamaal     (503) staff       (20)       32 2023-07-28 20:02:56.000000 xctools_kamaalio-0.0.1/src/xctools_kamaalio/__init__.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-28 20:09:55.073349 xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-28 20:09:55.000000 xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)      241 2023-07-28 20:09:55.000000 xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-28 20:09:55.000000 xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-28 20:09:55.000000 xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 08:47:21.877530 xctools_kamaalio-0.0.2/
+-rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-28 18:57:31.000000 xctools_kamaalio-0.0.2/LICENSE
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 08:47:21.877408 xctools_kamaalio-0.0.2/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-28 19:49:50.000000 xctools_kamaalio-0.0.2/README.md
+-rw-r--r--   0 kamaal     (503) staff       (20)      597 2023-07-29 08:46:23.000000 xctools_kamaalio-0.0.2/pyproject.toml
+-rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-29 08:47:21.877573 xctools_kamaalio-0.0.2/setup.cfg
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 08:47:21.875516 xctools_kamaalio-0.0.2/src/
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 08:47:21.876606 xctools_kamaalio-0.0.2/src/xctools_kamaalio/
+-rw-r--r--   0 kamaal     (503) staff       (20)       80 2023-07-29 08:46:55.000000 xctools_kamaalio-0.0.2/src/xctools_kamaalio/__init__.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 08:47:21.877215 xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 08:47:21.000000 xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)      241 2023-07-29 08:47:21.000000 xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-29 08:47:21.000000 xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-29 08:47:21.000000 xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/top_level.txt
```

### Comparing `xctools_kamaalio-0.0.1/LICENSE` & `xctools_kamaalio-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.1/PKG-INFO` & `xctools_kamaalio-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.0.1/pyproject.toml` & `xctools_kamaalio-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xctools_kamaalio"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Kamaal Farah", email = "kamaal.f1@gmail.com" }]
 description = "A package to help deal with Xcode projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `xctools_kamaalio-0.0.1/src/xctools_kamaalio.egg-info/PKG-INFO` & `xctools_kamaalio-0.0.2/src/xctools_kamaalio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools-kamaalio
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

