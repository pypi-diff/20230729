# Comparing `tmp/aiscraper-0.0.2.tar.gz` & `tmp/aiscraper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiscraper-0.0.2.tar", last modified: Sat Jul 29 07:55:12 2023, max compression
+gzip compressed data, was "aiscraper-0.2.5.tar", last modified: Sat Jul 29 06:17:24 2023, max compression
```

## Comparing `aiscraper-0.0.2.tar` & `aiscraper-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 07:55:12.880552 aiscraper-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      301 2023-07-29 07:55:12.880045 aiscraper-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 07:55:12.865973 aiscraper-0.0.2/aiscraper/
--rw-rw-rw-   0        0        0       34 2023-07-29 07:42:35.000000 aiscraper-0.0.2/aiscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:55:12.877524 aiscraper-0.0.2/aiscraper.egg-info/
--rw-rw-rw-   0        0        0      301 2023-07-29 07:55:12.000000 aiscraper-0.0.2/aiscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-29 07:55:12.000000 aiscraper-0.0.2/aiscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 07:55:12.000000 aiscraper-0.0.2/aiscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 07:55:12.000000 aiscraper-0.0.2/aiscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 07:55:12.880552 aiscraper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-29 07:54:50.000000 aiscraper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 06:17:24.801337 aiscraper-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-07-29 06:17:24.800339 aiscraper-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 06:17:24.797343 aiscraper-0.2.5/aiscraper.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-29 06:17:24.000000 aiscraper-0.2.5/aiscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-07-29 06:17:24.000000 aiscraper-0.2.5/aiscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 06:17:24.000000 aiscraper-0.2.5/aiscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-29 06:17:24.000000 aiscraper-0.2.5/aiscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 06:17:24.799338 aiscraper-0.2.5/init/
+-rw-rw-rw-   0        0        0       41 2023-07-29 06:09:20.000000 aiscraper-0.2.5/init/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 06:17:24.801337 aiscraper-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-29 06:17:06.000000 aiscraper-0.2.5/setup.py
```

### Comparing `aiscraper-0.0.2/LICENSE` & `aiscraper-0.2.5/LICENSE`

 * *Files identical despite different names*

