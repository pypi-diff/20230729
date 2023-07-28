# Comparing `tmp/onefuzztypes-8.6.0.tar.gz` & `tmp/onefuzztypes-8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onefuzztypes-8.6.0.tar", last modified: Wed Jul 26 23:06:24 2023, max compression
+gzip compressed data, was "dist/onefuzztypes-8.6.1.tar", last modified: Fri Jul 28 22:45:22 2023, max compression
```

## Comparing `onefuzztypes-8.6.0.tar` & `onefuzztypes-8.6.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    12270 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    23125 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/onefuzztypes/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/onefuzztypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:24.000000 onefuzztypes-8.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/tests/test_alnum_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/tests/test_instance_config_update.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2947 2023-07-26 23:06:21.000000 onefuzztypes-8.6.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/onefuzztypes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/consts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12270 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23125 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/onefuzztypes/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-28 22:45:21.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 22:45:21.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 22:45:21.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-28 22:45:21.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-28 22:45:21.000000 onefuzztypes-8.6.1/onefuzztypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:22.000000 onefuzztypes-8.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/tests/test_alnum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/tests/test_instance_config_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2947 2023-07-28 22:45:19.000000 onefuzztypes-8.6.1/tests/test_models.py
```

### Comparing `onefuzztypes-8.6.0/PKG-INFO` & `onefuzztypes-8.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.6.0
+Version: 8.6.1
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.6.0/README.md` & `onefuzztypes-8.6.1/README.md`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/_monkeypatch.py` & `onefuzztypes-8.6.1/onefuzztypes/_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/enums.py` & `onefuzztypes-8.6.1/onefuzztypes/enums.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/events.py` & `onefuzztypes-8.6.1/onefuzztypes/events.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/job_templates.py` & `onefuzztypes-8.6.1/onefuzztypes/job_templates.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/models.py` & `onefuzztypes-8.6.1/onefuzztypes/models.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/primitives.py` & `onefuzztypes-8.6.1/onefuzztypes/primitives.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/requests.py` & `onefuzztypes-8.6.1/onefuzztypes/requests.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/responses.py` & `onefuzztypes-8.6.1/onefuzztypes/responses.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/validators.py` & `onefuzztypes-8.6.1/onefuzztypes/validators.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes/webhooks.py` & `onefuzztypes-8.6.1/onefuzztypes/webhooks.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/onefuzztypes.egg-info/PKG-INFO` & `onefuzztypes-8.6.1/onefuzztypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.6.0
+Version: 8.6.1
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.6.0/onefuzztypes.egg-info/SOURCES.txt` & `onefuzztypes-8.6.1/onefuzztypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/setup.py` & `onefuzztypes-8.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/tests/test_alnum_filter.py` & `onefuzztypes-8.6.1/tests/test_alnum_filter.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/tests/test_instance_config_update.py` & `onefuzztypes-8.6.1/tests/test_instance_config_update.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.6.0/tests/test_models.py` & `onefuzztypes-8.6.1/tests/test_models.py`

 * *Files identical despite different names*

