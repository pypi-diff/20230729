# Comparing `tmp/aiscraper-0.0.4.tar.gz` & `tmp/aiscraper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiscraper-0.0.4.tar", last modified: Sat Jul 29 12:17:21 2023, max compression
+gzip compressed data, was "aiscraper-0.0.5.tar", last modified: Sat Jul 29 15:44:28 2023, max compression
```

## Comparing `aiscraper-0.0.4.tar` & `aiscraper-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.107118 aiscraper-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      301 2023-07-29 12:17:21.106114 aiscraper-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.093104 aiscraper-0.0.4/aiscraper/
--rw-rw-rw-   0        0        0       71 2023-07-29 12:01:53.000000 aiscraper-0.0.4/aiscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 12:17:21.104113 aiscraper-0.0.4/aiscraper.egg-info/
--rw-rw-rw-   0        0        0      301 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-29 12:17:21.000000 aiscraper-0.0.4/aiscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-29 12:17:20.000000 aiscraper-0.0.4/aiscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 12:17:21.108115 aiscraper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      409 2023-07-29 12:17:16.000000 aiscraper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.305151 aiscraper-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-29 05:24:37.000000 aiscraper-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      301 2023-07-29 15:44:28.304155 aiscraper-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.286152 aiscraper-0.0.5/aiscraper/
+-rw-rw-rw-   0        0        0       77 2023-07-29 15:31:57.000000 aiscraper-0.0.5/aiscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.302170 aiscraper-0.0.5/aiscraper/vanila_crawler/
+-rw-rw-rw-   0        0        0      131 2023-07-29 15:36:37.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/__init__.py
+-rw-rw-rw-   0        0        0     1096 2023-07-29 15:32:57.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/requests_handler.py
+-rw-rw-rw-   0        0        0     1874 2023-07-29 15:33:04.000000 aiscraper-0.0.5/aiscraper/vanila_crawler/web_crawler.py
+drwxrwxrwx   0        0        0        0 2023-07-29 15:44:28.296153 aiscraper-0.0.5/aiscraper.egg-info/
+-rw-rw-rw-   0        0        0      301 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-29 15:44:28.000000 aiscraper-0.0.5/aiscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 15:44:28.305151 aiscraper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-29 15:38:49.000000 aiscraper-0.0.5/setup.py
```

### Comparing `aiscraper-0.0.4/LICENSE` & `aiscraper-0.0.5/LICENSE`

 * *Files identical despite different names*

