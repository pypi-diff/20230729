# Comparing `tmp/aiscraper-0.0.5.tar.gz` & `tmp/aiscraper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiscraper-0.0.5.tar", last modified: Sat Jul 29 15:44:28 2023, max compression
+gzip compressed data, was "aiscraper-0.0.6.tar", last modified: Sat Jul 29 16:06:08 2023, max compression
```

## Comparing `aiscraper-0.0.5.tar` & `aiscraper-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.305151 aiscraper-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      301 2023-07-29 15:44:28.304155 aiscraper-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.286152 aiscraper-0.0.5/aiscraper/
--rw-rw-rw-   0        0        0       77 2023-07-29 15:31:57.000000 aiscraper-0.0.5/aiscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.302170 aiscraper-0.0.5/aiscraper/vanila_crawler/
--rw-rw-rw-   0        0        0      131 2023-07-29 15:36:37.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/__init__.py
--rw-rw-rw-   0        0        0     1096 2023-07-29 15:32:57.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/requests_handler.py
--rw-rw-rw-   0        0        0     1874 2023-07-29 15:33:04.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/web_crawler.py
-drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.296153 aiscraper-0.0.5/aiscraper.egg-info/
--rw-rw-rw-   0        0        0      301 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 15:44:28.305151 aiscraper-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-29 15:38:49.000000 aiscraper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:06:08.005046 aiscraper-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-07-29 16:06:08.004042 aiscraper-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 16:06:07.986041 aiscraper-0.0.6/aiscraper/
+-rw-rw-rw-   0        0        0       77 2023-07-29 15:31:57.000000 aiscraper-0.0.6/aiscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:06:08.002047 aiscraper-0.0.6/aiscraper/vanila_crawler/
+-rw-rw-rw-   0        0        0      131 2023-07-29 15:36:37.000000 aiscraper-0.0.6/aiscraper/vanila_crawler/__init__.py
+-rw-rw-rw-   0        0        0     1096 2023-07-29 16:03:34.000000 aiscraper-0.0.6/aiscraper/vanila_crawler/requests_handler.py
+-rw-rw-rw-   0        0        0     1874 2023-07-29 16:05:52.000000 aiscraper-0.0.6/aiscraper/vanila_crawler/web_crawler.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:06:07.997040 aiscraper-0.0.6/aiscraper.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-29 16:06:07.000000 aiscraper-0.0.6/aiscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-29 16:06:07.000000 aiscraper-0.0.6/aiscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:06:07.000000 aiscraper-0.0.6/aiscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 16:06:07.000000 aiscraper-0.0.6/aiscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:06:08.006043 aiscraper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-29 16:05:59.000000 aiscraper-0.0.6/setup.py
```

### Comparing `aiscraper-0.0.5/LICENSE` & `aiscraper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiscraper-0.0.5/aiscraper/vanila_crawler/requests_handler.py` & `aiscraper-0.0.6/aiscraper/vanila_crawler/requests_handler.py`

 * *Files identical despite different names*

