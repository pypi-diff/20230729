# Comparing `tmp/notmongo-0.1.6.tar.gz` & `tmp/notmongo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notmongo-0.1.6.tar", last modified: Sat Jul 29 11:53:43 2023, max compression
+gzip compressed data, was "notmongo-0.1.7.tar", last modified: Sat Jul 29 12:04:12 2023, max compression
```

## Comparing `notmongo-0.1.6.tar` & `notmongo-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:53:42.995446 notmongo-0.1.6/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      280 2023-07-29 11:25:53.000000 notmongo-0.1.6/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-07-29 11:53:42.995446 notmongo-0.1.6/setup.cfg
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2891 2023-07-29 11:50:54.000000 notmongo-0.1.6/setup.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.992113 notmongo-0.1.6/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/src/notmongo/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      203 2023-07-29 10:40:35.000000 notmongo-0.1.6/src/notmongo/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5981 2023-07-29 06:41:16.000000 notmongo-0.1.6/src/notmongo/async_collection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4245 2023-07-28 13:36:39.000000 notmongo-0.1.6/src/notmongo/async_database.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8130 2023-07-29 10:41:00.000000 notmongo-0.1.6/src/notmongo/native.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3320 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/persistence.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1313 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/results.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    13020 2023-07-28 08:51:57.000000 notmongo-0.1.6/src/notmongo/sync_collection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6921 2023-07-28 13:37:28.000000 notmongo-0.1.6/src/notmongo/sync_database.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      481 2023-07-28 07:37:57.000000 notmongo-0.1.6/src/notmongo/typedefs.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/src/notmongo.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      643 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 10:43:44.000000 notmongo-0.1.6/src/notmongo.egg-info/not-zip-safe
--rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       35 2023-07-29 11:53:42.000000 notmongo-0.1.6/src/notmongo.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 11:53:42.995446 notmongo-0.1.6/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6294 2023-07-28 13:36:15.000000 notmongo-0.1.6/tests/test_database_async.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    11394 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_operations_async.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1162 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_persistence.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2797 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_projection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5039 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_queries.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3185 2023-07-28 08:51:57.000000 notmongo-0.1.6/tests/test_sorting.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 12:04:12.729125 notmongo-0.1.7/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 12:04:12.729125 notmongo-0.1.7/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      279 2023-07-29 12:00:51.000000 notmongo-0.1.7/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-07-29 12:04:12.729125 notmongo-0.1.7/setup.cfg
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2809 2023-07-29 12:01:26.000000 notmongo-0.1.7/setup.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 12:04:12.725791 notmongo-0.1.7/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 12:04:12.729125 notmongo-0.1.7/src/notmongo/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      193 2023-07-29 11:57:58.000000 notmongo-0.1.7/src/notmongo/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5981 2023-07-29 06:41:16.000000 notmongo-0.1.7/src/notmongo/async_collection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4245 2023-07-28 13:36:39.000000 notmongo-0.1.7/src/notmongo/async_database.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      145 2023-07-29 11:59:03.000000 notmongo-0.1.7/src/notmongo/meta.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8130 2023-07-29 10:41:00.000000 notmongo-0.1.7/src/notmongo/native.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3320 2023-07-28 08:51:57.000000 notmongo-0.1.7/src/notmongo/persistence.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1313 2023-07-28 08:51:57.000000 notmongo-0.1.7/src/notmongo/results.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    13020 2023-07-28 08:51:57.000000 notmongo-0.1.7/src/notmongo/sync_collection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6921 2023-07-28 13:37:28.000000 notmongo-0.1.7/src/notmongo/sync_database.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      481 2023-07-28 07:37:57.000000 notmongo-0.1.7/src/notmongo/typedefs.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        6 2023-07-29 11:59:29.000000 notmongo-0.1.7/src/notmongo/version.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 12:04:12.729125 notmongo-0.1.7/src/notmongo.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       72 2023-07-29 12:04:12.000000 notmongo-0.1.7/src/notmongo.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      689 2023-07-29 12:04:12.000000 notmongo-0.1.7/src/notmongo.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 12:04:12.000000 notmongo-0.1.7/src/notmongo.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-07-29 12:03:30.000000 notmongo-0.1.7/src/notmongo.egg-info/not-zip-safe
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2023-07-29 12:04:12.000000 notmongo-0.1.7/src/notmongo.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       21 2023-07-29 12:04:12.000000 notmongo-0.1.7/src/notmongo.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-07-29 12:04:12.729125 notmongo-0.1.7/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6294 2023-07-28 13:36:15.000000 notmongo-0.1.7/tests/test_database_async.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    11394 2023-07-28 08:51:57.000000 notmongo-0.1.7/tests/test_operations_async.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1162 2023-07-28 08:51:57.000000 notmongo-0.1.7/tests/test_persistence.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2797 2023-07-28 08:51:57.000000 notmongo-0.1.7/tests/test_projection.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5039 2023-07-28 08:51:57.000000 notmongo-0.1.7/tests/test_queries.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3185 2023-07-28 08:51:57.000000 notmongo-0.1.7/tests/test_sorting.py
```

### Comparing `notmongo-0.1.6/setup.py` & `notmongo-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,49 +3,51 @@
 import tarfile
 from pathlib import Path
 import urllib.request
 
 from setuptools import setup
 
 from setuptools_rust import Binding, RustExtension
