# Comparing `tmp/pydeum-0.0.1a1.tar.gz` & `tmp/pydeum-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeum-0.0.1a1.tar", last modified: Sat Jul 29 08:51:00 2023, max compression
+gzip compressed data, was "pydeum-0.0.2.tar", last modified: Sat Jul 29 08:36:48 2023, max compression
```

## Comparing `pydeum-0.0.1a1.tar` & `pydeum-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/src/Iodeum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/src/Iodeum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/src/Iodeum/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:50:41.000000 pydeum-0.0.1a1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:51:00.969637 pydeum-0.0.1a1/src/pydeum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-29 08:51:00.000000 pydeum-0.0.1a1/src/pydeum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-29 08:51:00.000000 pydeum-0.0.1a1/src/pydeum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:51:00.000000 pydeum-0.0.1a1/src/pydeum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 08:51:00.000000 pydeum-0.0.1a1/src/pydeum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:48.564075 pydeum-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-29 08:36:29.000000 pydeum-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 08:36:48.564075 pydeum-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-29 08:36:29.000000 pydeum-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-29 08:36:29.000000 pydeum-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:36:48.564075 pydeum-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:48.564075 pydeum-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:48.564075 pydeum-0.0.2/src/Iodeum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:29.000000 pydeum-0.0.2/src/Iodeum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-29 08:36:29.000000 pydeum-0.0.2/src/Iodeum/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:29.000000 pydeum-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:36:48.564075 pydeum-0.0.2/src/pydeum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-29 08:36:48.000000 pydeum-0.0.2/src/pydeum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-29 08:36:48.000000 pydeum-0.0.2/src/pydeum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:36:48.000000 pydeum-0.0.2/src/pydeum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-29 08:36:48.000000 pydeum-0.0.2/src/pydeum.egg-info/top_level.txt
```

### Comparing `pydeum-0.0.1a1/LICENSE` & `pydeum-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeum-0.0.1a1/PKG-INFO` & `pydeum-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydeum
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Blockchain access to Ideum
 Author-email: Louis Grange <louisgrange@ik.me>
-Project-URL: Bug Tracker, https://github.com/Iodeum/pydeum/issues
-Project-URL: Source, https://github.com/Iodeum/pydeum
+Project-URL: Homepage, https://github.com/Iodeum/pydeum
 Project-URL: Documentation, https://iodeum.org/doc/
-Project-URL: Homepage, https://iodeum.org
+Project-URL: Bug Tracker, https://github.com/Iodeum/pydeum/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pydeum-0.0.1a1/README.md` & `pydeum-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pydeum-0.0.1a1/pyproject.toml` & `pydeum-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydeum"
-version = "0.0.1a1"
+version = "0.0.2"
 authors = [
   { name="Louis Grange", email="louisgrange@ik.me" },
 ]
 description = "Blockchain access to Ideum"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -16,11 +16,10 @@
     'Intended Audience :: Financial and Insurance Industry',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     'Topic :: Office/Business :: Financial'
 ]
 
 [project.urls]
-"Bug Tracker" = "https://github.com/Iodeum/pydeum/issues"
-"Source" = "https://github.com/Iodeum/pydeum"
+"Homepage" = "https://github.com/Iodeum/pydeum"
 "Documentation" = "https://iodeum.org/doc/"
-"Homepage" = "https://iodeum.org"
+"Bug Tracker" = "https://github.com/Iodeum/pydeum/issues"
```

### Comparing `pydeum-0.0.1a1/src/Iodeum/main.py` & `pydeum-0.0.2/src/Iodeum/main.py`

 * *Files identical despite different names*

### Comparing `pydeum-0.0.1a1/src/pydeum.egg-info/PKG-INFO` & `pydeum-0.0.2/src/pydeum.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pydeum
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Blockchain access to Ideum
 Author-email: Louis Grange <louisgrange@ik.me>
-Project-URL: Bug Tracker, https://github.com/Iodeum/pydeum/issues
-Project-URL: Source, https://github.com/Iodeum/pydeum
+Project-URL: Homepage, https://github.com/Iodeum/pydeum
 Project-URL: Documentation, https://iodeum.org/doc/
-Project-URL: Homepage, https://iodeum.org
+Project-URL: Bug Tracker, https://github.com/Iodeum/pydeum/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

