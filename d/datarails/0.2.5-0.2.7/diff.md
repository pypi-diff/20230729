# Comparing `tmp/datarails-0.2.5.tar.gz` & `tmp/datarails-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.2.5.tar", last modified: Sat Jul 29 08:15:35 2023, max compression
+gzip compressed data, was "datarails-0.2.7.tar", last modified: Sat Jul 29 18:32:25 2023, max compression
```

## Comparing `datarails-0.2.5.tar` & `datarails-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:15:35.081457 datarails-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-29 08:15:35.081457 datarails-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-29 08:15:16.000000 datarails-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:15:35.081457 datarails-0.2.5/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 08:15:16.000000 datarails-0.2.5/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-29 08:15:16.000000 datarails-0.2.5/datarails/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-29 08:15:16.000000 datarails-0.2.5/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-29 08:15:16.000000 datarails-0.2.5/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 08:15:16.000000 datarails-0.2.5/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:15:35.081457 datarails-0.2.5/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-29 08:15:35.000000 datarails-0.2.5/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 08:15:35.000000 datarails-0.2.5/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 08:15:35.000000 datarails-0.2.5/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 08:15:35.000000 datarails-0.2.5/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 08:15:35.000000 datarails-0.2.5/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-29 08:15:16.000000 datarails-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 08:15:35.081457 datarails-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-29 08:15:16.000000 datarails-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 08:15:35.081457 datarails-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-29 08:15:16.000000 datarails-0.2.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-29 08:15:16.000000 datarails-0.2.5/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 08:15:16.000000 datarails-0.2.5/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-29 08:15:16.000000 datarails-0.2.5/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-29 18:32:25.108359 datarails-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-29 18:32:15.000000 datarails-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-29 18:32:15.000000 datarails-0.2.7/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-29 18:32:03.000000 datarails-0.2.7/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 18:32:25.000000 datarails-0.2.7/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-29 18:32:15.000000 datarails-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 18:32:25.108359 datarails-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-29 18:32:03.000000 datarails-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 18:32:25.108359 datarails-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-29 18:32:03.000000 datarails-0.2.7/tests/test_step.py
```

### Comparing `datarails-0.2.5/PKG-INFO` & `datarails-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: datarails
-Version: 0.2.5
+Version: 0.2.7
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.5 --
+####  -- VERSION 0.2.7 --
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
 this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
 a jupyter notebook.
 
 ## Basic Usage
 
 Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
```

### Comparing `datarails-0.2.5/README.md` & `datarails-0.2.7/datarails.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+Metadata-Version: 2.1
+Name: datarails
+Version: 0.2.7
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.5 --
+####  -- VERSION 0.2.7 --
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
 this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
 a jupyter notebook.
 
 ## Basic Usage
 
 Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
```

### Comparing `datarails-0.2.5/datarails/contexts.py` & `datarails-0.2.7/datarails/contexts.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/datarails/runner.py` & `datarails-0.2.7/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/datarails/step.py` & `datarails-0.2.7/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/datarails.egg-info/PKG-INFO` & `datarails-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-Metadata-Version: 2.1
-Name: datarails
-Version: 0.2.5
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-
 # datarails -- A Simple Framework for Dataframe ETL
-####  -- VERSION 0.2.5 --
+####  -- VERSION 0.2.7 --
 
 ## Official Documentation
 The official documentation is hosted on github pages at [jesse.maitland.github.io](https://jessemaitland.github.io/datarails/)
 
+## Example Project
+There is an example repo containing some simple ETL jobs, notebooks and commands for building documentation at [jessemaitland/datarails-example](https://github.com/JesseMaitland/datarails_examples)
+
 Datarails is a simple framework for organizing your in memory Dataframe based ETL jobs. It doesn't matter of you are using `pandas`, `spark`, `glue` or anything else
 this library serves as a simple way to structure your ETL jobs so that others don't come along and have to debug your 300 line script by copy / pasting sections of it into
 a jupyter notebook.
 
 ## Basic Usage
 
 Steps are defined as classes and then passed to a step runner. All methods in the class that start with `step_` will be run in the order they are defined.
```

### Comparing `datarails-0.2.5/pyproject.toml` & `datarails-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.2.5"
+version = "0.2.7"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.2.5/tests/test_context.py` & `datarails-0.2.7/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/tests/test_databox.py` & `datarails-0.2.7/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/tests/test_runner.py` & `datarails-0.2.7/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.5/tests/test_step.py` & `datarails-0.2.7/tests/test_step.py`

 * *Files identical despite different names*

