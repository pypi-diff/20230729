# Comparing `tmp/xctools_kamaalio-0.0.3.tar.gz` & `tmp/xctools_kamaalio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xctools_kamaalio-0.0.3.tar", last modified: Sat Jul 29 10:46:35 2023, max compression
+gzip compressed data, was "xctools_kamaalio-0.0.4.tar", last modified: Sat Jul 29 11:08:21 2023, max compression
```

## Comparing `xctools_kamaalio-0.0.3.tar` & `xctools_kamaalio-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 10:46:35.555801 xctools_kamaalio-0.0.3/
--rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-28 18:57:31.000000 xctools_kamaalio-0.0.3/LICENSE
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 10:46:35.555668 xctools_kamaalio-0.0.3/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-28 19:49:50.000000 xctools_kamaalio-0.0.3/README.md
--rw-r--r--   0 kamaal     (503) staff       (20)      597 2023-07-29 10:45:56.000000 xctools_kamaalio-0.0.3/pyproject.toml
--rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-29 10:46:35.555858 xctools_kamaalio-0.0.3/setup.cfg
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 10:46:35.553905 xctools_kamaalio-0.0.3/src/
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 10:46:35.554879 xctools_kamaalio-0.0.3/src/xctools_kamaalio/
--rw-r--r--   0 kamaal     (503) staff       (20)       32 2023-07-29 10:45:25.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio/__init__.py
--rw-r--r--   0 kamaal     (503) staff       (20)       83 2023-07-29 10:45:33.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio/__main__.py
-drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 10:46:35.555455 xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/
--rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 10:46:35.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/PKG-INFO
--rw-r--r--   0 kamaal     (503) staff       (20)      274 2023-07-29 10:46:35.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/SOURCES.txt
--rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-29 10:46:35.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/dependency_links.txt
--rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-29 10:46:35.000000 xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/top_level.txt
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.778981 xctools_kamaalio-0.0.4/
+-rw-r--r--   0 kamaal     (503) staff       (20)     1077 2023-07-28 18:57:31.000000 xctools_kamaalio-0.0.4/LICENSE
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 11:08:21.778861 xctools_kamaalio-0.0.4/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)       10 2023-07-28 19:49:50.000000 xctools_kamaalio-0.0.4/README.md
+-rw-r--r--   0 kamaal     (503) staff       (20)      653 2023-07-29 11:07:51.000000 xctools_kamaalio-0.0.4/pyproject.toml
+-rw-r--r--   0 kamaal     (503) staff       (20)       38 2023-07-29 11:08:21.779033 xctools_kamaalio-0.0.4/setup.cfg
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.777042 xctools_kamaalio-0.0.4/src/
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.777777 xctools_kamaalio-0.0.4/src/xctools_kamaalio/
+-rw-r--r--   0 kamaal     (503) staff       (20)        0 2023-07-29 11:03:49.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/__init__.py
+-rw-r--r--   0 kamaal     (503) staff       (20)       60 2023-07-29 11:04:53.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/__main__.py
+-rw-r--r--   0 kamaal     (503) staff       (20)       30 2023-07-29 11:03:05.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio/cli.py
+drwxr-xr-x   0 kamaal     (503) staff       (20)        0 2023-07-29 11:08:21.778647 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/
+-rw-r--r--   0 kamaal     (503) staff       (20)      534 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/PKG-INFO
+-rw-r--r--   0 kamaal     (503) staff       (20)      349 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/SOURCES.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)        1 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/dependency_links.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       53 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/entry_points.txt
+-rw-r--r--   0 kamaal     (503) staff       (20)       17 2023-07-29 11:08:21.000000 xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/top_level.txt
```

### Comparing `xctools_kamaalio-0.0.3/LICENSE` & `xctools_kamaalio-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xctools_kamaalio-0.0.3/PKG-INFO` & `xctools_kamaalio-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools_kamaalio
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xctools_kamaalio-0.0.3/pyproject.toml` & `xctools_kamaalio-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[project.scripts]
+xctools = "xctools_kamaalio:cli.cli"
+
 [project]
 name = "xctools_kamaalio"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Kamaal Farah", email = "kamaal.f1@gmail.com" }]
 description = "A package to help deal with Xcode projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `xctools_kamaalio-0.0.3/src/xctools_kamaalio.egg-info/PKG-INFO` & `xctools_kamaalio-0.0.4/src/xctools_kamaalio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xctools-kamaalio
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to help deal with Xcode projects.
 Author-email: Kamaal Farah <kamaal.f1@gmail.com>
 Project-URL: Homepage, https://github.com/kamaal111/xctools
 Project-URL: Bug Tracker, https://github.com/kamaal111/xctools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

