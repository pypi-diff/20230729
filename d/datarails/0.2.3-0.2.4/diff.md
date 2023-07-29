# Comparing `tmp/datarails-0.2.3.tar.gz` & `tmp/datarails-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.2.3.tar", last modified: Fri Jul 28 19:22:05 2023, max compression
+gzip compressed data, was "datarails-0.2.4.tar", last modified: Sat Jul 29 08:09:52 2023, max compression
```

## Comparing `datarails-0.2.3.tar` & `datarails-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.831837 datarails-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 19:22:05.831837 datarails-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-28 19:21:46.000000 datarails-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 19:21:46.000000 datarails-0.2.3/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 19:22:05.000000 datarails-0.2.3/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 19:21:46.000000 datarails-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:22:05.831837 datarails-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 19:21:46.000000 datarails-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:22:05.827837 datarails-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-28 19:21:46.000000 datarails-0.2.3/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:09:52.461940 datarails-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-29 08:09:52.461940 datarails-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-29 08:09:32.000000 datarails-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:09:52.461940 datarails-0.2.4/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 08:09:32.000000 datarails-0.2.4/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-29 08:09:32.000000 datarails-0.2.4/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-29 08:09:32.000000 datarails-0.2.4/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-29 08:09:32.000000 datarails-0.2.4/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 08:09:32.000000 datarails-0.2.4/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:09:52.461940 datarails-0.2.4/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-29 08:09:52.000000 datarails-0.2.4/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 08:09:52.000000 datarails-0.2.4/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:09:52.000000 datarails-0.2.4/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 08:09:52.000000 datarails-0.2.4/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 08:09:52.000000 datarails-0.2.4/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-29 08:09:32.000000 datarails-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:09:52.461940 datarails-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-29 08:09:32.000000 datarails-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:09:52.461940 datarails-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-29 08:09:32.000000 datarails-0.2.4/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-29 08:09:32.000000 datarails-0.2.4/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 08:09:32.000000 datarails-0.2.4/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-29 08:09:32.000000 datarails-0.2.4/tests/test_step.py
```

### Comparing `datarails-0.2.3/datarails/contexts.py` & `datarails-0.2.4/datarails/contexts.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/datarails/runner.py` & `datarails-0.2.4/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/datarails/step.py` & `datarails-0.2.4/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/pyproject.toml` & `datarails-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.2.3/tests/test_context.py` & `datarails-0.2.4/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/tests/test_databox.py` & `datarails-0.2.4/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/tests/test_runner.py` & `datarails-0.2.4/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.3/tests/test_step.py` & `datarails-0.2.4/tests/test_step.py`

 * *Files identical despite different names*

