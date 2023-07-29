# Comparing `tmp/aiscraper-0.0.3.tar.gz` & `tmp/aiscraper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiscraper-0.0.3.tar", last modified: Sat Jul 29 12:00:01 2023, max compression
+gzip compressed data, was "aiscraper-0.0.4.tar", last modified: Sat Jul 29 12:17:21 2023, max compression
```

## Comparing `aiscraper-0.0.3.tar` & `aiscraper-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:00:01.458761 aiscraper-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      301 2023-07-29 12:00:01.457755 aiscraper-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 12:00:01.444744 aiscraper-0.0.3/aiscraper/
--rw-rw-rw-   0        0        0       34 2023-07-29 07:42:35.000000 aiscraper-0.0.3/aiscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:00:01.454755 aiscraper-0.0.3/aiscraper.egg-info/
--rw-rw-rw-   0        0        0      301 2023-07-29 12:00:01.000000 aiscraper-0.0.3/aiscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-29 12:00:01.000000 aiscraper-0.0.3/aiscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:00:01.000000 aiscraper-0.0.3/aiscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 12:00:01.000000 aiscraper-0.0.3/aiscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 12:00:01.458761 aiscraper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-29 11:59:06.000000 aiscraper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.107118 aiscraper-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-07-29 12:17:21.106114 aiscraper-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.093104 aiscraper-0.0.4/aiscraper/
+-rw-rw-rw-   0        0        0       71 2023-07-29 12:01:53.000000 aiscraper-0.0.4/aiscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.104113 aiscraper-0.0.4/aiscraper.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-07-29 12:17:21.000000 aiscraper-0.0.4/aiscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 12:17:21.108115 aiscraper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-29 12:17:16.000000 aiscraper-0.0.4/setup.py
```

### Comparing `aiscraper-0.0.3/LICENSE` & `aiscraper-0.0.4/LICENSE`

 * *Files identical despite different names*

