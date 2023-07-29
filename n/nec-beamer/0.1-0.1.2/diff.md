# Comparing `tmp/nec_beamer-0.1.tar.gz` & `tmp/nec_beamer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nec_beamer-0.1.tar", last modified: Sat Jul 29 20:56:46 2023, max compression
+gzip compressed data, was "nec_beamer-0.1.2.tar", last modified: Sat Jul 29 21:41:22 2023, max compression
```

## Comparing `nec_beamer-0.1.tar` & `nec_beamer-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 20:56:46.698974 nec_beamer-0.1/
--rw-r--r--   0 mhp        (502) staff       (20)     1072 2023-07-29 19:57:55.000000 nec_beamer-0.1/LICENSE
--rw-r--r--   0 mhp        (502) staff       (20)      247 2023-07-29 20:56:46.698851 nec_beamer-0.1/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      188 2023-07-29 19:57:55.000000 nec_beamer-0.1/README.md
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 20:56:46.687013 nec_beamer-0.1/nec_beamer.egg-info/
--rw-r--r--   0 mhp        (502) staff       (20)      247 2023-07-29 20:56:46.000000 nec_beamer-0.1/nec_beamer.egg-info/PKG-INFO
--rw-r--r--   0 mhp        (502) staff       (20)      303 2023-07-29 20:56:46.000000 nec_beamer-0.1/nec_beamer.egg-info/SOURCES.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:56:46.000000 nec_beamer-0.1/nec_beamer.egg-info/dependency_links.txt
--rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:44:20.000000 nec_beamer-0.1/nec_beamer.egg-info/not-zip-safe
--rw-r--r--   0 mhp        (502) staff       (20)       25 2023-07-29 20:56:46.000000 nec_beamer-0.1/nec_beamer.egg-info/top_level.txt
-drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 20:56:46.698517 nec_beamer-0.1/nec_beamer_heinrich_foto/
--rw-r--r--   0 mhp        (502) staff       (20)       34 2023-07-29 20:47:52.000000 nec_beamer-0.1/nec_beamer_heinrich_foto/__init__.py
--rw-r--r--   0 mhp        (502) staff       (20)     5805 2023-07-29 20:38:23.000000 nec_beamer-0.1/nec_beamer_heinrich_foto/cli.py
--rw-r--r--   0 mhp        (502) staff       (20)    12534 2023-07-29 20:38:23.000000 nec_beamer-0.1/nec_beamer_heinrich_foto/nec_beamer.py
--rw-r--r--   0 mhp        (502) staff       (20)       38 2023-07-29 20:56:46.699022 nec_beamer-0.1/setup.cfg
--rw-r--r--   0 mhp        (502) staff       (20)      353 2023-07-29 20:45:28.000000 nec_beamer-0.1/setup.py
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.606684 nec_beamer-0.1.2/
+-rw-r--r--   0 mhp        (502) staff       (20)     1072 2023-07-29 19:57:55.000000 nec_beamer-0.1.2/LICENSE
+-rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 21:41:22.606570 nec_beamer-0.1.2/PKG-INFO
+-rw-r--r--   0 mhp        (502) staff       (20)      188 2023-07-29 19:57:55.000000 nec_beamer-0.1.2/README.md
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.605446 nec_beamer-0.1.2/nec_beamer/
+-rw-r--r--   0 mhp        (502) staff       (20)       34 2023-07-29 20:47:52.000000 nec_beamer-0.1.2/nec_beamer/__init__.py
+-rw-r--r--   0 mhp        (502) staff       (20)     5805 2023-07-29 20:38:23.000000 nec_beamer-0.1.2/nec_beamer/cli.py
+-rw-r--r--   0 mhp        (502) staff       (20)    12534 2023-07-29 20:38:23.000000 nec_beamer-0.1.2/nec_beamer/nec_beamer.py
+drwxr-xr-x   0 mhp        (502) staff       (20)        0 2023-07-29 21:41:22.606384 nec_beamer-0.1.2/nec_beamer.egg-info/
+-rw-r--r--   0 mhp        (502) staff       (20)      479 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/PKG-INFO
+-rw-r--r--   0 mhp        (502) staff       (20)      294 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/SOURCES.txt
+-rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/dependency_links.txt
+-rw-r--r--   0 mhp        (502) staff       (20)        1 2023-07-29 20:44:20.000000 nec_beamer-0.1.2/nec_beamer.egg-info/not-zip-safe
+-rw-r--r--   0 mhp        (502) staff       (20)       15 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/requires.txt
+-rw-r--r--   0 mhp        (502) staff       (20)       11 2023-07-29 21:41:22.000000 nec_beamer-0.1.2/nec_beamer.egg-info/top_level.txt
+-rw-r--r--   0 mhp        (502) staff       (20)       38 2023-07-29 21:41:22.606731 nec_beamer-0.1.2/setup.cfg
+-rw-r--r--   0 mhp        (502) staff       (20)      527 2023-07-29 21:41:16.000000 nec_beamer-0.1.2/setup.py
```

### Comparing `nec_beamer-0.1/LICENSE` & `nec_beamer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1/nec_beamer_heinrich_foto/cli.py` & `nec_beamer-0.1.2/nec_beamer/cli.py`

 * *Files identical despite different names*

### Comparing `nec_beamer-0.1/nec_beamer_heinrich_foto/nec_beamer.py` & `nec_beamer-0.1.2/nec_beamer/nec_beamer.py`

 * *Files identical despite different names*

