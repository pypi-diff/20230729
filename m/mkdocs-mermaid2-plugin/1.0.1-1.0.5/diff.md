# Comparing `tmp/mkdocs-mermaid2-plugin-1.0.1.tar.gz` & `tmp/mkdocs-mermaid2-plugin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-mermaid2-plugin-1.0.1.tar", last modified: Wed Jul 12 11:13:43 2023, max compression
+gzip compressed data, was "mkdocs-mermaid2-plugin-1.0.5.tar", last modified: Sat Jul 29 06:35:51 2023, max compression
```

## Comparing `mkdocs-mermaid2-plugin-1.0.1.tar` & `mkdocs-mermaid2-plugin-1.0.5.tar`

### file list

```diff
@@ -1,55 +1,79 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/.github/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/.github/workflows/
--rw-r--r--   0 laurent    (501) staff       (20)      359 2020-05-29 08:04:22.000000 mkdocs-mermaid2-plugin-1.0.1/.github/workflows/greetings.yml
--rw-r--r--   0 laurent    (501) staff       (20)     1203 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/.gitignore
--rw-r--r--   0 laurent    (501) staff       (20)     1079 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/LICENSE
--rw-r--r--   0 laurent    (501) staff       (20)       36 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/PKG-INFO
--rwxr-xr-x   0 laurent    (501) staff       (20)    26900 2023-04-30 12:54:23.000000 mkdocs-mermaid2-plugin-1.0.1/README.md
--rw-r--r--   0 laurent    (501) staff       (20)    18021 2020-08-20 13:19:58.000000 mkdocs-mermaid2-plugin-1.0.1/error.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/
--rwxr-xr-x   0 laurent    (501) staff       (20)      213 2020-08-24 08:41:41.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1735 2020-08-24 10:05:52.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/fence.py
--rwxr-xr-x   0 laurent    (501) staff       (20)    10260 2023-04-30 13:13:11.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/plugin.py
--rw-r--r--   0 laurent    (501) staff       (20)     3087 2020-09-06 14:18:16.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/pyjs.py
--rw-r--r--   0 laurent    (501) staff       (20)     1049 2020-09-06 09:45:38.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/util.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)      945 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       66 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      123 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        9 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)       38 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/setup.cfg
--rwxr-xr-x   0 laurent    (501) staff       (20)     1872 2023-07-12 11:13:09.000000 mkdocs-mermaid2-plugin-1.0.1/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     1174 2020-09-06 14:32:59.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/extra.js
--rw-r--r--   0 laurent    (501) staff       (20)      181 2020-12-16 12:46:31.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      643 2020-12-16 12:46:47.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      512 2023-04-27 13:33:52.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/extra.js
--rw-r--r--   0 laurent    (501) staff       (20)      266 2020-08-30 15:18:45.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      331 2020-09-06 15:02:02.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      302 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)      735 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/js/extra.js
--rw-r--r--   0 laurent    (501) staff       (20)      266 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      353 2023-04-27 12:40:01.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     1147 2020-09-06 14:41:13.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)    10474 2020-09-03 17:39:38.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/loader.js
--rw-r--r--   0 laurent    (501) staff       (20)      423 2020-09-06 15:09:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      872 2020-09-06 14:39:25.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/mkdocs.yml
--rwxr-xr-x   0 laurent    (501) staff       (20)     1118 2021-08-29 14:44:14.000000 mkdocs-mermaid2-plugin-1.0.1/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/.github/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/.github/workflows/
+-rw-r--r--   0 laurent    (501) staff       (20)      359 2020-05-29 08:04:22.000000 mkdocs-mermaid2-plugin-1.0.5/.github/workflows/greetings.yml
+-rw-r--r--   0 laurent    (501) staff       (20)     1203 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.5/.gitignore
+-rw-r--r--   0 laurent    (501) staff       (20)      600 2023-07-28 09:26:22.000000 mkdocs-mermaid2-plugin-1.0.5/.readthedocs.yml
+-rw-r--r--   0 laurent    (501) staff       (20)      613 2023-07-29 06:33:19.000000 mkdocs-mermaid2-plugin-1.0.5/CHANGELOG.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1079 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.5/LICENSE
+-rw-r--r--   0 laurent    (501) staff       (20)       36 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.5/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/PKG-INFO
+-rwxr-xr-x   0 laurent    (501) staff       (20)     4579 2023-07-28 10:28:12.000000 mkdocs-mermaid2-plugin-1.0.5/README.md
+-rwxr-xr-x   0 laurent    (501) staff       (20)    27663 2023-07-28 09:52:37.000000 mkdocs-mermaid2-plugin-1.0.5/README_old.md
+-rw-r--r--   0 laurent    (501) staff       (20)    18021 2020-08-20 13:19:58.000000 mkdocs-mermaid2-plugin-1.0.5/error.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/
+-rwxr-xr-x   0 laurent    (501) staff       (20)      213 2020-08-24 08:41:41.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1982 2023-07-19 07:43:28.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/fence.py
+-rwxr-xr-x   0 laurent    (501) staff       (20)    10712 2023-07-28 07:42:47.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/plugin.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3087 2020-09-06 14:18:16.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/pyjs.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1049 2020-09-06 09:45:38.000000 mkdocs-mermaid2-plugin-1.0.5/mermaid2/util.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-29 06:35:49.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     1398 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-07-29 06:35:49.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       66 2023-07-29 06:35:49.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      123 2023-07-29 06:35:49.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        9 2023-07-29 06:35:49.000000 mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/top_level.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       38 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/setup.cfg
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1872 2023-07-28 10:21:42.000000 mkdocs-mermaid2-plugin-1.0.5/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      520 2023-07-19 07:16:13.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2023-07-19 07:15:02.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      266 2023-07-19 07:15:02.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      305 2023-07-19 07:39:11.000000 mkdocs-mermaid2-plugin-1.0.5/test/material/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     1200 2023-07-19 08:00:01.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      194 2023-07-19 08:13:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      196 2023-07-17 08:12:28.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      817 2023-07-19 08:35:02.000000 mkdocs-mermaid2-plugin-1.0.5/test/medium/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      512 2023-04-27 13:33:52.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      266 2020-08-30 15:18:45.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      274 2023-07-18 06:52:16.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      302 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      266 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      353 2023-07-18 06:41:14.000000 mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     1147 2020-09-06 14:41:13.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)    10474 2020-09-03 17:39:38.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/js/loader.js
+-rw-r--r--   0 laurent    (501) staff       (20)      423 2020-09-06 15:09:03.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      831 2023-07-19 08:09:27.000000 mkdocs-mermaid2-plugin-1.0.5/test/superfences/mkdocs.yml
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1118 2021-08-29 14:44:14.000000 mkdocs-mermaid2-plugin-1.0.5/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     1992 2023-07-28 09:06:42.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/contribute.md
+-rw-r--r--   0 laurent    (501) staff       (20)     3133 2023-07-28 15:56:18.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/description.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-29 06:35:51.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/img/
+-rw-r--r--   0 laurent    (501) staff       (20)     7622 2023-07-27 08:11:58.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/img/custom_colors1.png
+-rw-r--r--   0 laurent    (501) staff       (20)    27520 2023-07-27 08:28:30.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/img/custom_colors2.png
+-rw-r--r--   0 laurent    (501) staff       (20)    18021 2023-07-26 11:41:37.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/img/error.png
+-rw-r--r--   0 laurent    (501) staff       (20)     7394 2023-07-28 09:43:06.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)     4166 2023-07-26 17:58:10.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/superfences.md
+-rw-r--r--   0 laurent    (501) staff       (20)     8147 2023-07-28 08:06:36.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/tips.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9209 2023-07-28 10:20:45.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/docs/troubleshooting.md
+-rw-r--r--   0 laurent    (501) staff       (20)       43 2023-07-28 09:46:17.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/extra_requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)     1172 2023-07-28 09:42:53.000000 mkdocs-mermaid2-plugin-1.0.5/webdoc/mkdocs.yml
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/.gitignore` & `mkdocs-mermaid2-plugin-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/LICENSE` & `mkdocs-mermaid2-plugin-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/PKG-INFO` & `mkdocs-mermaid2-plugin-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-mermaid2-plugin
-Version: 1.0.1
+Version: 1.0.5
 Summary: A MkDocs plugin for including mermaid graphs in markdown sources
 Home-page: https://github.com/fralau/mkdocs-mermaid2-plugin
 Author: pugong, Fralau
 Author-email: pugong.liu@gmail.com, fralau2035@yahoo.com
 License: MIT
 Keywords: mkdocs python markdown mermaid
 Classifier: Development Status :: 4 - Beta
