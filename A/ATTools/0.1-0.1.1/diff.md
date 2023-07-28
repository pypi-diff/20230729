# Comparing `tmp/ATTools-0.1.tar.gz` & `tmp/ATTools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATTools-0.1.tar", last modified: Fri Jul 28 10:27:58 2023, max compression
+gzip compressed data, was "ATTools-0.1.1.tar", last modified: Fri Jul 28 19:00:44 2023, max compression
```

## Comparing `ATTools-0.1.tar` & `ATTools-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 10:27:58.317683 ATTools-0.1/
-drwxrwxrwx   0        0        0        0 2023-07-28 10:27:58.313686 ATTools-0.1/ATTools.egg-info/
--rw-rw-rw-   0        0        0      493 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-07-28 10:27:58.000000 ATTools-0.1/ATTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 10:27:57.000000 ATTools-0.1/ATTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      493 2023-07-28 10:27:58.316684 ATTools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-28 10:27:58.317683 ATTools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-28 10:27:07.000000 ATTools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:00:44.451231 ATTools-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-28 19:00:44.425251 ATTools-0.1.1/ATTools/
+-rw-rw-rw-   0        0        0    11522 2023-07-28 18:54:08.000000 ATTools-0.1.1/ATTools/ATTools.py
+-rw-rw-rw-   0        0        0      457 2023-07-28 18:59:52.000000 ATTools-0.1.1/ATTools/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 19:00:44.447233 ATTools-0.1.1/ATTools.egg-info/
+-rw-rw-rw-   0        0        0      175 2023-07-28 19:00:43.000000 ATTools-0.1.1/ATTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-07-28 19:00:44.000000 ATTools-0.1.1/ATTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 19:00:43.000000 ATTools-0.1.1/ATTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-28 19:00:43.000000 ATTools-0.1.1/ATTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 19:00:43.000000 ATTools-0.1.1/ATTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      175 2023-07-28 19:00:44.449234 ATTools-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 19:00:44.451231 ATTools-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      457 2023-07-28 18:59:52.000000 ATTools-0.1.1/setup.py
```