-import notmongo_meta as meta
 
 
 PROJECT_ROOT_DIR = Path(__file__).resolve().parent
 SRC_DIR = PROJECT_ROOT_DIR / "src"
 BUILD_DIR = PROJECT_ROOT_DIR / "build"
 
 CRATE_TARBALL_PATH = SRC_DIR / "notmongo-rs.tar.gz"
 RUST_SOURCE_DIR = SRC_DIR / "notmongo-rs"
 PY_SOURCE_DIR = SRC_DIR / "notmongo"
 
 
+notmongo_version = (PY_SOURCE_DIR / 'version.txt').read_text().strip()
+
+
 # Download notmongo-rs from crates.io
 #
 # TODO: This should really be done in the build function, however `setup` fails
 #       if the rust sources don't already exist.
 def ensure_rust_source_code_exists():
     # Fetch the tarball, if needed
     if not CRATE_TARBALL_PATH.exists():
         print('Downloading "notmongo-rs" from crates.io')
         download_url = (
-            f"https://crates.io/api/v1/crates/notmongo/{meta.__version__}/download"
+            f"https://crates.io/api/v1/crates/notmongo/{notmongo_version}/download"
         )
 
         with urllib.request.urlopen(download_url) as response:
             with CRATE_TARBALL_PATH.open("wb") as outfile:
                 shutil.copyfileobj(response, outfile)
 
     # Unzip the archive, if needed
     if not RUST_SOURCE_DIR.exists():
         print("Extracting rust source")
         with tarfile.open(CRATE_TARBALL_PATH) as zfile:
             zfile.extractall(SRC_DIR)
 
-        shutil.move(SRC_DIR / f"notmongo-{meta.__version__}", RUST_SOURCE_DIR)
+        shutil.move(SRC_DIR / f"notmongo-{notmongo_version}", RUST_SOURCE_DIR)
 
 ensure_rust_source_code_exists()
 
 
 class BuildCommand(distutils.command.build.build):
     def run(self):
         # TODO: Would be great to download the rust source here, but this causes
@@ -61,30 +63,26 @@
 
         assert python_module_path.exists(), f"Could not find python module at {python_module_path}"
 
         shared_objects_dir = python_module_path / "shared_objects"
         shared_objects_dir.mkdir(exist_ok=True)
         shutil.move(so_path, shared_objects_dir / "libnotmongo.so")
 
-        shutil.copy(PROJECT_ROOT_DIR/ 'notmongo_meta.py', python_module_path / 'meta.py')
-
-
 setup(
     name="notmongo",
-    version=meta.__version__,
+    version=notmongo_version,
     rust_extensions=[
         RustExtension(
             "notmongo-rs",
             binding=Binding.NoBinding,
             path="src/notmongo-rs/Cargo.toml",
         )
     ],
     packages=["notmongo-rs", "notmongo"],
     package_dir={"": "src"},
-    py_modules=["notmongo_meta"],
     zip_safe=False,
     cmdclass={"build": BuildCommand},
     extras_require={
         "dev": [
             "black",
             "isort",
             "pre_commit",
```

### Comparing `notmongo-0.1.6/src/notmongo/async_collection.py` & `notmongo-0.1.7/src/notmongo/async_collection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/async_database.py` & `notmongo-0.1.7/src/notmongo/async_database.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/native.py` & `notmongo-0.1.7/src/notmongo/native.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/persistence.py` & `notmongo-0.1.7/src/notmongo/persistence.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/results.py` & `notmongo-0.1.7/src/notmongo/results.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/sync_collection.py` & `notmongo-0.1.7/src/notmongo/sync_collection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo/sync_database.py` & `notmongo-0.1.7/src/notmongo/sync_database.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/src/notmongo.egg-info/SOURCES.txt` & `notmongo-0.1.7/src/notmongo.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 pyproject.toml
 setup.py
 src/notmongo/__init__.py
 src/notmongo/async_collection.py
 src/notmongo/async_database.py
+src/notmongo/meta.py
 src/notmongo/native.py
 src/notmongo/persistence.py
 src/notmongo/results.py
 src/notmongo/sync_collection.py
 src/notmongo/sync_database.py
 src/notmongo/typedefs.py
+src/notmongo/version.txt
 src/notmongo.egg-info/PKG-INFO
 src/notmongo.egg-info/SOURCES.txt
 src/notmongo.egg-info/dependency_links.txt
 src/notmongo.egg-info/not-zip-safe
 src/notmongo.egg-info/requires.txt
 src/notmongo.egg-info/top_level.txt
 tests/test_database_async.py
```

### Comparing `notmongo-0.1.6/tests/test_database_async.py` & `notmongo-0.1.7/tests/test_database_async.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/tests/test_operations_async.py` & `notmongo-0.1.7/tests/test_operations_async.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/tests/test_persistence.py` & `notmongo-0.1.7/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/tests/test_projection.py` & `notmongo-0.1.7/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/tests/test_queries.py` & `notmongo-0.1.7/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `notmongo-0.1.6/tests/test_sorting.py` & `notmongo-0.1.7/tests/test_sorting.py`

 * *Files identical despite different names*

