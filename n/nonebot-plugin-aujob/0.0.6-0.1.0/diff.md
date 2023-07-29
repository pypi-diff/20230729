# Comparing `tmp/nonebot_plugin_aujob-0.0.6.tar.gz` & `tmp/nonebot_plugin_aujob-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aujob-0.0.6.tar", last modified: Fri Jul 28 11:25:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_aujob-0.1.0.tar", last modified: Sat Jul 29 02:42:50 2023, max compression
```

## Comparing `nonebot_plugin_aujob-0.0.6.tar` & `nonebot_plugin_aujob-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.519140 nonebot_plugin_aujob-0.0.6/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:25:51.517141 nonebot_plugin_aujob-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.503138 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob/
--rw-rw-rw-   0        0        0    15651 2023-07-28 11:25:23.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 11:25:51.515138 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/
--rw-rw-rw-   0        0        0      511 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-28 11:25:51.000000 nonebot_plugin_aujob-0.0.6/nonebot_plugin_aujob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      698 2023-07-28 11:25:35.000000 nonebot_plugin_aujob-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 11:25:51.519140 nonebot_plugin_aujob-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.197320 nonebot_plugin_aujob-0.1.0/
+-rw-rw-rw-   0        0        0      511 2023-07-29 02:42:50.197320 nonebot_plugin_aujob-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.182321 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/
+-rw-rw-rw-   0        0        0     1741 2023-07-29 02:41:43.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/__init__.py
+-rw-rw-rw-   0        0        0    11199 2023-07-29 02:41:44.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-29 02:42:50.194320 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/
+-rw-rw-rw-   0        0        0      511 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-29 02:42:50.000000 nonebot_plugin_aujob-0.1.0/nonebot_plugin_aujob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      698 2023-07-29 02:42:21.000000 nonebot_plugin_aujob-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-29 02:42:50.198319 nonebot_plugin_aujob-0.1.0/setup.cfg
```

### Comparing `nonebot_plugin_aujob-0.0.6/pyproject.toml` & `nonebot_plugin_aujob-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nonebot_plugin_aujob"
-version = "0.0.6"
+version = "0.1.0"
 authors = [
   { name="qwqZYLqwq", email="3422471182@qq.com" },
 ]
 description = "A nonebot plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

