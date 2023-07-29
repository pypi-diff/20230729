# Comparing `tmp/notmongo-0.1.5.tar.gz` & `tmp/notmongo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notmongo-0.1.5.tar", last modified: Sat Jul 29 11:28:53 2023, max compression
+gzip compressed data, was "notmongo-0.1.6.tar", last modified: Sat Jul 29 11:53:43 2023, max compression
```

## Comparing `notmongo-0.1.5.tar` & `notmongo-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:28:53.123728 notmongo-0.1.5/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:28:53.123728 notmongo-0.1.5/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      280 2023-07-29 11:25:53.000000 notmongo-0.1.5/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-07-29 11:28:53.123728 notmongo-0.1.5/setup.cfg
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2858 2023-07-29 10:46:00.000000 notmongo-0.1.5/setup.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:28:53.120395 notmongo-0.1.5/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:28:53.120395 notmongo-0.1.5/src/notmongo/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      203 2023-07-29 10:40:35.000000 notmongo-0.1.5/src/notmongo/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5981 2023-07-29 06:41:16.000000 notmongo-0.1.5/src/notmongo/async_collection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4245 2023-07-28 13:36:39.000000 notmongo-0.1.5/src/notmongo/async_database.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8130 2023-07-29 10:41:00.000000 notmongo-0.1.5/src/notmongo/native.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3320 2023-07-28 08:51:57.000000 notmongo-0.1.5/src/notmongo/persistence.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1313 2023-07-28 08:51:57.000000 notmongo-0.1.5/src/notmongo/results.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    13020 2023-07-28 08:51:57.000000 notmongo-0.1.5/src/notmongo/sync_collection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6921 2023-07-28 13:37:28.000000 notmongo-0.1.5/src/notmongo/sync_database.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      481 2023-07-28 07:37:57.000000 notmongo-0.1.5/src/notmongo/typedefs.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:28:53.120395 notmongo-0.1.5/src/notmongo.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:28:53.000000 notmongo-0.1.5/src/notmongo.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      643 2023-07-29 11:28:53.000000 notmongo-0.1.5/src/notmongo.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 11:28:53.000000 notmongo-0.1.5/src/notmongo.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 10:43:44.000000 notmongo-0.1.5/src/notmongo.egg-info/not-zip-safe
--rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2023-07-29 11:28:53.000000 notmongo-0.1.5/src/notmongo.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       21 2023-07-29 11:28:53.000000 notmongo-0.1.5/src/notmongo.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:28:53.123728 notmongo-0.1.5/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6294 2023-07-28 13:36:15.000000 notmongo-0.1.5/tests/test_database_async.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    11394 2023-07-28 08:51:57.000000 notmongo-0.1.5/tests/test_operations_async.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1162 2023-07-28 08:51:57.000000 notmongo-0.1.5/tests/test_persistence.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2797 2023-07-28 08:51:57.000000 notmongo-0.1.5/tests/test_projection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5039 2023-07-28 08:51:57.000000 notmongo-0.1.5/tests/test_queries.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3185 2023-07-28 08:51:57.000000 notmongo-0.1.5/tests/test_sorting.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:53:42.995446 notmongo-0.1.6/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      280 2023-07-29 11:25:53.000000 notmongo-0.1.6/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-07-29 11:53:42.995446 notmongo-0.1.6/setup.cfg
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2891 2023-07-29 11:50:54.000000 notmongo-0.1.6/setup.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.992113 notmongo-0.1.6/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/src/notmongo/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      203 2023-07-29 10:40:35.000000 notmongo-0.1.6/src/notmongo/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5981 2023-07-29 06:41:16.000000 notmongo-0.1.6/src/notmongo/async_collection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4245 2023-07-28 13:36:39.000000 notmongo-0.1.6/src/notmongo/async_database.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8130 2023-07-29 10:41:00.000000 notmongo-0.1.6/src/notmongo/native.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3320 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/persistence.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1313 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/results.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    13020 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/sync_collection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6921 2023-07-28 13:37:28.000000 notmongo-0.1.6/src/notmongo/sync_database.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      481 2023-07-28 07:37:57.000000 notmongo-0.1.6/src/notmongo/typedefs.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/src/notmongo.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      643 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 10:43:44.000000 notmongo-0.1.6/src/notmongo.egg-info/not-zip-safe
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       35 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6294 2023-07-28 13:36:15.000000 notmongo-0.1.6/tests/test_database_async.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    11394 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_operations_async.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1162 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_persistence.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2797 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_projection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5039 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_queries.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3185 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_sorting.py
```

### Comparing `notmongo-0.1.5/setup.py` & `notmongo-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -61,29 +61,30 @@
 
         assert python_module_path.exists(), f"Could not find python module at {python_module_path}"
 
         shared_objects_dir = python_module_path / "shared_objects"
         shared_objects_dir.mkdir(exist_ok=True)
         shutil.move(so_path, shared_objects_dir / "libnotmongo.so")
 
-        shutil.copy(PROJECT_ROOT_DIR / 'notmongo_meta.py', python_module_path / 'meta.py')
+        shutil.copy(PROJECT_ROOT_DIR/ 'notmongo_meta.py', python_module_path / 'meta.py')
 
 
 setup(
     name="notmongo",
     version=meta.__version__,
     rust_extensions=[
         RustExtension(
             "notmongo-rs",
             binding=Binding.NoBinding,
             path="src/notmongo-rs/Cargo.toml",
         )
     ],
     packages=["notmongo-rs", "notmongo"],
     package_dir={"": "src"},
+    py_modules=["notmongo_meta"],
     zip_safe=False,
     cmdclass={"build": BuildCommand},
     extras_require={
         "dev": [
             "black",
             "isort",
             "pre_commit",
```

### Comparing `notmongo-0.1.5/src/notmongo/async_collection.py` & `notmongo-0.1.6/src/notmongo/async_collection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/async_database.py` & `notmongo-0.1.6/src/notmongo/async_database.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/native.py` & `notmongo-0.1.6/src/notmongo/native.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/persistence.py` & `notmongo-0.1.6/src/notmongo/persistence.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/results.py` & `notmongo-0.1.6/src/notmongo/results.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/sync_collection.py` & `notmongo-0.1.6/src/notmongo/sync_collection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo/sync_database.py` & `notmongo-0.1.6/src/notmongo/sync_database.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/src/notmongo.egg-info/SOURCES.txt` & `notmongo-0.1.6/src/notmongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_database_async.py` & `notmongo-0.1.6/tests/test_database_async.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_operations_async.py` & `notmongo-0.1.6/tests/test_operations_async.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_persistence.py` & `notmongo-0.1.6/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_projection.py` & `notmongo-0.1.6/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_queries.py` & `notmongo-0.1.6/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.5/tests/test_sorting.py` & `notmongo-0.1.6/tests/test_sorting.py`

 * *Files identical despite different names*