@@ -12,12 +12,12 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
 A mkdocs plugin that interprets mermaid graphs in the markdown file.To install, please follow instructions in the readme file.This is a fork of the Pugong Liu's excellent project, which is no longer maintained.
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/README.md` & `mkdocs-mermaid2-plugin-1.0.5/README_old.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # mkdocs-mermaid2-plugin
 
 
+**THIS IS AN OLD VERSION, KEPT HERE FOR REFERENCE**
+
+[Use the documentation on ReadTheDocs](https://mkdocs-mermaid2.readthedocs.io).
+
+
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-mermaid2-plugin)](https://pypi.org/project/mkdocs-mermaid2-plugin/)
 ![Github](https://img.shields.io/github/v/tag/fralau/mkdocs-mermaid2-plugin?label=github%20tag)
 ![Downloads(PyPI)](https://img.shields.io/pypi/dm/mkdocs-mermaid2-plugin)
 
 
 An [MkDocs](https://www.mkdocs.org/) plugin that renders textual graph
@@ -259,15 +264,15 @@
 ```
 
 Where `js` is a subdirectory of the document directory (`docs`).
 
 If you are using a local javascript file, it is up to you to write the import,
 with a version of the Mermaid library > 10 e.g.:
 
-```yaml
+```javascript
 import mermaid from "https://unpkg.com/mermaid@10.0.2/dist/mermaid.esm.min.mjs"
 ```
 
 No explicit call to `mermaid.initialize()` is required, since it is
 automatically inserted by the plugin.
 
 
@@ -298,30 +303,26 @@
 
 ### Adding arguments to the Mermaid engine
 
 By default, the plugin automatically inserts 
 a Javascript command `mermaid.initialize();`
 in the HTML pages, which starts the interpretation.
 Sometimes, however, you may want to add some
-initialization commands (see [full list](https://github.com/knsv/mermaid/blob/master/docs/mermaidAPI.md#mermaidapi-configuration-defaults)).
+initialization commands (see [full list](https://github.com/mermaid-js/mermaid/blob/master/docs/config/setup/modules/mermaidAPI.md#mermaidapi-configuration-defaults)).
 
 For example, you could change the theme of the diagram, 
 using 'dark' instead of the default one. 
 Simply add those arguments in the config file, e.g.
 
 ```yaml
 plugins:
     - search
     - mermaid2:
         arguments:
           theme: 'dark'
-
-
-extra_javascript:
-    - https://unpkg.com/mermaid/dist/mermaid.min.js
 ```
 
 ### Testing
 
 To test your website with a diagram, restart the mkdocs server:
 
     mkdocs serve
@@ -330,14 +331,18 @@
 (by default: `https://localhost:8000`)
 
 
 ### Adding a Javascript callback function
 
 _New in 0.3.0_
 
+**CAUTION**: As of the [version 10.0.0 of the javascript Library(https://github.com/mermaid-js/mermaid/blob/develop/CHANGELOG.md#changelog)], callbacks are no longer accepted.
+If you wish to use callbacks, specify a lower version of the
+library in the config file.
+
 #### Use Case
 To make modifications that are not possible with css, it can be useful
 to insert a callback function (Javascript) into the target HTML page.
 
 This can be done using the standard pattern, e.g.:
 
 ```javascript
@@ -574,14 +579,16 @@
 | **minify**               | plugin    | NO     | Breaks the mermaid diagrams.                                     |
 | **pymdownx.highlight**   | extension | NO     | Use [pymdownx.superfences](#declaring-the-superfences-extension) |
 | **pymdownx.superfences** | extension | OK     | [see paragraph](#declaring-the-superfences-extension)            |
 | **search**               | plugin    | OK     | Do not forget to declare it in `config.yml`.                     |
 
 ### Using Mermaid and code highlighting at the same time
 
+>**IMPORTANT** Do NOT use Superfences unless you want code highlighting.
+
 #### Usage
 
 It is quite natural that we want to display **mermaid diagrams**,
 while having usual **code highlighting** (for bash, python, etc.).
 
 #### Use of markdown extensions
 **Symptom**: The mermaid code is not transformed into a diagram,
@@ -616,25 +623,41 @@
 It means: 
 
 1. Take the fenced parts marked with mermaid
 2. Turn them into `class='mermaid'`.
 3. To format those pieces, use the function `fence_mermaid`, 
    from the mermaid2 package.
 
+There are **two** functions:
+
+* `fence_mermaid` for the general case.
+* `fence_mermaid_custom` for the Material theme (note the use of
+the **custom** suffix)
+
+Hence, for the Material theme (only):
+```yaml
+markdown_extensions:
+  - pymdownx.superfences:
+      # make exceptions to highlighting of code:
+      custom_fences:
+        - name: mermaid
+          class: mermaid
+          format: !!python/name:mermaid2.fence_mermaid_custom
+```
+
+
 
 > **IMPORTANT:** Note that the superfences will be slightly more demanding with
 > HTML tags inside a mermaid diagram: 
 > **take care to always close the HTML tags that require it**
 > (e.g. `<small>` must have its corresponding `</small>` tag).
 > Otherwise, the extension system will attempt to close those tags 
 > and it will break the diagram.
 
 
-
-
 ## Troubleshooting
 
 ### The mermaid diagram is not displayed (or displayed incorrectly)
 
 > To start with, use a simple diagram that you know is syntactically correct.
 
 e.g.
@@ -660,18 +683,14 @@
 the mermaid javascript library was called.
 
 #### The mermaid source code appears as-is (not read)?
 In that case, the javascript library was probably not called.
 See the next questions.
 
 
-#### Using another theme than material ?
-
-If the diagram is not rendered, upgrade to plugin version >= 0.5.0
-
 #### Using superfences, but no diagram is displayed?
 
 If you are using the superfences extension, but you see the source
 code, you probably forgot to declare the custom_fences. 
 Se more explanations under [Declaring the superfences extension](#declaring-the-superfences-extension)
 
 #### Is mkdocs' version up to date (>= 1.1) ?
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/error.png` & `mkdocs-mermaid2-plugin-1.0.5/error.png`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/mermaid2/fence.py` & `mkdocs-mermaid2-plugin-1.0.5/mermaid2/fence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """
 Special fence for PyMdown Extensions Superfences
 See: https://facelessuser.github.io/pymdown-extensions/extensions/superfences/#formatters
+
+NOTE: SUPERFENCES AND CUSTOM_FENCES ARE NOT NEEDED UNLESS
+      CODE HIGHLIGHTING IS REQUIRED.
+
+- fence_mermaid() for most Mkdocs themes
+- fence_mermaid_custom() for Material theme
 """
 from functools import partial
 
 
 def fence_mermaid(source, language, css_class, options, md, 
             classes=None, id_value='', custom=False, **kwargs):
     """
     For mermaid loose mode:
 
     This function is needed for correctly displaying the mermaid
-    HTML in diagrams when pymdownx.superfences is activated.
+    HTML in diagrams when pymdownx.superfences is activated,
+    so that code highlighting is activated.
 
     Contrary to the standard fence_div_format used in
     https://github.com/facelessuser/pymdown-extensions/blob/9489bd8d94eebf4a109b7dada613bc2db378e31f/pymdownx/superfences.py#L149,
     this function it format sources as <div>...</div> but
     WITHOUT escaping the < and > characters in the HTML.
 
     It should be called in the mkdocs.yaml file as:
@@ -40,10 +47,11 @@
                 (id_value, classes, source)
     else:
         html = '<div %s class="%s">%s\n</div>' % \
                 (id_value, classes, source)
     # print("--- Mermaid ---\n", html, "\n------")
     return html
 
-# special custom function (do not forget to specify name!)
+# special custom function for Material theme
+# (do not forget to specify name!)
 fence_mermaid_custom = partial(fence_mermaid, custom=True)
 fence_mermaid_custom.__name__ = 'fence_mermaid_custom'
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/mermaid2/plugin.py` & `mkdocs-mermaid2-plugin-1.0.5/mermaid2/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .util import info, libname, url_exists
 
 
 # ------------------------
 # Constants and utilities
 # ------------------------
 # the default (recommended) mermaid lib
-MERMAID_LIB_VERSION = '10.0.2'
+MERMAID_LIB_VERSION = '10.1.0'
 # MERMAID_LIB = "https://unpkg.com/mermaid@%s/dist/mermaid.min.js"
 MERMAID_LIB_PRE_10 = "https://unpkg.com/mermaid@%s/dist/mermaid.min.js"
 MERMAID_LIB = "https://unpkg.com/mermaid@%s/dist/mermaid.esm.min.mjs"
 
 
 MERMAID_CODE_PRE_10 = '<script src="%s">\n'
 MERMAID_CODE = '<script type="module">import mermaid from "%s"</script>\n'
@@ -92,15 +92,20 @@
 
 
     @property
     def extra_mermaid_lib(self) -> str:
         """
         Provides the mermaid library defined in mkdocs.yml (if any)
         """
-        extra_javascript = self.full_config.get('extra_javascript', [])
+        # As of mkdocs 1.5, extra_javascript is a list of objects; 
+        # no longer a string. Call to str was used.
+        # Patched in 1.5.1, with __fspath___ method, 
+        # see https://github.com/mkdocs/mkdocs/issues/3310
+        # But we keep it, to guarantee it's a string. 
+        extra_javascript = map(str, self.full_config.get('extra_javascript', []))
         for lib in extra_javascript:
             # get the actual library name
             if  libname(lib) == 'mermaid':
                 return lib
         return ''
 
 
@@ -257,10 +262,14 @@
             if self.activate_custom_loader:
                 # if the superfences extension is present, use the specific loader
                 self.mermaid_args['startOnLoad'] = False
                 js_args =  pyjs.dumps(self.mermaid_args) 
                 new_tag.string = "window.mermaidConfig = {default: %s}" % js_args
             else:
                 js_args =  pyjs.dumps(self.mermaid_args) 
-                new_tag.string="mermaid.initialize(%s);" % js_args
+                if self.mermaid_major_version >= 10:
+                    new_tag.string="mermaidAPI.initialize(%s);" % js_args
+                else:
+                    new_tag.string="mermaid.initialize(%s);" % js_args
+
             soup.body.append(new_tag)
         return str(soup)
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/mermaid2/pyjs.py` & `mkdocs-mermaid2-plugin-1.0.5/mermaid2/pyjs.py`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/mermaid2/util.py` & `mkdocs-mermaid2-plugin-1.0.5/mermaid2/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/PKG-INFO` & `mkdocs-mermaid2-plugin-1.0.5/mkdocs_mermaid2_plugin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-mermaid2-plugin
-Version: 1.0.1
+Version: 1.0.5
 Summary: A MkDocs plugin for including mermaid graphs in markdown sources
 Home-page: https://github.com/fralau/mkdocs-mermaid2-plugin
 Author: pugong, Fralau
 Author-email: pugong.liu@gmail.com, fralau2035@yahoo.com
 License: MIT
 Keywords: mkdocs python markdown mermaid
 Classifier: Development Status :: 4 - Beta
@@ -12,12 +12,12 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
 A mkdocs plugin that interprets mermaid graphs in the markdown file.To install, please follow instructions in the readme file.This is a fork of the Pugong Liu's excellent project, which is no longer maintained.
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/setup.py` & `mkdocs-mermaid2-plugin-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.5'
 
 # required if you want to run tests
 # pip install 'mkdocs-mermaid2-plugin[test]'
 TEST_REQUIRE = ['mkdocs-material']
 
 
 def readme():
@@ -27,15 +27,15 @@
     description='A MkDocs plugin for including mermaid graphs in markdown sources',
     long_description=LONG_DESCRIPTION,
     keywords='mkdocs python markdown mermaid',
     url='https://github.com/fralau/mkdocs-mermaid2-plugin',
     author='pugong, Fralau',
     author_email='pugong.liu@gmail.com, fralau2035@yahoo.com',
     license='MIT',
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     install_requires=[
         'setuptools>=18.5',
         'beautifulsoup4>=4.6.3',
         'mkdocs>=1.0.4',
         'jsbeautifier',
         'requests',
         'pymdown-extensions >= 8.0'
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/index.md` & `mkdocs-mermaid2-plugin-1.0.5/test/medium/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,27 +31,27 @@
     click mermaid "https://mermaid-js.github.io/mermaid" "Website"
 ```
 
 > The box **mermaid web site** is clickable!
 
 
 ## Normal fences
-This is usual fenced code (with no highlighting)
+This is usual fenced code (with color highlighting)
 
 ```python
 for page in pages:
     page.read()
 ```
 
 ## Javascript callback
-Check in the web console that a message of that type is displayed:
+Check **in the web console** that a message of that type is displayed:
 
 ```
 Hello, this is myMermaidCallbackFunction mermaid-1598273751083 14:55:51
 ```
 
-This is the result of this directive:
+This is the result of this directive in the config file:
 
 ```
 extra_javascript:
      - js/extra.js
 ```
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/extra.js` & `mkdocs-mermaid2-plugin-1.0.5/test/material/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/medium/mkdocs.yml` & `mkdocs-mermaid2-plugin-1.0.5/test/medium/mkdocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,27 @@
 nav:
   - Main: index.md
   - Second: second.md
 
 plugins:
   - search
   - mermaid2:
-      version: 8.6.4 # just because we can
+      version: '10.1.0' # just because we can
       arguments:
         securityLevel: 'loose'
         theme: forest # we want also that to work
         mermaid:
               callback: ^myMermaidCallbackFunction
 
 markdown_extensions:
   - admonition
   - pymdownx.details
+  - pymdownx.superfences:
+      # make exceptions to highlighting of code:
+      custom_fences:
+        - name: mermaid
+          class: mermaid
+          format: !!python/name:mermaid2.fence_mermaid_custom
 
 extra_javascript:
-     # - https://unpkg.com/mermaid@8.6.4/dist/mermaid.min.js
+     # Callback function
      - js/extra.js
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/index.md` & `mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/extra.js` & `mkdocs-mermaid2-plugin-1.0.5/test/simple/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/js/extra.js` & `mkdocs-mermaid2-plugin-1.0.5/test/simple_pre_10/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/index.md` & `mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/loader.js` & `mkdocs-mermaid2-plugin-1.0.5/test/superfences/docs/js/loader.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-1.0.1/test/superfences/mkdocs.yml` & `mkdocs-mermaid2-plugin-1.0.5/test/superfences/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,9 +27,8 @@
       custom_fences:
         - name: mermaid
           class: mermaid
           format: !!python/name:mermaid2.fence_mermaid_custom
           # format: !!python/name:pymdownx.superfences.fence_div_format
 extra_javascript:
      # - https://unpkg.com/mermaid@8.6.4/dist/mermaid.min.js
-     # This is mandatory for the moment:
      - js/loader.js
```

### Comparing `mkdocs-mermaid2-plugin-1.0.1/update_pypi.sh` & `mkdocs-mermaid2-plugin-1.0.5/update_pypi.sh`

 * *Files identical despite different names*

