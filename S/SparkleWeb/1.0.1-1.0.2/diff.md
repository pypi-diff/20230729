# Comparing `tmp/SparkleWeb-1.0.1.tar.gz` & `tmp/SparkleWeb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleWeb-1.0.1.tar", last modified: Sat Jul 29 06:07:35 2023, max compression
+gzip compressed data, was "SparkleWeb-1.0.2.tar", last modified: Sat Jul 29 07:53:20 2023, max compression
```

## Comparing `SparkleWeb-1.0.1.tar` & `SparkleWeb-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 06:07:35.947733 SparkleWeb-1.0.1/
--rw-rw-rw-   0        0        0      179 2023-07-29 06:07:35.947733 SparkleWeb-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 06:07:35.914629 SparkleWeb-1.0.1/SparkleWeb/
--rw-rw-rw-   0        0        0     4806 2023-07-29 06:06:52.000000 SparkleWeb-1.0.1/SparkleWeb/SparkleWeb.py
--rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-1.0.1/SparkleWeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 06:07:35.942677 SparkleWeb-1.0.1/SparkleWeb.egg-info/
--rw-rw-rw-   0        0        0      179 2023-07-29 06:07:35.000000 SparkleWeb-1.0.1/SparkleWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-29 06:07:35.000000 SparkleWeb-1.0.1/SparkleWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 06:07:35.000000 SparkleWeb-1.0.1/SparkleWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-29 06:07:35.000000 SparkleWeb-1.0.1/SparkleWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-29 06:07:35.000000 SparkleWeb-1.0.1/SparkleWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 06:07:35.947733 SparkleWeb-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-07-29 06:07:30.000000 SparkleWeb-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/
+-rw-rw-rw-   0        0        0      179 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.629070 SparkleWeb-1.0.2/SparkleWeb/
+-rw-rw-rw-   0        0        0     8335 2023-07-29 07:52:24.000000 SparkleWeb-1.0.2/SparkleWeb/SparkleWeb.py
+-rw-rw-rw-   0        0        0       30 2023-07-28 20:05:17.000000 SparkleWeb-1.0.2/SparkleWeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 07:53:20.650421 SparkleWeb-1.0.2/SparkleWeb.egg-info/
+-rw-rw-rw-   0        0        0      179 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-29 07:53:20.000000 SparkleWeb-1.0.2/SparkleWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-29 07:53:20.658743 SparkleWeb-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-07-29 07:53:13.000000 SparkleWeb-1.0.2/setup.py
```

