# Comparing `tmp/SparkleWeb-1.0.2.tar.gz` & `tmp/sparkleweb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleWeb-1.0.2.tar", last modified: Sat Jul 29 07:53:20 2023, max compression
+gzip compressed data, was "sparkleweb-1.0.3.tar", max compression
```

## Comparing `SparkleWeb-1.0.2.tar` & `sparkleweb-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,6 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/
--rw-rw-rw-   0        0        0      179 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.629070 SparkleWeb-1.0.2/SparkleWeb/
--rw-rw-rw-   0        0        0     8335 2023-07-29 07:52:24.000000 SparkleWeb-1.0.2/SparkleWeb/SparkleWeb.py
--rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-1.0.2/SparkleWeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/SparkleWeb.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 07:53:20.658743 SparkleWeb-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-07-29 07:53:13.000000 SparkleWeb-1.0.2/setup.py
+-rw-r--r--   0        0        0     1055 2023-07-29 08:09:46.488414 sparkleweb-1.0.3/LICENSE
+-rw-r--r--   0        0        0      346 2023-07-29 08:23:22.464163 sparkleweb-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      481 2023-07-29 08:13:00.430374 sparkleweb-1.0.3/README.md
+-rw-r--r--   0        0        0       30 2023-07-28 20:05:17.368311 sparkleweb-1.0.3/SparkleWeb/__init__.py
+-rw-r--r--   0        0        0     8294 2023-07-29 07:56:57.682257 sparkleweb-1.0.3/SparkleWeb/SparkleWeb.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 sparkleweb-1.0.3/PKG-INFO
```

### Comparing `SparkleWeb-1.0.2/SparkleWeb/SparkleWeb.py` & `sparkleweb-1.0.3/SparkleWeb/SparkleWeb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,18 @@
     This is a class for creating an instance of Flask-based SparkleWeb server.
     ::
     ~~~~
     `Directory Structure` =>
     >>> .
     ... ├── main.py
     ... ├── static
-    ... │   ├── extra.css
-    ... │   ├── extra.js
-    ... │   ├── main.css
-    ... │   ├── main.js
+    ... │   ├── Your_CSS_files.css
+    ... │   ├── Your_JS_files.js
     ... ├── templates
-    ... │   ├── index.html
+    ... │   ├── Your_templates.html
 
     ::
     ~~~~
 
     `Initilization` =>
     >>> from SparkleWeb import Server
     >>> app = Server()
```

