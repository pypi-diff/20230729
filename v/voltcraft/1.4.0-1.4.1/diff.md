# Comparing `tmp/voltcraft-1.4.0.tar.gz` & `tmp/voltcraft-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voltcraft-1.4.0.tar", last modified: Sat Jul 29 09:41:25 2023, max compression
+gzip compressed data, was "voltcraft-1.4.1.tar", last modified: Sat Jul 29 09:46:58 2023, max compression
```

## Comparing `voltcraft-1.4.0.tar` & `voltcraft-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.057239 voltcraft-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.045239 voltcraft-1.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.049239 voltcraft-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.github/workflows/build_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-29 09:41:13.000000 voltcraft-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-29 09:41:13.000000 voltcraft-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 09:41:13.000000 voltcraft-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:41:25.057239 voltcraft-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-29 09:41:13.000000 voltcraft-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 09:41:13.000000 voltcraft-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-29 09:41:25.057239 voltcraft-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.053239 voltcraft-1.4.0/voltcraft/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-29 09:41:13.000000 voltcraft-1.4.0/voltcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 09:41:24.000000 voltcraft-1.4.0/voltcraft/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-29 09:41:13.000000 voltcraft-1.4.0/voltcraft/pps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:41:25.057239 voltcraft-1.4.0/voltcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 09:41:25.000000 voltcraft-1.4.0/voltcraft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:58.794230 voltcraft-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:58.794230 voltcraft-1.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-29 09:46:47.000000 voltcraft-1.4.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:58.794230 voltcraft-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-29 09:46:47.000000 voltcraft-1.4.1/.github/workflows/build_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-29 09:46:47.000000 voltcraft-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-29 09:46:47.000000 voltcraft-1.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 09:46:47.000000 voltcraft-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:46:58.794230 voltcraft-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-29 09:46:47.000000 voltcraft-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-29 09:46:47.000000 voltcraft-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-29 09:46:58.798230 voltcraft-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:58.794230 voltcraft-1.4.1/voltcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-29 09:46:47.000000 voltcraft-1.4.1/voltcraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-29 09:46:47.000000 voltcraft-1.4.1/voltcraft/pps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 09:46:58.794230 voltcraft-1.4.1/voltcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-29 09:46:58.000000 voltcraft-1.4.1/voltcraft.egg-info/top_level.txt
```

### Comparing `voltcraft-1.4.0/.github/workflows/build_publish.yaml` & `voltcraft-1.4.1/.github/workflows/build_publish.yaml`

 * *Files identical despite different names*

### Comparing `voltcraft-1.4.0/.pre-commit-config.yaml` & `voltcraft-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `voltcraft-1.4.0/LICENSE.md` & `voltcraft-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.4.0/PKG-INFO` & `voltcraft-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.4.0
+Version: 1.4.1
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `voltcraft-1.4.0/README.md` & `voltcraft-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `voltcraft-1.4.0/setup.cfg` & `voltcraft-1.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 
 [options]
 packages = find:
 install_requires = 
 	pyserial
 python_requires = >=3.8
 
-[bdist_wheel]
-universal = 1
-
 [flake8]
 max-line-length = 88
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `voltcraft-1.4.0/voltcraft/pps.py` & `voltcraft-1.4.1/voltcraft/pps.py`

 * *Files identical despite different names*

### Comparing `voltcraft-1.4.0/voltcraft.egg-info/PKG-INFO` & `voltcraft-1.4.1/voltcraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voltcraft
-Version: 1.4.0
+Version: 1.4.1
 Summary: library for controlling Voltcraft PPS power supplies
 Home-page: https://github.com/ap--/voltcraft.git
 Download-URL: https://github.com/ap--/voltcraft
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
```

