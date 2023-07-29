# Comparing `tmp/runusb-2023.0.0.tar.gz` & `tmp/runusb-2023.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runusb-2023.0.0.tar", last modified: Sat Jul 29 17:06:51 2023, max compression
+gzip compressed data, was "runusb-2023.0.0rc2.tar", last modified: Sat Jul 29 14:07:07 2023, max compression
```

## Comparing `runusb-2023.0.0.tar` & `runusb-2023.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:06:51.979332 runusb-2023.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-29 17:06:34.000000 runusb-2023.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 17:06:51.979332 runusb-2023.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-29 17:06:34.000000 runusb-2023.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:06:51.975331 runusb-2023.0.0/runusb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 17:06:34.000000 runusb-2023.0.0/runusb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11238 2023-07-29 17:06:34.000000 runusb-2023.0.0/runusb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 17:06:51.979332 runusb-2023.0.0/runusb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 17:06:51.000000 runusb-2023.0.0/runusb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-29 17:06:51.979332 runusb-2023.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 17:06:34.000000 runusb-2023.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/runusb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/runusb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11238 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/runusb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/runusb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 14:07:07.000000 runusb-2023.0.0rc2/runusb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-29 14:07:07.728374 runusb-2023.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:06:46.000000 runusb-2023.0.0rc2/setup.py
```

### Comparing `runusb-2023.0.0/LICENSE` & `runusb-2023.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `runusb-2023.0.0/runusb/__main__.py` & `runusb-2023.0.0rc2/runusb/__main__.py`

 * *Files identical despite different names*

### Comparing `runusb-2023.0.0/setup.cfg` & `runusb-2023.0.0rc2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = runusb
-version = 2023.0.0
+version = 2023.0.0rc2
 description = Automagic running of USB sticks
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = "Alistair Lynn"
 url = https://github.com/sourcebots/runusb
```

